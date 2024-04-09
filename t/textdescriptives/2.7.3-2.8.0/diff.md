# Comparing `tmp/textdescriptives-2.7.3.tar.gz` & `tmp/textdescriptives-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.7.3.tar", last modified: Tue Feb  6 10:12:12 2024, max compression
+gzip compressed data, was "textdescriptives-2.8.0.tar", last modified: Tue Apr  9 13:29:22 2024, max compression
```

## Comparing `textdescriptives-2.7.3.tar` & `textdescriptives-2.8.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.424688 textdescriptives-2.7.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.400688 textdescriptives-2.7.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.400688 textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.404688 textdescriptives-2.7.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1247 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2592 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2254 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1396 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)   181770 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    24905 2024-02-06 10:12:12.424688 textdescriptives-2.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9398 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.408688 textdescriptives-2.7.3/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.408688 textdescriptives-2.7.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3547 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2374 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2790 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     7051 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      388 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.408688 textdescriptives-2.7.3/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96689 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    13090 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/tutorials/sklearn_integration.ipynb
--rw-r--r--   0 root         (0) root         (0)     7465 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.412688 textdescriptives-2.7.3/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     2947 2024-02-06 10:12:05.000000 textdescriptives-2.7.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-06 10:12:12.424688 textdescriptives-2.7.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.396688 textdescriptives-2.7.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.412688 textdescriptives-2.7.3/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.416688 textdescriptives-2.7.3/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     8335 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     6231 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4374 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22255 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10427 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     8209 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.416688 textdescriptives-2.7.3/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6127 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/extractors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.416688 textdescriptives-2.7.3/src/textdescriptives/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/integrations/sklearn_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     1331 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.420688 textdescriptives-2.7.3/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24905 2024-02-06 10:12:12.000000 textdescriptives-2.7.3/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2508 2024-02-06 10:12:12.000000 textdescriptives-2.7.3/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 10:12:12.000000 textdescriptives-2.7.3/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      472 2024-02-06 10:12:12.000000 textdescriptives-2.7.3/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-06 10:12:12.000000 textdescriptives-2.7.3/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 10:12:12.420688 textdescriptives-2.7.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1384 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9305 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     5308 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2024-02-06 10:12:04.000000 textdescriptives-2.7.3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.608338 textdescriptives-2.8.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.608338 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.612338 textdescriptives-2.8.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1395 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)   185655 2024-04-09 13:29:19.000000 textdescriptives-2.8.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24980 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9398 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.612338 textdescriptives-2.8.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     7051 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    86776 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    13090 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.616338 textdescriptives-2.8.0/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-04-09 13:29:19.000000 textdescriptives-2.8.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.604339 textdescriptives-2.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.620338 textdescriptives-2.8.0/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     8335 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     6231 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22261 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10429 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     8209 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6127 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.624338 textdescriptives-2.8.0/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6212 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24980 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 13:29:22.000000 textdescriptives-2.8.0/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 13:29:22.628338 textdescriptives-2.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9308 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2024-04-09 13:29:09.000000 textdescriptives-2.8.0/tests/test_utils.py
```

### Comparing `textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.8.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/dependabot.yml` & `textdescriptives-2.8.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.8.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/workflows/documentation.yml` & `textdescriptives-2.8.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/workflows/draft-pdf.yml` & `textdescriptives-2.8.0/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/workflows/release.yml` & `textdescriptives-2.8.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           token: ${{ secrets.RELEASE }}
 
       - name: Python Semantic Release
         id: release
-        uses: python-semantic-release/python-semantic-release@v8.0.4
+        uses: python-semantic-release/python-semantic-release@v9.4.1
         with:
           github_token: ${{ secrets.RELEASE }}
           root_options: "-vv"
 
           # repository_username: __token__
           # repository_password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `textdescriptives-2.7.3/.github/workflows/stale.yml` & `textdescriptives-2.8.0/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.github/workflows/tests.yml` & `textdescriptives-2.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.gitignore` & `textdescriptives-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/.pre-commit-config.yaml` & `textdescriptives-2.8.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.0
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/bwhmather/ssort
-    rev: 0.12.3
+    rev: 0.12.4
     hooks:
       - id: ssort
 
   - repo: https://github.com/asottile/add-trailing-comma
     rev: v3.1.0
     hooks:
       - id: add-trailing-comma
@@ -43,21 +43,21 @@
   #           --wrap-descriptions,
   #           "80",
   #           --wrap-summaries,
   #           "80",
   #         ]
 
   - repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.2.0
     hooks:
       - id: black
         #args: [--line-length, "88"]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.2.1
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.8.0
     hooks:
       - id: mypy
