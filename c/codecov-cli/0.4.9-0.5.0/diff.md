# Comparing `tmp/codecov-cli-0.4.9.tar.gz` & `tmp/codecov-cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.4.9.tar", last modified: Wed Mar 27 15:10:21 2024, max compression
+gzip compressed data, was "codecov-cli-0.5.0.tar", last modified: Tue Apr  9 17:20:47 2024, max compression
```

## Comparing `codecov-cli-0.4.9.tar` & `codecov-cli-0.5.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.643744 codecov-cli-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-03-27 15:10:21.643744 codecov-cli-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.627745 codecov-cli-0.4.9/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.627745 codecov-cli-0.4.9/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/empty_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/send_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/commands/upload_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.631744 codecov-cli-0.4.9/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.631744 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/git.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.631744 codecov-cli-0.4.9/codecov_cli/helpers/git_services/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/git_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/git_services/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.631744 codecov-cli-0.4.9/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/compress_pycoverage_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/runners/pytest_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/empty_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/empty_upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload/upload_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/codecov_cli/services/upload_completion/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/services/upload_completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.627745 codecov-cli-0.4.9/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 15:10:21.000000 codecov-cli-0.4.9/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.635744 codecov-cli-0.4.9/languages/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.623744 codecov-cli-0.4.9/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.639744 codecov-cli-0.4.9/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-03-27 15:10:08.000000 codecov-cli-0.4.9/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-27 15:10:08.000000 codecov-cli-0.4.9/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.639744 codecov-cli-0.4.9/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-03-27 15:10:08.000000 codecov-cli-0.4.9/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.623744 codecov-cli-0.4.9/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.643744 codecov-cli-0.4.9/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-03-27 15:10:10.000000 codecov-cli-0.4.9/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-27 15:10:10.000000 codecov-cli-0.4.9/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:10:21.643744 codecov-cli-0.4.9/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-03-27 15:10:10.000000 codecov-cli-0.4.9/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:10:21.643744 codecov-cli-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-27 15:10:05.000000 codecov-cli-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.847977 codecov-cli-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18631 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/empty_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/send_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/commands/upload_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.831977 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.831977 codecov-cli-0.5.0/codecov_cli/helpers/git_services/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/git_services/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/compress_pycoverage_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/pytest_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/empty_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/empty_upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload/upload_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.835977 codecov-cli-0.5.0/codecov_cli/services/upload_completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/services/upload_completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.827977 codecov-cli-0.5.0/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 17:20:47.000000 codecov-cli-0.5.0/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2277994 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.839977 codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-09 17:20:37.000000 codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.823977 codecov-cli-0.5.0/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  2658198 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:20:47.843977 codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-09 17:20:38.000000 codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:20:47.847977 codecov-cli-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 17:20:35.000000 codecov-cli-0.5.0/setup.py
```

### Comparing `codecov-cli-0.4.9/LICENSE` & `codecov-cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/PKG-INFO` & `codecov-cli-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.4.9/README.md` & `codecov-cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/base_picking.py` & `codecov-cli-0.5.0/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/commit.py` & `codecov-cli-0.5.0/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.5.0/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/empty_upload.py` & `codecov-cli-0.5.0/codecov_cli/commands/empty_upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.5.0/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.5.0/codecov_cli/commands/labelanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/report.py` & `codecov-cli-0.5.0/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/send_notifications.py` & `codecov-cli-0.5.0/codecov_cli/commands/send_notifications.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.5.0/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/upload.py` & `codecov-cli-0.5.0/codecov_cli/commands/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,14 +160,22 @@
     ),
     click.option(
         "--report-type",
         help="The type of the file to upload, coverage by default. Possible values are: testing, coverage.",
         default="coverage",
         type=click.Choice(["coverage", "test_results"]),
     ),
+    click.option(
+        "--network-filter",
+        help="Specify a filter on the files listed in the network section of the Codecov report. This will only add files whose path begin with the specified filter. Useful for upload-specific path fixing",
+    ),
+    click.option(
+        "--network-prefix",
+        help="Specify a prefix on files listed in the network section of the Codecov report. Useful to help resolve path fixing",
+    ),
 ]
 
 
 def global_upload_options(func):
     for option in reversed(_global_upload_options):
         func = option(func)
     return func
