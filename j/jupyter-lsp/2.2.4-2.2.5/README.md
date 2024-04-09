# Comparing `tmp/jupyter-lsp-2.2.4.tar.gz` & `tmp/jupyter-lsp-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-lsp-2.2.4.tar", last modified: Tue Mar  5 10:59:35 2024, max compression
+gzip compressed data, was "jupyter-lsp-2.2.5.tar", last modified: Tue Apr  9 16:13:54 2024, max compression
```

## Comparing `jupyter-lsp-2.2.4.tar` & `jupyter-lsp-2.2.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.527998 jupyter-lsp-2.2.4/jupyter_lsp/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.531998 jupyter-lsp-2.2.4/jupyter_lsp/etc/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/non_blocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.531998 jupyter-lsp-2.2.4/jupyter_lsp/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/serverextension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.531998 jupyter-lsp-2.2.4/jupyter_lsp/specs/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/bash_language_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/bash-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/julia-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pyls.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pylsp.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pyright.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/r-languageserver.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/sql-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/texlab.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/typescript-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/config/yaml-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/javascript_typescript_langserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/jedi_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/julia_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/pyls.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/pyright.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/python_lsp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/r_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/sql_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/texlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/typescript_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/unified_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_css_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_html_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_json_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/specs/yaml_language_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/jupyter_lsp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_bad_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_conf_d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/tests/test_virtual_documents_shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/trait_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/jupyter_lsp/virtual_documents_shadow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-05 10:59:35.000000 jupyter-lsp-2.2.4/jupyter_lsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-03-05 10:59:35.535998 jupyter-lsp-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-05 10:56:55.000000 jupyter-lsp-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.577342 jupyter-lsp-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 16:13:54.577342 jupyter-lsp-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.569342 jupyter-lsp-2.2.5/jupyter_lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.569342 jupyter-lsp-2.2.5/jupyter_lsp/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/non_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.569342 jupyter-lsp-2.2.5/jupyter_lsp/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/serverextension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.573342 jupyter-lsp-2.2.5/jupyter_lsp/specs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/bash_language_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.573342 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/bash-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/julia-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pyls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pylsp.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27670 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pyright.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/r-languageserver.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/sql-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/texlab.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/typescript-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/config/yaml-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/javascript_typescript_langserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/jedi_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/julia_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/pyright.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/python_lsp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/r_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/sql_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/texlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/typescript_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/unified_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_css_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_html_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_json_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/specs/yaml_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.577342 jupyter-lsp-2.2.5/jupyter_lsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_bad_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_conf_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/tests/test_virtual_documents_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/jupyter_lsp/virtual_documents_shadow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:13:54.577342 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:13:54.000000 jupyter-lsp-2.2.5/jupyter_lsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 16:13:54.577342 jupyter-lsp-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 16:11:12.000000 jupyter-lsp-2.2.5/setup.py
```

### Comparing `jupyter-lsp-2.2.4/LICENSE` & `jupyter-lsp-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/PKG-INFO` & `jupyter-lsp-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.2.4
+Version: 2.2.5
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.2.4/README.md` & `jupyter-lsp-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/handlers.py` & `jupyter-lsp-2.2.5/jupyter_lsp/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/manager.py` & `jupyter-lsp-2.2.5/jupyter_lsp/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/non_blocking.py` & `jupyter-lsp-2.2.5/jupyter_lsp/non_blocking.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/paths.py` & `jupyter-lsp-2.2.5/jupyter_lsp/paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/schema/__init__.py` & `jupyter-lsp-2.2.5/jupyter_lsp/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/schema/schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/schema/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/serverextension.py` & `jupyter-lsp-2.2.5/jupyter_lsp/serverextension.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/session.py` & `jupyter-lsp-2.2.5/jupyter_lsp/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 
 import asyncio
 import atexit
 import os
 import string
 import subprocess
