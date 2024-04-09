# Comparing `tmp/rich-click-1.7.4.tar.gz` & `tmp/rich-click-1.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-click-1.7.4.tar", last modified: Tue Mar 12 04:37:35 2024, max compression
+gzip compressed data, was "rich-click-1.8.0.dev0.tar", last modified: Tue Apr  9 11:19:35 2024, max compression
```

## Comparing `rich-click-1.7.4.tar` & `rich-click-1.8.0.dev0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:37:35.682416 rich-click-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 04:37:31.000000 rich-click-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-03-12 04:37:35.682416 rich-click-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-03-12 04:37:31.000000 rich-click-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-12 04:37:31.000000 rich-click-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-12 04:37:35.686416 rich-click-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-12 04:37:31.000000 rich-click-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:37:35.678416 rich-click-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:37:35.682416 rich-click-1.7.4/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    35279 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-12 04:37:31.000000 rich-click-1.7.4/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:37:35.682416 rich-click-1.7.4/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22300 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 04:37:35.000000 rich-click-1.7.4/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 04:37:35.682416 rich-click-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-12 04:37:31.000000 rich-click-1.7.4/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-03-12 04:37:31.000000 rich-click-1.7.4/tests/test_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.708014 rich-click-1.8.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:19:35.000000 rich-click-1.8.0.dev0/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:19:35.712014 rich-click-1.8.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-04-09 11:19:31.000000 rich-click-1.8.0.dev0/tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.7.4/LICENSE` & `rich-click-1.8.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-click-1.7.4/src/rich_click/__init__.py` & `rich-click-1.8.0.dev0/src/rich_click/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# flake8: noqa: F401
+# ruff: noqa: F401
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
-The intention is to provide attractive help output from click, formatted with rich, with minimal
+The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.7.4"
+__version__ = "1.8.0dev0"
 
 # Import the entire click API here.
-# We need to manually import these instead of `from click import *` to force mypy to recognize a few type annotation overrides for the rich_click decorators.
+# We need to manually import these instead of `from click import *` to force
+# mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
 from click.core import Context as Context
 from click.core import Group as Group
 from click.core import Option as Option
 from click.core import Parameter as Parameter
@@ -46,46 +47,46 @@
 from click.termui import pause as pause
 from click.termui import progressbar as progressbar
 from click.termui import prompt as prompt
 from click.termui import secho as secho
 from click.termui import style as style
 from click.termui import unstyle as unstyle
 from click.types import BOOL as BOOL
+from click.types import FLOAT as FLOAT
+from click.types import INT as INT
+from click.types import STRING as STRING
+from click.types import UNPROCESSED as UNPROCESSED
+from click.types import UUID as UUID
 from click.types import Choice as Choice
 from click.types import DateTime as DateTime
 from click.types import File as File
-from click.types import FLOAT as FLOAT
 from click.types import FloatRange as FloatRange
-from click.types import INT as INT
 from click.types import IntRange as IntRange
 from click.types import ParamType as ParamType
 from click.types import Path as Path
-from click.types import STRING as STRING
 from click.types import Tuple as Tuple
-from click.types import UNPROCESSED as UNPROCESSED
-from click.types import UUID as UUID
 from click.utils import echo as echo
 from click.utils import format_filename as format_filename
 from click.utils import get_app_dir as get_app_dir
 from click.utils import get_binary_stream as get_binary_stream
 from click.utils import get_text_stream as get_text_stream
 from click.utils import open_file as open_file
 
-from . import rich_click as rich_click
-
 from rich_click.decorators import command as command
 from rich_click.decorators import group as group
 from rich_click.decorators import pass_context as pass_context
 from rich_click.decorators import rich_config as rich_config
 from rich_click.rich_command import RichCommand as RichCommand
 from rich_click.rich_command import RichCommandCollection as RichCommandCollection
 from rich_click.rich_command import RichGroup as RichGroup
 from rich_click.rich_context import RichContext as RichContext
 from rich_click.rich_help_configuration import RichHelpConfiguration as RichHelpConfiguration
 
+from . import rich_click as rich_click
+
 
 def __getattr__(name: str) -> object:
     from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_9X
 
     if name == "RichMultiCommand" and CLICK_IS_BEFORE_VERSION_9X:
         import warnings
```

### Comparing `rich-click-1.7.4/src/rich_click/decorators.py` & `rich-click-1.8.0.dev0/src/rich_click/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,62 @@
-"""
-rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
+from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Optional, Type, TypeVar, Union, cast, overload
 
-The intention is to provide attractive help output from click, formatted with rich, with minimal
-customisation required.
-"""
-
-from typing import Any, Callable, cast, Dict, Optional, overload, Type, TYPE_CHECKING, TypeVar, Union
-
-from click import Command
+from click import Command, Group
 from click import command as click_command
-from click import Group
-from click import group as click_group
 from click import pass_context as click_pass_context
-from rich.console import Console
 from typing_extensions import Concatenate, ParamSpec
 
-from . import rich_click  # noqa: F401
-
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X
 from rich_click.rich_command import RichCommand, RichGroup, RichMultiCommand  # noqa: F401
 from rich_click.rich_context import RichContext
 from rich_click.rich_help_configuration import RichHelpConfiguration
 
-# MyPy does not like star imports. Therefore when we are type checking, we import each individual module
-# from click here. This way MyPy will recognize the import and not throw any errors. Furthermore, because of
-# the TYPE_CHECKING check, it does not influence the start routine at all.
+from . import rich_click  # noqa: F401
+
+
+if TYPE_CHECKING:
+    from rich.console import Console
+
 
 _AnyCallable = Callable[..., Any]
 F = TypeVar("F", bound=Callable[..., Any])
 FC = TypeVar("FC", bound=Union[Command, _AnyCallable])
 
 
 GrpType = TypeVar("GrpType", bound=Group)
 
 
 # variant: no call, directly as decorator for a function.
 @overload
-def group(name: _AnyCallable) -> RichGroup:
-    ...
+def group(name: _AnyCallable) -> RichGroup: ...
 
 
 # variant: with positional name and with positional or keyword cls argument:
 # @group(namearg, GroupCls, ...) or @group(namearg, cls=GroupCls, ...)
 @overload
 def group(
     name: Optional[str],
     cls: Type[GrpType],
     **attrs: Any,
-) -> Callable[[_AnyCallable], GrpType]:
-    ...
+) -> Callable[[_AnyCallable], GrpType]: ...
 
 
 # variant: name omitted, cls _must_ be a keyword argument, @group(cmd=GroupCls, ...)
 @overload
 def group(
     name: None = None,
     *,
     cls: Type[GrpType],
     **attrs: Any,
-) -> Callable[[_AnyCallable], GrpType]:
-    ...
+) -> Callable[[_AnyCallable], GrpType]: ...
 
 
 # variant: with optional string name, no cls argument provided.
 @overload
-def group(name: Optional[str] = ..., cls: None = None, **attrs: Any) -> Callable[[_AnyCallable], RichGroup]:
-    ...
+def group(name: Optional[str] = ..., cls: None = None, **attrs: Any) -> Callable[[_AnyCallable], RichGroup]: ...
 
 
 def group(
     name: Union[str, _AnyCallable, None] = None,
     cls: Optional[Type[GrpType]] = None,
     **attrs: Any,
 ) -> Union[Group, Callable[[_AnyCallable], Union[RichGroup, GrpType]]]:
@@ -88,44 +75,40 @@
 
 
 CmdType = TypeVar("CmdType", bound=Command)
 
 
 # variant: no call, directly as decorator for a function.
 @overload
-def command(name: _AnyCallable) -> RichCommand:
-    ...
+def command(name: _AnyCallable) -> RichCommand: ...
 
 
 # variant: with positional name and with positional or keyword cls argument:
 # @command(namearg, CommandCls, ...) or @command(namearg, cls=CommandCls, ...)
 @overload
 def command(
     name: Optional[str],
     cls: Type[CmdType],
     **attrs: Any,
-) -> Callable[[_AnyCallable], CmdType]:
-    ...
+) -> Callable[[_AnyCallable], CmdType]: ...
 
 
 # variant: name omitted, cls _must_ be a keyword argument, @command(cls=CommandCls, ...)
 @overload
 def command(
     name: None = None,
     *,
     cls: Type[CmdType],
     **attrs: Any,
-) -> Callable[[_AnyCallable], CmdType]:
-    ...
+) -> Callable[[_AnyCallable], CmdType]: ...
 
 
 # variant: with optional string name, no cls argument provided.
 @overload
