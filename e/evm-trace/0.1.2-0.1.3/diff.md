# Comparing `tmp/evm-trace-0.1.2.tar.gz` & `tmp/evm-trace-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evm-trace-0.1.2.tar", last modified: Sat Dec 16 16:18:52 2023, max compression
+gzip compressed data, was "evm-trace-0.1.3.tar", last modified: Tue Apr  9 17:42:28 2024, max compression
```

## Comparing `evm-trace-0.1.2.tar` & `evm-trace-0.1.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.368673 evm-trace-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.356673 evm-trace-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.356673 evm-trace-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.360673 evm-trace-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-16 16:18:25.000000 evm-trace-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-12-16 16:18:25.000000 evm-trace-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-16 16:18:25.000000 evm-trace-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-16 16:18:52.368673 evm-trace-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-12-16 16:18:25.000000 evm-trace-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.360673 evm-trace-0.1.2/evm_trace/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/display.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/geth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/parity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2023-12-16 16:18:25.000000 evm-trace-0.1.2/evm_trace/vmtrace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.360673 evm-trace-0.1.2/evm_trace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-16 16:18:52.000000 evm-trace-0.1.2/evm_trace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-16 16:18:25.000000 evm-trace-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-16 16:18:52.368673 evm-trace-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-16 16:18:25.000000 evm-trace-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.360673 evm-trace-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.356673 evm-trace-0.1.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.364673 evm-trace-0.1.2/tests/data/evm_trace/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/evm_trace/call.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/evm_trace/delegate_call.json
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/evm_trace/frame.json
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/evm_trace/mutable_call.json
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/evm_trace/static_call.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.368673 evm-trace-0.1.2/tests/data/geth/
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/geth/call.json
--rw-r--r--   0 runner    (1001) docker     (127)  3934899 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/geth/create2_structlogs.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/geth/create_call.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 16:18:52.368673 evm-trace-0.1.2/tests/data/parity/
--rw-r--r--   0 runner    (1001) docker     (127)   137258 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/call.json
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/create.json
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/create2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/create_revert.json
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/error.json
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/revert.json
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/revert_with_message.json
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/data/parity/selfdestruct.json
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/test_geth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-16 16:18:25.000000 evm-trace-0.1.2/tests/test_parity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 17:42:07.000000 evm-trace-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 17:42:07.000000 evm-trace-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 17:42:07.000000 evm-trace-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-09 17:42:28.680019 evm-trace-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 17:42:07.000000 evm-trace-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/evm_trace/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/geth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/parity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-09 17:42:07.000000 evm-trace-0.1.3/evm_trace/vmtrace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/evm_trace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:42:28.000000 evm-trace-0.1.3/evm_trace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 17:42:07.000000 evm-trace-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 17:42:28.680019 evm-trace-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 17:42:07.000000 evm-trace-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.668018 evm-trace-0.1.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.672019 evm-trace-0.1.3/tests/data/evm_trace/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/delegate_call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/frame.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/mutable_call.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/evm_trace/static_call.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/tests/data/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)  3934899 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/create2_structlogs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/geth/create_call.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:42:28.680019 evm-trace-0.1.3/tests/data/parity/
+-rw-r--r--   0 runner    (1001) docker     (127)   137258 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/call.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/create_revert.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/error.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/revert.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/revert_with_message.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/data/parity/selfdestruct.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_geth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-09 17:42:07.000000 evm-trace-0.1.3/tests/test_parity.py
```

### Comparing `evm-trace-0.1.2/.github/ISSUE_TEMPLATE/bug.md` & `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/ISSUE_TEMPLATE/feature.md` & `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/ISSUE_TEMPLATE/work-item.md` & `evm-trace-0.1.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/release-drafter.yml` & `evm-trace-0.1.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/workflows/commitlint.yaml` & `evm-trace-0.1.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/workflows/prtitle.yaml` & `evm-trace-0.1.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/workflows/publish.yaml` & `evm-trace-0.1.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.github/workflows/test.yaml` & `evm-trace-0.1.3/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `evm-trace-0.1.2/.gitignore` & `evm-trace-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/.pre-commit-config.yaml` & `evm-trace-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/CONTRIBUTING.md` & `evm-trace-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/LICENSE` & `evm-trace-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/PKG-INFO` & `evm-trace-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.2
+Version: 0.1.3
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `evm-trace-0.1.2/README.md` & `evm-trace-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/__init__.py` & `evm-trace-0.1.3/evm_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/base.py` & `evm-trace-0.1.3/evm_trace/base.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/display.py` & `evm-trace-0.1.3/evm_trace/display.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/enums.py` & `evm-trace-0.1.3/evm_trace/enums.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/gas.py` & `evm-trace-0.1.3/evm_trace/gas.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/geth.py` & `evm-trace-0.1.3/evm_trace/geth.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/parity.py` & `evm-trace-0.1.3/evm_trace/parity.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace/vmtrace.py` & `evm-trace-0.1.3/evm_trace/vmtrace.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace.egg-info/PKG-INFO` & `evm-trace-0.1.3/evm_trace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evm-trace
-Version: 0.1.2
+Version: 0.1.3
 Summary: evm-trace: Ethereum Virtual Machine transaction tracing tool
 Home-page: https://github.com/ApeWorX/evm-trace
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `evm-trace-0.1.2/evm_trace.egg-info/SOURCES.txt` & `evm-trace-0.1.3/evm_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/evm_trace.egg-info/requires.txt` & `evm-trace-0.1.3/evm_trace.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/pyproject.toml` & `evm-trace-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `evm-trace-0.1.2/setup.py` & `evm-trace-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,9 +82,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `evm-trace-0.1.2/tests/conftest.py` & `evm-trace-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/evm_trace/call.json` & `evm-trace-0.1.3/tests/data/evm_trace/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/evm_trace/frame.json` & `evm-trace-0.1.3/tests/data/evm_trace/frame.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/evm_trace/mutable_call.json` & `evm-trace-0.1.3/tests/data/evm_trace/mutable_call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/geth/call.json` & `evm-trace-0.1.3/tests/data/geth/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/geth/create2_structlogs.json` & `evm-trace-0.1.3/tests/data/geth/create2_structlogs.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/geth/create_call.json` & `evm-trace-0.1.3/tests/data/geth/create_call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/call.json` & `evm-trace-0.1.3/tests/data/parity/call.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/create.json` & `evm-trace-0.1.3/tests/data/parity/create.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/create2.json` & `evm-trace-0.1.3/tests/data/parity/create2.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/create_revert.json` & `evm-trace-0.1.3/tests/data/parity/create_revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/error.json` & `evm-trace-0.1.3/tests/data/parity/error.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/revert.json` & `evm-trace-0.1.3/tests/data/parity/revert.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/revert_with_message.json` & `evm-trace-0.1.3/tests/data/parity/revert_with_message.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/data/parity/selfdestruct.json` & `evm-trace-0.1.3/tests/data/parity/selfdestruct.json`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/expected_traces.py` & `evm-trace-0.1.3/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/test_base.py` & `evm-trace-0.1.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/test_gas.py` & `evm-trace-0.1.3/tests/test_gas.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/test_geth.py` & `evm-trace-0.1.3/tests/test_geth.py`

 * *Files identical despite different names*

### Comparing `evm-trace-0.1.2/tests/test_parity.py` & `evm-trace-0.1.3/tests/test_parity.py`

 * *Files identical despite different names*