@@ -177,97 +185,103 @@
 @global_upload_options
 @global_options
 @click.pass_context
 def do_upload(
     ctx: click.Context,
     commit_sha: str,
     report_code: str,
+    branch: typing.Optional[str],
     build_code: typing.Optional[str],
     build_url: typing.Optional[str],
-    job_code: typing.Optional[str],
+    disable_file_fixes: bool,
+    disable_search: bool,
+    dry_run: bool,
     env_vars: typing.Dict[str, str],
+    fail_on_error: bool,
+    files_search_exclude_folders: typing.List[pathlib.Path],
+    files_search_explicitly_listed_files: typing.List[pathlib.Path],
+    files_search_root_folder: pathlib.Path,
     flags: typing.List[str],
+    git_service: typing.Optional[str],
+    handle_no_reports_found: bool,
+    job_code: typing.Optional[str],
     name: typing.Optional[str],
+    network_filter: typing.Optional[str],
+    network_prefix: typing.Optional[str],
     network_root_folder: pathlib.Path,
-    files_search_root_folder: pathlib.Path,
-    files_search_exclude_folders: typing.List[pathlib.Path],
-    files_search_explicitly_listed_files: typing.List[pathlib.Path],
-    disable_search: bool,
-    disable_file_fixes: bool,
-    token: typing.Optional[str],
     plugin_names: typing.List[str],
-    branch: typing.Optional[str],
-    slug: typing.Optional[str],
     pull_request_number: typing.Optional[str],
-    use_legacy_uploader: bool,
-    fail_on_error: bool,
-    dry_run: bool,
-    git_service: typing.Optional[str],
-    handle_no_reports_found: bool,
     report_type: str,
+    slug: typing.Optional[str],
+    token: typing.Optional[str],
+    use_legacy_uploader: bool,
 ):
     versioning_system = ctx.obj["versioning_system"]
     codecov_yaml = ctx.obj["codecov_yaml"] or {}
     cli_config = codecov_yaml.get("cli", {})
     ci_adapter = ctx.obj.get("ci_adapter")
     enterprise_url = ctx.obj.get("enterprise_url")
     logger.debug(
         "Starting upload processing",
         extra=dict(
             extra_log_attributes=dict(
-                upload_file_type=report_type,
-                commit_sha=commit_sha,
-                report_code=report_code,
+                branch=branch,
                 build_code=build_code,
                 build_url=build_url,
-                job_code=job_code,
+                commit_sha=commit_sha,
+                disable_file_fixes=disable_file_fixes,
+                disable_search=disable_search,
+                enterprise_url=enterprise_url,
                 env_vars=env_vars,
+                files_search_exclude_folders=files_search_exclude_folders,
+                files_search_explicitly_listed_files=files_search_explicitly_listed_files,
+                files_search_root_folder=files_search_root_folder,
                 flags=flags,
+                git_service=git_service,
+                handle_no_reports_found=handle_no_reports_found,
+                job_code=job_code,
                 name=name,
+                network_filter=network_filter,
+                network_prefix=network_prefix,
                 network_root_folder=network_root_folder,
-                files_search_root_folder=files_search_root_folder,
-                files_search_exclude_folders=files_search_exclude_folders,
-                files_search_explicitly_listed_files=files_search_explicitly_listed_files,
                 plugin_names=plugin_names,
-                token=token,
-                branch=branch,
-                slug=slug,
                 pull_request_number=pull_request_number,
-                git_service=git_service,
-                enterprise_url=enterprise_url,
-                disable_search=disable_search,
-                disable_file_fixes=disable_file_fixes,
-                handle_no_reports_found=handle_no_reports_found,
+                report_code=report_code,
+                slug=slug,
+                token=token,
+                upload_file_type=report_type,
             )
         ),
     )
     do_upload_logic(
         cli_config,
         versioning_system,
         ci_adapter,
-        upload_file_type=report_type,
-        commit_sha=commit_sha,
-        report_code=report_code,
+        branch=branch,
         build_code=build_code,
         build_url=build_url,
-        job_code=job_code,
+        commit_sha=commit_sha,
+        disable_file_fixes=disable_file_fixes,
+        disable_search=disable_search,
+        dry_run=dry_run,
+        enterprise_url=enterprise_url,
         env_vars=env_vars,
+        fail_on_error=fail_on_error,
+        files_search_exclude_folders=list(files_search_exclude_folders),
+        files_search_explicitly_listed_files=list(files_search_explicitly_listed_files),
+        files_search_root_folder=files_search_root_folder,
         flags=flags,
+        git_service=git_service,
+        handle_no_reports_found=handle_no_reports_found,
+        job_code=job_code,
         name=name,
+        network_filter=network_filter,
+        network_prefix=network_prefix,
         network_root_folder=network_root_folder,
-        files_search_root_folder=files_search_root_folder,
-        files_search_exclude_folders=list(files_search_exclude_folders),
-        files_search_explicitly_listed_files=list(files_search_explicitly_listed_files),
         plugin_names=plugin_names,
-        token=token,
-        branch=branch,
-        slug=slug,
         pull_request_number=pull_request_number,
+        report_code=report_code,
+        slug=slug,
+        token=token,
+        upload_file_type=report_type,
         use_legacy_uploader=use_legacy_uploader,
-        fail_on_error=fail_on_error,
-        dry_run=dry_run,
-        git_service=git_service,
-        enterprise_url=enterprise_url,
-        disable_search=disable_search,
-        handle_no_reports_found=handle_no_reports_found,
-        disable_file_fixes=disable_file_fixes,
     )
