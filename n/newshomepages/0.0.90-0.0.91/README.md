# Comparing `tmp/newshomepages-0.0.90.tar.gz` & `tmp/newshomepages-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newshomepages-0.0.90.tar", last modified: Tue Mar 19 09:58:20 2024, max compression
+gzip compressed data, was "newshomepages-0.0.91.tar", last modified: Tue Apr  9 19:12:12 2024, max compression
```

## Comparing `newshomepages-0.0.90.tar` & `newshomepages-0.0.91.tar`

### file list

```diff
@@ -1,635 +1,635 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.271146 newshomepages-0.0.90/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.139145 newshomepages-0.0.90/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.devcontainer/postCreateCommand.sh
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.139145 newshomepages-0.0.90/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.143145 newshomepages-0.0.90/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/ISSUE_TEMPLATE/add-a-site.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/ISSUE_TEMPLATE/report-a-broken-site.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.143145 newshomepages-0.0.90/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.github/workflows/site.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-19 09:57:58.000000 newshomepages-0.0.90/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-03-19 09:57:58.000000 newshomepages-0.0.90/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-19 09:57:58.000000 newshomepages-0.0.90/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 09:57:58.000000 newshomepages-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-19 09:57:58.000000 newshomepages-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-19 09:57:58.000000 newshomepages-0.0.90/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-19 09:58:20.271146 newshomepages-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-19 09:57:58.000000 newshomepages-0.0.90/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)   202742 2024-03-19 09:57:58.000000 newshomepages-0.0.90/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-19 09:57:58.000000 newshomepages-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-19 09:57:58.000000 newshomepages-0.0.90/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-19 09:57:58.000000 newshomepages-0.0.90/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.143145 newshomepages-0.0.90/newshomepages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/adstxt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/drudge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/lighthouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/analyze/us_right_wing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.131145 newshomepages-0.0.90/newshomepages/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.127145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/bn/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/bn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ca/
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ca/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.147145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (127)    32176 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/el/
--rw-r--r--   0 runner    (1001) docker     (127)    35861 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/el/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es_419/
--rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es_419/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (127)    24231 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fil/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fil/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (127)    34308 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (127)    35288 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hi/
--rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (127)    32258 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.151146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/kn/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/kn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/lv/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/lv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/mk-MK/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ms/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ms/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nb/
--rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nb/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (127)    33052 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (127)    33333 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (127)    33424 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (127)    40337 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sr-Latn/
--rw-r--r--   0 runner    (1001) docker     (127)    31450 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ta/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ta/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/te/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/te/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.155146 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/th/
--rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/th/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (127)    33471 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (127)    39572 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (127)    35067 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.131145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/alert-popup.css
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/c3.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.159145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/layout.css
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/log.css
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/nanobar.css
--rw-r--r--   0 runner    (1001) docker     (127)    54145 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.163145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    66004 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    66708 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    65764 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.163145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/gray-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/gray-38.png
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-128.png
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-38.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.167146 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/app-store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/avatar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/chrome.svg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/cross.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/dropbox.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/filters.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/google-play.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/hero-green.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/hero-red.svg
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo-shield.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/reload-ico.svg
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/shield.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/tick.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/trash.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.167146 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/js/preload-theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.131145 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.167146 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/libs/scriptlets/
--rw-r--r--   0 runner    (1001) docker     (127)   141578 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.167146 newshomepages-0.0.90/newshomepages/extensions/adguard/content-script/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/content-script/subscribe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.199146 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/
--rw-r--r--   0 runner    (1001) docker     (127)  1206317 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    73188 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   313462 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    94026 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)   402899 2024-03-19 09:57:58.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2213341 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)   928335 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)   774091 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4655227 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   735758 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_224.txt
--rw-r--r--   0 runner    (1001) docker     (127)   914459 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   585242 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   496599 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_6.txt
--rw-r--r--   0 runner    (1001) docker     (127)   271134 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_7.txt
--rw-r--r--   0 runner    (1001) docker     (127)    69106 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_8.txt
--rw-r--r--   0 runner    (1001) docker     (127)   237431 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_9.txt
--rw-r--r--   0 runner    (1001) docker     (127)   483303 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    67127 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   256792 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    71645 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)   363915 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1223256 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)   899376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)   341390 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1640295 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   710272 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
--rw-r--r--   0 runner    (1001) docker     (127)   806171 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   361755 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   193843 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
--rw-r--r--   0 runner    (1001) docker     (127)   249182 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
--rw-r--r--   0 runner    (1001) docker     (127)    58256 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191331 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
--rw-r--r--   0 runner    (1001) docker     (127)    51441 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filters.json
--rw-r--r--   0 runner    (1001) docker     (127)   799078 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filters_i18n.json
--rw-r--r--   0 runner    (1001) docker     (127)  1545375 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/filters/local_script_rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.215146 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/ad-blocked.html
--rw-r--r--   0 runner    (1001) docker     (127)   177876 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/ad-blocked.js
--rw-r--r--   0 runner    (1001) docker     (127)   650939 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/background.html
--rw-r--r--   0 runner    (1001) docker     (127)  3189967 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/background.js
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/content-script-end.js
--rw-r--r--   0 runner    (1001) docker     (127)   288034 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/content-script-start.js
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools.html
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filter-download.html
--rw-r--r--   0 runner    (1001) docker     (127)    62185 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filter-download.js
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filtering-log.html
--rw-r--r--   0 runner    (1001) docker     (127)  1408341 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filtering-log.js
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
--rw-r--r--   0 runner    (1001) docker     (127)   582536 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/options.html
--rw-r--r--   0 runner    (1001) docker     (127)  1079105 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/options.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/popup.html
--rw-r--r--   0 runner    (1001) docker     (127)  1072410 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/popup.js
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/safebrowsing.html
--rw-r--r--   0 runner    (1001) docker     (127)   177879 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/safebrowsing.js
--rw-r--r--   0 runner    (1001) docker     (127)    62942 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/pages/thankyou.js
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.215146 newshomepages-0.0.90/newshomepages/extensions/adguard/shared/
--rw-r--r--   0 runner    (1001) docker     (127)  1063347 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/shared/editor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.219146 newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)   176243 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/mobx.js
--rw-r--r--   0 runner    (1001) docker     (127)   135893 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/react.js
--rw-r--r--   0 runner    (1001) docker     (127)    50712 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/xstate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.131145 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.135145 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.227146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/no/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/no/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.231146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.135145 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.235146 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/content-script.js
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/options.js
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/popup.css
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/popup.html
--rw-r--r--   0 runner    (1001) docker     (127)   158820 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extensions/adguardextra/userscript.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.235146 newshomepages-0.0.90/newshomepages/extract/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/consolidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/hyperlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/lighthouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/extract/wayback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/hyperlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.239146 newshomepages-0.0.90/newshomepages/site/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/accessibility_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/bundle_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/bundle_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/country_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/country_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/drudge.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/language_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/language_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/latest_screenshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/performance_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/site_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/source_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/site/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.239146 newshomepages-0.0.90/newshomepages/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/bundles.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.271146 newshomepages-0.0.90/newshomepages/sources/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/20minutes.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/404mediaco.js
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/abc_es.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/adnkronos.js
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/andscape.js
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/arthasarokar.js
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/asahi.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/baltimorebanner.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/baltimoremag.js
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/baltimoresun.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/bariweiss.js
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/bbc.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/blaw.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/bloombergjapan.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/bonginoreport.js
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/breitbartnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/calgaryherald.js
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/capradionews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/cbcnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/chess24com.js
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/chicagotribune.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/civilbeat.js
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/cnn.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/corriere.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/crucessunnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/daily_record.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/dailycaller.js
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/dailymirror.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/dallasnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/diariope.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/dmregister.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/drudge.js
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/el_universal_mx.js
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/elcorreo_com.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/eltiempo.js
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/estadao.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/examinationnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/financialpost.js
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/fiquemsabendo.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/firstthingsmag.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/fortunemagazine.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/foxnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/france24.js
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/france24_en.js
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/franceinfo.js
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/frednewspost.js
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/ft.js
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/gazettedotcom.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/gbpressgazette.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/georgiastraight.js
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/gfherald.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/globalnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/globeandmail.js
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/gridnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/guardian.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/harpers.js
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/htrnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/humanevents.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/ilmanifesto.js
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/independent.js
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/izvestia_ru.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/jdemontreal.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/jessicavalenti.js
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/jornaloglobo.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/journalsentinel.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/kcautv.js
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/kccinews.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/kpbs.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/kpcc.js
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/laist.js
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lajornada.js
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lanacion.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/larazon_es.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lastampa.js
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/latimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lavozdegalicia.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/le_figaro.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/le_parisien.js
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/ledevoir.js
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lehuffpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lemonde_en.js
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lemondefr.js
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/libe.js
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lobs.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/lp_lapresse.js
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/maroelamedia.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/mediapart.js
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/moreperfectus.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/motherjones.js
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/msnbc.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/mtlgazette.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/mtnstspotlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nationalpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nbcnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/news_letter.js
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/newshour.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nhk_news.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nikkei.js
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/ntdaily.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nybooks.js
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/nytimes.js
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/oann.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/occrp.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/opensecretsdc.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/openvallejo.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/ottawacitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/pajaropolitico.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/pioneerpress.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/platformer.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/postcrescent.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/presscitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/propublica.js
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/publicintegrity.js
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/pulitzercenter.js
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/qctimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/realdailywire.js
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/repubblica.js
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/rfi.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sahanjournal.js
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sankei_news.js
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sdut.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/seikyoofficial.js
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sfchronicle.js
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sjvwater.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sowetanlive.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/spotlightpa.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/sputnikint.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/startribune.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/statnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/stevenspointjrl.js
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/teamtrace.js
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/telegraph.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theathletic.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thebabylonbee.js
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theblaze.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thedbk.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thedispatch.js
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theeconomist.js
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thehilltimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theintercept.js
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theinterceptbr.js
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theonion.js
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thephilacitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/theriotimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thesun.js
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thetimes.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thetorontosun.js
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thetriibe.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/thewrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/timeslive.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/torontostar.js
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/tribunedelyon.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/usatoday.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/uvaldenews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/vancouversun.js
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/vcstar.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/votebeatus.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/vryeweekblad.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/washingtonpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/wcfcourier.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/wonkette.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/javascript/zerohora.js
--rw-r--r--   0 runner    (1001) docker     (127)   115071 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/sources/sites.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/telegrammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/toot.py
--rw-r--r--   0 runner    (1001) docker     (127)    29225 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-19 09:57:59.000000 newshomepages-0.0.90/newshomepages/wayback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:20.271146 newshomepages-0.0.90/newshomepages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26988 2024-03-19 09:58:20.000000 newshomepages-0.0.90/newshomepages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-19 09:58:19.000000 newshomepages-0.0.90/newshomepages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 09:58:20.271146 newshomepages-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-19 09:57:59.000000 newshomepages-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.devcontainer/postCreateCommand.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/add-a-site.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/report-a-broken-site.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/workflows/site.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-09 19:11:53.000000 newshomepages-0.0.91/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 19:11:53.000000 newshomepages-0.0.91/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 19:11:53.000000 newshomepages-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 19:11:53.000000 newshomepages-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 19:12:12.321858 newshomepages-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)   203048 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 19:11:53.000000 newshomepages-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 19:11:53.000000 newshomepages-0.0.91/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 19:11:53.000000 newshomepages-0.0.91/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/adstxt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/drudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/lighthouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/us_right_wing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bn/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (127)    32176 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/
+-rw-r--r--   0 runner    (1001) docker     (127)    35861 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/
+-rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    24231 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fil/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fil/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)    34308 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (127)    35288 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (127)    32258 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/kn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/mk-MK/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)    33052 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (127)    33333 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)    33424 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)    40337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/
+-rw-r--r--   0 runner    (1001) docker     (127)    31450 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ta/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/te/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/te/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)    33471 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    39572 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)    35067 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/alert-popup.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/c3.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/layout.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/log.css
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/nanobar.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54145 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    66004 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    66708 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    65764 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-38.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/app-store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/avatar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/chrome.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/dropbox.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/filters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/google-play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-green.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-red.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-shield.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/shield.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/tick.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/trash.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/preload-theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/
+-rw-r--r--   0 runner    (1001) docker     (127)   141578 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/subscribe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.257858 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)  1206317 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    73188 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   313462 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    94026 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   402899 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2213341 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   928335 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   774091 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4655227 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   735758 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   914459 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   585242 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   496599 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   271134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    69106 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   237431 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   483303 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67127 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   256792 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    71645 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   363915 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1223256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   899376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   341390 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1640295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   710272 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   806171 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   361755 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   193843 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   249182 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    58256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191331 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    51441 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   799078 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters_i18n.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1545375 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/local_script_rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.html
+-rw-r--r--   0 runner    (1001) docker     (127)   177876 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.js
+-rw-r--r--   0 runner    (1001) docker     (127)   650939 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.html
+-rw-r--r--   0 runner    (1001) docker     (127)  3189967 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-end.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288034 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-start.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.html
+-rw-r--r--   0 runner    (1001) docker     (127)    62185 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.js
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1408341 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.js
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
+-rw-r--r--   0 runner    (1001) docker     (127)   582536 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1079105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1072410 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.js
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.html
+-rw-r--r--   0 runner    (1001) docker     (127)   177879 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62942 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/thankyou.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)  1063347 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/shared/editor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)   176243 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/mobx.js
+-rw-r--r--   0 runner    (1001) docker     (127)   135893 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/react.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50712 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/xstate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.193858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.193858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/content-script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.css
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)   158820 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/userscript.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.293858 newshomepages-0.0.91/newshomepages/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/consolidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/hyperlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/lighthouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/hyperlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.293858 newshomepages-0.0.91/newshomepages/site/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/accessibility_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/bundle_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/bundle_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/country_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/country_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/drudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/language_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/language_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/latest_screenshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/performance_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/site_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/source_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.297858 newshomepages-0.0.91/newshomepages/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/bundles.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/newshomepages/sources/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/20minutes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/404mediaco.js
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/abc_es.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/adnkronos.js
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/andscape.js
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/arthasarokar.js
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/asahi.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimorebanner.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimoremag.js
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimoresun.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bariweiss.js
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/blaw.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bloombergjapan.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bonginoreport.js
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/breitbartnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/calgaryherald.js
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/capradionews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/cbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/chess24com.js
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/chicagotribune.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/civilbeat.js
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/cnn.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/corriere.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/crucessunnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/daily_record.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dailycaller.js
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dailymirror.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dallasnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/diariope.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dmregister.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/drudge.js
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/el_universal_mx.js
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/elcorreo_com.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/eltiempo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/estadao.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/examinationnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/financialpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/fiquemsabendo.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/firstthingsmag.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/fortunemagazine.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/foxnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/france24.js
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/france24_en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/franceinfo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/frednewspost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ft.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gazettedotcom.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gbpressgazette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/georgiastraight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gfherald.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/globalnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/globeandmail.js
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gridnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/guardian.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/harpers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/htrnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/humanevents.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ilmanifesto.js
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/independent.js
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/izvestia_ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jdemontreal.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jessicavalenti.js
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jornaloglobo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/journalsentinel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kcautv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kccinews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kpbs.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kpcc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/laist.js
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lajornada.js
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lanacion.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/larazon_es.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lastampa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/latimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lavozdegalicia.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/le_figaro.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/le_parisien.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ledevoir.js
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lehuffpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lemonde_en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lemondefr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/libe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lobs.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lp_lapresse.js
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/maroelamedia.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mediapart.js
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/moreperfectus.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/motherjones.js
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/msnbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mtlgazette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mtnstspotlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nationalpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/news_letter.js
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/newshour.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nhk_news.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nikkei.js
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ntdaily.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nybooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nytimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/oann.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/occrp.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/opensecretsdc.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/openvallejo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ottawacitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pajaropolitico.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pioneerpress.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/platformer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/postcrescent.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/presscitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/propublica.js
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/publicintegrity.js
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pulitzercenter.js
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/qctimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/realdailywire.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/repubblica.js
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/rfi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sahanjournal.js
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sankei_news.js
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sdut.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/seikyoofficial.js
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sfchronicle.js
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sjvwater.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sowetanlive.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/spotlightpa.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sputnikint.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/startribune.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/statnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/stevenspointjrl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/teamtrace.js
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/telegraph.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theathletic.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thebabylonbee.js
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theblaze.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thedbk.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thedispatch.js
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theeconomist.js
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thehilltimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theintercept.js
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theinterceptbr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theonion.js
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thephilacitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theriotimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thesun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetorontosun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetriibe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thewrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/timeslive.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/torontostar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/tribunedelyon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/usatoday.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/uvaldenews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vancouversun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vcstar.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/votebeatus.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vryeweekblad.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/washingtonpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/wcfcourier.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/wonkette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/zerohora.js
+-rw-r--r--   0 runner    (1001) docker     (127)   115162 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/sites.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/telegrammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/toot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29225 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/wayback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/newshomepages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26988 2024-04-09 19:12:12.000000 newshomepages-0.0.91/newshomepages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:12:12.321858 newshomepages-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-09 19:11:53.000000 newshomepages-0.0.91/setup.py
```

### Comparing `newshomepages-0.0.90/.github/ISSUE_TEMPLATE/add-a-site.yaml` & `newshomepages-0.0.91/.github/ISSUE_TEMPLATE/add-a-site.yaml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/.github/workflows/continuous-deployment.yml` & `newshomepages-0.0.91/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/.github/workflows/site.yml` & `newshomepages-0.0.91/.github/workflows/site.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/.gitignore` & `newshomepages-0.0.91/.gitignore`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/.pre-commit-config.yaml` & `newshomepages-0.0.91/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/CODE_OF_CONDUCT.md` & `newshomepages-0.0.91/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/LICENSE` & `newshomepages-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/Makefile` & `newshomepages-0.0.91/Makefile`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/PKG-INFO` & `newshomepages-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.90
+Version: 0.0.91
 Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