-def command(name: Optional[str] = ..., cls: None = None, **attrs: Any) -> Callable[[_AnyCallable], RichCommand]:
-    ...
+def command(name: Optional[str] = ..., cls: None = None, **attrs: Any) -> Callable[[_AnyCallable], RichCommand]: ...
 
 
 def command(
     name: Union[Optional[str], _AnyCallable] = None,
     cls: Optional[Type[CmdType]] = None,
     **attrs: Any,
 ) -> Union[Command, Callable[[_AnyCallable], Union[RichCommand, CmdType]]]:
@@ -146,33 +129,59 @@
 class NotSupportedError(Exception):
     """Not Supported Error."""
 
     pass
 
 
 def rich_config(
-    console: Optional[Console] = None, help_config: Optional[RichHelpConfiguration] = None
+    help_config: Optional[Union[Mapping[str, Any], RichHelpConfiguration]] = None,
+    *,
+    console: Optional["Console"] = None,
 ) -> Callable[[FC], FC]:
-    """Use decorator to configure Rich Click settings.
+    """
+    Use decorator to configure Rich Click settings.
 
     Args:
-        console: A Rich Console that will be accessible from the `RichContext`, `RichCommand`, and `RichGroup` instances
-            Defaults to None.
+    ----
         help_config: Rich help configuration that is used internally to format help messages and exceptions
             Defaults to None.
+        console: A Rich Console that will be accessible from the `RichContext`, `RichCommand`, and `RichGroup` instances
+            Defaults to None.
     """
+    from rich.console import Console
+
+    if isinstance(help_config, Console) and console is None:
+        import warnings
+
+        warnings.warn(
+            "`rich_config()`'s args have been swapped."
+            " Please set the config first, and use a kwarg to set the console.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        console = help_config
+    elif isinstance(help_config, Console):
+        import warnings
+
+        warnings.warn(
+            "We have no idea what just happened. Tread carefully.",
+            RuntimeWarning,
+            stacklevel=2,
+        )
+
     if CLICK_IS_BEFORE_VERSION_8X:
 
         def decorator_with_warning(obj: FC) -> FC:
             import warnings
 
             warnings.warn(
                 "`rich_config()` does not work with versions of click prior to version 8.0.0."
                 " Please update to a newer version of click to use this functionality.",
                 RuntimeWarning,
+                stacklevel=2,
             )
             return obj
 
         return decorator_with_warning
 
     def decorator(obj: FC) -> FC:
         extra: Dict[str, Any] = {}
@@ -206,11 +215,9 @@
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 def pass_context(f: Callable[Concatenate[RichContext, P], R]) -> Callable[P, R]:
     # flake8: noqa: D400,D401
-    """Marks a callback as wanting to receive the current context
-    object as first argument.
-    """
+    """Marks a callback as wanting to receive the current context object as first argument."""
     return click_pass_context(f)  # type: ignore[arg-type]
```

### Comparing `rich-click-1.7.4/src/rich_click/rich_click.py` & `rich-click-1.8.0.dev0/src/rich_click/rich_help_rendering.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,224 +1,112 @@
 import inspect
 import re
-from typing import Dict, Iterable, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, Union
 
 import click
-import rich.columns
-import rich.markdown
-import rich.text
 
 # Due to how rich_click.cli.patch() works, it is safer to import Command types directly
 # rather than use the click module e.g. click.Command
 from click import Command, Group
 from rich import box
 from rich.align import Align
 from rich.columns import Columns
+from rich.console import RenderableType
 from rich.emoji import Emoji
 from rich.highlighter import RegexHighlighter
 from rich.markdown import Markdown
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.style import StyleType
 from rich.table import Table
 from rich.text import Text
-from typing_extensions import Literal
 
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X, CLICK_IS_BEFORE_VERSION_9X, CLICK_IS_VERSION_80
-from rich_click.rich_help_configuration import (
-    force_terminal_default,
-    OptionHighlighter,
-    RichHelpConfiguration,
-    terminal_width_default,
-)
 from rich_click.rich_help_formatter import RichHelpFormatter
+from rich_click.utils import OptionGroupDict
+
 
 # Support rich <= 10.6.0
 try:
     from rich.console import group
 except ImportError:
     from rich.console import render_group as group  # type: ignore[attr-defined,no-redef]
 
 
 if CLICK_IS_BEFORE_VERSION_9X:
-    from click import MultiCommand
+    # We need to load from here to help with patching.
+    from rich_click.rich_command import MultiCommand  # type: ignore[attr-defined]
 else:
     MultiCommand = Group  # type: ignore[misc,assignment]
 
 
-# Default styles
-STYLE_OPTION: rich.style.StyleType = "bold cyan"
-STYLE_ARGUMENT: rich.style.StyleType = "bold cyan"
-STYLE_COMMAND: rich.style.StyleType = "bold cyan"
-STYLE_SWITCH: rich.style.StyleType = "bold green"
-STYLE_METAVAR: rich.style.StyleType = "bold yellow"
-STYLE_METAVAR_APPEND: rich.style.StyleType = "dim yellow"
-STYLE_METAVAR_SEPARATOR: rich.style.StyleType = "dim"
-STYLE_HEADER_TEXT: rich.style.StyleType = ""
-STYLE_EPILOG_TEXT: rich.style.StyleType = ""
-STYLE_FOOTER_TEXT: rich.style.StyleType = ""
-STYLE_USAGE: rich.style.StyleType = "yellow"
-STYLE_USAGE_COMMAND: rich.style.StyleType = "bold"
-STYLE_DEPRECATED: rich.style.StyleType = "red"
-STYLE_HELPTEXT_FIRST_LINE: rich.style.StyleType = ""
-STYLE_HELPTEXT: rich.style.StyleType = "dim"
-STYLE_OPTION_HELP: rich.style.StyleType = ""
-STYLE_OPTION_DEFAULT: rich.style.StyleType = "dim"
-STYLE_OPTION_ENVVAR: rich.style.StyleType = "dim yellow"
-STYLE_REQUIRED_SHORT: rich.style.StyleType = "red"
-STYLE_REQUIRED_LONG: rich.style.StyleType = "dim red"
-STYLE_OPTIONS_PANEL_BORDER: rich.style.StyleType = "dim"
-ALIGN_OPTIONS_PANEL: rich.align.AlignMethod = "left"
-STYLE_OPTIONS_TABLE_SHOW_LINES: bool = False
-STYLE_OPTIONS_TABLE_LEADING: int = 0
-STYLE_OPTIONS_TABLE_PAD_EDGE: bool = False
-STYLE_OPTIONS_TABLE_PADDING: rich.padding.PaddingDimensions = (0, 1)
-STYLE_OPTIONS_TABLE_BOX: rich.style.StyleType = ""
-STYLE_OPTIONS_TABLE_ROW_STYLES: Optional[List[rich.style.StyleType]] = None
-STYLE_OPTIONS_TABLE_BORDER_STYLE: Optional[rich.style.StyleType] = None
-STYLE_COMMANDS_PANEL_BORDER: rich.style.StyleType = "dim"
-ALIGN_COMMANDS_PANEL: rich.align.AlignMethod = "left"
-STYLE_COMMANDS_TABLE_SHOW_LINES: bool = False
-STYLE_COMMANDS_TABLE_LEADING: int = 0
-STYLE_COMMANDS_TABLE_PAD_EDGE: bool = False
-STYLE_COMMANDS_TABLE_PADDING: rich.padding.PaddingDimensions = (0, 1)
-STYLE_COMMANDS_TABLE_BOX: rich.style.StyleType = ""
-STYLE_COMMANDS_TABLE_ROW_STYLES: Optional[List[rich.style.StyleType]] = None
-STYLE_COMMANDS_TABLE_BORDER_STYLE: Optional[rich.style.StyleType] = None
-STYLE_COMMANDS_TABLE_COLUMN_WIDTH_RATIO: Optional[Union[Tuple[None, None], Tuple[int, int]]] = (None, None)
-STYLE_ERRORS_PANEL_BORDER: rich.style.StyleType = "red"
-ALIGN_ERRORS_PANEL: rich.align.AlignMethod = "left"
-STYLE_ERRORS_SUGGESTION: rich.style.StyleType = "dim"
-STYLE_ERRORS_SUGGESTION_COMMAND: rich.style.StyleType = "blue"
-STYLE_ABORTED: rich.style.StyleType = "red"
-WIDTH: Optional[int] = terminal_width_default()
-MAX_WIDTH: Optional[int] = terminal_width_default()
-COLOR_SYSTEM: Optional[
-    Literal["auto", "standard", "256", "truecolor", "windows"]
-] = "auto"  # Set to None to disable colors
-FORCE_TERMINAL: Optional[bool] = force_terminal_default()
-
-# Fixed strings
-HEADER_TEXT: Optional[str] = None
-FOOTER_TEXT: Optional[str] = None
-DEPRECATED_STRING: str = "(Deprecated) "
-DEFAULT_STRING: str = "[default: {}]"
-ENVVAR_STRING: str = "[env var: {}]"
-REQUIRED_SHORT_STRING: str = "*"
-REQUIRED_LONG_STRING: str = "[required]"
-RANGE_STRING: str = " [{}]"
-APPEND_METAVARS_HELP_STRING: str = "({})"
-ARGUMENTS_PANEL_TITLE: str = "Arguments"
-OPTIONS_PANEL_TITLE: str = "Options"
-COMMANDS_PANEL_TITLE: str = "Commands"
-ERRORS_PANEL_TITLE: str = "Error"
-ERRORS_SUGGESTION: Optional[str] = None  # Default: Try 'cmd -h' for help. Set to False to disable.
-ERRORS_EPILOGUE: Optional[str] = None
-ABORTED_TEXT: str = "Aborted."
-
-# Behaviours
-SHOW_ARGUMENTS: bool = False  # Show positional arguments
-SHOW_METAVARS_COLUMN: bool = True  # Show a column with the option metavar (eg. INTEGER)
-APPEND_METAVARS_HELP: bool = False  # Append metavar (eg. [TEXT]) after the help text
-GROUP_ARGUMENTS_OPTIONS: bool = False  # Show arguments with options instead of in own panel
-OPTION_ENVVAR_FIRST: bool = False  # Show env vars before option help text instead of avert
-USE_MARKDOWN: bool = False  # Parse help strings as markdown
-USE_MARKDOWN_EMOJI: bool = True  # Parse emoji codes in markdown :smile:
-USE_RICH_MARKUP: bool = False  # Parse help strings for rich markup (eg. [red]my text[/])
-# Define sorted groups of panels to display subcommands
-COMMAND_GROUPS: Dict[str, List[Dict[str, Union[str, List[str]]]]] = {}
-# Define sorted groups of panels to display options and arguments
-OPTION_GROUPS: Dict[str, List[Dict[str, Union[str, List[str], Dict[str, List[str]]]]]] = {}
-USE_CLICK_SHORT_HELP: bool = False  # Use click's default function to truncate help text
-
-highlighter: rich.highlighter.Highlighter = OptionHighlighter()
-_formatter: Optional[RichHelpFormatter] = None
-
-
-def _get_rich_formatter(formatter: Optional[click.HelpFormatter] = None) -> RichHelpFormatter:
-    """Get Rich Help Formatter.
-
-    Resolves the rich help formatter from the following:
-        - formatter, if exists and is a `RichHelpFormatter` object
-        - cached, module-level formatter
-        - active click Context, that is cached as module-level attr
-        - module-level settings (default)
-
-    Args:
-        formatter: A possible Rich help formatter
+def _make_rich_rext(text: str, style: StyleType, formatter: RichHelpFormatter) -> Union[Markdown, Text]:
     """
-    if formatter and isinstance(formatter, RichHelpFormatter):
-        return formatter
-
-    global _formatter
-    if _formatter:
-        return _formatter
-    ctx = click.get_current_context(True)
-    if ctx:
-        formatter = ctx.make_formatter()
-        if isinstance(formatter, RichHelpFormatter):
-            _formatter = formatter
-            return _formatter
-
-    _formatter = RichHelpFormatter(config=get_module_help_configuration())
-    return _formatter
-
-
-def _make_rich_rext(
-    text: str, style: StyleType = "", formatter: Optional[RichHelpFormatter] = None
-) -> Union[rich.markdown.Markdown, Text]:
-    """Take a string, remove indentations, and return styled text.
-
+    Take a string, remove indentations, and return styled text.
     By default, return the text as a Rich Text with the request style.
     If config.use_rich_markup is True, also parse the text for Rich markup strings.
     If config.use_markdown is True, parse as Markdown.
