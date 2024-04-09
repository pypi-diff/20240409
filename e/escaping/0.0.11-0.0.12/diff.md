# Comparing `tmp/escaping-0.0.11.tar.gz` & `tmp/escaping-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escaping-0.0.11.tar", last modified: Sun Mar 31 13:26:49 2024, max compression
+gzip compressed data, was "escaping-0.0.12.tar", last modified: Tue Apr  9 17:01:25 2024, max compression
```

## Comparing `escaping-0.0.11.tar` & `escaping-0.0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 13:26:49.436653 escaping-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-31 13:26:33.000000 escaping-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-03-31 13:26:49.436653 escaping-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-31 13:26:33.000000 escaping-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 13:26:49.436653 escaping-0.0.11/escape/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-31 13:26:33.000000 escaping-0.0.11/escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-31 13:26:33.000000 escaping-0.0.11/escape/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-03-31 13:26:33.000000 escaping-0.0.11/escape/proxy_module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 13:26:33.000000 escaping-0.0.11/escape/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-31 13:26:33.000000 escaping-0.0.11/escape/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 13:26:49.436653 escaping-0.0.11/escaping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-03-31 13:26:49.000000 escaping-0.0.11/escaping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-31 13:26:49.000000 escaping-0.0.11/escaping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 13:26:49.000000 escaping-0.0.11/escaping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 13:26:49.000000 escaping-0.0.11/escaping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 13:26:49.000000 escaping-0.0.11/escaping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-31 13:26:33.000000 escaping-0.0.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 13:26:49.436653 escaping-0.0.11/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:01:25.358498 escaping-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 17:01:11.000000 escaping-0.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-09 17:01:25.358498 escaping-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-04-09 17:01:11.000000 escaping-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:01:25.358498 escaping-0.0.12/escape/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 17:01:11.000000 escaping-0.0.12/escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 17:01:11.000000 escaping-0.0.12/escape/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-09 17:01:11.000000 escaping-0.0.12/escape/proxy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:01:11.000000 escaping-0.0.12/escape/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-09 17:01:11.000000 escaping-0.0.12/escape/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:01:25.358498 escaping-0.0.12/escaping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-09 17:01:25.000000 escaping-0.0.12/escaping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 17:01:25.000000 escaping-0.0.12/escaping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:01:25.000000 escaping-0.0.12/escaping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 17:01:25.000000 escaping-0.0.12/escaping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 17:01:25.000000 escaping-0.0.12/escaping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-09 17:01:11.000000 escaping-0.0.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:01:25.358498 escaping-0.0.12/setup.cfg
```

### Comparing `escaping-0.0.11/LICENSE` & `escaping-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `escaping-0.0.11/PKG-INFO` & `escaping-0.0.12/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,26 @@
-Metadata-Version: 2.1
-Name: escaping
-Version: 0.0.11
-Summary: Try not to stand out
-Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
-Project-URL: Source, https://github.com/pomponchik/escaping
-Project-URL: Tracker, https://github.com/pomponchik/escaping/issues
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![logo](https://raw.githubusercontent.com/pomponchik/escaping/develop/docs/assets/logo_16.svg)
 
 [![Downloads](https://static.pepy.tech/badge/escaping/month)](https://pepy.tech/project/escaping)
 [![Downloads](https://static.pepy.tech/badge/escaping)](https://pepy.tech/project/escaping)
 [![codecov](https://codecov.io/gh/pomponchik/escaping/graph/badge.svg?token=q7eAfV5g7q)](https://codecov.io/gh/pomponchik/escaping)
 [![Lines of code](https://sloc.xyz/github/pomponchik/escaping/?category=code)](https://github.com/boyter/scc/)
 [![Hits-of-Code](https://hitsofcode.com/github/pomponchik/escaping?branch=main)](https://hitsofcode.com/github/pomponchik/escaping/view?branch=main)
 [![Test-Package](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/escaping.svg)](https://pypi.python.org/pypi/escaping)
 [![PyPI version](https://badge.fury.io/py/escaping.svg)](https://badge.fury.io/py/escaping)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
-If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree.
+If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree :) Seriously, the library allows you to solve the problem of exception handling in a more adult way by providing:
+
+- 🛡️ A universal interface for the decorator and context manager.
+- 🛡️ Built-in logging.
+- 🛡️ Calling callbacks.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Decorator mode**](#decorator-mode)
 - [**Context manager mode**](#context-manager-mode)
@@ -71,15 +49,15 @@
 ```
 
 Read about other library features below.
 
 
 ## Decorator mode
 
-The `@escape` decorator suppresses exceptions in a wrapped function (including a coroutine one), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
+The `@escape` decorator suppresses exceptions in a wrapped function (including generator and coroutine ones), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
 
 ```python
 import asyncio
 import escape
 
 @escape(ValueError, ZeroDivisionError)
 def function():
@@ -195,24 +173,59 @@
     1/0
 
 # You will see a description of the error in the console.
 ```
 
 It works in any mode: both in the case of the context manager and the decorator.
 