```

### Comparing `codecov-cli-0.4.9/codecov_cli/commands/upload_process.py` & `codecov-cli-0.5.0/codecov_cli/commands/upload_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     report_code: str,
     build_code: typing.Optional[str],
     build_url: typing.Optional[str],
     job_code: typing.Optional[str],
     env_vars: typing.Dict[str, str],
     flags: typing.List[str],
     name: typing.Optional[str],
+    network_filter: typing.Optional[str],
+    network_prefix: typing.Optional[str],
     network_root_folder: pathlib.Path,
     files_search_root_folder: pathlib.Path,
     files_search_exclude_folders: typing.List[pathlib.Path],
     files_search_explicitly_listed_files: typing.List[pathlib.Path],
     disable_search: bool,
     disable_file_fixes: bool,
     token: typing.Optional[str],
```

### Comparing `codecov-cli-0.4.9/codecov_cli/fallbacks.py` & `codecov-cli-0.5.0/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.5.0/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/config.py` & `codecov-cli-0.5.0/codecov_cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/encoder.py` & `codecov-cli-0.5.0/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.5.0/codecov_cli/helpers/folder_searcher.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/git.py` & `codecov-cli-0.5.0/codecov_cli/helpers/git.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/git_services/github.py` & `codecov-cli-0.5.0/codecov_cli/helpers/git_services/github.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.5.0/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/options.py` & `codecov-cli-0.5.0/codecov_cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/request.py` & `codecov-cli-0.5.0/codecov_cli/helpers/request.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.5.0/codecov_cli/helpers/versioning_systems.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/main.py` & `codecov-cli-0.5.0/codecov_cli/main.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/plugins/__init__.py` & `codecov-cli-0.5.0/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/plugins/compress_pycoverage_contexts.py` & `codecov-cli-0.5.0/codecov_cli/plugins/compress_pycoverage_contexts.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/plugins/gcov.py` & `codecov-cli-0.5.0/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.5.0/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/plugins/xcode.py` & `codecov-cli-0.5.0/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/runners/__init__.py` & `codecov-cli-0.5.0/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.5.0/codecov_cli/runners/dan_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/runners/pytest_standard_runner.py` & `codecov-cli-0.5.0/codecov_cli/runners/pytest_standard_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/runners/types.py` & `codecov-cli-0.5.0/codecov_cli/runners/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.5.0/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/empty_upload/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/empty_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/report/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/general.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/general.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/javascript_es6/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.5.0/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/upload/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,53 +21,60 @@
 
 
 def do_upload_logic(
     cli_config: typing.Dict,
     versioning_system: VersioningSystemInterface,
     ci_adapter: CIAdapterBase,
     *,
-    commit_sha: str,
-    report_code: str,
+    branch: typing.Optional[str],
     build_code: typing.Optional[str],
     build_url: typing.Optional[str],
-    job_code: typing.Optional[str],
+    commit_sha: str,
+    disable_file_fixes: bool = False,
+    disable_search: bool = False,
+    dry_run: bool = False,
+    enterprise_url: typing.Optional[str],
     env_vars: typing.Dict[str, str],
+    fail_on_error: bool = False,
+    files_search_exclude_folders: typing.List[Path],
+    files_search_explicitly_listed_files: typing.List[Path],
+    files_search_root_folder: Path,
     flags: typing.List[str],
+    git_service: typing.Optional[str],
+    handle_no_reports_found: bool = False,
+    job_code: typing.Optional[str],
     name: typing.Optional[str],
+    network_filter: typing.Optional[str],
+    network_prefix: typing.Optional[str],
     network_root_folder: Path,
-    files_search_root_folder: Path,
-    files_search_exclude_folders: typing.List[Path],
-    files_search_explicitly_listed_files: typing.List[Path],
     plugin_names: typing.List[str],
-    token: str,
-    branch: typing.Optional[str],
-    slug: typing.Optional[str],
     pull_request_number: typing.Optional[str],
+    report_code: str,
+    slug: typing.Optional[str],
+    token: str,
     upload_file_type: str = "coverage",
     use_legacy_uploader: bool = False,
-    fail_on_error: bool = False,
-    dry_run: bool = False,
-    git_service: typing.Optional[str],
-    enterprise_url: typing.Optional[str],
-    disable_search: bool = False,
-    handle_no_reports_found: bool = False,
-    disable_file_fixes: bool = False,
 ):
     if upload_file_type == "coverage":
         preparation_plugins = select_preparation_plugins(cli_config, plugin_names)
     elif upload_file_type == "test_results":
         preparation_plugins = []
     file_selector = select_file_finder(
         files_search_root_folder,
         files_search_exclude_folders,
         files_search_explicitly_listed_files,
         disable_search,
         upload_file_type,
     )