-
     Only one of config.use_markdown or config.use_rich_markup can be True.
     If both are True, config.use_markdown takes precedence.
 
     Args:
-        text (str): Text to style
-        style (str): Rich style to apply
+    ----
+        text (str): Text to style.
+        style (StyleType): Rich style to apply.
+        formatter: formatter object.
 
     Returns:
+    -------
         MarkdownElement or Text: Styled text object
     """
-    formatter = _get_rich_formatter(formatter)
     config = formatter.config
     # Remove indentations from input text
     text = inspect.cleandoc(text)
-    if config.use_markdown:
+    if config.text_markup == "markdown":
+        use_markdown = True
+        use_rich = False
+    elif config.text_markup == "rich":
+        use_markdown = False
+        use_rich = True
+    else:
+        use_markdown = config.use_markdown
+        use_rich = config.use_rich_markup
+
+    # TODO:
+    #  In a future major version release, decouple emojis and markdown.
+    #  Decoupling isn't something that is sensible without breaking the API.
+    if use_markdown:
         if config.use_markdown_emoji:
             text = Emoji.replace(text)
         return Markdown(text, style=style)
-    if config.use_rich_markup:
-        return config.highlighter(Text.from_markup(text, style=style))
+    elif use_rich:
+        return formatter.highlighter(Text.from_markup(text, style=style))
     else:
-        return config.highlighter(Text(text, style=style))
+        return formatter.highlighter(Text(text, style=style))
 
 
 @group()
-def _get_help_text(
-    obj: Union[Command, Group], formatter: Optional[RichHelpFormatter] = None
-) -> Iterable[Union[rich.markdown.Markdown, rich.text.Text]]:
-    """Build primary help text for a click command or group.
-
+def _get_help_text(obj: Union[Command, Group], formatter: RichHelpFormatter) -> Iterable[Union[Markdown, Text]]:
+    """
+    Build primary help text for a click command or group.
     Returns the prose help text for a command or group, rendered either as a
     Rich Text object or as Markdown.
     If the command is marked as depreciated, the depreciated string will be prepended.
 
     Args:
-        obj (click.Command or click.Group): Command or group to build help text for
+    ----
+        obj (click.Command or click.Group): Command or group to build help text for.
+        formatter: formatter object.
 
     Yields:
+    ------
         Text or Markdown: Multiple styled objects (depreciated, usage)
     """
     if TYPE_CHECKING:
         assert isinstance(obj.help, str)
-    formatter = _get_rich_formatter(formatter)
     config = formatter.config
     # Prepend deprecated status
     if obj.deprecated:
         yield Text(config.deprecated_string, style=config.style_deprecated)
 
     # Fetch and dedent the help text
     help_text = inspect.cleandoc(obj.help)
@@ -248,32 +136,34 @@
             # Join with double linebreaks if markdown
             remaining_lines = "\n\n".join(remaining_paragraphs)
 
         yield _make_rich_rext(remaining_lines, config.style_helptext, formatter)
 
 
 def _get_option_help(
-    param: Union[click.Argument, click.Option], ctx: click.Context, formatter: Optional[RichHelpFormatter] = None
-) -> rich.columns.Columns:
-    """Build primary help text for a click option or argument.
-
+    param: Union[click.Argument, click.Option], ctx: click.Context, formatter: RichHelpFormatter
+) -> Columns:
+    """
+    Build primary help text for a click option or argument.
     Returns the prose help text for an option or argument, rendered either
     as a Rich Text object or as Markdown.
     Additional elements are appended to show the default and required status if applicable.
 
     Args:
-        param (click.Argument or click.Option): Parameter to build help text for
-        ctx (click.Context): Click Context object
+    ----
+        param (click.Argument or click.Option): Parameter to build help text for.
+        ctx (click.Context): Click Context object.
+        formatter (RichHelpFormatter): formatter object.
 
     Returns:
