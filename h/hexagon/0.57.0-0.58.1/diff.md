# Comparing `tmp/hexagon-0.57.0.tar.gz` & `tmp/hexagon-0.58.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexagon-0.57.0.tar", last modified: Sat Mar  2 19:53:00 2024, max compression
+gzip compressed data, was "hexagon-0.58.1.tar", last modified: Mon Apr  8 22:18:59 2024, max compression
```

## Comparing `hexagon-0.57.0.tar` & `hexagon-0.58.1.tar`

### file list

```diff
@@ -1,123 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:53:00.001701 hexagon-0.57.0/
--rw-r--r--   0 root         (0) root         (0)    27296 2024-03-02 19:52:58.000000 hexagon-0.57.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11345 2024-03-02 19:52:56.000000 hexagon-0.57.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-02 19:52:56.000000 hexagon-0.57.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2666 2024-03-02 19:53:00.001701 hexagon-0.57.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20346 2024-03-02 19:52:56.000000 hexagon-0.57.0/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)     2170 2024-03-02 19:52:58.000000 hexagon-0.57.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2045 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon/actions/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon/actions/__templates/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/__templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon/actions/__templates/custom_tool/
--rw-r--r--   0 root         (0) root         (0)     1546 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/__templates/custom_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon/actions/external/
--rw-r--r--   0 root         (0) root         (0)       24 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/external/__init__.py
--rw-r--r--   0 root         (0) root         (0)      228 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/external/open_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.989701 hexagon-0.57.0/hexagon/actions/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/create_new_tool.py
--rw-r--r--   0 root         (0) root         (0)     2534 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/install_cli.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/replay.py
--rw-r--r--   0 root         (0) root         (0)     2599 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/save_new_alias.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/actions/internal/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.989701 hexagon-0.57.0/hexagon/domain/
--rw-r--r--   0 root         (0) root         (0)       54 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      227 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/cli.py
--rw-r--r--   0 root         (0) root         (0)      204 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/env.py
--rw-r--r--   0 root         (0) root         (0)       43 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/errors.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/hexagon_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.989701 hexagon-0.57.0/hexagon/domain/hooks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      741 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/hooks/execution.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/hooks/wax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.989701 hexagon-0.57.0/hexagon/domain/tool/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/domain/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5598 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/dependencies/
--rw-r--r--   0 root         (0) root         (0)      800 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/dependencies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      389 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/dependencies/fs.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/dependencies/node.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/dependencies/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/execute/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/execute/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7007 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/execute/action.py
--rw-r--r--   0 root         (0) root         (0)     4600 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/execute/errors.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/execute/execution_hook.py
--rw-r--r--   0 root         (0) root         (0)     3222 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/execute/tool.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/help.py
--rw-r--r--   0 root         (0) root         (0)     2103 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/options.py
--rw-r--r--   0 root         (0) root         (0)     5281 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/parse_args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/plugins/
--rw-r--r--   0 root         (0) root         (0)      861 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      351 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/singletons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/update/
--rw-r--r--   0 root         (0) root         (0)       47 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.993701 hexagon-0.57.0/hexagon/runtime/update/changelog/
--rw-r--r--   0 root         (0) root         (0)      953 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/changelog/fetch.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/changelog/format.py
--rw-r--r--   0 root         (0) root         (0)     2309 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/changelog/parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/runtime/update/cli/
--rw-r--r--   0 root         (0) root         (0)     2158 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      693 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/cli/command.py
--rw-r--r--   0 root         (0) root         (0)     1653 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/cli/git.py
--rw-r--r--   0 root         (0) root         (0)      246 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/github.py
--rw-r--r--   0 root         (0) root         (0)     2532 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/hexagon.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/shared.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/silent_fail.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/update/version.py
--rw-r--r--   0 root         (0) root         (0)     3151 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/wax.py
--rw-r--r--   0 root         (0) root         (0)     3508 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/runtime/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/hooks/
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1629 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/hooks/hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/input/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9713 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/args.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/input/prompt/
--rw-r--r--   0 root         (0) root         (0)       74 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/prompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      307 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/prompt/for_all_methods.py
--rw-r--r--   0 root         (0) root         (0)     5053 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/prompt/hints.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/prompt/key_bindings.py
--rw-r--r--   0 root         (0) root         (0)    15635 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/prompt/prompt.py
--rw-r--r--   0 root         (0) root         (0)     2525 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/input/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/output/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/output/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.997701 hexagon-0.57.0/hexagon/support/output/printer/
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/output/printer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11061 2024-03-02 19:52:57.000000 hexagon-0.57.0/hexagon/support/output/printer/en.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/output/printer/i18n.py
--rw-r--r--   0 root         (0) root         (0)     5156 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/output/printer/logger.py
--rw-r--r--   0 root         (0) root         (0)     2080 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/output/printer/themes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:53:00.001701 hexagon-0.57.0/hexagon/support/storage/
--rw-r--r--   0 root         (0) root         (0)     6043 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)      468 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/storage/merge_dictionaries.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/support/tracer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:53:00.001701 hexagon-0.57.0/hexagon/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-03-02 19:52:56.000000 hexagon-0.57.0/hexagon/utils/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.985701 hexagon-0.57.0/hexagon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2666 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2926 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-02 19:52:59.000000 hexagon-0.57.0/hexagon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.981701 hexagon-0.57.0/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.981701 hexagon-0.57.0/locales/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:53:00.001701 hexagon-0.57.0/locales/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11061 2024-03-02 19:52:57.000000 hexagon-0.57.0/locales/en/LC_MESSAGES/hexagon.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:52:59.981701 hexagon-0.57.0/locales/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 19:53:00.001701 hexagon-0.57.0/locales/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    11705 2024-03-02 19:52:57.000000 hexagon-0.57.0/locales/es/LC_MESSAGES/hexagon.mo
--rw-r--r--   0 root         (0) root         (0)      582 2024-03-02 19:52:56.000000 hexagon-0.57.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-02 19:53:00.001701 hexagon-0.57.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1615 2024-03-02 19:52:58.000000 hexagon-0.57.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/
+-rw-r--r--   0 root         (0) root         (0)    27868 2024-04-08 22:18:57.000000 hexagon-0.58.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11345 2024-04-08 22:18:56.000000 hexagon-0.58.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-08 22:18:56.000000 hexagon-0.58.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2576 2024-04-08 22:18:59.637069 hexagon-0.58.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20317 2024-04-08 22:18:56.000000 hexagon-0.58.1/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 22:18:57.000000 hexagon-0.58.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/__templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/__templates/custom_tool/
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/__templates/custom_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon/actions/external/
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/external/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      228 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/external/open_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/actions/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/create_new_tool.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/install_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/replay.py
+-rw-r--r--   0 root         (0) root         (0)     2599 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/save_new_alias.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/actions/internal/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/cli.py
+-rw-r--r--   0 root         (0) root         (0)      204 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/env.py
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/errors.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hexagon_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/hooks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/execution.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/hooks/wax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/domain/tool/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/domain/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.625069 hexagon-0.58.1/hexagon/runtime/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5598 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/dependencies/
+-rw-r--r--   0 root         (0) root         (0)      800 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      389 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/fs.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/node.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/dependencies/python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/execute/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7007 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/action.py
+-rw-r--r--   0 root         (0) root         (0)     4600 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/errors.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/execution_hook.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/execute/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/help.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/options.py
+-rw-r--r--   0 root         (0) root         (0)     5347 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/parse_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/plugins/
+-rw-r--r--   0 root         (0) root         (0)      861 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/singletons.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/update/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.629069 hexagon-0.58.1/hexagon/runtime/update/changelog/
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/fetch.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/format.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/changelog/parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/runtime/update/cli/
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/command.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/cli/git.py
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/github.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/hexagon.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/shared.py
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/silent_fail.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/update/version.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/wax.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/runtime/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/hooks/
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/hooks/hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/args/
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/cli_args.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/hexagon_args.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/args/tool_args.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/input/prompt/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/for_all_methods.py
+-rw-r--r--   0 root         (0) root         (0)     5053 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/hints.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/key_bindings.py
+-rw-r--r--   0 root         (0) root         (0)    15635 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/prompt/prompt.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/input/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.633069 hexagon-0.58.1/hexagon/support/output/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/support/output/printer/
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11084 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/en.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/i18n.py
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/output/printer/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/support/storage/
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/storage/merge_dictionaries.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/support/tracer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/hexagon/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-08 22:18:56.000000 hexagon-0.58.1/hexagon/utils/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.621069 hexagon-0.58.1/hexagon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2576 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3057 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 22:18:59.000000 hexagon-0.58.1/hexagon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/locales/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11084 2024-04-08 22:18:56.000000 hexagon-0.58.1/locales/en/LC_MESSAGES/hexagon.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.617069 hexagon-0.58.1/locales/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 22:18:59.637069 hexagon-0.58.1/locales/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    11728 2024-04-08 22:18:56.000000 hexagon-0.58.1/locales/es/LC_MESSAGES/hexagon.mo
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-08 22:18:56.000000 hexagon-0.58.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 22:18:59.637069 hexagon-0.58.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-08 22:18:57.000000 hexagon-0.58.1/setup.py
```

### Comparing `hexagon-0.57.0/CHANGELOG.md` & `hexagon-0.58.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.58.1 (2024-04-08)
+
+### Fix
+
+* **install:** Make bin_path optional arg ([`741044a`](https://github.com/lt-mayonesa/hexagon/commit/741044a2244770c18b66dfd972bc1220cab910ad))
+
+## v0.58.0 (2024-03-30)
+
+### Feature
+
+* **logger:** Add file & panel log APIs ([#80](https://github.com/lt-mayonesa/hexagon/issues/80)) ([`5e4a2db`](https://github.com/lt-mayonesa/hexagon/commit/5e4a2dbb9328d43a5921a51cc3b0ed42c6abbea6))
+
+### Documentation
+
+* **readme:** Install from pypi ([`6968d45`](https://github.com/lt-mayonesa/hexagon/commit/6968d45b54222086f940f9b635771214c0352bd5))
+
 ## v0.57.0 (2024-03-02)
 
 ### Feature
 
 * **prompt:** Allow passing callable to skip_trace ([`608d5dd`](https://github.com/lt-mayonesa/hexagon/commit/608d5dd99ee059bdf11528a661b501e70d186a48))
 
 ## v0.56.0 (2024-02-19)
```

### Comparing `hexagon-0.57.0/LICENSE` & `hexagon-0.58.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/PKG-INFO` & `hexagon-0.58.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hexagon
-Version: 0.57.0
+Version: 0.58.1
 Summary: Build your Team's CLI
 Home-page: https://github.com/lt-mayonesa/hexagon
 Author: Joaco Campero
 Author-email: juacocampero@gmail.com
 Project-URL: Bug Tracker, https://github.com/lt-mayonesa/hexagon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hexagon
 Make your team's knowledge truly accessible, truly shared, and truly empowering by creating your own CLI.
 
 [![01_ci-cd](https://github.com/lt-mayonesa/hexagon/actions/workflows/01-python-package.yml/badge.svg)](https://github.com/lt-mayonesa/hexagon/actions/workflows/01-python-package.yml)
@@ -23,15 +23,15 @@
 
 ---
 
 ## Getting Started
 
 ### Install hexagon
 ```bash
-python3 -m pip install https://github.com/lt-mayonesa/hexagon/releases/download/v0.57.0/hexagon-0.57.0.tar.gz
+pip install hexagon
 ```
 
 ### Create your teams CLI
 
 Either use our [template repo](https://github.com/lt-mayonesa/hexagon-tools) or create a YAML like the following
 ```yaml
 cli:
```

### Comparing `hexagon-0.57.0/Pipfile.lock` & `hexagon-0.58.1/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333332%*

 * *Differences: {"'develop'": "{'black': {'hashes': "*

 * *              "['sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f', "*

 * *              "'sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93', "*

 * *              "'sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11', "*

 * *              "'sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0', "*

 * *              "'sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9', "*

 * *              […]*

```diff
@@ -236,40 +236,40 @@
                 "sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.2.0"
         },
         "black": {
             "hashes": [
-                "sha256:057c3dc602eaa6fdc451069bd027a1b2635028b575a6c3acfd63193ced20d9c8",
-                "sha256:08654d0797e65f2423f850fc8e16a0ce50925f9337fb4a4a176a7aa4026e63f8",
-                "sha256:163baf4ef40e6897a2a9b83890e59141cc8c2a98f2dda5080dc15c00ee1e62cd",
-                "sha256:1e08fb9a15c914b81dd734ddd7fb10513016e5ce7e6704bdd5e1251ceee51ac9",
-                "sha256:4dd76e9468d5536abd40ffbc7a247f83b2324f0c050556d9c371c2b9a9a95e31",
-                "sha256:4f9de21bafcba9683853f6c96c2d515e364aee631b178eaa5145fc1c61a3cc92",
-                "sha256:61a0391772490ddfb8a693c067df1ef5227257e72b0e4108482b8d41b5aee13f",
-                "sha256:6981eae48b3b33399c8757036c7f5d48a535b962a7c2310d19361edeef64ce29",
-                "sha256:7e53a8c630f71db01b28cd9602a1ada68c937cbf2c333e6ed041390d6968faf4",
-                "sha256:810d445ae6069ce64030c78ff6127cd9cd178a9ac3361435708b907d8a04c693",
-                "sha256:93601c2deb321b4bad8f95df408e3fb3943d85012dddb6121336b8e24a0d1218",
-                "sha256:992e451b04667116680cb88f63449267c13e1ad134f30087dec8527242e9862a",
-                "sha256:9db528bccb9e8e20c08e716b3b09c6bdd64da0dd129b11e160bf082d4642ac23",
-                "sha256:a0057f800de6acc4407fe75bb147b0c2b5cbb7c3ed110d3e5999cd01184d53b0",
-                "sha256:ba15742a13de85e9b8f3239c8f807723991fbfae24bad92d34a2b12e81904982",
-                "sha256:bce4f25c27c3435e4dace4815bcb2008b87e167e3bf4ee47ccdc5ce906eb4894",
-                "sha256:ca610d29415ee1a30a3f30fab7a8f4144e9d34c89a235d81292a1edb2b55f540",
-                "sha256:d533d5e3259720fdbc1b37444491b024003e012c5173f7d06825a77508085430",
-                "sha256:d84f29eb3ee44859052073b7636533ec995bd0f64e2fb43aeceefc70090e752b",
-                "sha256:e37c99f89929af50ffaf912454b3e3b47fd64109659026b678c091a4cd450fb2",
-                "sha256:e8a6ae970537e67830776488bca52000eaa37fa63b9988e8c487458d9cd5ace6",
-                "sha256:faf2ee02e6612577ba0181f4347bcbcf591eb122f7841ae5ba233d12c39dcb4d"
+                "sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f",
+                "sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93",
+                "sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11",
+                "sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0",
+                "sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9",
+                "sha256:56f52cfbd3dabe2798d76dbdd299faa046a901041faf2cf33288bc4e6dae57b5",
+                "sha256:65b76c275e4c1c5ce6e9870911384bff5ca31ab63d19c76811cb1fb162678213",
+                "sha256:65c02e4ea2ae09d16314d30912a58ada9a5c4fdfedf9512d23326128ac08ac3d",
+                "sha256:6905238a754ceb7788a73f02b45637d820b2f5478b20fec82ea865e4f5d4d9f7",
+                "sha256:79dcf34b33e38ed1b17434693763301d7ccbd1c5860674a8f871bd15139e7837",
+                "sha256:7bb041dca0d784697af4646d3b62ba4a6b028276ae878e53f6b4f74ddd6db99f",
+                "sha256:7d5e026f8da0322b5662fa7a8e752b3fa2dac1c1cbc213c3d7ff9bdd0ab12395",
+                "sha256:9f50ea1132e2189d8dff0115ab75b65590a3e97de1e143795adb4ce317934995",
+                "sha256:a0c9c4a0771afc6919578cec71ce82a3e31e054904e7197deacbc9382671c41f",
+                "sha256:aadf7a02d947936ee418777e0247ea114f78aff0d0959461057cae8a04f20597",
+                "sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959",
+                "sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5",
+                "sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb",
+                "sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4",
+                "sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7",
+                "sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd",
+                "sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==24.2.0"
+            "version": "==24.3.0"
         },
         "click": {
             "hashes": [
                 "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28",
                 "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"
             ],
             "markers": "python_version >= '3.7'",
@@ -315,20 +315,19 @@
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
-            "index": "pypi",
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pathspec": {
             "hashes": [
                 "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08",
                 "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"
             ],
             "markers": "python_version >= '3.8'",
```

### Comparing `hexagon-0.57.0/README.md` & `hexagon-0.58.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ---
 
 ## Getting Started
 
 ### Install hexagon
 ```bash
-python3 -m pip install https://github.com/lt-mayonesa/hexagon/releases/download/v0.57.0/hexagon-0.57.0.tar.gz
+pip install hexagon
 ```
 
 ### Create your teams CLI
 
 Either use our [template repo](https://github.com/lt-mayonesa/hexagon-tools) or create a YAML like the following
 ```yaml
 cli:
```

### Comparing `hexagon-0.57.0/hexagon/__main__.py` & `hexagon-0.58.1/hexagon/__main__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/actions/__templates/custom_tool/__init__.py` & `hexagon-0.58.1/hexagon/actions/__templates/custom_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/actions/internal/create_new_tool.py` & `hexagon-0.58.1/hexagon/actions/internal/create_new_tool.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/actions/internal/install_cli.py` & `hexagon-0.58.1/hexagon/actions/internal/install_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 import os
 from pathlib import Path
 
 from pydantic import FilePath, validator, DirectoryPath
 
 from hexagon.runtime.dependencies import scan_and_install_dependencies
 from hexagon.runtime.singletons import configuration
-from hexagon.support.input.args import ToolArgs, Arg, PositionalArg
+from hexagon.support.input.args import ToolArgs, Arg, PositionalArg, OptionalArg
 from hexagon.support.output.printer import log
 from hexagon.support.storage import (
     load_user_data,
     HexagonStorageKeys,
     store_user_data,
 )
 
 
 class Args(ToolArgs):
     src_path: PositionalArg[FilePath] = Arg(
         None,
         prompt_message=_("action.actions.internal.install_cli.config_file_location"),
     )
-    bin_path: PositionalArg[DirectoryPath] = Arg(
-        str(os.path.expanduser(os.path.join("~", "bin"))),
+    bin_path: OptionalArg[DirectoryPath] = Arg(
+        None,
         prompt_message=_("action.actions.internal.install_cli.commands_path"),
+        prompt_default=str(os.path.expanduser(os.path.join("~", ".local", "bin"))),
     )
 
     @validator("src_path")
     def is_yaml(cls, arg):
         if isinstance(arg, str):
             if arg.endswith(".yaml") or arg.endswith(".yml"):
                 return arg
         else:
             if arg.value.suffix == ".yaml" or arg.value.suffix == ".yml":
                 return arg
         raise ValueError(_("error.actions.internal.install_cli.select_valid_file"))
 
 
-def main(tool, env, env_args, cli_args: Args):
+def main(_tool, _env, _env_args, cli_args: Args):
     if not cli_args.src_path.value:
         cli_args.src_path.prompt(default=str(Path.cwd()))
 
     cli, tools, envs = configuration.init_config(cli_args.src_path.value.resolve())
 
-    bin_path = load_user_data(HexagonStorageKeys.cli_install_path.value)
+    bin_path = (
+        load_user_data(HexagonStorageKeys.cli_install_path.value)
+        or cli_args.bin_path.value
+    )
 
     if not bin_path:
-        bin_path = cli_args.bin_path.prompt().resolve()
+        if not cli_args.bin_path.value:
+            bin_path = cli_args.bin_path.prompt().resolve()
         store_user_data(HexagonStorageKeys.cli_install_path.value, str(bin_path))
 
     command_path = os.path.join(bin_path, cli.command)
     with open(command_path, "w") as command:
         command.write(
             "#!/bin/bash\n"
             "# file create by hexagon\n"
```

### Comparing `hexagon-0.57.0/hexagon/actions/internal/replay.py` & `hexagon-0.58.1/hexagon/actions/internal/replay.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/actions/internal/save_new_alias.py` & `hexagon-0.58.1/hexagon/actions/internal/save_new_alias.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/actions/internal/schema.py` & `hexagon-0.58.1/hexagon/actions/internal/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def main(tool, env, env_args, cli_args):
     if not cli_args.target.value:
         cli_args.target.prompt()
 
     if cli_args.target.value == Target.STDOUT:
-        log.example(ConfigFile.schema_json(indent=2))
+        log.example(ConfigFile.schema_json(indent=2), syntax="json")
     else:
         if not cli_args.file_path.value:
             cli_args.file_path.prompt()
         with open(cli_args.file_path.value, "w") as schema_file:
             schema_file.write(ConfigFile.schema_json(indent=2))
 
         log.result(f"[green]Schema saved to [b]{cli_args.file_path.value}[/green]")
```

### Comparing `hexagon-0.57.0/hexagon/domain/hexagon_error.py` & `hexagon-0.58.1/hexagon/domain/hexagon_error.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/domain/hooks/execution.py` & `hexagon-0.58.1/hexagon/domain/hooks/execution.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/domain/tool/__init__.py` & `hexagon-0.58.1/hexagon/domain/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/configuration.py` & `hexagon-0.58.1/hexagon/runtime/configuration.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/dependencies/__init__.py` & `hexagon-0.58.1/hexagon/runtime/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/dependencies/node.py` & `hexagon-0.58.1/hexagon/runtime/dependencies/node.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/dependencies/python.py` & `hexagon-0.58.1/hexagon/runtime/dependencies/python.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/execute/action.py` & `hexagon-0.58.1/hexagon/runtime/execute/action.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/execute/errors.py` & `hexagon-0.58.1/hexagon/runtime/execute/errors.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/execute/execution_hook.py` & `hexagon-0.58.1/hexagon/runtime/execute/execution_hook.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/execute/tool.py` & `hexagon-0.58.1/hexagon/runtime/execute/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from hexagon.domain.tool import (
     FunctionTool,
     GroupTool,
     Tool,
     ToolType,
 )
 from hexagon.runtime.execute.action import execute_action
-from hexagon.runtime.parse_args import CliArgs, parse_cli_args
+from hexagon.runtime.parse_args import parse_cli_args
+from hexagon.support.input.args import CliArgs
 from hexagon.runtime.wax import search_by_name_or_alias, select_env, select_tool
 from hexagon.support.hooks import HexagonHooks
 from hexagon.support.tracer import tracer
 
 
 def select_and_execute_tool(
     tools: List[Tool],
```

### Comparing `hexagon-0.57.0/hexagon/runtime/help.py` & `hexagon-0.58.1/hexagon/runtime/help.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/options.py` & `hexagon-0.58.1/hexagon/runtime/options.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/parse_args.py` & `hexagon-0.58.1/hexagon/runtime/parse_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pydantic.fields import ModelField
 
 from hexagon.support.input.args import (
     CliArgs,
     ARGUMENT_KEY_PREFIX,
     OptionalArg,
     PositionalArg,
-    bool_negated_key,
 )
 from hexagon.utils.typing import should_support_multiple_args, field_info
 
 
 # noinspection PyProtectedMember
 class HexagonFormatter(argparse.RawDescriptionHelpFormatter):
     pass
@@ -91,15 +90,15 @@
         nargs=nargs,
         action=action,
         const=constant_default,
         help=f"{field.field_info.description or field.name} (default: {field.default})",
     )
     if is_bool:
         parser.add_argument(
-            *[bool_negated_key(r.replace("-", "")) for r in reprs if r],
+            *[__bool_negated_key(r.replace("-", "")) for r in reprs if r],
             action="store_const",
             dest=field.name,
             const="false",
             help=f"Disable {field.name}",
         )
 
 
@@ -178,7 +177,11 @@
                 if isinstance(d[k], list):
                     d[k].append(v)
                 else:
                     d[k] = [d[k], v]
             else:
                 d[k] = v
     return d
+
+
+def __bool_negated_key(name: str):
+    return f"{ARGUMENT_KEY_PREFIX * 2}no-{name}"
```

### Comparing `hexagon-0.57.0/hexagon/runtime/plugins/__init__.py` & `hexagon-0.58.1/hexagon/runtime/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/changelog/__init__.py` & `hexagon-0.58.1/hexagon/runtime/update/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/changelog/fetch.py` & `hexagon-0.58.1/hexagon/runtime/update/changelog/fetch.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/changelog/format.py` & `hexagon-0.58.1/hexagon/runtime/update/changelog/format.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/changelog/parse.py` & `hexagon-0.58.1/hexagon/runtime/update/changelog/parse.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/cli/__init__.py` & `hexagon-0.58.1/hexagon/runtime/update/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/cli/command.py` & `hexagon-0.58.1/hexagon/runtime/update/cli/command.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/cli/git.py` & `hexagon-0.58.1/hexagon/runtime/update/cli/git.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/hexagon.py` & `hexagon-0.58.1/hexagon/runtime/update/hexagon.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/shared.py` & `hexagon-0.58.1/hexagon/runtime/update/shared.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/update/version.py` & `hexagon-0.58.1/hexagon/runtime/update/version.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/wax.py` & `hexagon-0.58.1/hexagon/runtime/wax.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/runtime/yaml.py` & `hexagon-0.58.1/hexagon/runtime/yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Any, Type
 
 from pydantic import ValidationError
-from rich.syntax import Syntax
 from ruamel import yaml
 from ruamel.yaml import YAML
 
 from hexagon.domain.hexagon_error import HexagonError
+from hexagon.support.output.printer import Logger
 
 
 def read_file(path: str) -> Any:
     try:
         return YAML().load(open(path, "r"))
     except FileNotFoundError:
         return None
@@ -33,15 +33,15 @@
     def __init__(self, error: ValidationError, yaml_content=None, yaml_path=None):
         self.yaml_content = yaml_content
         self.yaml_path = yaml_path
         self.errors = error.errors()
         self.actual_yaml_file = open(yaml_path, "r").read() if yaml_path else None
         super().__init__(self._error_printer)
 
-    def _error_printer(self, logger):
+    def _error_printer(self, logger: Logger):
         logger.error(
             _("error.support.yaml.invalid_yaml").format(
                 errors_length=len(self.errors), yaml_path=self.yaml_path
             )
         )
         for err in self.errors:
             logger.error(
@@ -51,20 +51,18 @@
                 )
             )
             if self.yaml_content and yaml:
                 (start, line_number, end) = self.__lines_of_error(
                     err, self.yaml_content
                 )
                 logger.example(
-                    Syntax(
-                        "\n".join(self.actual_yaml_file.splitlines()[start:end]),
-                        "yaml",
-                        line_numbers=True,
-                        start_line=start + 1,
-                    ),
+                    "\n".join(self.actual_yaml_file.splitlines()[start:end]),
+                    syntax="yaml",
+                    show_line_numbers=True,
+                    start_line=start + 1,
                     decorator_start=False,
                     decorator_end=False,
                 )
 
     @classmethod
     def __lines_of_error(cls, err, ruamel_yaml):
         line_number = cls.__yaml_line_number(ruamel_yaml, err["loc"])
```

### Comparing `hexagon-0.57.0/hexagon/support/hooks/__init__.py` & `hexagon-0.58.1/hexagon/support/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/hooks/hook.py` & `hexagon-0.58.1/hexagon/support/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/input/prompt/hints.py` & `hexagon-0.58.1/hexagon/support/input/prompt/hints.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/input/prompt/key_bindings.py` & `hexagon-0.58.1/hexagon/support/input/prompt/key_bindings.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/input/prompt/prompt.py` & `hexagon-0.58.1/hexagon/support/input/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/input/types.py` & `hexagon-0.58.1/hexagon/support/input/types.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/output/printer/en.py` & `hexagon-0.58.1/hexagon/support/output/printer/en.py`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hexagon-0.57.0/hexagon/support/output/printer/i18n.py` & `hexagon-0.58.1/hexagon/support/output/printer/i18n.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/output/printer/themes.py` & `hexagon-0.58.1/hexagon/support/output/printer/themes.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/storage/__init__.py` & `hexagon-0.58.1/hexagon/support/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon/support/tracer.py` & `hexagon-0.58.1/hexagon/support/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, Union, Optional
 
-from hexagon.runtime.parse_args import CliArgs
+from hexagon.support.input.args import CliArgs
 
 
 @dataclass
 class Trace:
     ref: str
     value: str
     value_alias: str
```

### Comparing `hexagon-0.57.0/hexagon/utils/typing.py` & `hexagon-0.58.1/hexagon/utils/typing.py`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/hexagon.egg-info/PKG-INFO` & `hexagon-0.58.1/hexagon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hexagon
-Version: 0.57.0
+Version: 0.58.1
 Summary: Build your Team's CLI
 Home-page: https://github.com/lt-mayonesa/hexagon
 Author: Joaco Campero
 Author-email: juacocampero@gmail.com
 Project-URL: Bug Tracker, https://github.com/lt-mayonesa/hexagon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hexagon
 Make your team's knowledge truly accessible, truly shared, and truly empowering by creating your own CLI.
 
 [![01_ci-cd](https://github.com/lt-mayonesa/hexagon/actions/workflows/01-python-package.yml/badge.svg)](https://github.com/lt-mayonesa/hexagon/actions/workflows/01-python-package.yml)
@@ -23,15 +23,15 @@
 
 ---
 
 ## Getting Started
 
 ### Install hexagon
 ```bash
-python3 -m pip install https://github.com/lt-mayonesa/hexagon/releases/download/v0.57.0/hexagon-0.57.0.tar.gz
+pip install hexagon
 ```
 
 ### Create your teams CLI
 
 Either use our [template repo](https://github.com/lt-mayonesa/hexagon-tools) or create a YAML like the following
 ```yaml
 cli:
```

### Comparing `hexagon-0.57.0/hexagon.egg-info/SOURCES.txt` & `hexagon-0.58.1/hexagon.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,19 @@
 hexagon/runtime/update/cli/command.py
 hexagon/runtime/update/cli/git.py
 hexagon/support/__init__.py
 hexagon/support/tracer.py
 hexagon/support/hooks/__init__.py
 hexagon/support/hooks/hook.py
 hexagon/support/input/__init__.py
-hexagon/support/input/args.py
 hexagon/support/input/types.py
+hexagon/support/input/args/__init__.py
+hexagon/support/input/args/cli_args.py
+hexagon/support/input/args/hexagon_args.py
+hexagon/support/input/args/tool_args.py
 hexagon/support/input/prompt/__init__.py
 hexagon/support/input/prompt/for_all_methods.py
 hexagon/support/input/prompt/hints.py
 hexagon/support/input/prompt/key_bindings.py
 hexagon/support/input/prompt/prompt.py
 hexagon/support/output/__init__.py
 hexagon/support/output/printer/__init__.py
```

### Comparing `hexagon-0.57.0/locales/en/LC_MESSAGES/hexagon.mo` & `hexagon-0.58.1/locales/en/LC_MESSAGES/hexagon.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: en\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hexagon-0.57.0/locales/es/LC_MESSAGES/hexagon.mo` & `hexagon-0.58.1/locales/es/LC_MESSAGES/hexagon.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,10 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `hexagon-0.57.0/pyproject.toml` & `hexagon-0.58.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexagon-0.57.0/setup.py` & `hexagon-0.58.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import glob
 import json
 from os.path import dirname
 
 import setuptools
 
 # this updates automatically https://python-semantic-release.readthedocs.io/en/latest/index.html
-__version__ = "0.57.0"
+__version__ = "0.58.1"
 
 
 def __markers(config: dict):
     return f"; {config['markers']}" if "markers" in config else ""
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
@@ -41,14 +41,14 @@
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(
         exclude=["tests", "tests.*", "tests_e2e", "tests_e2e.*"]
     ),
     include_package_data=True,
     install_requires=requires,
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     entry_points="""
         [console_scripts]
         hexagon=hexagon.__main__:main
     """,
     data_files=translations,
 )
```