-from copy import copy
 from datetime import datetime, timezone
 
 from tornado.ioloop import IOLoop
 from tornado.queues import Queue
 from tornado.websocket import WebSocketHandler
 from traitlets import Bunch, Instance, Set, Unicode, UseEnum, observe
 from traitlets.config import LoggingConfigurable
@@ -157,15 +156,15 @@
     def init_writer(self):
         """create the stdin writer (to the language server)"""
         self.writer = stdio.LspStdIoWriter(
             stream=self.process.stdin, queue=self.to_lsp, parent=self
         )
 
     def substitute_env(self, env, base):
-        final_env = copy(os.environ)
+        final_env = base.copy()
 
         for key, value in env.items():
             final_env.update({key: string.Template(value).safe_substitute(base)})
 
         return final_env
 
     async def _read_lsp(self):
```

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/__init__.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/bash_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/bash_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/bash-language-server.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/bash-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/julia-language-server.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/julia-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pyls.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pyls.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pylsp.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pylsp.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/pyright.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/r-languageserver.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/r-languageserver.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/sql-language-server.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/sql-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/texlab.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/texlab.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/typescript-language-server.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/typescript-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/config/yaml-language-server.schema.json` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/config/yaml-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/dockerfile_language_server_nodejs.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/dockerfile_language_server_nodejs.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/javascript_typescript_langserver.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/javascript_typescript_langserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/jedi_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/jedi_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/julia_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/julia_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/pyls.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/pyls.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/pyright.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/pyright.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/python_lsp_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/python_lsp_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/r_languageserver.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/r_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/sql_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/sql_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/texlab.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/texlab.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/typescript_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/typescript_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/unified_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/unified_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/utils.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_css_languageserver.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_css_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_html_languageserver.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_html_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/vscode_json_languageserver.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/vscode_json_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/specs/yaml_language_server.py` & `jupyter-lsp-2.2.5/jupyter_lsp/specs/yaml_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/stdio.py` & `jupyter-lsp-2.2.5/jupyter_lsp/stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/conftest.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_auth.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_detect.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_extension.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_listener.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_paths.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_session.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import os
 
 import pytest
 
 from ..schema import SERVERS_RESPONSE
 
 
 async def assert_status_set(handler, expected_statuses, language_server=None):
@@ -96,7 +97,29 @@
 
     assert ws_handler.ping_callback is not None and ws_handler.ping_callback.is_running
     await asyncio.sleep(ws_handler.ping_interval * 3)
 
     assert ws_handler._ping_sent is True
 
     ws_handler.on_close()
+
+
+@pytest.mark.asyncio
+async def test_substitute_env(handlers):
+    """should not leak environment variables"""
+    a_server = "pylsp"
+
+    handler, ws_handler = handlers
+    manager = handler.manager
+
+    manager.initialize()
+
+    await assert_status_set(handler, {"not_started"})
+
+    await ws_handler.open(a_server)
+    session = manager.sessions[ws_handler.language_server]
+    new_env = session.substitute_env({"test-variable": "value"}, os.environ)
+
+    assert "test-variable" in new_env
+    assert "test-variable" not in os.environ
+
+    ws_handler.on_close()
```

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_stdio.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/tests/test_virtual_documents_shadow.py` & `jupyter-lsp-2.2.5/jupyter_lsp/tests/test_virtual_documents_shadow.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/trait_types.py` & `jupyter-lsp-2.2.5/jupyter_lsp/trait_types.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/types.py` & `jupyter-lsp-2.2.5/jupyter_lsp/types.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp/virtual_documents_shadow.py` & `jupyter-lsp-2.2.5/jupyter_lsp/virtual_documents_shadow.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp.egg-info/PKG-INFO` & `jupyter-lsp-2.2.5/jupyter_lsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.2.4
+Version: 2.2.5
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp.egg-info/SOURCES.txt` & `jupyter-lsp-2.2.5/jupyter_lsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/jupyter_lsp.egg-info/entry_points.txt` & `jupyter-lsp-2.2.5/jupyter_lsp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.2.4/setup.cfg` & `jupyter-lsp-2.2.5/setup.cfg`

 * *Files identical despite different names*