```

### Comparing `textdescriptives-2.7.3/.zenodo.json` & `textdescriptives-2.8.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/CHANGELOG.md` & `textdescriptives-2.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,86 @@
 # CHANGELOG
 
 
 
+## v2.8.0 (2024-04-09)
+
+### Build
+
+* build: update autodoc_pydantic to support pydantic 2 ([`e236d0d`](https://github.com/HLasse/TextDescriptives/commit/e236d0da869a71d331ac3ce19bf5c4e0045520a5))
+
+* build: require pydantic &lt;2.0.0 ([`e18a6aa`](https://github.com/HLasse/TextDescriptives/commit/e18a6aa613fed976bb86ad7010312eccd9c90fb3))
+
+### Ci
+
+* ci: update semrelease version for pydantic support ([`3baa06d`](https://github.com/HLasse/TextDescriptives/commit/3baa06d183733caeb4185f36b80f4438516adb70))
+
+### Documentation
+
+* docs: bin pydantic version in docs building ([`8631fc8`](https://github.com/HLasse/TextDescriptives/commit/8631fc8fe84b29962bc4ecd378c7c32f108b30c7))
+
+### Feature
+
+* feat: bump pydantic version to 2.0 ([`ce91e56`](https://github.com/HLasse/TextDescriptives/commit/ce91e568fe0926593de4b43fde8108f8b7b1da15))
+
+### Fix
+
+* fix: misc ([`844c240`](https://github.com/HLasse/TextDescriptives/commit/844c2403f34c7dcea9f83cfaf764176aac7e674b))
+
+### Unknown
+
+* Merge pull request #326 from HLasse/pydantic-2
+
+feat: bump pydantic version to 2.0 and spacy version to &gt;=3.6 ([`d900c46`](https://github.com/HLasse/TextDescriptives/commit/d900c4656d958b77efc0caaff01038c92836f766))
+
+* tests: update spacy model version for tests to 3.6 ([`4e2029f`](https://github.com/HLasse/TextDescriptives/commit/4e2029f9d0e0cf12ec36d8c8f0ce67bd5f01f24b))
+
+* CI: update sem ver version ([`7b24af8`](https://github.com/HLasse/TextDescriptives/commit/7b24af8fe2bbf549643bedd431f59e340a3e970c))
+
+* deps: update min spacy version to 3.6 ([`d7d5a30`](https://github.com/HLasse/TextDescriptives/commit/d7d5a30ea19a399e3800e94e220264bbd2bb45c8))
+
+* Merge pull request #320 from HLasse/pre-commit-ci-update-config
+
+[pre-commit.ci] pre-commit autoupdate ([`5c7015a`](https://github.com/HLasse/TextDescriptives/commit/5c7015a541c717bd1001637585b65d25ac8ee70d))
+
+* [pre-commit.ci] pre-commit autoupdate
+
+updates:
+- [github.com/bwhmather/ssort: 0.12.3 → 0.12.4](https://github.com/bwhmather/ssort/compare/0.12.3...0.12.4)
+- [github.com/psf/black: 24.1.1 → 24.2.0](https://github.com/psf/black/compare/24.1.1...24.2.0)
+- [github.com/astral-sh/ruff-pre-commit: v0.1.14 → v0.2.1](https://github.com/astral-sh/ruff-pre-commit/compare/v0.1.14...v0.2.1) ([`b6ba478`](https://github.com/HLasse/TextDescriptives/commit/b6ba47829f2b86a0858998570f34e5102fcd5436))
+
+* lint ([`2ec4aa9`](https://github.com/HLasse/TextDescriptives/commit/2ec4aa90e122a65ddc23712afa6cfccd160e4d41))
+
+* Merge branch &#39;pydantic-2&#39; of https://github.com/HLasse/TextDescriptives into pydantic-2
+something? ([`8a5f03e`](https://github.com/HLasse/TextDescriptives/commit/8a5f03e7154904bab75d132d6474e35540936eca))
+
+* tests: fix type ([`7854c8d`](https://github.com/HLasse/TextDescriptives/commit/7854c8da6a6f02db4156e61ed3f17977f20dfd20))
+
+* Merge branch &#39;main&#39; into pydantic-2 ([`8682679`](https://github.com/HLasse/TextDescriptives/commit/8682679b756329054b3c4dffbbb67fbece6c5232))
+
+* Merge pull request #325 from HLasse/HLasse-patch-1
+
+build: require pydantic &lt;2.0.0 ([`8589099`](https://github.com/HLasse/TextDescriptives/commit/8589099fd2a31a138559f0049ea77e7a34cb1aff))
+
+* Merge pull request #322 from HLasse/HLasse/tutorials-quality-tutorial-failing-due-to-DAGW-not-being-available-at-the-moment
+
+tutorials: quality tutorial failing due to DAGW not being available at the moment ([`b23beb2`](https://github.com/HLasse/TextDescriptives/commit/b23beb2adb98c0d0651981e685a63d28509c3428))
+
+* tutorials: quality tutorial failing due to DAGW not being available at the moment
+Fixes #321 ([`fbaa00d`](https://github.com/HLasse/TextDescriptives/commit/fbaa00d0d7ec1a78a0620977a18f54aa17898131))
+
+
+## v2.7.3 (2024-02-06)
+
+### Fix
+
+* fix: pin autodoc_pydantic version to support pydantic version &lt;2 ([`4b91006`](https://github.com/HLasse/TextDescriptives/commit/4b910069491794a1144cd8f9ccf8872879315f75))
+
+
 ## v2.7.2 (2024-02-06)
 
 ### Fix
 
 * fix: update furo to fix doc builidng ([`3e73e61`](https://github.com/HLasse/TextDescriptives/commit/3e73e61a4a734edf7d3cda20ba6a427de48bd8c9))
 
 ### Unknown
```

### Comparing `textdescriptives-2.7.3/CITATION.cff` & `textdescriptives-2.8.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/CODE_OF_CONDUCT.md` & `textdescriptives-2.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/CONTRIBUTING.md` & `textdescriptives-2.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/LICENSE` & `textdescriptives-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/PKG-INFO` & `textdescriptives-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.7.3
+Version: 2.8.0
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,35 +221,37 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: spacy[lookups]>=3.1.0
+Requires-Dist: spacy[lookups]>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pyphen<0.15.0,>=0.11.0
 Requires-Dist: ftfy<6.1.0,>=6.0.3
+Requires-Dist: pydantic>=2.0
 Provides-Extra: style
 Requires-Dist: black==24.1.1; extra == "style"
 Requires-Dist: pre-commit==3.6.0; extra == "style"
 Requires-Dist: ruff==0.1.15; extra == "style"
 Requires-Dist: mypy==1.8.0; extra == "style"
 Provides-Extra: tests
 Requires-Dist: pytest>=7.1.3; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: pydantic==2.1; extra == "docs"
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: furo==2022.12.7; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinxext-opengraph>=0.7.3; extra == "docs"
 Requires-Dist: myst-nb>=0.6.0; extra == "docs"
 Requires-Dist: sphinx_design>=0.3.0; extra == "docs"
-Requires-Dist: autodoc_pydantic==1.9.0; extra == "docs"
+Requires-Dist: autodoc_pydantic==2.1.0; extra == "docs"
 Provides-Extra: tutorials
 Requires-Dist: jupyter; extra == "tutorials"
 Requires-Dist: seaborn; extra == "tutorials"
 Requires-Dist: matplotlib; extra == "tutorials"
 Requires-Dist: datasets>=2.8.0; extra == "tutorials"
 Requires-Dist: scikit-learn>=1.1.1; extra == "tutorials"
 Requires-Dist: ipython<=8.21.0; extra == "tutorials"
```

### Comparing `textdescriptives-2.7.3/README.md` & `textdescriptives-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/Makefile` & `textdescriptives-2.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/_static/icon.png` & `textdescriptives-2.8.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/_static/icon_dark_old.png` & `textdescriptives-2.8.0/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/_static/icon_old.png` & `textdescriptives-2.8.0/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/coherence.rst` & `textdescriptives-2.8.0/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/conf.py` & `textdescriptives-2.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/dependencydistance.rst` & `textdescriptives-2.8.0/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/descriptivestats.rst` & `textdescriptives-2.8.0/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/faq.rst` & `textdescriptives-2.8.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/index.rst` & `textdescriptives-2.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/information_theory.rst` & `textdescriptives-2.8.0/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/installation.rst` & `textdescriptives-2.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/make.bat` & `textdescriptives-2.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/news.rst` & `textdescriptives-2.8.0/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/posstats.rst` & `textdescriptives-2.8.0/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/quality.rst` & `textdescriptives-2.8.0/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/readability.rst` & `textdescriptives-2.8.0/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.8.0/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960884388908583%*

 * *Differences: {"'cells'": "{27: {'source': {insert: [(1, 'We can download the dataset using the following "*

 * *            "command:\\n'), (2, '\\n'), (3, '#### NOTE: The DAGW dataset is currently unavailable "*

 * *            'due to a copyright dispute. The remainder of the tutorial has been disabled for now '*

 * *            "(converted to markdown), and will be re-enabled once the dispute settles.')], delete: "*

 * *            "[1]}}, 28: {'execution_count': 2, 'outputs': [], 'source': {insert: [(0, '%%script "*

 * *            "false - […]*

```diff
@@ -406,252 +406,44 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
-                "We can download the dataset using the following command:"
+                "We can download the dataset using the following command:\n",
+                "\n",
+                "#### NOTE: The DAGW dataset is currently unavailable due to a copyright dispute. The remainder of the tutorial has been disabled for now (converted to markdown), and will be re-enabled once the dispute settles."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Using custom data configuration DDSC--partial-danish-gigaword-small-test-sample-6518b630de09688d\n",
-                        "Found cached dataset parquet (/Users/au561649/.cache/huggingface/datasets/DDSC___parquet/DDSC--partial-danish-gigaword-small-test-sample-6518b630de09688d/0.0.0/2a3b91fbd88a2c90d1dbbb32b460cf621d31bd5b05b934492fdef7d8d6f236ec)\n"
-                    ]
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "2c78220f7f1e4c119901389899b11a7b",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "  0%|          | 0/1 [00:00<?, ?it/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
+            "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "from datasets import load_dataset\n",
                 "\n",
                 "# note that this can take a little while\n",
                 "dataset = load_dataset(\"DDSC/partial-danish-gigaword-small-test-sample\")\n",
                 "\n",
                 "# All of the dataset is available in the train split\n",
                 "dataset = dataset[\"train\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>text</th>\n",
-                            "      <th>source</th>\n",
-                            "      <th>doc_id</th>\n",
-                            "      <th>LICENSE</th>\n",
-                            "      <th>uri</th>\n",
-                            "      <th>date_built</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>Den fulde tekst Pressen\u00e6vnets kendelse i sag n...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_173889</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:51:31 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>Resume\\n\\nEfter at der var sket afskedigelser ...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_39059</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:51:14 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>Resume\\n\\nContainere kunne ikke anses som genb...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_15045</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:51:28 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>Resume\\n\\nEn forhandler ved \u00bbhome-parties\u00ab af ...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_37261</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:49:27 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>Den fulde tekst\\n\\nSkrivelse om lov om fleksyd...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_19415</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:52:27 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>5</th>\n",
-                            "      <td>Resume\\n\\nResum\u00e9\\n\\nKlage over p\u00e5bud om s\u00e6rlig...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_31217</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:49:18 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>6</th>\n",
-                            "      <td>Resume\\n\\nResum\u00e9\\n\\nI en r\u00e6kke af de af Danmar...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_14387</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:49:49 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>7</th>\n",
-                            "      <td>Oversigt (indholdsfortegnelse)\\n\\nBilag 1\\n\\nD...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_166197</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:49:44 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>8</th>\n",
-                            "      <td>Den fulde tekst\\n\\nBekendtg\u00f8relse om afregning...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_76994</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:52:52 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9</th>\n",
-                            "      <td>Den fulde tekst Ligebehandlingsn\u00e6vnets afg\u00f8rel...</td>\n",
-                            "      <td>retsinformationdk</td>\n",
-                            "      <td>retsinformationdk_192325</td>\n",
-                            "      <td>Danish Copyright law at https://www.retsinform...</td>\n",
-                            "      <td>https://www.retsinformation.dk/Forms/R0710.asp...</td>\n",
-                            "      <td>Fri Nov 22 00:51:41 2019 +0100</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "                                                text             source  \\\n",
-                            "0  Den fulde tekst Pressen\u00e6vnets kendelse i sag n...  retsinformationdk   \n",
-                            "1  Resume\\n\\nEfter at der var sket afskedigelser ...  retsinformationdk   \n",
-                            "2  Resume\\n\\nContainere kunne ikke anses som genb...  retsinformationdk   \n",
-                            "3  Resume\\n\\nEn forhandler ved \u00bbhome-parties\u00ab af ...  retsinformationdk   \n",
-                            "4  Den fulde tekst\\n\\nSkrivelse om lov om fleksyd...  retsinformationdk   \n",
-                            "5  Resume\\n\\nResum\u00e9\\n\\nKlage over p\u00e5bud om s\u00e6rlig...  retsinformationdk   \n",
-                            "6  Resume\\n\\nResum\u00e9\\n\\nI en r\u00e6kke af de af Danmar...  retsinformationdk   \n",
-                            "7  Oversigt (indholdsfortegnelse)\\n\\nBilag 1\\n\\nD...  retsinformationdk   \n",
-                            "8  Den fulde tekst\\n\\nBekendtg\u00f8relse om afregning...  retsinformationdk   \n",
-                            "9  Den fulde tekst Ligebehandlingsn\u00e6vnets afg\u00f8rel...  retsinformationdk   \n",
-                            "\n",
-                            "                     doc_id  \\\n",
-                            "0  retsinformationdk_173889   \n",
-                            "1   retsinformationdk_39059   \n",
-                            "2   retsinformationdk_15045   \n",
-                            "3   retsinformationdk_37261   \n",
-                            "4   retsinformationdk_19415   \n",
-                            "5   retsinformationdk_31217   \n",
-                            "6   retsinformationdk_14387   \n",
-                            "7  retsinformationdk_166197   \n",
-                            "8   retsinformationdk_76994   \n",
-                            "9  retsinformationdk_192325   \n",
-                            "\n",
-                            "                                             LICENSE  \\\n",
-                            "0  Danish Copyright law at https://www.retsinform...   \n",
-                            "1  Danish Copyright law at https://www.retsinform...   \n",
-                            "2  Danish Copyright law at https://www.retsinform...   \n",
-                            "3  Danish Copyright law at https://www.retsinform...   \n",
-                            "4  Danish Copyright law at https://www.retsinform...   \n",
-                            "5  Danish Copyright law at https://www.retsinform...   \n",
-                            "6  Danish Copyright law at https://www.retsinform...   \n",
-                            "7  Danish Copyright law at https://www.retsinform...   \n",
-                            "8  Danish Copyright law at https://www.retsinform...   \n",
-                            "9  Danish Copyright law at https://www.retsinform...   \n",
-                            "\n",
-                            "                                                 uri  \\\n",
-                            "0  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "1  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "2  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "3  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "4  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "5  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "6  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "7  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "8  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "9  https://www.retsinformation.dk/Forms/R0710.asp...   \n",
-                            "\n",
-                            "                       date_built  \n",
-                            "0  Fri Nov 22 00:51:31 2019 +0100  \n",
-                            "1  Fri Nov 22 00:51:14 2019 +0100  \n",
-                            "2  Fri Nov 22 00:51:28 2019 +0100  \n",
-                            "3  Fri Nov 22 00:49:27 2019 +0100  \n",
-                            "4  Fri Nov 22 00:52:27 2019 +0100  \n",
-                            "5  Fri Nov 22 00:49:18 2019 +0100  \n",
-                            "6  Fri Nov 22 00:49:49 2019 +0100  \n",
-                            "7  Fri Nov 22 00:49:44 2019 +0100  \n",
-                            "8  Fri Nov 22 00:52:52 2019 +0100  \n",
-                            "9  Fri Nov 22 00:51:41 2019 +0100  "
-                        ]
-                    },
-                    "execution_count": 15,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# We can take a look at one of the examples:\n",
                 "ten_samples = dataset.select(range(10))\n",
                 "ten_samples.to_pandas()"
             ]
         },
         {
             "attachments": {},
@@ -659,61 +451,20 @@
             "metadata": {},
             "source": [
                 "As previously mentioned, the Danish Gigaword corpus consist of multiple domains. For this tutorial, we will look at three of these domains. `retsinformationdk` which consists of legal documents, `hest` which contains post from a Danish debate forum ([heste-nettet.dk](https://www.heste-nettet.dk/)) and `spont` which contains texts transcribed from spontaneous speech."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 4,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "cf05115807f14affa8d479778d1c466a",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "  0%|          | 0/3 [00:00<?, ?ba/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "b4e3b0d54e724294b184fc8389fa6a69",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "  0%|          | 0/3 [00:00<?, ?ba/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5e2b9e6a5a3243008c0972e66b54e426",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "  0%|          | 0/3 [00:00<?, ?ba/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
+            "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# we can filter out these three datasets based on the \"source\"\n",
                 "legal = dataset.filter(lambda x: x[\"source\"] == \"retsinformationdk\", num_proc=1)\n",
                 "news = dataset.filter(lambda x: x[\"source\"] == \"tv2r\", num_proc=1)\n",
                 "speech = dataset.filter(lambda x: x[\"source\"] == \"spont\", num_proc=1)"
             ]
         },
         {
@@ -736,14 +487,16 @@
                         "Legal contains 1000 examples\n",
                         "News contains 1000 examples\n",
                         "Speech contains 411 examples\n"
                     ]
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "print(f\"Legal contains {len(legal)} examples\")\n",
                 "print(f\"News contains {len(news)} examples\")\n",
                 "print(f\"Speech contains {len(speech)} examples\")"
             ]
         },
         {
             "attachments": {},
@@ -768,14 +521,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# 1. Crease a blank spaCy model with a sentencizer as that's the only component required for the quality metrics\n",
                 "nlp = spacy.blank(\"da\")\n",
                 "nlp.add_pipe(\"sentencizer\")\n",
                 "nlp.max_length = (\n",
                 "    2000000  # as some of the documents are quite long we can increase the max length\n",
                 ")\n",
                 "# however it might be worth filtering out these documents beforehand for very very long documents.\n",
@@ -808,23 +563,27 @@
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "legal_docs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "legal_docs = list(legal_docs)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -859,14 +618,16 @@
                     },
                     "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "legal_doc = legal_docs[0]\n",
                 "\n",
                 "print(legal_doc[:100])  # print the first 100 tokens\n",
                 "print(\"----\")\n",
                 "print(\"This passed the quality filter:\")\n",
                 "legal_doc._.passed_quality_check"
             ]
@@ -892,14 +653,16 @@
                     },
                     "execution_count": 43,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "legal_doc._.quality"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -918,14 +681,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# 4. Filter out the documents that do not pass the quality\n",
                 "legal_docs_filtered = [doc for doc in legal_docs if doc._.passed_quality_check]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
@@ -936,14 +701,16 @@
                     "output_type": "stream",
                     "text": [
                         "We had a total of 1000 which we filtered down to 264.\n"
                     ]
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "print(\n",
                 "    f\"We had a total of {len(legal['text'])} which we filtered down to {len(legal_docs_filtered)}.\"\n",
                 ")"
             ]
         },
         {
             "attachments": {},
@@ -976,14 +743,16 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "import seaborn as sns\n",
                 "\n",
                 "\n",
                 "def get_duplicate_10_gram_fraction(doc):\n",
                 "    quality = doc._.quality\n",
                 "    duplicate_10_gram_fraction = quality.duplicate_ngram_chr_fraction[\"10\"]\n",
                 "    return duplicate_10_gram_fraction.value\n",
@@ -1024,14 +793,16 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "alpha_ratio = [doc._.quality.alpha_ratio.value for doc in legal_docs]\n",
                 "sns.histplot(alpha_ratio)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -1049,27 +820,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": 32,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# first we apply the pipeline to the other domains\n",
                 "news_docs = nlp.pipe(news[\"text\"])\n",
                 "news_docs = list(news_docs)\n",
                 "speech_docs = nlp.pipe(speech[\"text\"])\n",
                 "speech_docs = list(speech_docs)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 36,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "# extract alpha ratio:\n",
                 "news_alpha_ratio = [doc._.quality.alpha_ratio.value for doc in news_docs]\n",
                 "speech_alpha_ratio = [doc._.quality.alpha_ratio.value for doc in speech_docs]"
             ]
         },
         {
             "attachments": {},
@@ -1102,14 +877,16 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "# histogram\n",
                 "sns.histplot(news_alpha_ratio, label=\"News\", alpha=0.5, binwidth=0.05)\n",
                 "sns.histplot(alpha_ratio, label=\"Legal\", alpha=0.5, binwidth=0.05)\n",
                 "sns.histplot(speech_alpha_ratio, label=\"Speech\", alpha=0.5, binwidth=0.05)\n",
                 "\n",
@@ -1153,14 +930,16 @@
                         "Taler 6: ja\n",
                         "Taler 6: ja\n",
                         "Taler 6: NA\n"
                     ]
                 }
             ],
             "source": [
+                "%%script false --no-raise-error\n",
+                "\n",
                 "doc = speech_docs[0]\n",
                 "# examine the first 100 tokens in the first document\n",
                 "print(doc[:100])"
             ]
         },
         {
             "attachments": {},
@@ -1190,15 +969,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.15"
+            "version": "3.10.13"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "31387647799921bb85032eec7bb02e281325ae7f8ffa6f9cd7cdead815b36c88"
             }
         }
```

### Comparing `textdescriptives-2.7.3/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.8.0/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/tutorials/sklearn_integration.ipynb` & `textdescriptives-2.8.0/docs/tutorials/sklearn_integration.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/docs/usingthepackage.rst` & `textdescriptives-2.8.0/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/paper/paper.bib` & `textdescriptives-2.8.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/paper/paper.md` & `textdescriptives-2.8.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/paper/paper_quarto.pdf` & `textdescriptives-2.8.0/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/paper/paper_quarto.qmd` & `textdescriptives-2.8.0/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/pyproject.toml` & `textdescriptives-2.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.7.3"
+version = "2.8.0"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [
     { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
     { name = "Kenneth Enevoldsen" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -30,39 +30,41 @@
     "text statistics",
     "text descriptives",
     "text analytics",
     "text mining",
 ]
 
 dependencies = [
-    "spacy[lookups]>=3.1.0",
+    "spacy[lookups]>=3.6.0",
     "numpy>=1.20.0",
     "pandas>=1.0.0",
     "pyphen>=0.11.0,<0.15.0",
     "ftfy>=6.0.3,<6.1.0",
+    "pydantic>=2.0",
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://hlasse.github.io/TextDescriptives/"
 repository = "https://github.com/HLasse/textdescriptives"
 documentation = "https://hlasse.github.io/TextDescriptives/"
 
 [project.optional-dependencies]
 style = ["black==24.1.1", "pre-commit==3.6.0", "ruff==0.1.15", "mypy==1.8.0"]
 tests = ["pytest>=7.1.3", "pytest-cov>=3.0.0"]
 docs = [
+    "pydantic==2.1",
     "sphinx>=5.3.0",
     "furo==2022.12.7",
     "sphinx-copybutton>=0.5.1",
     "sphinxext-opengraph>=0.7.3",
     "myst-nb>=0.6.0",
     "sphinx_design>=0.3.0",
-    "autodoc_pydantic==1.9.0",
+    "autodoc_pydantic==2.1.0",
 ]
 tutorials = [
     "jupyter",
     "seaborn",
     "matplotlib",
     "datasets>=2.8.0",
     "scikit-learn>=1.1.1",
```

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/coherence.py` & `textdescriptives-2.8.0/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.8.0/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.8.0/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.8.0/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.8.0/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/quality.py` & `textdescriptives-2.8.0/src/textdescriptives/components/quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
 
         Args:
             doc (Doc): spaCy doc object
         """
         # to allow the variable to json serializable we convert it to json
         # it is then converted back into a quality output object in the getter
 
-        doc._._quality = self.quality_setter(doc).dict()
+        doc._._quality = self.quality_setter(doc).model_dump()
         doc._.passed_quality_check = self.passed_quality_thresholds(doc)
 
     def passed_quality_thresholds(self, span: Union[Span, Doc]) -> bool:
         """Check if a span passes the quality thresholds.
 
         Args:
             span (Union[Span, Doc]): spaCy span or doc object
```

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.8.0/src/textdescriptives/components/quality_data_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Data classes used for the quality component."""
 
 from typing import Any, Dict, Optional, Tuple, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import ConfigDict, BaseModel, Field
 
 Interval = Tuple[Optional[float], Optional[float]]
 
 
 class ThresholdsOutput(BaseModel):
     """An output which contains an three items. 1) a thresholds which is either
     an interval or a accepted boolean value. 2) a value which is the value of
@@ -17,16 +17,15 @@
         >>> t_out = ThresholdsOutput(threshold=(0, 2), value=2)
         >>> t_out
         ThresholdsOutput(value=2.0, passed=True, threshold=(0.0, 2.0))
         >>> t_out.passed
         True
     """
 
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     threshold: Union[Interval, bool, None]
     value: Union[float, None]
 
     @property
     def passed(self) -> Optional[bool]:
         """Return True if the value is within the thresholds."""
@@ -57,16 +56,15 @@
             return self.value == other.value and self.threshold == other.threshold
         return self.value == other
 
 
 class QualityThresholds(BaseModel):
     """Thresholds for quality metrics."""
 
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     n_stop_words: Interval = Field(
         (2, None),
         description="A Range for the number of stop words. Default: (2, None), i.e. "
         + "at least 2 stop words, but no upper limit.",
     )
     alpha_ratio: Interval = Field(
@@ -160,16 +158,15 @@
         + r" i.e. no lower limit, but at most 20% of words are out-of-vocabulary.",
     )
 
 
 class QualityOutput(BaseModel):
     """The output of the quality function."""
 
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     n_stop_words: ThresholdsOutput = Field(
         ...,
         description="The thresholds output for the number of stop words.",
     )
     alpha_ratio: ThresholdsOutput = Field(
         ...,
```

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/readability.py` & `textdescriptives-2.8.0/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/components/utils.py` & `textdescriptives-2.8.0/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/data/spam.csv` & `textdescriptives-2.8.0/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/extractors.py` & `textdescriptives-2.8.0/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/integrations/sklearn_featurizer.py` & `textdescriptives-2.8.0/src/textdescriptives/integrations/sklearn_featurizer.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/load_components.py` & `textdescriptives-2.8.0/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives/utils.py` & `textdescriptives-2.8.0/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.8.0/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.7.3
+Version: 2.8.0
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,35 +221,37 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: spacy[lookups]>=3.1.0
+Requires-Dist: spacy[lookups]>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pyphen<0.15.0,>=0.11.0
 Requires-Dist: ftfy<6.1.0,>=6.0.3
+Requires-Dist: pydantic>=2.0
 Provides-Extra: style
 Requires-Dist: black==24.1.1; extra == "style"
 Requires-Dist: pre-commit==3.6.0; extra == "style"
 Requires-Dist: ruff==0.1.15; extra == "style"
 Requires-Dist: mypy==1.8.0; extra == "style"
 Provides-Extra: tests
 Requires-Dist: pytest>=7.1.3; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: pydantic==2.1; extra == "docs"
 Requires-Dist: sphinx>=5.3.0; extra == "docs"
 Requires-Dist: furo==2022.12.7; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.5.1; extra == "docs"
 Requires-Dist: sphinxext-opengraph>=0.7.3; extra == "docs"
 Requires-Dist: myst-nb>=0.6.0; extra == "docs"
 Requires-Dist: sphinx_design>=0.3.0; extra == "docs"
-Requires-Dist: autodoc_pydantic==1.9.0; extra == "docs"
+Requires-Dist: autodoc_pydantic==2.1.0; extra == "docs"
 Provides-Extra: tutorials
 Requires-Dist: jupyter; extra == "tutorials"
 Requires-Dist: seaborn; extra == "tutorials"
 Requires-Dist: matplotlib; extra == "tutorials"
 Requires-Dist: datasets>=2.8.0; extra == "tutorials"
 Requires-Dist: scikit-learn>=1.1.1; extra == "tutorials"
 Requires-Dist: ipython<=8.21.0; extra == "tutorials"
```

### Comparing `textdescriptives-2.7.3/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.8.0/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/books.py` & `textdescriptives-2.8.0/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_coherence.py` & `textdescriptives-2.8.0/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_dependency_distance.py` & `textdescriptives-2.8.0/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_descriptive_stats.py` & `textdescriptives-2.8.0/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_extractors.py` & `textdescriptives-2.8.0/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_information.py` & `textdescriptives-2.8.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_load_components.py` & `textdescriptives-2.8.0/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_pos_proportions.py` & `textdescriptives-2.8.0/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_quality.py` & `textdescriptives-2.8.0/tests/test_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Tests for the quality module."""
 
 from typing import List, Tuple
 
 import pytest
 import spacy
-
 import textdescriptives as td
 from textdescriptives.components.quality import (
     alpha_ratio,
     duplicate_ngram_fraction,
     mean_word_length,
     n_stop_words,
     oov_ratio,
@@ -204,15 +203,15 @@
         mean_word_length=(1, 10),
         doc_length=(10, 100_000),
         symbol_to_word_ratio={".": (None, 0.3)},
         proportion_ellipsis=(None, 0.3),
         proportion_bullet_points=(None, 0.8),
         duplicate_line_chr_fraction=(None, 0.2),
         duplicate_paragraph_chr_fraction=(None, 0.2),
-        top_ngram_chr_fraction={2: (None, 0.6), 3: (None, 0.6)},
+        top_ngram_chr_fraction={"2": (None, 0.6), "3": (None, 0.6)},
         duplicate_ngram_chr_fraction={},
         contains={"lorem ipsum": False},
         oov_ratio=(None, 0.3),
     )
 
     quality_pipe = nlp.add_pipe(
         "textdescriptives/quality",
```

### Comparing `textdescriptives-2.7.3/tests/test_readability.py` & `textdescriptives-2.8.0/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.7.3/tests/test_utils.py` & `textdescriptives-2.8.0/tests/test_utils.py`

 * *Files identical despite different names*