-Only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+By default only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+
+But! You can change the standard logging behavior.
+
+If you want the log to be recorded for any outcome, including the one where no errors occurred, specify the `success_logging=True` flag (messages will be recorded with the `info` level):
+
+```python
+with escape(success_logging=True, logger=logger):
+    pass
+    # > The code block was executed successfully.
+```
+
+In addition, you can change the standard messages that you see in the logs. Keep in mind that this feature narrows down the variety of standard messages, which differ depending on where the error occurred (in a regular function, in a generator or asynchronous function, or perhaps in a block of code wrapped by a context manager), or whether the error was intercepted. You can define your own messages for only two types of situations: when the code was executed without exceptions, and when with an exception.
+
+Pass your message as `error_log_message` if you want to see it when an error occurred inside the code:
+
+```python
+with escape(..., error_log_message='Oh my God!', logger=logger):
+    raise ValueError
+    # > Oh my God!
+```
+
+By analogy, pass `success_log_message` as a message if there are no errors in the code block (but don't forget to set `success_logging=True`!):
+
+```python
+with escape(success_log_message='Good news, everyone!', success_logging=True, logger=logger):
+    pass
+    # > Good news, everyone!
+```
+
+In addition, if the exception was suppressed inside the `escape`, the log will be recorded using the `exception` method - this means that the trace will be saved. Otherwise, the `error` method will be used - without saving the traceback, because otherwise, if you catch this exception somewhere else and pledge the traceback, there will be several duplicate tracebacks in your log file.
 
 
 ## Callbacks
 
 You can pass [callback](https://en.wikipedia.org/wiki/Callback_(computer_programming)) functions to `escape`, which will be automatically called when the wrapped code block or function has completed.
 
 A callback passed as `success_callback` will be called when the code is executed without errors:
 
 ```python
-import escape
-
 with escape(success_callback=lambda: print('The code block ended without errors.')):
     pass
 ```
 
+By analogy, if you pass `error_callback`, this function will be called when an exception is raised inside:
+
+```python
+with escape(error_callback=lambda: print('Attention!')):
+    pass
+```
+
 If an error occurs in one of the callbacks, the exception will be suppressed if it would have been suppressed if it had happened in a wrapped code block or function. You can see the corresponding log entry about this if you [pass the logger object](#logging) for registration. If the error inside the callback has been suppressed, it will not affect the logic that was wrapped by `escape` in any way.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `escaping-0.0.11/README.md` & `escaping-0.0.12/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,53 @@
+Metadata-Version: 2.1
+Name: escaping
+Version: 0.0.12
+Summary: Try not to stand out
+Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
+Project-URL: Source, https://github.com/pomponchik/escaping
+Project-URL: Tracker, https://github.com/pomponchik/escaping/issues
+Keywords: exception handling,exception logging,containerized code,safe code,callbacks
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![logo](https://raw.githubusercontent.com/pomponchik/escaping/develop/docs/assets/logo_16.svg)
 
 [![Downloads](https://static.pepy.tech/badge/escaping/month)](https://pepy.tech/project/escaping)
 [![Downloads](https://static.pepy.tech/badge/escaping)](https://pepy.tech/project/escaping)
 [![codecov](https://codecov.io/gh/pomponchik/escaping/graph/badge.svg?token=q7eAfV5g7q)](https://codecov.io/gh/pomponchik/escaping)
 [![Lines of code](https://sloc.xyz/github/pomponchik/escaping/?category=code)](https://github.com/boyter/scc/)
 [![Hits-of-Code](https://hitsofcode.com/github/pomponchik/escaping?branch=main)](https://hitsofcode.com/github/pomponchik/escaping/view?branch=main)
 [![Test-Package](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/escaping.svg)](https://pypi.python.org/pypi/escaping)
 [![PyPI version](https://badge.fury.io/py/escaping.svg)](https://badge.fury.io/py/escaping)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
-If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree.
+If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree :) Seriously, the library allows you to solve the problem of exception handling in a more adult way by providing:
+
+- 🛡️ A universal interface for the decorator and context manager.
+- 🛡️ Built-in logging.
+- 🛡️ Calling callbacks.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Decorator mode**](#decorator-mode)
 - [**Context manager mode**](#context-manager-mode)
@@ -45,15 +76,15 @@
 ```
 
 Read about other library features below.
 
 
 ## Decorator mode
 
-The `@escape` decorator suppresses exceptions in a wrapped function (including a coroutine one), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
+The `@escape` decorator suppresses exceptions in a wrapped function (including generator and coroutine ones), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
 
 ```python
 import asyncio
 import escape
 
 @escape(ValueError, ZeroDivisionError)
 def function():
@@ -169,24 +200,59 @@
     1/0
 
 # You will see a description of the error in the console.
 ```
 
 It works in any mode: both in the case of the context manager and the decorator.
 
-Only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+By default only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+
+But! You can change the standard logging behavior.
+
+If you want the log to be recorded for any outcome, including the one where no errors occurred, specify the `success_logging=True` flag (messages will be recorded with the `info` level):
+
+```python
+with escape(success_logging=True, logger=logger):
+    pass
+    # > The code block was executed successfully.
+```
+
+In addition, you can change the standard messages that you see in the logs. Keep in mind that this feature narrows down the variety of standard messages, which differ depending on where the error occurred (in a regular function, in a generator or asynchronous function, or perhaps in a block of code wrapped by a context manager), or whether the error was intercepted. You can define your own messages for only two types of situations: when the code was executed without exceptions, and when with an exception.
+
+Pass your message as `error_log_message` if you want to see it when an error occurred inside the code:
+
+```python
+with escape(..., error_log_message='Oh my God!', logger=logger):
+    raise ValueError
+    # > Oh my God!
+```
+
+By analogy, pass `success_log_message` as a message if there are no errors in the code block (but don't forget to set `success_logging=True`!):
+
+```python
+with escape(success_log_message='Good news, everyone!', success_logging=True, logger=logger):
+    pass
+    # > Good news, everyone!
+```
+
+In addition, if the exception was suppressed inside the `escape`, the log will be recorded using the `exception` method - this means that the trace will be saved. Otherwise, the `error` method will be used - without saving the traceback, because otherwise, if you catch this exception somewhere else and pledge the traceback, there will be several duplicate tracebacks in your log file.
 
 
 ## Callbacks
 
 You can pass [callback](https://en.wikipedia.org/wiki/Callback_(computer_programming)) functions to `escape`, which will be automatically called when the wrapped code block or function has completed.
 
 A callback passed as `success_callback` will be called when the code is executed without errors:
 
 ```python
-import escape
-
 with escape(success_callback=lambda: print('The code block ended without errors.')):
     pass
 ```
 
+By analogy, if you pass `error_callback`, this function will be called when an exception is raised inside:
+
+```python
+with escape(error_callback=lambda: print('Attention!')):
+    pass
+```
+
 If an error occurs in one of the callbacks, the exception will be suppressed if it would have been suppressed if it had happened in a wrapped code block or function. You can see the corresponding log entry about this if you [pass the logger object](#logging) for registration. If the error inside the callback has been suppressed, it will not affect the logic that was wrapped by `escape` in any way.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `escaping-0.0.11/escape/proxy_module.py` & `escaping-0.0.12/escape/proxy_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 from escape.wrapper import Wrapper
 
 
 if sys.version_info < (3, 11):
     muted_by_default_exceptions: Tuple[Type[BaseException], ...] = (Exception,)  # pragma: no cover
 else:
-    muted_by_default_exceptions = (Exception, BaseExceptionGroup)
+    muted_by_default_exceptions = (Exception, BaseExceptionGroup)  # pragma: no cover
 
 class ProxyModule(sys.modules[__name__].__class__):  # type: ignore[misc]
-    def __call__(self, *args: Union[Callable[..., Any], Type[BaseException], EllipsisType], default: Any = None, logger: LoggerProtocol = EmptyLogger(), success_callback: Callable[[], Any] = lambda: None) -> Union[Callable[..., Any], Callable[[Callable[..., Any]], Callable[..., Any]]]:
+    def __call__(self, *args: Union[Callable[..., Any], Type[BaseException], EllipsisType], default: Any = None, logger: LoggerProtocol = EmptyLogger(), success_callback: Callable[[], Any] = lambda: None, error_callback: Callable[[], Any] = lambda: None, error_log_message: Optional[str] = None, success_log_message: Optional[str] = None, success_logging: bool = False) -> Union[Callable[..., Any], Callable[[Callable[..., Any]], Callable[..., Any]]]:
         """
         https://docs.python.org/3/library/exceptions.html#exception-hierarchy
         """
         if self.are_it_function(args):
             exceptions: Tuple[Type[BaseException], ...] = muted_by_default_exceptions
         else:
             if self.is_there_ellipsis(args):
                 exceptions = tuple(chain((x for x in args if x is not Ellipsis), muted_by_default_exceptions))  # type: ignore[misc]
             else:
                 exceptions = args  # type: ignore[assignment]
 
-        wrapper_of_wrappers = Wrapper(default, exceptions, logger, success_callback)
+        wrapper_of_wrappers = Wrapper(default, exceptions, logger, success_callback, error_log_message, success_logging, success_log_message, error_callback)
 
         if self.are_it_exceptions(args):
             return wrapper_of_wrappers
 
         elif self.are_it_function(args):
             return wrapper_of_wrappers(args[0])
```

### Comparing `escaping-0.0.11/escaping.egg-info/PKG-INFO` & `escaping-0.0.12/escaping.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: escaping
-Version: 0.0.11
+Version: 0.0.12
 Summary: Try not to stand out
 Author-email: Evgeniy Blinov <zheni-b@yandex.ru>
 Project-URL: Source, https://github.com/pomponchik/escaping
 Project-URL: Tracker, https://github.com/pomponchik/escaping/issues
+Keywords: exception handling,exception logging,containerized code,safe code,callbacks
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,15 +35,19 @@
 [![Test-Package](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml/badge.svg)](https://github.com/pomponchik/escaping/actions/workflows/tests_and_coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/escaping.svg)](https://pypi.python.org/pypi/escaping)
 [![PyPI version](https://badge.fury.io/py/escaping.svg)](https://badge.fury.io/py/escaping)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
-If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree.
+If you've just confessed and you can't wait to sin again, try this package. It will help you [hide your mistakes](https://en.wikipedia.org/wiki/Error_hiding) and make your life more carefree :) Seriously, the library allows you to solve the problem of exception handling in a more adult way by providing:
+
+- 🛡️ A universal interface for the decorator and context manager.
+- 🛡️ Built-in logging.
+- 🛡️ Calling callbacks.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**Decorator mode**](#decorator-mode)
 - [**Context manager mode**](#context-manager-mode)
@@ -71,15 +76,15 @@
 ```
 
 Read about other library features below.
 
 
 ## Decorator mode
 
-The `@escape` decorator suppresses exceptions in a wrapped function (including a coroutine one), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
+The `@escape` decorator suppresses exceptions in a wrapped function (including generator and coroutine ones), which are passed in parentheses. In this way, you can pass any number of exceptions, for example:
 
 ```python
 import asyncio
 import escape
 
 @escape(ValueError, ZeroDivisionError)
 def function():
@@ -195,24 +200,59 @@
     1/0
 
 # You will see a description of the error in the console.
 ```
 
 It works in any mode: both in the case of the context manager and the decorator.
 
-Only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+By default only exceptions are logged. If the code block or function was executed without errors, the log will not be recorded. Also the log is recorded regardless of whether the exception was suppressed or not. However, depending on this, you will see different log messages to distinguish one situation from another.
+
+But! You can change the standard logging behavior.
+
+If you want the log to be recorded for any outcome, including the one where no errors occurred, specify the `success_logging=True` flag (messages will be recorded with the `info` level):
+
+```python
+with escape(success_logging=True, logger=logger):
+    pass
+    # > The code block was executed successfully.
+```
+
+In addition, you can change the standard messages that you see in the logs. Keep in mind that this feature narrows down the variety of standard messages, which differ depending on where the error occurred (in a regular function, in a generator or asynchronous function, or perhaps in a block of code wrapped by a context manager), or whether the error was intercepted. You can define your own messages for only two types of situations: when the code was executed without exceptions, and when with an exception.
+
+Pass your message as `error_log_message` if you want to see it when an error occurred inside the code:
+
+```python
+with escape(..., error_log_message='Oh my God!', logger=logger):
+    raise ValueError
+    # > Oh my God!
+```
+
+By analogy, pass `success_log_message` as a message if there are no errors in the code block (but don't forget to set `success_logging=True`!):
+
+```python
+with escape(success_log_message='Good news, everyone!', success_logging=True, logger=logger):
+    pass
+    # > Good news, everyone!
+```
+
+In addition, if the exception was suppressed inside the `escape`, the log will be recorded using the `exception` method - this means that the trace will be saved. Otherwise, the `error` method will be used - without saving the traceback, because otherwise, if you catch this exception somewhere else and pledge the traceback, there will be several duplicate tracebacks in your log file.
 
 
 ## Callbacks
 
 You can pass [callback](https://en.wikipedia.org/wiki/Callback_(computer_programming)) functions to `escape`, which will be automatically called when the wrapped code block or function has completed.
 
 A callback passed as `success_callback` will be called when the code is executed without errors:
 
 ```python
-import escape
-
 with escape(success_callback=lambda: print('The code block ended without errors.')):
     pass
 ```
 
+By analogy, if you pass `error_callback`, this function will be called when an exception is raised inside:
+
+```python
+with escape(error_callback=lambda: print('Attention!')):
+    pass
+```
+
 If an error occurs in one of the callbacks, the exception will be suppressed if it would have been suppressed if it had happened in a wrapped code block or function. You can see the corresponding log entry about this if you [pass the logger object](#logging) for registration. If the error inside the callback has been suppressed, it will not affect the logic that was wrapped by `escape` in any way.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