+    -------
         Columns: A columns element with multiple styled objects (help, default, required)
     """
-    formatter = _get_rich_formatter(formatter)
     config = formatter.config
-    items: List[rich.console.RenderableType] = []
+    items: List[RenderableType] = []
 
     if TYPE_CHECKING:
         assert isinstance(param.name, str)
 
     # Get the environment variable first
     envvar = getattr(param, "envvar", None)
     # https://github.com/pallets/click/blob/0aec1168ac591e159baf6f61026d6ae322c53aaf/src/click/core.py#L2720-L2726
@@ -281,15 +171,15 @@
         if (
             getattr(param, "allow_from_autoenv", None)
             and getattr(ctx, "auto_envvar_prefix", None) is not None
             and param.name is not None
         ):
             envvar = f"{ctx.auto_envvar_prefix}_{param.name.upper()}"
     if envvar is not None:
-        envvar = ", ".join(envvar) if type(envvar) is list else envvar
+        envvar = ", ".join(envvar) if isinstance(envvar, list) else envvar
 
     # Environment variable config.before help text
     if getattr(param, "show_envvar", None) and config.option_envvar_first and envvar is not None:
         items.append(Text(config.envvar_string.format(envvar), style=config.style_option_envvar))
 
     # Main help text
     if getattr(param, "help", None):
@@ -369,158 +259,142 @@
         items.append(Text(config.required_long_string, style=config.style_required_long))
 
     # Use Columns - this allows us to group different renderable types
     # (Text, Markdown) onto a single line.
     return Columns(items)
 
 
-def _make_command_help(
-    help_text: str, formatter: Optional[RichHelpFormatter] = None
-) -> Union[rich.text.Text, rich.markdown.Markdown]:
-    """Build cli help text for a click group command.
-
+def _make_command_help(help_text: str, formatter: RichHelpFormatter, is_deprecated: bool) -> Union[Text, Markdown]:
+    """
+    Build cli help text for a click group command.
     That is, when calling help on groups with multiple subcommands
     (not the main help text when calling the subcommand help).
-
     Returns the first paragraph of help text for a command, rendered either as a
     Rich Text object or as Markdown.
     Ignores single newlines as paragraph markers, looks for double only.
 
     Args:
+    ----
         help_text (str): Help text
+        formatter: formatter object
+        is_deprecated (bool): Object marked by user as deprecated.
 
     Returns:
+    -------
         Text or Markdown: Styled object
     """
-    formatter = _get_rich_formatter(formatter)
-    config = formatter.config
     paragraphs = inspect.cleandoc(help_text).split("\n\n")
     # Remove single linebreaks
-    if not config.use_markdown and not paragraphs[0].startswith("\b"):
+    if not formatter.config.use_markdown and not paragraphs[0].startswith("\b"):
         paragraphs[0] = paragraphs[0].replace("\n", " ")
     elif paragraphs[0].startswith("\b"):
         paragraphs[0] = paragraphs[0].replace("\b\n", "")
+    help_text = paragraphs[0].strip()
+    if is_deprecated:
+        # TODO: Format the deprecation text.
+        help_text = f"{formatter.config.deprecated_string}{help_text}"
+    renderable = _make_rich_rext(help_text, formatter.config.style_option_help, formatter)
+    return renderable
 
-    return _make_rich_rext(paragraphs[0].strip(), config.style_option_help, formatter)
 
+def get_rich_usage(formatter: RichHelpFormatter, prog: str, args: str = "", prefix: Optional[str] = None) -> None:
+    """Richly render usage text."""
+    if prefix is None:
+        prefix = "Usage:"
 
-def get_rich_usage(
-    obj: Union[Command, Group],
-    ctx: click.Context,
-    formatter: click.HelpFormatter,
-) -> None:
-    """Get usage text for a command."""
-    formatter = _get_rich_formatter(formatter)
     config = formatter.config
-    console = formatter.console
+
+    # Header text if we have it
+    if config.header_text:
+        formatter.write(
+            Padding(
+                _make_rich_rext(config.header_text, config.style_header_text, formatter),
+                (1, 1, 0, 1),
+            ),
+        )
 
     # Highlighter for options and arguments
     class UsageHighlighter(RegexHighlighter):
         highlights = [
             r"(?P<argument>\w+)",
         ]
 
     usage_highlighter = UsageHighlighter()
 
     # Print usage