-    network_finder = select_network_finder(versioning_system)
+    network_finder = select_network_finder(
+        versioning_system,
+        network_filter=network_filter,
+        network_prefix=network_prefix,
+        network_root_folder=network_root_folder,
+    )
     collector = UploadCollector(
         preparation_plugins, network_finder, file_selector, disable_file_fixes
     )
     try:
         upload_data = collector.generate_upload_data(upload_file_type)
     except click.ClickException as exp:
         if handle_no_reports_found:
```

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload/file_finder.py` & `codecov-cli-0.5.0/codecov_cli/services/upload/file_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.5.0/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.5.0/codecov_cli/services/upload/upload_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         disable_file_fixes: bool = False,
     ):
         self.preparation_plugins = preparation_plugins
         self.network_finder = network_finder
         self.file_finder = file_finder
         self.disable_file_fixes = disable_file_fixes
 
-    def _produce_file_fixes_for_network(
-        self, network: typing.List[str]
+    def _produce_file_fixes(
+        self, files: typing.List[str]
     ) -> typing.List[UploadCollectionResultFileFixer]:
-        if not network or self.disable_file_fixes:
+        if not files or self.disable_file_fixes:
             return []
         # patterns that we don't need to specify a reason for
         empty_line_regex = re.compile(r"^\s*$")
         comment_regex = re.compile(r"^\s*\/\/.*$")
         bracket_regex = re.compile(r"^\s*[\{\}]\s*(\/\/.*)?$")
         list_regex = re.compile(r"^\s*[\]\[]\s*(\/\/.*)?$")
         go_function_regex = re.compile(r"^\s*func\s*[\{]\s*(\/\/.*)?$")
@@ -90,15 +90,15 @@
             "*.hpp": cpp_swift_vala_patterns_to_apply,
             "*.m": cpp_swift_vala_patterns_to_apply,
             "*.swift": cpp_swift_vala_patterns_to_apply,
             "*.vala": cpp_swift_vala_patterns_to_apply,
         }
 
         result = []
-        for filename in network:
+        for filename in files:
             for glob, fix_patterns in file_regex_patterns.items():
                 if fnmatch(filename, glob):
                     result.append(self._get_file_fixes(filename, fix_patterns))
                     break
 
         return result
 
@@ -146,31 +146,31 @@
 
     def generate_upload_data(self, report_type="coverage") -> UploadCollectionResult:
         for prep in self.preparation_plugins:
             logger.debug(f"Running preparation plugin: {type(prep)}")
             prep.run_preparation(self)
         logger.debug("Collecting relevant files")
         network = self.network_finder.find_files()
-        files = self.file_finder.find_files()
-        logger.info(f"Found {len(files)} {report_type} files to upload")
-        if not files:
+        report_files = self.file_finder.find_files()
+        logger.info(f"Found {len(report_files)} {report_type} files to report")
+        if not report_files:
             if report_type == "test_results":
                 error_message = "No JUnit XML reports found. Please review our documentation (https://docs.codecov.com/docs/test-result-ingestion-beta) to generate and upload the file."
             else:
                 error_message = "No coverage reports found. Please make sure you're generating reports successfully."
             raise click.ClickException(
                 click.style(
                     error_message,
                     fg="red",
                 )
             )
-        for file in files:
+        for file in report_files:
             logger.info(f"> {file}")
         return UploadCollectionResult(
             network=network,
-            files=files,
+            files=report_files,
             file_fixes=(
-                self._produce_file_fixes_for_network(network)
+                self._produce_file_fixes(self.network_finder.find_files(True))
                 if report_type == "coverage"
                 else []
             ),
         )
```

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.5.0/codecov_cli/services/upload/upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/services/upload_completion/__init__.py` & `codecov-cli-0.5.0/codecov_cli/services/upload_completion/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli/types.py` & `codecov-cli-0.5.0/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.5.0/codecov_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.4.9
+Version: 0.5.0
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `codecov-cli-0.4.9/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.5.0/codecov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.5.0/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.5.0/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.5.0/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterpython/src/parser.c` & `codecov-cli-0.5.0/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.5.0/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.5.0/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.4.9/setup.py` & `codecov-cli-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.4.9",
+    version="0.5.0",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=[
```