```

### Comparing `newshomepages-0.0.90/Pipfile` & `newshomepages-0.0.91/Pipfile`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/Pipfile.lock` & `newshomepages-0.0.91/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970568783068782%*

 * *Differences: {"'default'": "{'playwright': {'hashes': "*

 * *              "['sha256:283887f0bdd0039c3d720e32fbc73a045c24fa800599a6ad60fb199c29580534', "*

 * *              "'sha256:313f2551a772f57c9ccca017c4dd4661f2277166f9e1d84bbf5a2e316f0f892c', "*

 * *              "'sha256:4e1fc1c049a0af64626ddd50814d14a01f316bcbb4d1aa83c3416fe420add558', "*

 * *              "'sha256:b2a46a24641e5d468046cde567c98fdb8d85e32df901630b14dfb288cbd1ed4f', "*

 * *              "'sha256:dbf473496808d4c2c816902c1dee2aabc029648e56ce8514b643f5a1a6fc8e22', "*

 * *         […]*

```diff
@@ -781,24 +781,25 @@
                 "sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868"
             ],
             "index": "pypi",
             "version": "==10.2.0"
         },
         "playwright": {
             "hashes": [
-                "sha256:0608717cbf291a625ba6f751061af0fc0cc9bdace217e69d87b1eb1383b03406",
-                "sha256:431e3a05f8c99147995e2b3e8475d07818745294fd99f1510b61756e73bdcf68",
-                "sha256:4bf214d812092cf5b9b9648ba84611aa35e28685519911342a7da3a3031f9ed6",
-                "sha256:71ead0f33e00f5a8533c037c647938b99f219436a1b27d4ba4de4e6bf0567278",
-                "sha256:cf68335a5dfa4038fa797a4ba0105faee0094ebbb372547d7a27feec5b23c672",
-                "sha256:eaa17ab44622c447de26ed8f7d99912719568d8dbc3a9db0e07f0ae1487709d9",
-                "sha256:edb210a015e70bb0d328bf1c9b65fa3a08361f33e4d7c4ddd1ad2adb6d9b4479"
+                "sha256:283887f0bdd0039c3d720e32fbc73a045c24fa800599a6ad60fb199c29580534",
+                "sha256:313f2551a772f57c9ccca017c4dd4661f2277166f9e1d84bbf5a2e316f0f892c",
+                "sha256:4e1fc1c049a0af64626ddd50814d14a01f316bcbb4d1aa83c3416fe420add558",
+                "sha256:b2a46a24641e5d468046cde567c98fdb8d85e32df901630b14dfb288cbd1ed4f",
+                "sha256:dbf473496808d4c2c816902c1dee2aabc029648e56ce8514b643f5a1a6fc8e22",
+                "sha256:e092c6cfbf797bff03fbdfc53c3e6a9e29fbcf6b82f9e43113d37494aee0561b",
+                "sha256:e2b293f077efeaa45253fde31cea4bc6b0ae8be6b5e65e8ce8b4aa3b9f0d55b6"
             ],
             "index": "pypi",
-            "version": "==1.41.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.42.0"
         },
         "preshed": {
             "hashes": [
                 "sha256:0de63a560f10107a3f0a9e252cc3183b8fdedcb5f81a86938fd9f1dcf8a64adf",
                 "sha256:182138033c0730c683a6d97e567ceb8a3e83f3bff5704f300d582238dbd384b3",
                 "sha256:1fa6d3d5529b08296ff9b7b4da1485c080311fd8744bbf3a86019ff88007b382",
                 "sha256:23906d114fc97c17c5f8433342495d7562e96ecfd871289c2bb2ed9a9df57c3f",
@@ -1673,69 +1674,69 @@
             "version": "==0.2.1"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa",
-                "sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003",
-                "sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f",
-                "sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c",
-                "sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e",
-                "sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0",
-                "sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9",
-                "sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52",
-                "sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e",
-                "sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454",
-                "sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0",
-                "sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079",
-                "sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352",
-                "sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f",
-                "sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30",
-                "sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe",
-                "sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113",
-                "sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765",
-                "sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc",
-                "sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e",
-                "sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501",
-                "sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7",
-                "sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2",
-                "sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f",
-                "sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4",
-                "sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524",
-                "sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c",
-                "sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51",
-                "sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840",
-                "sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6",
-                "sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee",
-                "sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e",
-                "sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45",
-                "sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba",
-                "sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d",
-                "sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3",
-                "sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10",
-                "sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e",
-                "sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb",
-                "sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9",
-                "sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a",
-                "sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47",
-                "sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1",
-                "sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3",
-                "sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914",
-                "sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328",
-                "sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6",
-                "sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d",
-                "sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0",
-                "sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94",
-                "sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc",
-                "sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2"
+                "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c",
+                "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63",
+                "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7",
+                "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f",
+                "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8",
+                "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf",
+                "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0",
+                "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384",
+                "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76",
+                "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7",
+                "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d",
+                "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70",
+                "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f",
+                "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818",
+                "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b",
+                "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d",
+                "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec",
+                "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083",
+                "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2",
+                "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9",
+                "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd",
+                "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade",
+                "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e",
+                "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a",
+                "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227",
+                "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87",
+                "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c",
+                "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e",
+                "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c",
+                "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e",
+                "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd",
+                "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec",
+                "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562",
+                "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8",
+                "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677",
+                "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357",
+                "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c",
+                "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd",
+                "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49",
+                "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286",
+                "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1",
+                "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf",
+                "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51",
+                "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409",
+                "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384",
+                "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e",
+                "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978",
+                "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57",
+                "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e",
+                "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2",
+                "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48",
+                "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==7.4.3"
+            "version": "==7.4.4"
         },
         "cryptography": {
             "hashes": [
                 "sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee",
                 "sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576",
                 "sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d",
                 "sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30",
@@ -1824,19 +1825,19 @@
                 "sha256:eac49ca94516ccc753f9fb5ce82603156e590b27525a8bc32cce8ae302eb61bc"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==2.0.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e",
-                "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"
+                "sha256:5ffa845303983e7a0b7ae17636509bc97997d58afeafa72fb141a17b152284cb",
+                "sha256:a79895a25bbefdf55d1a2a0a80968f7dbb28edcd6d4234a0afb3f37ecde4b546"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.13.1"
+            "version": "==3.13.3"
         },
         "flake8": {
             "hashes": [
                 "sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132",
                 "sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3"
             ],
             "index": "pypi",
@@ -2185,44 +2186,45 @@
                 "sha256:fe5d7785250541f7f5019ab9cba2c71169dc7d74d0f45253f8313f436458a4ef"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.5"
         },
         "mypy": {
             "hashes": [
-                "sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6",
-                "sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d",
-                "sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02",
-                "sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d",
-                "sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3",
-                "sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3",
-                "sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3",
-                "sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66",
-                "sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259",
-                "sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835",
-                "sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd",
-                "sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d",
-                "sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8",
-                "sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07",
-                "sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b",
-                "sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e",
-                "sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6",
-                "sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae",
-                "sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9",
-                "sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d",
-                "sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a",
-                "sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592",
-                "sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218",
-                "sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817",
-                "sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4",
-                "sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410",
-                "sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55"
+                "sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6",
+                "sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913",
+                "sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129",
+                "sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc",
+                "sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974",
+                "sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374",
+                "sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150",
+                "sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03",
+                "sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9",
+                "sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02",
+                "sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89",
+                "sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2",
+                "sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d",
+                "sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3",
+                "sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612",
+                "sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e",
+                "sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3",
+                "sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e",
+                "sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd",
+                "sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04",
+                "sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed",
+                "sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185",
+                "sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf",
+                "sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b",
+                "sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4",
+                "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f",
+                "sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6"
             ],
             "index": "pypi",
-            "version": "==1.8.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.9.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -2305,19 +2307,19 @@
                 "sha256:ffa75af20b44f8dba823498024771d5ac50620e6915abac414251bd971b4529f"
             ],
             "markers": "python_version >= '3.9'",
             "version": "==1.26.4"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pandas": {
             "hashes": [
                 "sha256:04f6ec3baec203c13e3f8b139fb0f9f86cd8c0b94603ae3ae8ce9a422e9f5bee",
                 "sha256:06cf591dbaefb6da9de8472535b185cba556d0ce2e6ed28e21d919704fef1a9e",
                 "sha256:0ab90f87093c13f3e8fa45b48ba9f39181046e8f3317d3aadb2fffbb1b978572",
                 "sha256:0f573ab277252ed9aaf38240f3b54cfc90fff8e5cab70411ee1d03f5d51f3944",
@@ -2395,19 +2397,20 @@
                 "sha256:68597934193c08a08eb2bf6a1d85593f627c22f9b065cc727a4f03f669d96d86",
                 "sha256:9320f1a3c6f7a9133fe3b571f283bcf3353cd70249025ae8d618e40e9f7e92b3"
             ],
             "version": "==0.9.1"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:ba637c2d7a670c10daedc059f5c49b5bd0aadbccfcd7ec15592cf9665117532c",
-                "sha256:c3ef34f463045c88658c5b99f38c1e297abdcc0ff13f98d3370055fbbfabc67e"
+                "sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab",
+                "sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060"
             ],
             "index": "pypi",
-            "version": "==3.6.2"
+            "markers": "python_version >= '3.9'",
+            "version": "==3.7.0"
         },
         "prompt-toolkit": {
             "hashes": [
                 "sha256:3527b7af26106cbc65a040bcc84839a3566ec1b051bb0bfe953631e704b0ff7d",
                 "sha256:a11a29cb3bf0a28a387fe5122cdb649816a957cd9261dcedf8c9f1fef33eacf6"
             ],
             "markers": "python_version >= '3.7'",
@@ -2464,27 +2467,29 @@
                 "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.17.2"
         },
         "pytest": {
             "hashes": [
-                "sha256:d4051d623a2e0b7e51960ba963193b09ce6daeb9759a451844a21e4ddedfc1bd",
-                "sha256:edfaaef32ce5172d5466b5127b42e0d6d35ebbe4453f0e3505d96afd93f6b096"
+                "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7",
+                "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"
             ],
             "index": "pypi",
-            "version": "==8.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==8.1.1"
         },
         "pytest-cov": {
             "hashes": [
-                "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
-                "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
+                "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
+                "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
         "pytest-env": {
             "hashes": [
                 "sha256:aada77e6d09fcfb04540a6e462c58533c37df35fa853da78707b17ec04d17dfc",
                 "sha256:fcd7dc23bb71efd3d35632bde1bbe5ee8c8dc4489d6617fb010674880d96216b"
             ],
             "index": "pypi",
@@ -2698,19 +2703,19 @@
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:02fa291a0471b3a18b2b2481ed902af520c69e8ae0919c13da936542754b4c56",
-                "sha256:5c0806c7d9af348e6dd3777b4f4dbb42c7ad85b190104837488eab9a7c945cf8"
+                "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
+                "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==69.1.1"
+            "version": "==69.2.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:b47844cd2a84b83b3187a5782c71128c28b4c94cad8bfb871da2784a5cb54c4f",
                 "sha256:b5f43ff6800669595193fd09891564ee9d1d7dcb196cab4b2506d53a2e1c95c7"
             ],
             "index": "pypi",
@@ -2897,19 +2902,20 @@
                 "sha256:c93751ee20dfc6e054a0148f8f5227b9a00b79c90a4d3c9f464711a73179c89e"
             ],
             "index": "pypi",
             "version": "==2024.1.0.20240203"
         },
         "types-pyyaml": {
             "hashes": [
-                "sha256:334373d392fde0fdf95af5c3f1661885fa10c52167b14593eb856289e1855062",
-                "sha256:c05bc6c158facb0676674b7f11fe3960db4f389718e19e62bd2b84d6205cfd24"
+                "sha256:a9e0f0f88dc835739b0c1ca51ee90d04ca2a897a71af79de9aec5f38cb0a5342",
+                "sha256:b845b06a1c7e54b8e5b4c683043de0d9caf205e7434b3edc678ff2411979b8f6"
             ],
             "index": "pypi",
-            "version": "==6.0.12.12"
+            "markers": "python_version >= '3.8'",
+            "version": "==6.0.12.20240311"
         },
         "types-requests": {
             "hashes": [
                 "sha256:a82807ec6ddce8f00fe0e949da6d6bc1fbf1715420218a9640d695f70a9e5a9b",
                 "sha256:f1721dba8385958f504a5386240b92de4734e047a08a40751c1654d1ac3349c5"
             ],
             "index": "pypi",
```

### Comparing `newshomepages-0.0.90/README.md` & `newshomepages-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/accessibility.py` & `newshomepages-0.0.91/newshomepages/accessibility.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/adstxt.py` & `newshomepages-0.0.91/newshomepages/adstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/analyze/drudge.py` & `newshomepages-0.0.91/newshomepages/analyze/drudge.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/analyze/lighthouse.py` & `newshomepages-0.0.91/newshomepages/analyze/lighthouse.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/analyze/us_right_wing.py` & `newshomepages-0.0.91/newshomepages/analyze/us_right_wing.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/archive.py` & `newshomepages-0.0.91/newshomepages/archive.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/batch.py` & `newshomepages-0.0.91/newshomepages/batch.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ar/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/be/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/bg/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ca/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/cs/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/da/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/de/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/el/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/en/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/es_419/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/et/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fa/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fi/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/fr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/he/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hi/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hu/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/hy/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/id/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/it/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ja/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ko/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/lt/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ms/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nb/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/nl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_BR/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/pt_PT/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ro/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/ru/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sk/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/sv/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/th/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/tr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/uk/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/vi/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_CN/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/_locales/zh_TW/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/alert-popup.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/alert-popup.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/c3.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/c3.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/custom.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/custom.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/dark.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/dark.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/layout.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/layout.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/log.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/log.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/css/style.css` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-off-19.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-off-38.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-on-19.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/b13-on-38.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/gray-19.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/gray-38.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-128.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-16.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-19.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/icons/green-38.png` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/alert.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/alert.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/app-store.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/arrow-down.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/avatar.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/avatar.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/checked.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/checked.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/chrome.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/chrome.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/cross.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/cross.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/dropbox.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/dropbox.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/favicon.ico` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/filters.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/filters.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/google-play.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/google-play.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/hero-green.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/hero-red.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-red.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo-dark.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo-shield.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-shield.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/logo_adguard.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo_adguard.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/reload-ico.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/tick.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/tick.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/images/toggler-bg.svg` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/toggler-bg.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/js/preload-theme.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/preload-theme.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml` & `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/content-script/subscribe.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/subscribe.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_1.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_10.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_11.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_12.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_13.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_14.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_15.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_16.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_17.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_2.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_224.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_3.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_4.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_5.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_6.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_7.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_8.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_9.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_1.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_10.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_11.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_12.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_13.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_14.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_15.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_16.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_17.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_2.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_224.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_3.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_4.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_5.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_6.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_7.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_8.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filter_mobile_9.txt` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filters.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/filters_i18n.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters_i18n.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/filters/local_script_rules.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/local_script_rules.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/manifest.json` & `newshomepages-0.0.91/newshomepages/extensions/adguard/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/ad-blocked.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/assistant.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/assistant.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/background.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/content-script-end.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-end.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/content-script-start.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-start.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/devtools.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filter-download.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filter-download.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/filtering-log.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/options.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/options.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/popup.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/safebrowsing.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/safebrowsing.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/pages/thankyou.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/thankyou.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/runtime.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/runtime.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/shared/editor.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/shared/editor.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/mobx.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/mobx.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/react.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/react.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/vendors/xstate.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/xstate.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js` & `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/be/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/cs/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/da/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/de/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/en/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/es/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fi/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/fr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/he/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/hu/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/id/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/it/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ja/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ko/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/lt/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/nl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/no/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ro/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/ru/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sk/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sl/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/sr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/tr/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/uk/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/vi/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_installed.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_installed.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/assets/images/extra_logo.png` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_logo.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/content-script.js` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/content-script.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/manifest.json` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/options.js` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/popup.html` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extensions/adguardextra/userscript.js` & `newshomepages-0.0.91/newshomepages/extensions/adguardextra/userscript.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/accessibility.py` & `newshomepages-0.0.91/newshomepages/extract/accessibility.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/cli.py` & `newshomepages-0.0.91/newshomepages/extract/cli.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/consolidate.py` & `newshomepages-0.0.91/newshomepages/extract/consolidate.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/hyperlinks.py` & `newshomepages-0.0.91/newshomepages/extract/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/items.py` & `newshomepages-0.0.91/newshomepages/extract/items.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/lighthouse.py` & `newshomepages-0.0.91/newshomepages/extract/lighthouse.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/robotstxt.py` & `newshomepages-0.0.91/newshomepages/extract/robotstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/utils.py` & `newshomepages-0.0.91/newshomepages/extract/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/extract/wayback.py` & `newshomepages-0.0.91/newshomepages/extract/wayback.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/hyperlinks.py` & `newshomepages-0.0.91/newshomepages/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/mosaic.py` & `newshomepages-0.0.91/newshomepages/mosaic.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/robotstxt.py` & `newshomepages-0.0.91/newshomepages/robotstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/rss.py` & `newshomepages-0.0.91/newshomepages/rss.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/screenshot.py` & `newshomepages-0.0.91/newshomepages/screenshot.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/accessibility_ranking.py` & `newshomepages-0.0.91/newshomepages/site/accessibility_ranking.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/bundle_detail.py` & `newshomepages-0.0.91/newshomepages/site/bundle_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/cli.py` & `newshomepages-0.0.91/newshomepages/site/cli.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/country_detail.py` & `newshomepages-0.0.91/newshomepages/site/country_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/country_list.py` & `newshomepages-0.0.91/newshomepages/site/country_list.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/drudge.py` & `newshomepages-0.0.91/newshomepages/site/drudge.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/language_detail.py` & `newshomepages-0.0.91/newshomepages/site/language_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/language_list.py` & `newshomepages-0.0.91/newshomepages/site/language_list.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/latest_screenshots.py` & `newshomepages-0.0.91/newshomepages/site/latest_screenshots.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/openai.py` & `newshomepages-0.0.91/newshomepages/site/openai.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/performance_ranking.py` & `newshomepages-0.0.91/newshomepages/site/performance_ranking.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/site_detail.py` & `newshomepages-0.0.91/newshomepages/site/site_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/status_report.py` & `newshomepages-0.0.91/newshomepages/site/status_report.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/site/utils.py` & `newshomepages-0.0.91/newshomepages/site/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/slack.py` & `newshomepages-0.0.91/newshomepages/slack.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/sources/bundles.csv` & `newshomepages-0.0.91/newshomepages/sources/bundles.csv`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/sources/javascript/news_letter.js` & `newshomepages-0.0.91/newshomepages/sources/javascript/news_letter.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/sources/sites.csv` & `newshomepages-0.0.91/newshomepages/sources/sites.csv`

 * *Files 0% similar despite different names*

```diff
@@ -875,14 +875,15 @@
 semafor,https://www.semafor.com/,Semafor,New York City,America/New_York,US,en,,,
 setopati,https://www.setopati.com/,Setopati,Kathmandu,Asia/Kathmandu,NP,ne,,,
 sfchronicle,https://www.sfchronicle.com/,San Francisco Chronicle,San Francisco,America/Los_Angeles,US,en,bay-area|california,,
 sfstandard,https://sfstandard.com/,The San Francisco Standard,San Francisco,America/Los_Angeles,US,en,bay-area|california,,
 sgfcitizen,https://sgfcitizen.org/,Springfield Daily Citizen,Springfield,America/Chicago,US,en,missouri,,
 sheboyganpress,https://www.sheboyganpress.com/,Sheboygan Press,Sheboygan,America/Chicago,US,en,wisconsin|gannett,,
 shelbystar,https://www.shelbystar.com/,The Shelby Star,Shelby,America/New_York,US,en,north-carolina|gannett,,
+sherwood_news,https://sherwood.news/,Sherwood News,New York City,America/New_York,US,en,,,
 shillsalmanac,https://thealmanac.net/,South Hills Almanac,South Hills,America/New_York,US,en,,,
 shinysheet,https://www.palmbeachdailynews.com/,Palm Beach Daily News,West Palm Beach,America/New_York,US,en,florida|gannett,,
 shreveporttimes,https://www.shreveporttimes.com/,Shreveport Times,Shreveport,America/Chicago,US,en,louisiana|gannett,,
 signalcleveland,https://signalcleveland.org/,Signal Cleveland,Cleveland,America/New_York,US,en,,,
 simple_flying,https://simpleflying.com/,Simple Flying,London,Europe/London,GB,en,aviation,,
 sinembargomx,https://www.sinembargo.mx/,SinEmbargo,Mexico City,America/Mexico_City,MX,es,,,
 sinow,https://www.si.com/,Sports Illustrated,New York City,America/New_York,US,en,sports,,
```

### Comparing `newshomepages-0.0.90/newshomepages/telegrammer.py` & `newshomepages-0.0.91/newshomepages/telegrammer.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/toot.py` & `newshomepages-0.0.91/newshomepages/toot.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/utils.py` & `newshomepages-0.0.91/newshomepages/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages/wayback.py` & `newshomepages-0.0.91/newshomepages/wayback.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages.egg-info/PKG-INFO` & `newshomepages-0.0.91/newshomepages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.90
+Version: 0.0.91
 Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
```

### Comparing `newshomepages-0.0.90/newshomepages.egg-info/SOURCES.txt` & `newshomepages-0.0.91/newshomepages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/newshomepages.egg-info/entry_points.txt` & `newshomepages-0.0.91/newshomepages.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.90/setup.py` & `newshomepages-0.0.91/setup.py`

 * *Files identical despite different names*