-    console.print(
+    formatter.write(
         Padding(
             Columns(
                 (
-                    Text("Usage:", style=config.style_usage),
-                    Text(ctx.command_path, style=config.style_usage_command),
-                    usage_highlighter(" ".join(obj.collect_usage_pieces(ctx))),
+                    Text(prefix, style=config.style_usage),
+                    Text(prog, style=config.style_usage_command),
+                    usage_highlighter(args),
                 )
             ),
             1,
         ),
     )
 
 
-def rich_format_help(
-    obj: Command,
-    ctx: click.Context,
-    formatter: click.HelpFormatter,
-) -> None:
-    """Print nicely formatted help text using rich.
-
-    Based on original code from rich-cli, by @willmcgugan.
-    https://github.com/Textualize/rich-cli/blob/8a2767c7a340715fc6fbf4930ace717b9b2fc5e5/src/rich_cli/__main__.py#L162-L236
-
-    Replacement for the click function format_help().
-    Takes a command or group and builds the help text output.
-
-    Args:
-        obj (click.Command or click.Group): Command or group to build help text for
-        ctx (click.Context): Click Context object
-        formatter (click.HelpFormatter): Click HelpFormatter object
-    """
-    formatter = _get_rich_formatter(formatter)
-    config = formatter.config
-    console = formatter.console
-    highlighter = formatter.config.highlighter
-
-    # Header text if we have it
-    if config.header_text:
-        console.print(
-            Padding(
-                _make_rich_rext(config.header_text, config.style_header_text, formatter),
-                (1, 1, 0, 1),
-            ),
-        )
-
-    # Print usage
-    get_rich_usage(obj, ctx, formatter)
-
+def get_rich_help_text(self: Command, ctx: click.Context, formatter: RichHelpFormatter) -> None:
+    """Write rich help text to the formatter if it exists."""
     # Print command / group help if we have some
-    if obj.help:
+    if self.help:
         # Print with some padding
-        console.print(
+        formatter.write(
             Padding(
-                Align(_get_help_text(obj, formatter), pad=False),
+                Align(_get_help_text(self, formatter), pad=False),
                 (0, 1, 1, 1),
             )
         )
 
+
+def get_rich_options(
+    obj: Command,
+    ctx: click.Context,
+    formatter: RichHelpFormatter,
+) -> None:
+    """Richly render a click Command's options."""
     # Look through config.option_groups for this command
     # stick anything unmatched into a default group at the end
-    option_groups = config.option_groups.get(ctx.command_path, []).copy()
+    option_groups = formatter.config.option_groups.get(ctx.command_path, []).copy()
     option_groups.append({"options": []})
     argument_group_options = []
 
     for param in obj.get_params(ctx):
         # Skip positional arguments - they don't have opts or helptext and are covered in usage
         # See https://click.palletsprojects.com/en/8.0.x/documentation/#documenting-arguments
-        if isinstance(param, click.core.Argument) and not config.show_arguments:
+        if isinstance(param, click.core.Argument) and not formatter.config.show_arguments:
             continue
 
         # Skip if option is hidden
         if getattr(param, "hidden", False):
             continue
 
         # Already mentioned in a config option group
         for option_group in option_groups:
             if any([opt in option_group.get("options", []) for opt in param.opts]):
                 break
 
         # No break, no mention - add to the default group
         else:
-            if isinstance(param, click.core.Argument) and not config.group_arguments_options:
+            if isinstance(param, click.core.Argument) and not formatter.config.group_arguments_options:
                 argument_group_options.append(param.opts[0])
             else:
-                list_of_option_groups: List[str] = option_groups[-1]["options"]  # type: ignore[assignment]
+                list_of_option_groups = option_groups[-1]["options"]
                 list_of_option_groups.append(param.opts[0])
 
     # If we're not grouping arguments and we got some, prepend before default options
     if len(argument_group_options) > 0:
-        extra_option_group = {"name": config.arguments_panel_title, "options": argument_group_options}
+        extra_option_group: OptionGroupDict = {
+            "name": formatter.config.arguments_panel_title,
+            "options": argument_group_options,
+        }
         option_groups.insert(len(option_groups) - 1, extra_option_group)
 
-    # print("!", option_groups)
-
     # Print each option group panel
     for option_group in option_groups:
         options_rows = []
         for opt in option_group.get("options", []):
             # Get the param
             for param in obj.get_params(ctx):
                 if any([opt in param.opts]):
@@ -543,15 +417,15 @@
                     opt_long_strs.append(opt_str.upper())
                 elif "--" in opt:
                     opt_long_strs.append(opt_str)
                 else:
                     opt_short_strs.append(opt_str)
 
             # Column for a metavar, if we have one
-            metavar = Text(style=config.style_metavar, overflow="fold")
+            metavar = Text(style=formatter.config.style_metavar, overflow="fold")
             metavar_str = param.make_metavar()
 
             if TYPE_CHECKING:
                 assert isinstance(param.name, str)
                 assert isinstance(param, click.Option)
 
             # Do it ourselves if this is a positional argument
@@ -569,205 +443,222 @@
             try:
                 # skip count with default range type
                 if isinstance(param.type, click.types._NumberRangeBase) and not (
                     param.count and param.type.min == 0 and param.type.max is None
                 ):
                     range_str = param.type._describe_range()
                     if range_str:
-                        metavar.append(config.range_string.format(range_str))
+                        metavar.append(formatter.config.range_string.format(range_str))
             except AttributeError:
                 # click.types._NumberRangeBase is only in Click 8x onwards
                 pass
 
             # Required asterisk
             required: Union[Text, str] = ""
             if param.required:
-                required = Text(config.required_short_string, style=config.style_required_short)
+                required = Text(formatter.config.required_short_string, style=formatter.config.style_required_short)
 
             # Highlighter to make [ | ] and <> dim
             class MetavarHighlighter(RegexHighlighter):
                 highlights = [
                     r"^(?P<metavar_sep>(\[|<))",
                     r"(?P<metavar_sep>\|)",
                     r"(?P<metavar_sep>(\]|>)$)",
                 ]
 
             metavar_highlighter = MetavarHighlighter()
 
             rows = [
                 required,
-                highlighter(highlighter(",".join(opt_long_strs))),
-                highlighter(highlighter(",".join(opt_short_strs))),
+                formatter.highlighter(formatter.highlighter(",".join(opt_long_strs))),
+                formatter.highlighter(formatter.highlighter(",".join(opt_short_strs))),
                 metavar_highlighter(metavar),
                 _get_option_help(param, ctx, formatter),
             ]
 
             # Remove metavar if specified in config
-            if not config.show_metavars_column:
+            if not formatter.config.show_metavars_column:
                 rows.pop(3)
 
             options_rows.append(rows)
 
         if len(options_rows) > 0:
             t_styles = {
-                "show_lines": config.style_options_table_show_lines,
-                "leading": config.style_options_table_leading,
-                "box": config.style_options_table_box,
-                "border_style": config.style_options_table_border_style,
-                "row_styles": config.style_options_table_row_styles,
-                "pad_edge": config.style_options_table_pad_edge,
-                "padding": config.style_options_table_padding,
+                "show_lines": formatter.config.style_options_table_show_lines,
+                "leading": formatter.config.style_options_table_leading,
+                "box": formatter.config.style_options_table_box,
+                "border_style": formatter.config.style_options_table_border_style,
+                "row_styles": formatter.config.style_options_table_row_styles,
+                "pad_edge": formatter.config.style_options_table_pad_edge,
+                "padding": formatter.config.style_options_table_padding,
             }
-            t_styles.update(option_group.get("table_styles", {}))  # type: ignore[arg-type]
+            t_styles.update(option_group.get("table_styles", {}))
             box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
 
             options_table = Table(
                 highlight=True,
                 show_header=False,
                 expand=True,
                 box=box_style,
                 **t_styles,  # type: ignore[arg-type]
             )
             # Strip the required column if none are required
             if all([x[0] == "" for x in options_rows]):
                 options_rows = [x[1:] for x in options_rows]
             for row in options_rows:
                 options_table.add_row(*row)
-            console.print(
+            formatter.write(
                 Panel(
                     options_table,
-                    border_style=config.style_options_panel_border,
-                    title=option_group.get("name", config.options_panel_title),
-                    title_align=config.align_options_panel,
+                    border_style=formatter.config.style_options_panel_border,
+                    title=option_group.get("name", formatter.config.options_panel_title),
+                    title_align=formatter.config.align_options_panel,
                 )
             )
 
-    #
-    # Groups only:
-    # List click command groups
-    #
-
-    if isinstance(obj, MultiCommand):
-        # Look through COMMAND_GROUPS for this command
-        # stick anything unmatched into a default group at the end
-        cmd_groups = config.command_groups.get(ctx.command_path, []).copy()
-        cmd_groups.append({"commands": []})
-        for command in obj.list_commands(ctx):
-            for cmd_group in cmd_groups:
-                if command in cmd_group.get("commands", []):
-                    break
-            else:
-                commands: List[str] = cmd_groups[-1]["commands"]  # type: ignore[assignment]
-                commands.append(command)
 
-        # Print each command group panel
+def get_rich_commands(
+    obj: MultiCommand,
+    ctx: click.Context,
+    formatter: RichHelpFormatter,
+) -> None:
+    """Richly render a click Command's options."""
+    # Look through config.option_groups for this command
+    # stick anything unmatched into a default group at the end
+
+    # Look through COMMAND_GROUPS for this command
+    # stick anything unmatched into a default group at the end
+    cmd_groups = formatter.config.command_groups.get(ctx.command_path, []).copy()
+    cmd_groups.append({"commands": []})
+    for command in obj.list_commands(ctx):
         for cmd_group in cmd_groups:
-            t_styles = {
-                "show_lines": config.style_commands_table_show_lines,
-                "leading": config.style_commands_table_leading,
-                "box": config.style_commands_table_box,
-                "border_style": config.style_commands_table_border_style,
-                "row_styles": config.style_commands_table_row_styles,
-                "pad_edge": config.style_commands_table_pad_edge,
-                "padding": config.style_commands_table_padding,
-            }
-            t_styles.update(cmd_group.get("table_styles", {}))  # type: ignore[arg-type]
-            box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
+            if command in cmd_group.get("commands", []):
+                break
+        else:
+            commands = cmd_groups[-1]["commands"]
+            commands.append(command)
 
-            commands_table = Table(
-                highlight=False,
-                show_header=False,
-                expand=True,
-                box=box_style,
-                **t_styles,  # type: ignore[arg-type]
-            )
-            # Define formatting in first column, as commands don't match highlighter regex
-            # and set column ratio for first and second column, if a ratio has been set
-            if config.style_commands_table_column_width_ratio is None:
-                table_column_width_ratio: Union[Tuple[None, None], Tuple[int, int]] = (None, None)
-            else:
-                table_column_width_ratio = config.style_commands_table_column_width_ratio
+    # Print each command group panel
+    for cmd_group in cmd_groups:
+        t_styles = {
+            "show_lines": formatter.config.style_commands_table_show_lines,
+            "leading": formatter.config.style_commands_table_leading,
+            "box": formatter.config.style_commands_table_box,
+            "border_style": formatter.config.style_commands_table_border_style,
+            "row_styles": formatter.config.style_commands_table_row_styles,
+            "pad_edge": formatter.config.style_commands_table_pad_edge,
+            "padding": formatter.config.style_commands_table_padding,
+        }
+        t_styles.update(cmd_group.get("table_styles", {}))
+        box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore[arg-type]
+
+        commands_table = Table(
+            highlight=False,
+            show_header=False,
+            expand=True,
+            box=box_style,
+            **t_styles,  # type: ignore[arg-type]
+        )
+        # Define formatting in first column, as commands don't match highlighter regex
+        # and set column ratio for first and second column, if a ratio has been set
+        if formatter.config.style_commands_table_column_width_ratio is None:
+            table_column_width_ratio: Union[Tuple[None, None], Tuple[int, int]] = (None, None)
+        else:
+            table_column_width_ratio = formatter.config.style_commands_table_column_width_ratio
 
-            commands_table.add_column(style=config.style_command, no_wrap=True, ratio=table_column_width_ratio[0])
-            commands_table.add_column(
-                no_wrap=False,
-                ratio=table_column_width_ratio[1],
-            )
-            for command in cmd_group.get("commands", []):
-                # Skip if command does not exist
-                if command not in obj.list_commands(ctx):
-                    continue
-                cmd = obj.get_command(ctx, command)
-                if TYPE_CHECKING:
-                    assert cmd is not None
-                if cmd.hidden:
-                    continue
-                # Use the truncated short text as with vanilla text if requested
-                if config.use_click_short_help:
-                    helptext = cmd.get_short_help_str()
-                else:
-                    # Use short_help function argument if used, or the full help
-                    helptext = cmd.short_help or cmd.help or ""
-                commands_table.add_row(command, _make_command_help(helptext, formatter))
-            if commands_table.row_count > 0:
-                console.print(
-                    Panel(
-                        commands_table,
-                        border_style=config.style_commands_panel_border,
-                        title=cmd_group.get("name", config.commands_panel_title),
-                        title_align=config.align_commands_panel,
-                    )
+        commands_table.add_column(style=formatter.config.style_command, no_wrap=True, ratio=table_column_width_ratio[0])
+        commands_table.add_column(
+            no_wrap=False,
+            ratio=table_column_width_ratio[1],
+        )
+        for command in cmd_group.get("commands", []):
+            # Skip if command does not exist
+            if command not in obj.list_commands(ctx):
+                continue
+            cmd = obj.get_command(ctx, command)
+            if TYPE_CHECKING:
+                assert cmd is not None
+            if cmd.hidden:
+                continue
+            # Use the truncated short text as with vanilla text if requested
+            if formatter.config.use_click_short_help:
+                helptext = cmd.get_short_help_str()
+            else:
+                # Use short_help function argument if used, or the full help
+                helptext = cmd.short_help or cmd.help or ""
+            commands_table.add_row(command, _make_command_help(helptext, formatter, is_deprecated=cmd.deprecated))
+        if commands_table.row_count > 0:
+            formatter.write(
+                Panel(
+                    commands_table,
+                    border_style=formatter.config.style_commands_panel_border,
+                    title=cmd_group.get("name", formatter.config.commands_panel_title),
+                    title_align=formatter.config.align_commands_panel,
                 )
+            )
 
-    # Epilogue if we have it
-    if isinstance(obj, Command) and obj.epilog:
+
+def get_rich_epilog(
+    self: Command,
+    ctx: click.Context,
+    formatter: RichHelpFormatter,
+) -> None:
+    """Richly render a click Command's epilog if it exists."""
+    if self.epilog:
         # Remove single linebreaks, replace double with single
-        lines = obj.epilog.split("\n\n")
-        epilogue = "\n".join([x.replace("\n", " ").strip() for x in lines])
-        console.print(Padding(Align(_make_rich_rext(epilogue, config.style_epilog_text, formatter), pad=False), 1))
+        lines = self.epilog.split("\n\n")
+        epilog = "\n".join([x.replace("\n", " ").strip() for x in lines])
+        formatter.write(
+            Padding(Align(_make_rich_rext(epilog, formatter.config.style_epilog_text, formatter), pad=False), 1)
+        )
 
     # Footer text if we have it
-    if config.footer_text:
-        console.print(Padding(_make_rich_rext(config.footer_text, config.style_footer_text, formatter), (1, 1, 0, 1)))
+    if formatter.config.footer_text:
+        formatter.write(
+            Padding(
+                _make_rich_rext(formatter.config.footer_text, formatter.config.style_footer_text, formatter),
+                (1, 1, 0, 1),
+            )
+        )
 
 
-def rich_format_error(self: click.ClickException, formatter: Optional[RichHelpFormatter] = None) -> None:
-    """Print richly formatted click errors.
+def rich_format_error(self: click.ClickException, formatter: RichHelpFormatter) -> None:
+    """
+    Print richly formatted click errors.
 
     Called by custom exception handler to print richly formatted click errors.
     Mimics original click.ClickException.echo() function but with rich formatting.
 
     Args:
-        click.ClickException: Click exception to format.
+    ----
+        self (click.ClickException): Click exception to format.
+        formatter: formatter object.
     """
-    formatter = _get_rich_formatter(formatter)
-    console = formatter.console
     config = formatter.config
-    highlighter = formatter.config.highlighter
     # Print usage
     if getattr(self, "ctx", None) is not None:
         if TYPE_CHECKING:
             assert hasattr(self, "ctx")
-        get_rich_usage(self.ctx.command, self.ctx, formatter)
+        self.ctx.get_usage()
     if config.errors_suggestion:
-        console.print(
+        formatter.write(
             Padding(
                 config.errors_suggestion,
                 (0, 1, 0, 1),
             ),
             style=config.style_errors_suggestion,
         )
     elif (
         config.errors_suggestion is None
         and getattr(self, "ctx", None) is not None
         and self.ctx.command.get_help_option(self.ctx) is not None  # type: ignore[attr-defined]
     ):
         cmd_path = self.ctx.command_path  # type: ignore[attr-defined]
         help_option = self.ctx.help_option_names[0]  # type: ignore[attr-defined]
-        console.print(
+        formatter.write(
             Padding(
                 Columns(
                     (
                         Text("Try"),
                         Text(f"'{cmd_path} {help_option}'", style=config.style_errors_suggestion_command),
                         Text("for help"),
                     )
@@ -778,116 +669,25 @@
         )
 
     # A major Python library using click (dbt-core) has its own exception
     # logic that subclasses ClickException, but does not use the message
     # attribute. Checking for the 'message' attribute works to make the
     # rich-click CLI compatible.
     if hasattr(self, "message"):
-        console.print(
+        formatter.write(
             Padding(
                 Panel(
-                    highlighter(self.format_message()),
+                    formatter.highlighter(self.format_message()),
                     border_style=config.style_errors_panel_border,
                     title=config.errors_panel_title,
                     title_align=config.align_errors_panel,
                 ),
                 (0, 0, 1, 0),
             )
         )
     if config.errors_epilogue:
-        console.print(Padding(config.errors_epilogue, (0, 1, 1, 1)))
+        formatter.write(Padding(config.errors_epilogue, (0, 1, 1, 1)))
 
 
-def rich_abort_error(formatter: Optional[RichHelpFormatter] = None) -> None:
+def rich_abort_error(formatter: RichHelpFormatter) -> None:
     """Print richly formatted abort error."""
-    formatter = _get_rich_formatter(formatter)
-    config = formatter.config
-    formatter.console.print(config.aborted_text, style=config.style_aborted)
-
-
-module_config: Optional[RichHelpConfiguration] = None
-
-
-def get_module_help_configuration() -> RichHelpConfiguration:
-    """Get Module-level help configuration resolved into a `RichHelpConfiguration` instance."""
-    global module_config
-    if module_config:
-        return module_config
-    module_config = RichHelpConfiguration(
-        STYLE_OPTION,
-        STYLE_ARGUMENT,
-        STYLE_COMMAND,
-        STYLE_SWITCH,
-        STYLE_METAVAR,
-        STYLE_METAVAR_APPEND,
-        STYLE_METAVAR_SEPARATOR,
-        STYLE_HEADER_TEXT,
-        STYLE_EPILOG_TEXT,
-        STYLE_FOOTER_TEXT,
-        STYLE_USAGE,
-        STYLE_USAGE_COMMAND,
-        STYLE_DEPRECATED,
-        STYLE_HELPTEXT_FIRST_LINE,
-        STYLE_HELPTEXT,
-        STYLE_OPTION_HELP,
-        STYLE_OPTION_DEFAULT,
-        STYLE_OPTION_ENVVAR,
-        STYLE_REQUIRED_SHORT,
-        STYLE_REQUIRED_LONG,
-        STYLE_OPTIONS_PANEL_BORDER,
-        ALIGN_OPTIONS_PANEL,
-        STYLE_OPTIONS_TABLE_SHOW_LINES,
-        STYLE_OPTIONS_TABLE_LEADING,
-        STYLE_OPTIONS_TABLE_PAD_EDGE,
-        STYLE_OPTIONS_TABLE_PADDING,
-        STYLE_OPTIONS_TABLE_BOX,
-        STYLE_OPTIONS_TABLE_ROW_STYLES,
-        STYLE_OPTIONS_TABLE_BORDER_STYLE,
-        STYLE_COMMANDS_PANEL_BORDER,
-        ALIGN_COMMANDS_PANEL,
-        STYLE_COMMANDS_TABLE_SHOW_LINES,
-        STYLE_COMMANDS_TABLE_LEADING,
-        STYLE_COMMANDS_TABLE_PAD_EDGE,
-        STYLE_COMMANDS_TABLE_PADDING,
-        STYLE_COMMANDS_TABLE_BOX,
-        STYLE_COMMANDS_TABLE_ROW_STYLES,
-        STYLE_COMMANDS_TABLE_BORDER_STYLE,
-        STYLE_COMMANDS_TABLE_COLUMN_WIDTH_RATIO,
-        STYLE_ERRORS_PANEL_BORDER,
-        ALIGN_ERRORS_PANEL,
-        STYLE_ERRORS_SUGGESTION,
-        STYLE_ERRORS_SUGGESTION_COMMAND,
-        STYLE_ABORTED,
-        WIDTH,
-        MAX_WIDTH,
-        COLOR_SYSTEM,
-        FORCE_TERMINAL,
-        HEADER_TEXT,
-        FOOTER_TEXT,
-        DEPRECATED_STRING,
-        DEFAULT_STRING,
-        ENVVAR_STRING,
-        REQUIRED_SHORT_STRING,
-        REQUIRED_LONG_STRING,
-        RANGE_STRING,
-        APPEND_METAVARS_HELP_STRING,
-        ARGUMENTS_PANEL_TITLE,
-        OPTIONS_PANEL_TITLE,
-        COMMANDS_PANEL_TITLE,
-        ERRORS_PANEL_TITLE,
-        ERRORS_SUGGESTION,
-        ERRORS_EPILOGUE,
-        ABORTED_TEXT,
-        SHOW_ARGUMENTS,
-        SHOW_METAVARS_COLUMN,
-        APPEND_METAVARS_HELP,
-        GROUP_ARGUMENTS_OPTIONS,
-        OPTION_ENVVAR_FIRST,
-        USE_MARKDOWN,
-        USE_MARKDOWN_EMOJI,
-        USE_RICH_MARKUP,
-        COMMAND_GROUPS,
-        OPTION_GROUPS,
-        USE_CLICK_SHORT_HELP,
-        highlighter,
-    )
-    return module_config
+    formatter.write(formatter.config.aborted_text, style=formatter.config.style_aborted)
```

### Comparing `rich-click-1.7.4/src/rich_click/rich_help_formatter.py` & `rich-click-1.8.0.dev0/src/rich_click/rich_context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,95 @@
-from typing import Any, IO, Optional
+from typing import TYPE_CHECKING, Any, Mapping, Optional, Type, Union
 
 import click
-import rich
-import rich.highlighter
-import rich.markdown
-import rich.padding
-import rich.text
-import rich.theme
-from rich.console import Console
+from typing_extensions import Literal, NoReturn
 
 from rich_click.rich_help_configuration import RichHelpConfiguration
+from rich_click.rich_help_formatter import RichHelpFormatter
 
 
-def create_console(config: RichHelpConfiguration, file: Optional[IO[str]] = None) -> Console:
-    """Create a Rich Console configured from Rich Help Configuration.
+if TYPE_CHECKING:
+    from types import TracebackType
 
-    Args:
-        config: Rich Help Configuration instance
-        file: Optional IO stream to write Rich Console output
-            Defaults to None.
-    """
-    console = Console(
-        theme=rich.theme.Theme(
-            {
-                "option": config.style_option,
-                "command": config.style_command,
-                "argument": config.style_argument,
-                "switch": config.style_switch,
-                "metavar": config.style_metavar,
-                "metavar_sep": config.style_metavar_separator,
-                "usage": config.style_usage,
-            }
-        ),
-        highlighter=config.highlighter,
-        color_system=config.color_system,
-        force_terminal=config.force_terminal,
-        file=file,
-        width=config.width,
-        legacy_windows=config.legacy_windows,
-    )
-    if isinstance(config.max_width, int):
-        console.width = min(config.max_width, console.size.width)
-    return console
-
-
-def get_module_config() -> RichHelpConfiguration:
-    """Get the module-level help configuration.
-
-    A function-level import is used to avoid a circular dependency
-    between the formatter and formatter operations.
-    """
-    from rich_click.rich_click import get_module_help_configuration
-
-    return get_module_help_configuration()
-
-
-class RichHelpFormatter(click.HelpFormatter):
-    """Rich Help Formatter.
-
-    This class is a container for the help configuration and Rich Console that
-    are used internally by the help and error printing methods.
-    """
+    from rich.console import Console
+
+
+class RichContext(click.Context):
+    """Click Context class endowed with Rich superpowers."""
+
+    formatter_class: Type[RichHelpFormatter] = RichHelpFormatter
+    console: Optional["Console"] = None
+    export_console_as: Literal[None, "html", "svg"] = None
 
     def __init__(
         self,
-        indent_increment: int = 2,
-        width: Optional[int] = None,
-        max_width: Optional[int] = None,
         *args: Any,
-        config: Optional[RichHelpConfiguration] = None,
+        rich_console: Optional["Console"] = None,
+        rich_help_config: Optional[Union[Mapping[str, Any], RichHelpConfiguration]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Rich Help Formatter.
+        """
+        Create Rich Context instance.
 
         Args:
-            config: Configuration.
-                Defaults to None.
+        ----
+            *args: Args that get passed to click.Context.
+            rich_console: Rich Console. Defaults to None.
+            rich_help_config: Rich help configuration.  Defaults to None.
+            **kwargs: Kwargs that get passed to click.Context.
         """
-        if config is not None:
-            # Rich config overrides width and max width if set.
-            width = config.width or width
-            max_width = config.max_width or max_width
-        super().__init__(indent_increment, width, max_width, *args, **kwargs)
-        self._config = config or get_module_config()
-        self._console = create_console(self._config)
-
-    @property
-    def config(self) -> RichHelpConfiguration:
-        """Rich Help Configuration."""
-        return self._config
-
-    @property
-    def console(self) -> Console:
-        """Rich Console created from the help configuration.
+        super().__init__(*args, **kwargs)
+        parent: Optional[RichContext] = kwargs.pop("parent", None)
 
-        This console is meant only for use with the formatter and should
-        not be created directly
-        """
-        return self._console
+        if rich_console is None and hasattr(parent, "console"):
+            rich_console = parent.console  # type: ignore[union-attr]
+
+        if rich_console is not None:
+            self.console = rich_console
 
-    def write(self, string: str) -> None:
-        return self._console.print(string)
+        if rich_help_config is None:
+            if hasattr(parent, "help_config"):
+                self.help_config = parent.help_config  # type: ignore[has-type,union-attr]
+            else:
+                self.help_config = RichHelpConfiguration.load_from_globals()
+        elif isinstance(rich_help_config, Mapping):
+            if hasattr(parent, "help_config"):
+                if TYPE_CHECKING:
+                    assert parent is not None
+                kw = parent.help_config.__dict__.copy()
+                kw.update(rich_help_config)
+                self.help_config = RichHelpConfiguration(**kw)
+            else:
+                self.help_config = RichHelpConfiguration.load_from_globals(**rich_help_config)
+        else:
+            self.help_config = rich_help_config
+
+    def make_formatter(self) -> RichHelpFormatter:
+        """Create the Rich Help Formatter."""
+        formatter = self.formatter_class(
+            width=self.terminal_width,
+            max_width=self.max_content_width,
+            config=self.help_config,
+            console=self.console,
+        )
+        return formatter
+
+    if TYPE_CHECKING:
+
+        def __enter__(self) -> "RichContext":
+            return super().__enter__()  # type: ignore[return-value]
+
+        def __exit__(
+            self,
+            exc_type: Optional[Type[BaseException]],
+            exc_value: Optional[BaseException],
+            tb: Optional[TracebackType],
+        ) -> None:
+            return super().__exit__(exc_type, exc_value, tb)
+
+    def exit(self, code: int = 0) -> NoReturn:
+        if self.console is not None and self.console.record:
+            if self.export_console_as == "html":
+                print(self.console.export_html(inline_styles=True, code_format="{code}"))
+            elif self.export_console_as == "svg":
+                print(self.console.export_svg())
+        super().exit(code)
```

### Comparing `rich-click-1.7.4/src/rich_click.egg-info/SOURCES.txt` & `rich-click-1.8.0.dev0/src/rich_click.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 src/rich_click/__init__.py
 src/rich_click/__main__.py
 src/rich_click/_compat_click.py
 src/rich_click/cli.py
 src/rich_click/decorators.py
+src/rich_click/patch.py
 src/rich_click/py.typed
 src/rich_click/rich_click.py
 src/rich_click/rich_command.py
 src/rich_click/rich_context.py
 src/rich_click/rich_group.py
 src/rich_click/rich_help_configuration.py
 src/rich_click/rich_help_formatter.py
+src/rich_click/rich_help_rendering.py
 src/rich_click/utils.py
 src/rich_click.egg-info/PKG-INFO
 src/rich_click.egg-info/SOURCES.txt
 src/rich_click.egg-info/dependency_links.txt
 src/rich_click.egg-info/entry_points.txt
 src/rich_click.egg-info/requires.txt
 src/rich_click.egg-info/top_level.txt
+tests/test_config.py
 tests/test_exit_code.py
-tests/test_help.py
+tests/test_help.py
+tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.7.4/tests/test_exit_code.py` & `rich-click-1.8.0.dev0/tests/test_exit_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+# ruff: noqa: D101,D103,D401
 import sys
 
 import click
 import pytest
 from click.testing import CliRunner
 
-from rich_click import command, group, pass_context, RichContext
+from rich_click import RichContext, command, group, pass_context
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X
 
+
 # Don't use the 'invoke' fixture because we want control over the standalone_mode kwarg.
 
 
 def test_command_exit_code_with_context() -> None:
     for expected_exit_code in range(10):
 
         @command("cli")
```

### Comparing `rich-click-1.7.4/tests/test_help.py` & `rich-click-1.8.0.dev0/tests/test_help.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,43 @@
+# ruff: noqa: D101,D103,D401
 from typing import Any, Callable, Optional, Type, Union
 
 import click
 import pytest
 from click import UsageError
+from click.testing import CliRunner
 from packaging import version
 from rich.console import Console
 
-from tests.conftest import AssertRichFormat, AssertStr, InvokeCli
-
 import rich_click.rich_click as rc
-from rich_click import command, group, pass_context, rich_config, RichContext, RichHelpConfiguration
+from rich_click import RichContext, RichHelpConfiguration, command, group, pass_context, rich_config
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X, CLICK_IS_VERSION_80
 from rich_click.rich_command import RichCommand, RichGroup
+from tests.conftest import AssertRichFormat, AssertStr
+
 
 try:
     from importlib import metadata  # type: ignore[import,unused-ignore]
 except ImportError:
     # Python < 3.8
-    import importlib_metadata as metadata  # type: ignore[no-redef,import-not-found]
+    import importlib_metadata as metadata  # type: ignore[no-redef,import-not-found,unused-ignore]
 
 
 rich_version = version.parse(metadata.version("rich"))
 click_version = version.parse(metadata.version("click"))
 
 
+@pytest.fixture(autouse=True)
+def default_config(initialize_rich_click: None) -> None:
+    # Default config settings from https://github.com/Textualize/rich/blob/master/tests/render.py
+    rc.WIDTH = 100
+    rc.COLOR_SYSTEM = None
+    rc.FORCE_TERMINAL = True
+
+
 @pytest.mark.parametrize(
     "cmd, args, error, rich_config",
     [
         pytest.param("arguments", "--help", None, None, id="test arguments"),
         pytest.param(
             "context_settings",
             "--help",
@@ -215,58 +225,58 @@
 class ClickGroupWithRichCommandClass(click.Group):
     command_class = RichCommand
     group_class = RichGroup
 
 
 if rich_version.major == 12:
     command_help_output = """
- Usage: cli [OPTIONS]                                       
+ Usage: cli [OPTIONS]
 
- Some help                                                  
- ╔════════════════════════════════════════════════════════╗ 
- ║                         Header                         ║ 
- ╚════════════════════════════════════════════════════════╝ 
+ Some help.
+ ╔════════════════════════════════════════════════════════╗
+ ║                         Header                         ║
+ ╚════════════════════════════════════════════════════════╝
 
 ╭─ Options ────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                  │
 ╰──────────────────────────────────────────────────────────╯
 """
     group_help_output = """
- Usage: cli [OPTIONS] COMMAND [ARGS]...                     
-                                                            
- Some help                                                  
- ╔════════════════════════════════════════════════════════╗ 
- ║                         Header                         ║ 
- ╚════════════════════════════════════════════════════════╝ 
-                                                            
+ Usage: cli [OPTIONS] COMMAND [ARGS]...
+
+ Some help.
+ ╔════════════════════════════════════════════════════════╗
+ ║                         Header                         ║
+ ╚════════════════════════════════════════════════════════╝
+
 ╭─ Options ────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                  │
 ╰──────────────────────────────────────────────────────────╯
 """
 else:
     command_help_output = """
- Usage: cli [OPTIONS]                                       
+ Usage: cli [OPTIONS]
 
- Some help                                                  
- ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓ 
- ┃                         Header                         ┃ 
- ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ 
+ Some help.
+ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+ ┃                         Header                         ┃
+ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
 
 ╭─ Options ────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                  │
 ╰──────────────────────────────────────────────────────────╯
 """
     group_help_output = """
- Usage: cli [OPTIONS] COMMAND [ARGS]...                     
-                                                            
- Some help                                                  
- ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓ 
- ┃                         Header                         ┃ 
- ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛ 
-                                                            
+ Usage: cli [OPTIONS] COMMAND [ARGS]...
+
+ Some help.
+ ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+ ┃                         Header                         ┃
+ ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
+
 ╭─ Options ────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                  │
 ╰──────────────────────────────────────────────────────────╯
 """
 
 
 @pytest.mark.skipif(CLICK_IS_BEFORE_VERSION_8X, reason="rich_config not supported prior to click v8")
@@ -345,98 +355,98 @@
             RichGroup,
             group_help_output,
             id="ClickGroup4",
         ),
     ],
 )
 def test_rich_config_decorator_order(
-    invoke: InvokeCli,
+    cli_runner: CliRunner,
     assert_str: AssertStr,
     command_callable: Callable[..., Any],
     expected_command_type: Type[RichCommand],
     expected_help_output: str,
 ) -> None:
     @command_callable()  # type: ignore[misc]
-    @rich_config(Console(), RichHelpConfiguration(max_width=60, use_markdown=True, color_system=None))
+    @rich_config(help_config=RichHelpConfiguration(max_width=60, use_markdown=True, color_system=None))
     def cli() -> None:
-        """Some help
+        """
+        Some help.
 
         # Header
         """
         pass
 
     assert hasattr(cli, "__rich_context_settings__") is False
     assert type(cli) is expected_command_type
-    assert cli.console is not None
     assert cli.__doc__ is not None
     assert_str(
         cli.__doc__,
         """
-    Some help
+    Some help.
 
     # Header
     """,
     )
 
-    result = invoke(cli, "--help")
+    result = cli_runner.invoke(cli, "--help")
 
     assert_str(
         actual=result.stdout,
         expectation=expected_help_output,
     )
 
 
-def test_rich_config_max_width(invoke: InvokeCli, assert_str: AssertStr) -> None:
+def test_rich_config_max_width(cli_runner: CliRunner, assert_str: AssertStr) -> None:
     rc.WIDTH = 100
     rc.MAX_WIDTH = 64
 
     @command()
     def cli() -> None:
-        """Some help text"""
+        """Some help text."""
         pass
 
-    result = invoke(cli, "--help")
+    result = cli_runner.invoke(cli, "--help")
 
     assert_str(
         result.stdout,
         """
-Usage: cli [OPTIONS]                                            
-                                                                
- Some help text                                                 
-                                                                
+Usage: cli [OPTIONS]
+
+ Some help text.
+
 ╭─ Options ────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                      │
 ╰──────────────────────────────────────────────────────────────╯
         """,
     )
 
 
 @pytest.mark.skipif(CLICK_IS_BEFORE_VERSION_8X, reason="rich_config not supported prior to click v8")
-def test_rich_config_context_settings(invoke: InvokeCli) -> None:
+def test_rich_config_context_settings(cli_runner: CliRunner) -> None:
     @click.command(
         cls=RichCommand, context_settings={"rich_console": Console(), "rich_help_config": RichHelpConfiguration()}
     )
     @pass_context
     def cli(ctx: RichContext) -> None:
         assert isinstance(ctx, RichContext)
         assert ctx.console is not None
         assert ctx.help_config is not None
 
-    result = invoke(cli)
+    result = cli_runner.invoke(cli)
     assert result.exit_code == 0
     assert result.exception is None
 
 
 @pytest.mark.skipif(not CLICK_IS_BEFORE_VERSION_8X, reason="This is to test a warning when using for click v7.")
-def test_rich_config_warns_before_click_v8(invoke: InvokeCli) -> None:
+def test_rich_config_warns_before_click_v8(cli_runner: CliRunner) -> None:
     with pytest.warns(RuntimeWarning, match="does not work with versions of click prior to version 8[.]0[.]0"):
 
         @rich_config(help_config=RichHelpConfiguration())
         @click.command("test-cmd")
         def cli() -> None:
             # Command should still work, regardless.
             click.echo("hello, world!")
 
-    result = invoke(cli)
+    result = cli_runner.invoke(cli)
     assert result.exit_code == 0
     assert result.exception is None
     assert result.stdout == "hello, world!\n"
```

