# Comparing `tmp/pyoma-0.13.2.tar.gz` & `tmp/pyoma-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoma-0.13.2.tar", last modified: Tue Apr  9 13:50:07 2024, max compression
+gzip compressed data, was "dist/pyoma-0.9.4.tar", last modified: Thu Apr  1 10:39:09 2021, max compression
```

## Comparing `pyoma-0.13.2.tar` & `pyoma-0.9.4.tar`

### file list

```diff
@@ -1,92 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.272519 pyoma-0.13.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 13:50:01.000000 pyoma-0.13.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-09 13:50:07.272519 pyoma-0.13.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-09 13:50:01.000000 pyoma-0.13.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.256519 pyoma-0.13.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2657 2024-04-09 13:50:01.000000 pyoma-0.13.2/bin/importdata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5621 2024-04-09 13:50:01.000000 pyoma-0.13.2/bin/map_to_closest_seq
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-09 13:50:07.000000 pyoma-0.13.2/bin/oma2hdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.256519 pyoma-0.13.2/pyoma/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.256519 pyoma-0.13.2/pyoma/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/application/enrichment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.264519 pyoma-0.13.2/pyoma/browser/
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/KmerEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/OrthoXMLSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/ancestral_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/ancestral_synteny.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/check_db_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/compute_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/convert.drw
--rw-r--r--   0 runner    (1001) docker     (127)   112392 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/convert_omastandalone.drw
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/convert_omastandalone.py
--rw-r--r--   0 runner    (1001) docker     (127)   147985 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/db_contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/geneontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hoghelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogidmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.264519 pyoma-0.13.2/pyoma/browser/hogprofile/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17785 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/hashutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/pyhamutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/hogprofile/tree_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/homoeologs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/idmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/linkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/locus_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    24809 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/sanitychecks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/suffixsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/synteny.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/tablefmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/browser/xref_contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/hpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.264519 pyoma-0.13.2/pyoma/inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/inference/algo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/inference/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/inference/tabledef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/pyoma/orthoxml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/orthoxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyoma/orthoxml/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/pyoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-09 13:50:07.000000 pyoma-0.13.2/pyoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-09 13:50:07.000000 pyoma-0.13.2/pyoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:50:07.000000 pyoma-0.13.2/pyoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 13:50:07.000000 pyoma-0.13.2/pyoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 13:50:07.000000 pyoma-0.13.2/pyoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 13:50:01.000000 pyoma-0.13.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 13:50:07.272519 pyoma-0.13.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-09 13:50:01.000000 pyoma-0.13.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/tests/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/application/test_enrichment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/tests/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_compare_hog_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    37353 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_hoghelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_hogidmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_locusparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_orthoxmlsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_performance_bigdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_suffixsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_xref_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/browser/test_xrefs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:07.268519 pyoma-0.13.2/tests/inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/inference/test_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-09 13:50:01.000000 pyoma-0.13.2/tests/test_common.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.946269 pyoma-0.9.4/
+-rw-r--r--   0 adriaal    (501) staff       (20)     1875 2021-04-01 10:39:09.946572 pyoma-0.9.4/PKG-INFO
+-rw-r--r--   0 adriaal    (501) staff       (20)      760 2021-04-01 10:17:08.000000 pyoma-0.9.4/README.md
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.880997 pyoma-0.9.4/bin/
+-rwxr-xr-x   0 adriaal    (501) staff       (20)     2122 2021-04-01 10:12:38.000000 pyoma-0.9.4/bin/importdata.py
+-rwxr-xr-x   0 adriaal    (501) staff       (20)     4956 2020-10-28 08:46:39.000000 pyoma-0.9.4/bin/map_to_closest_seq
+-rw-r--r--   0 adriaal    (501) staff       (20)     2122 2021-04-01 10:39:09.000000 pyoma-0.9.4/bin/oma2hdf
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.883274 pyoma-0.9.4/pyoma/
+-rw-r--r--   0 adriaal    (501) staff       (20)      149 2021-01-25 10:24:13.000000 pyoma-0.9.4/pyoma/__init__.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.918360 pyoma-0.9.4/pyoma/browser/
+-rw-r--r--   0 adriaal    (501) staff       (20)     2186 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/KmerEncoder.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     8841 2021-04-01 10:12:39.000000 pyoma-0.9.4/pyoma/browser/OrthoXMLSplitter.py
+-rw-r--r--   0 adriaal    (501) staff       (20)        0 2020-07-21 11:56:35.000000 pyoma-0.9.4/pyoma/browser/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    13611 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/ancestral_synteny.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     5034 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/check_db_consistency.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    16860 2021-04-01 10:12:39.000000 pyoma-0.9.4/pyoma/browser/compute_cache.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     7862 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/convert.drw
+-rw-r--r--   0 adriaal    (501) staff       (20)   110447 2021-04-01 10:12:39.000000 pyoma-0.9.4/pyoma/browser/convert.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    13654 2021-03-30 13:31:39.000000 pyoma-0.9.4/pyoma/browser/convert_omastandalone.drw
+-rw-r--r--   0 adriaal    (501) staff       (20)    10002 2021-03-30 13:31:39.000000 pyoma-0.9.4/pyoma/browser/convert_omastandalone.py
+-rw-r--r--   0 adriaal    (501) staff       (20)   127791 2021-04-01 10:12:39.000000 pyoma-0.9.4/pyoma/browser/db.py
+-rw-r--r--   0 adriaal    (501) staff       (20)      874 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/decorators.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    15265 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/geneontology.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4804 2021-01-25 10:24:13.000000 pyoma-0.9.4/pyoma/browser/hoghelper.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     3619 2021-04-01 10:12:39.000000 pyoma-0.9.4/pyoma/browser/hogidmap.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.929637 pyoma-0.9.4/pyoma/browser/hogprofile/
+-rw-r--r--   0 adriaal    (501) staff       (20)       28 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/hogprofile/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    13021 2020-10-28 08:46:40.000000 pyoma-0.9.4/pyoma/browser/hogprofile/build.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     3203 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/hogprofile/hashutils.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     1058 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/hogprofile/pyhamutils.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4074 2021-01-25 10:24:14.000000 pyoma-0.9.4/pyoma/browser/hogprofile/query.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     1774 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/hogprofile/tree_helper.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    18397 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/homoeologs.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    10615 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/linkout.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     2310 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/locus_parser.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    16040 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/models.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     5278 2021-01-25 10:24:14.000000 pyoma-0.9.4/pyoma/browser/sanitychecks.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    16730 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/suffixsearch.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     5455 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/synteny.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     7573 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/browser/tablefmt.py
+-rw-r--r--   0 adriaal    (501) staff       (20)      109 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/common.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     2089 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/hpc.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.934806 pyoma-0.9.4/pyoma/inference/
+-rw-r--r--   0 adriaal    (501) staff       (20)        0 2020-04-15 22:53:54.000000 pyoma-0.9.4/pyoma/inference/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)       57 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/inference/algo.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     7564 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/inference/db.py
+-rw-r--r--   0 adriaal    (501) staff       (20)      956 2020-04-15 22:53:54.000000 pyoma-0.9.4/pyoma/inference/tabledef.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.936088 pyoma-0.9.4/pyoma/orthoxml/
+-rw-r--r--   0 adriaal    (501) staff       (20)        0 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/orthoxml/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     2947 2020-10-28 08:46:41.000000 pyoma-0.9.4/pyoma/orthoxml/compare.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.886440 pyoma-0.9.4/pyoma.egg-info/
+-rw-r--r--   0 adriaal    (501) staff       (20)     1875 2021-04-01 10:39:09.000000 pyoma-0.9.4/pyoma.egg-info/PKG-INFO
+-rw-r--r--   0 adriaal    (501) staff       (20)     1662 2021-04-01 10:39:09.000000 pyoma-0.9.4/pyoma.egg-info/SOURCES.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)        1 2021-04-01 10:39:09.000000 pyoma-0.9.4/pyoma.egg-info/dependency_links.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)      310 2021-04-01 10:39:09.000000 pyoma-0.9.4/pyoma.egg-info/requires.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)       12 2021-04-01 10:39:09.000000 pyoma-0.9.4/pyoma.egg-info/top_level.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)       74 2021-04-01 10:39:09.947577 pyoma-0.9.4/setup.cfg
+-rw-r--r--   0 adriaal    (501) staff       (20)     2236 2021-04-01 10:28:51.000000 pyoma-0.9.4/setup.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.877390 pyoma-0.9.4/tests/
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.943140 pyoma-0.9.4/tests/browser/
+-rw-r--r--   0 adriaal    (501) staff       (20)        0 2020-04-15 22:53:54.000000 pyoma-0.9.4/tests/browser/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4069 2021-01-25 10:24:14.000000 pyoma-0.9.4/tests/browser/test_compare_hog_levels.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    27034 2020-11-17 13:16:51.000000 pyoma-0.9.4/tests/browser/test_db.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    11855 2021-04-01 10:12:39.000000 pyoma-0.9.4/tests/browser/test_import.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     9192 2020-10-28 08:46:42.000000 pyoma-0.9.4/tests/browser/test_locusparser.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     6041 2020-10-28 08:46:42.000000 pyoma-0.9.4/tests/browser/test_models.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4023 2021-04-01 10:12:39.000000 pyoma-0.9.4/tests/browser/test_orthoxmlsplitter.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    11639 2020-10-28 08:46:42.000000 pyoma-0.9.4/tests/browser/test_suffixsearch.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    14526 2020-10-28 08:46:42.000000 pyoma-0.9.4/tests/browser/test_xrefs.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-01 10:39:09.944932 pyoma-0.9.4/tests/inference/
+-rw-r--r--   0 adriaal    (501) staff       (20)        0 2020-04-15 22:53:55.000000 pyoma-0.9.4/tests/inference/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     5582 2020-10-28 08:46:42.000000 pyoma-0.9.4/tests/inference/test_db.py
```

### Comparing `pyoma-0.13.2/README.md` & `pyoma-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pyoma-0.13.2/bin/importdata.py` & `pyoma-0.9.4/bin/importdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,70 +13,56 @@
         raise RuntimeError("oma2hdf requires darwin: can't find darwin on your system.")
 
     # Argument parsing
     parser = argparse.ArgumentParser("Convert a OMA Browser release into hdf5 format.")
     parser.add_argument(
         "-r",
         "--release",
-        help="path to release. If not set, DARWIN_BROWSERDATA_PATH " "from the environment is used.",
+        help="path to release. If not set, DARWIN_BROWSERDATA_PATH "
+        "from the environment is used.",
     )
     parser.add_argument(
         "out",
         default="OmaServer.h5",
         help="name of the hdf5 database that is created. The file is "
         "stored in the same path as the release is stored, i.e. "
         "see option -r/--release and it's default.",
     )
     parser.add_argument(
         "-s",
         "--standalone",
         action="store_true",
-        help="a flag which needs to be set if you intend to import " "the results from an OmaStandalone run.",
+        help="a flag which needs to be set if you intend to import "
+        "the results from an OmaStandalone run.",
     )
     parser.add_argument(
         "-d",
         "--domains",
         nargs="+",
         help="absolute path or url to domain annotations in mdas.csv format. "
         "Not specifying any domains is equivalent to the --no-domains "
         "option.",
     )
     parser.add_argument(
-        "--hog-release-char",
-        required=("--standalone" not in sys.argv and "-s" not in sys.argv),
-        help="A single character indicating the release in the hog ids. "
-        "This argument is ignored for oma standalone imports",
-    )
-    parser.add_argument(
         "-v",
         default=0,
         action="count",
         help="Increase verbosity level to INFO or DEBUG level",
     )
-    parser.add_argument(
-        "--phases",
-        type=int,
-        nargs="+",
-        help="select phases to run individually. By default, all phases are run.",
-    )
 
     options = parser.parse_args(args)
     log_level = 30 - (10 * min(options.v, 2))
     if options.standalone:
         pyoma.browser.convert_omastandalone.import_oma_run(
             options.release, options.out, domains=options.domains, log_level=log_level
         )
     else:
         if options.release:
             os.environ["DARWIN_BROWSERDATA_PATH"] = options.release
         print(options.out)
         pyoma.browser.convert.main(
-            options.out,
-            domains=options.domains,
-            log_level=log_level,
-            release=options.hog_release_char,
-            phases=options.phases,
+            options.out, domains=options.domains, log_level=log_level
         )
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `pyoma-0.13.2/bin/map_to_closest_seq` & `pyoma-0.9.4/bin/map_to_closest_seq`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
+import gzip
 import os
 
 import pyoma.browser.db
-from pyoma.common import auto_open
 import pyoma.hpc
 import Bio.SeqIO
 import logging
 import csv
 import hashlib
 import sys
 import signal
@@ -19,69 +19,14 @@
         "signal handler called with signal {}. Raise a KeybordInterupt Exception".format(
             signum
         )
     )
     raise KeyboardInterrupt("time is up")
 
 
-class DefaultFormater:
-    def get_header(self):
-        return [
-            "query",
-            "target",
-            "is_main_isoform",
-            "HOG",
-            "OMA_group",
-            "PAM_distance",
-            "Alignment_score",
-        ]
-
-    def get_row_data(self, map_res):
-        if map_res.target.hog_family_nr != 0:
-            hog_id = db.format_hogid(map_res.target.hog_family_nr)
-        else:
-            hog_id = "n/a"
-        if map_res.target.oma_group != 0:
-            oma_grp = "OmaGroup:{}".format(map_res.target.oma_group)
-        else:
-            oma_grp = "n/a"
-        return [
-            map_res.query,
-            map_res.target.omaid,
-            map_res.target.entry_nr == map_res.closest_entry_nr,
-            hog_id,
-            oma_grp,
-            map_res.distance,
-            map_res.score,
-        ]
-
-
-class OMAmerLikeFormatter:
-    def get_header(self):
-        return [
-            "qseqid",
-            "hogid",
-            "target",
-            "is_main_isoform",
-            "distance",
-            "alignment_score",
-        ]
-
-    def get_row_data(self, map_res):
-        hog_id = map_res.target.oma_hog if map_res.target.oma_hog != "" else "na"
-        return [
-            map_res.query,
-            hog_id,
-            map_res.target.omaid,
-            map_res.target.entry_nr == map_res.closest_entry_nr,
-            map_res.distance,
-            map_res.score,
-        ]
-
-
 signal.signal(signal.SIGUSR2, handler)
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser(description="Map sequences to HOGs")
     parser.add_argument("hdf5", help="Path to the hdf5 database")
@@ -102,68 +47,85 @@
     )
     parser.add_argument(
         "-t",
         "--target",
         default=None,
         help="Target species. If not set, no restriction applies.",
     )
-    parser.add_argument(
-        "-f",
-        "--format",
-        choices=("default", "OMAmer-like"),
-        default="default",
-        help="output format, either the default closest seq data or a format that is similar to OMAmer output",
-    )
     conf = parser.parse_args()
     logging.basicConfig(level=30 - 10 * min(conf.v, 2))
     nr_procs = conf.nr_proc
     if nr_procs is None:
         nr_procs = int(os.getenv("NR_PROCESSES", "1"))
     pInf = pyoma.hpc.detect_hpc_jobarray(nr_procs, this_proc_nr=conf.procnr)
     logger.info(pInf)
     outfn = pInf.modify_filename(conf.out)
 
-    if conf.format == "OMAmer-like":
-        formatter = OMAmerLikeFormatter()
-    else:
-        formatter = DefaultFormater()
-
     db = pyoma.browser.db.Database(conf.hdf5)
     mapper = pyoma.browser.db.ClosestSeqMapper(db)
 
     last_id = None
     if os.path.exists(outfn + ".ckpt"):
         with open(outfn + ".ckpt") as fh:
             last_id = fh.read()
 
-    with auto_open(outfn, "at") as fout:
+    open_ = gzip.open if outfn.endswith(".gz") else open
+    with open_(outfn, "at") as fout:
         csv_writer = csv.writer(fout, delimiter="\t")
         if last_id is None and pInf.this_proc_nr == 1:
-            csv_writer.writerow(formatter.get_header())
+            csv_writer.writerow(
+                [
+                    "query",
+                    "target",
+                    "is_main_isoform",
+                    "HOG",
+                    "OMA_group",
+                    "PAM_distance",
+                    "Alignment_score",
+                ]
+            )
 
         for infn in conf.fasta:
-            with auto_open(infn, "rt") as fin:
+            with open(infn, "rt") as fin:
                 seqs = Bio.SeqIO.parse(fin, "fasta")
                 myjobs = filter(lambda srec: pInf.is_my_job(srec.id), seqs)
                 # forward in case we have a
                 if last_id is not None:
                     for xx in myjobs:
                         if xx.id == last_id:
                             break
                 try:
                     it = mapper.imap_sequences(myjobs, target_species=conf.target)
                     seen_queries = set([])
                     for map_res in it:
                         if map_res.query in seen_queries:
                             continue  # we keep just the very best mapping
                         seen_queries.add(map_res.query)
-                        csv_writer.writerow(formatter.get_row_data(map_res))
+                        if map_res.target.hog_family_nr != 0:
+                            hog_id = db.format_hogid(map_res.target.hog_family_nr)
+                        else:
+                            hog_id = "n/a"
+                        if map_res.target.oma_group != 0:
+                            oma_grp = "OmaGroup:{}".format(map_res.target.oma_group)
+                        else:
+                            oma_grp = "n/a"
+                        csv_writer.writerow(
+                            [
+                                map_res.query,
+                                map_res.target.omaid,
+                                map_res.target.entry_nr == map_res.closest_entry_nr,
+                                hog_id,
+                                oma_grp,
+                                map_res.distance,
+                                map_res.score,
+                            ]
+                        )
                         last_id = map_res.query
                 except KeyboardInterrupt as e:
-                    logger.info("received KeyboardInterrupt: %s", e)
+                    logger.info("received KeyboardInterrupt: {}".format(e))
                     logger.info("writing checkpoint")
                     with open(outfn + ".ckpt", "w") as ckpt:
                         ckpt.write(last_id)
                     logger.info("quiting with 99")
                     if len(conf.fasta) > 1:
                         logger.warning(
                             "checkpointing does only properly work with a single input file. You used more than one file. please investigate how to recover"
```

### Comparing `pyoma-0.13.2/bin/oma2hdf` & `pyoma-0.9.4/bin/oma2hdf`

 * *Files 10% similar despite different names*

```diff
@@ -13,70 +13,56 @@
         raise RuntimeError("oma2hdf requires darwin: can't find darwin on your system.")
 
     # Argument parsing
     parser = argparse.ArgumentParser("Convert a OMA Browser release into hdf5 format.")
     parser.add_argument(
         "-r",
         "--release",
-        help="path to release. If not set, DARWIN_BROWSERDATA_PATH " "from the environment is used.",
+        help="path to release. If not set, DARWIN_BROWSERDATA_PATH "
+        "from the environment is used.",
     )
     parser.add_argument(
         "out",
         default="OmaServer.h5",
         help="name of the hdf5 database that is created. The file is "
         "stored in the same path as the release is stored, i.e. "
         "see option -r/--release and it's default.",
     )
     parser.add_argument(
         "-s",
         "--standalone",
         action="store_true",
-        help="a flag which needs to be set if you intend to import " "the results from an OmaStandalone run.",
+        help="a flag which needs to be set if you intend to import "
+        "the results from an OmaStandalone run.",
     )
     parser.add_argument(
         "-d",
         "--domains",
         nargs="+",
         help="absolute path or url to domain annotations in mdas.csv format. "
         "Not specifying any domains is equivalent to the --no-domains "
         "option.",
     )
     parser.add_argument(
-        "--hog-release-char",
-        required=("--standalone" not in sys.argv and "-s" not in sys.argv),
-        help="A single character indicating the release in the hog ids. "
-        "This argument is ignored for oma standalone imports",
-    )
-    parser.add_argument(
         "-v",
         default=0,
         action="count",
         help="Increase verbosity level to INFO or DEBUG level",
     )
-    parser.add_argument(
-        "--phases",
-        type=int,
-        nargs="+",
-        help="select phases to run individually. By default, all phases are run.",
-    )
 
     options = parser.parse_args(args)
     log_level = 30 - (10 * min(options.v, 2))
     if options.standalone:
         pyoma.browser.convert_omastandalone.import_oma_run(
             options.release, options.out, domains=options.domains, log_level=log_level
         )
     else:
         if options.release:
             os.environ["DARWIN_BROWSERDATA_PATH"] = options.release
         print(options.out)
         pyoma.browser.convert.main(
-            options.out,
-            domains=options.domains,
-            log_level=log_level,
-            release=options.hog_release_char,
-            phases=options.phases,
+            options.out, domains=options.domains, log_level=log_level
         )
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `pyoma-0.13.2/pyoma/browser/KmerEncoder.py` & `pyoma-0.9.4/pyoma/browser/KmerEncoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,61 +7,63 @@
 
     -- Alex Warwick Vesztrocy, May-June 2017
 """
 import numpy as np
 
 
 # "digits"
-DIGITS_AA = np.frombuffer(b"ACDEFGHIKLMNPQRSTVWXY", dtype="S1")
-DIGITS_DNA = np.frombuffer(b"ACGTX", dtype="S1")
+DIGITS_AA = np.fromstring("ACDEFGHIKLMNPQRSTVWXY", dtype="S1")
+DIGITS_DNA = np.fromstring("ACGTX", dtype="S1")
 
 
 class KmerEncoder(object):
     def __init__(self, k, is_protein=True):
         """
-        Initialise the kmer converter. k is the kmer length.
-        If is_dna=True then DNA else AA.
+            Initialise the kmer converter. k is the kmer length.
+            If is_dna=True then DNA else AA.
         """
         self.digits = DIGITS_AA if is_protein else DIGITS_DNA
         self.k = int(k)  # Cast incase np-type for n below.
         self.max = (len(self.digits) ** self.k) - 1
         self.n = self.decode(self.digits[-1] * self.k) + 1
         self._prot = np.zeros((self.k,), dtype="S1")
 
     def __len__(self):
         """
-        Return the maximum integer-representation of the kmer length
-        in this converter.
+            Return the maximum integer-representation of the kmer length
+            in this converter.
         """
         return self.n
 
     def encode(self, seq):
         """
-        Encode integer kmer in protein chars.
+            Encode integer kmer in protein chars.
         """
         if seq <= self.max:
             self._prot[:] = self.digits[0]
             i = -1
             while seq > 0:
                 self._prot[i] = self.digits[seq % self.digits.size]
                 seq //= self.digits.size
                 i -= 1
             return self._prot.tostring()
         else:
-            raise ValueError("{} Larger than largest kmer of size {}".format(seq, self.k))
+            raise ValueError(
+                "{} Larger than largest kmer of size {}".format(seq, self.k)
+            )
 
     def decode(self, seq):
         """
-        Decode a protein kmer -> integer. NOTE: sanitisation to a byte
-        string required first.
+            Decode a protein kmer -> integer. NOTE: sanitisation to a byte
+            string required first.
         """
         x = 0
         for digit in seq[: self.k].decode("ascii"):
             x = (x * self.digits.size) + np.searchsorted(self.digits, digit)
         return x
 
     def decompose(self, seq):
         """
-        Decompose a sequence into counts of its constituent (decoded) kmers.
+            Decompose a sequence into counts of its constituent (decoded) kmers.
         """
         for i in range(len(seq) - self.k + 1):
             yield self.decode(seq[i : (i + self.k)])
```

### Comparing `pyoma-0.13.2/pyoma/browser/OrthoXMLSplitter.py` & `pyoma-0.9.4/pyoma/browser/OrthoXMLSplitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import unicode_literals, division
 from builtins import str
 import lxml.etree as etree
 import os
 import errno
 import logging
-import re
 
 logger = logging.getLogger(__name__)
 
 
 class OrthoXMLSplitter(object):
     """Convert orthoxml files with several families.
 
@@ -31,29 +30,19 @@
     :Example:
 
       splitter = OrthoXMLSplitter("data.orthoxml", cache_dir="./splits")
       splitter()
 
     will create files HOGxxxxxx.orthoxml in the ./splits directory."""
 
-    def __init__(self, xml_file, cache_dir=None, release_char=None):
+    def __init__(self, xml_file, cache_dir=None):
         self.xml_file = xml_file
         if cache_dir is not None:
             self._assert_cache_dir(cache_dir)
-        if release_char is None:
-            self.release_char = ""
-        elif re.match(r"^[A-Z]?$", release_char):
-            self.release_char = release_char
-        else:
-            raise ValueError(
-                "unexpected value for release_char: '{}'. Needs to be a single capital ascii letter".format(
-                    release_char
-                )
-            )
-        logger.info("loading xml file %s...", xml_file)
+        logger.info("loading xml file {}...".format(xml_file))
         parser = etree.XMLParser(remove_blank_text=True)
         self.Etree_XML = etree.parse(self.xml_file, parser=parser)
         self.Etree_root = self.Etree_XML.getroot()
         logger.info("building lookup table for genes")
         self.gene_lookup = {gene.get("id"): gene for gene in self._iter_gene_elements()}
         logger.info("init of OrthoXMLSplitter finished")
 
@@ -120,28 +109,34 @@
         if cache_dir is not None:
             self._assert_cache_dir(cache_dir)
         elif self.cache_dir is None:
             raise RuntimeError("cache dir to output files to is not set")
 
         if single_hog_files:
             if hogs_to_extract is None:
-                raise RuntimeError("useless to extract all hogs into single output file")
+                raise RuntimeError(
+                    "useless to extract all hogs into single output file"
+                )
             if basename is None or not isinstance(basename, (str, bytes)):
                 raise ValueError("basename needs to be specified: {}".format(basename))
-            ogs = [og for og in self._iter_toplevel_groups() if int(og.get("id")) in hogs_to_extract]
+            ogs = [
+                og
+                for og in self._iter_toplevel_groups()
+                if int(og.get("id")) in hogs_to_extract
+            ]
             fn = os.path.join(self.cache_dir, basename)
-            logger.info("extracting %d hogs into %s", len(ogs), fn)
+            logger.info("extracting {:d} hogs into {:s}".format(len(ogs), fn))
             self.create_new_orthoxml(fn, ogs)
         else:
             for og in self._iter_toplevel_groups():
                 if hogs_to_extract is None or int(og.get("id")) in hogs_to_extract:
                     hog_nr = int(og.get("id"))
-                    hog_id = "HOG{:07d}.orthoxml".format(hog_nr)
+                    hog_id = "HOG{:06d}.orthoxml".format(hog_nr)
                     fname = os.path.join(self.cache_dir, hog_id)
-                    logger.info("extracting %s into %s", hog_id, fname)
+                    logger.info("extracting {} into {}".format(hog_id, fname))
                     self.create_new_orthoxml(fname, [og])
 
     def iter_generefs_in_og(self, og_node):
         for node in og_node.iterdescendants("{http://orthoXML.org/2011/}geneRef"):
             yield node
 
     def get_gene_via_generef(self, genesref_ids):
@@ -153,15 +148,18 @@
 
         :param fn: the filename of the output file. The path needs to exists
             prior to calling this method.
         :param OGs: the orthologGroup elements that should be included in the
             new output file."""
         # Get element to store
         for og_node in OGs:
-            gene_ids = [gene_ref_elem.get("id") for gene_ref_elem in self.iter_generefs_in_og(og_node)]
+            gene_ids = [
+                gene_ref_elem.get("id")
+                for gene_ref_elem in self.iter_generefs_in_og(og_node)
+            ]
         gene_els = self.get_gene_via_generef(gene_ids)
 
         # Get all information to store
         zoo = {}  # <- {key:sp_etree || value: {key:db_el || values:[list_genes]}}
         for gene_el in gene_els:  # <- for all gene el
             db_el = gene_el.getparent().getparent()
             sp_el = db_el.getparent()
@@ -199,16 +197,15 @@
                 for gene_el in zoo[species_el][db_el]:
                     gene_xml = etree.SubElement(genes_xml, "gene")
                     for attr, value in gene_el.attrib.items():
                         gene_xml.set(attr, value)
 
         groupsxml = etree.SubElement(etree_2_dump, "groups")
         for og_et in OGs:
-            if not og_et.get("id").startswith("HOG:{:s}".format(self.release_char)):
-                og_et.set(
-                    "id",
-                    "HOG:{:s}{:07d}".format(self.release_char, int(og_et.get("id"))),
-                )
+            if not og_et.get("id").startswith("HOG:"):
+                og_et.set("id", "HOG:{:07d}".format(int(og_et.get("id"))))
             groupsxml.append(og_et)
 
         tree = etree.ElementTree(etree_2_dump)
-        tree.write(fn, xml_declaration=True, encoding="utf-8", method="xml", pretty_print=True)
+        tree.write(
+            fn, xml_declaration=True, encoding="utf-8", method="xml", pretty_print=True
+        )
```

### Comparing `pyoma-0.13.2/pyoma/browser/ancestral_synteny.py` & `pyoma-0.9.4/pyoma/browser/ancestral_synteny.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,49 +44,58 @@
 
 
 def assign_ancestral_synteny(ham):
     for tree_node in ham.taxonomy.tree.traverse("postorder"):
         try:
             genome = tree_node.genome
         except AttributeError:
-            logger.warning("No genome stored for %s", tree_node.name)
+            logger.warning("No genome stored for {}".format(tree_node.name))
             continue
 
         if isinstance(tree_node.genome, pyham.ExtantGenome):
-            logger.info("synteny for extant genome '%s' already assigned", tree_node.genome)
+            logger.info(
+                "synteny for extant genome '{}' already assigned".format(
+                    tree_node.genome
+                )
+            )
             continue
         elif isinstance(tree_node.genome, pyham.AncestralGenome):
             graph = nx.Graph()
             graph.add_nodes_from(tree_node.genome.genes)
             for child in tree_node.children:
                 # we remove nodes that do not have a parent hog and connect their neighbors
                 # (given they have exactly two neighbors) in a working copy that is used
                 # to propagate the synteny graph to the higher level.
                 G = child.synteny.copy()
                 remove_nodes_on_path_without_parents(G)
                 # cleanup graph if they get too big
                 delete_irrelevant_edges(G, min_importance=7, max_neighbors=8)
                 for u, v, weight in G.edges.data("weight", default=1):
-                    if u.parent is not None and v.parent is not None and u.parent != v.parent:
+                    if (
+                        u.parent is not None
+                        and v.parent is not None
+                        and u.parent != v.parent
+                    ):
                         assert u.parent in graph.nodes
                         assert v.parent in graph.nodes
                         parent_edge = (u.parent, v.parent)
                         if graph.has_edge(*parent_edge):
                             graph[parent_edge[0]][parent_edge[1]]["weight"] += weight
                         else:
                             graph.add_edge(*parent_edge, weight=weight)
-            logger.info("build graph for %s: %s", tree_node.name, nx.info(graph))
+            logger.info("build graph for {}: {}".format(tree_node.name, nx.info(graph)))
             remove_forks_from_gene_losses(graph)
             tree_node.add_feature("synteny", graph)
             logger.info(
-                "Synteny for ancestral genome '%s' created. |V|=%d, |E|=%d, |CC|=%d",
-                tree_node.name,
-                graph.number_of_nodes(),
-                graph.number_of_edges(),
-                nx.number_connected_components(graph),
+                "Synteny for ancestral genome '{}' created. |V|={}, |E|={}, |CC|={}".format(
+                    tree_node.name,
+                    graph.number_of_nodes(),
+                    graph.number_of_edges(),
+                    nx.number_connected_components(graph),
+                )
             )
             yield tree_node.name, graph
 
 
 def remove_nodes_on_path_without_parents(G: nx.Graph):
     """Modifies inplace the Graph such that all nodes
     that have exactly two neighbors and do not have a parent
@@ -122,15 +131,19 @@
                 G.add_edge(
                     left,
                     right,
                     weight=max(G[left][node]["weight"], G[right][node]["weight"]),
                 )
                 G.remove_node(node)
                 cnt_removed_nodes += 1
-    logger.info("removed {} nodes that have synteny but no parent hog.".format(cnt_removed_nodes))
+    logger.info(
+        "removed {} nodes that have synteny but no parent hog.".format(
+            cnt_removed_nodes
+        )
+    )
 
 
 def delete_irrelevant_edges(G: nx.Graph, min_importance=10, max_neighbors=10):
     """removes edges that are no longer relevant.
 
     :Example:
     >>> G = nx.Graph()
@@ -164,15 +177,15 @@
                 if eattr["weight"] < remove_edge_under_weight:
                     if "remove" in eattr:
                         to_remove.append((u, v))
                     else:
                         eattr["remove"] = 1
         G.remove_edges_from(to_remove)
         cnt_removed_edges += len(to_remove)
-    logger.info("removed %d irrelevant edges", cnt_removed_edges)
+    logger.info("removed {} irrelevant edges".format(cnt_removed_edges))
 
 
 def remove_forks_from_gene_losses(G: nx.Graph):
     """Remove forks in the graph that originate from gene losses
     on the child level.
 
     <h_a>  --  <h_i>  --  <h_j>  -- <h_b>
@@ -182,15 +195,17 @@
     this is the base case to remove the edge between h_i and h_j.
     <h_k> has to be at least one hog, but can also be more, but
     the path from h_i to h_j via h_k needs to be simple, e.g. no
     further branching.
     """
     logger.info("starting remove_fork_from_gene_losses...")
     deg_3_nodes = (n[0] for n in G.degree if n[1] == 3)
-    pot_cases = list(filter(lambda uv: G.has_edge(*uv), itertools.combinations(deg_3_nodes, 2)))
+    pot_cases = list(
+        filter(lambda uv: G.has_edge(*uv), itertools.combinations(deg_3_nodes, 2))
+    )
     removed_forks = 0
     for u, v in pot_cases:
         pgen = nx.shortest_simple_paths(G, u, v)
         direct = next(pgen)  # direct edge between u,v. to be removed
         try:
             next_path = next(pgen)
         except StopIteration:
@@ -205,17 +220,23 @@
         # remove direct path, reweight next_path
         w = G.edges[u, v]["weight"]
         G.remove_edge(u, v)
         for i in range(len(next_path) - 1):
             G.edges[next_path[i], next_path[i + 1]]["weight"] += w
         removed_forks += 1
         logger.debug(
-            "removed edge from ({},{}), found other path of len {}: {}".format(u, v, len(next_path), next_path)
+            "removed edge from ({},{}), found other path of len {}: {}".format(
+                u, v, len(next_path), next_path
+            )
+        )
+    logger.info(
+        "removed {} forks in G(|V|={},|E|={})".format(
+            removed_forks, G.number_of_nodes(), G.number_of_edges()
         )
-    logger.info("removed {} forks in G(|V|={},|E|={})".format(removed_forks, G.number_of_nodes(), G.number_of_edges()))
+    )
     logger.info("finished remove_fork_from_gene_losses")
 
 
 def extract_hog_row_links(graph, hogid_2_hogrow_lookup, level):
     def map_id(id):
         try:
             k = id.index("_")
@@ -227,40 +248,43 @@
     edges = []
     nr_errors = 0
     for u, v, w in graph.edges.data("weight", default=1):
         try:
             edges.append((map_id(u), map_id(v), w))
         except KeyError as e:
             nr_errors += 1
-            logger.error("unmappable relation ({}, {}) on level {}: {}".format(u, v, level, e))
+            logger.error(
+                "unmappable relation ({}, {}) on level {}: {}".format(u, v, level, e)
+            )
     if nr_errors > 0:
-        logger.warning("%s errors on level %s", nr_errors, level)
+        logger.warning("{} errors on level {}".format(nr_errors, level))
     return numpy.array(edges, dtype=tables.dtype_from_descr(AncestralSyntenyRels()))
 
 
 def taxid_from_level(h5, level):
     try:
         taxnode = h5.tax.get_taxnode_from_name_or_taxid(level)
         taxid = int(taxnode["NCBITaxonId"])
     except KeyError as e:
         if level == "LUCA":
             taxid = 0
         else:
             raise
-    logger.info("level '%s' -> taxid = %s", level, taxid)
+    logger.info("level '{}' -> taxid = {}".format(level, taxid))
     return taxid
 
 
 @concurrent.process(timeout=1200)
 def hogid_2_rownr(h5, level):
     lookup = {}
-    row_iter = h5.get_hdf5_handle().root.HogLevel.where("Level == lev", {"lev": level.encode("utf-8")})
+    level_query = "Level == {!r}".format(level.encode("utf-8"))
+    row_iter = h5.get_hdf5_handle().root.HogLevel.where(level_query)
     for row in row_iter:
         lookup[row["ID"].decode()] = row.nrow
-    logger.info("hogmap: found %s hog at level %s", len(lookup), level)
+    logger.info("hogmap: found {} hog at level {}".format(len(lookup), level))
     return lookup
 
 
 def level_only_graph_with_hogid_nodes(graph: nx.Graph) -> nx.Graph:
     G = nx.relabel_nodes(graph, lambda n: n.hog_id)
     return G
 
@@ -281,22 +305,24 @@
         future = hogid_2_rownr(h5, level)
         try:
             hogid_lookup = future.result()
             taxid = taxid_from_level(h5, level)
             edges = extract_hog_row_links(shallow_graph, hogid_lookup, level)
             synteny_graphs_mapped[taxid] = edges
         except TimeoutError as error:
-            logger.error("hogid_2_rownr took longer than %d seconds".format(error.args[1]))
+            logger.error(
+                "hogid_2_rownr took longer than %d seconds".format(error.args[1])
+            )
         except ProcessExpired as error:
-            logger.error("%s. Exit code: %s}", error, error.exitcode)
+            logger.error("{}. Exit code: {}}".format(error, error.exitcode))
         except Exception as error:
-            logger.exception("hogid_2_rownr raised %s", error)
+            logger.exception("hogid_2_rownr raised {}".format(error))
 
         if cnt % 200 == 0:
-            logger.info("closing and reopening %s file", h5name)
+            logger.info("closing and reopening {} file".format(h5name))
             h5.close()
             h5 = db.Database(h5name)
     h5.close()
     return ham, synteny_graphs_mapped
 
 
 def plot_graph_neighborhood(G, node, steps=2):
@@ -324,15 +350,17 @@
     with tables.open_file(h5name, "a") as h5:
         node = h5.create_group(
             "/",
             "AncestralSynteny",
             title="Graph of HOGs (identified by rowidx in HogLevel table). Per tax level",
         )
         for level, edges in hog_edges_per_level.items():
-            h5.create_table(node, "tax{}".format(level), obj=edges, expectedrows=len(edges))
+            h5.create_table(
+                node, "tax{}".format(level), obj=edges, expectedrows=len(edges)
+            )
 
 
 if __name__ == "__main__":
     orthoxml = "/Volumes/TOSHIBA EXT/basf/All.May2020/downloads/oma-hogs.orthoXML.gz"
     tree = "/Volumes/TOSHIBA EXT/basf/All.May2020/downloads/speciestree.nwk"
     h5db = "/Volumes/TOSHIBA EXT/basf/All.May2020/data/OmaServer.h5"
     infer_synteny(orthoxml, h5db, tree)
```

### Comparing `pyoma-0.13.2/pyoma/browser/check_db_consistency.py` & `pyoma-0.9.4/pyoma/browser/check_db_consistency.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,36 +42,34 @@
         This is done for a random sample of 1000 entries"""
         SAMPLES = 1000
         nr_entries = self.db.id_resolver.max_entry_nr
         for entry_nr in random.sample(range(nr_entries + 1), SAMPLES):
             with self.subTest(entry_nr=entry_nr):
                 cdna = self.db.get_cdna(entry_nr).decode()
                 prot = self.db.get_sequence(entry_nr).decode()
-                self.assertTrue(
-                    abs(3 * len(prot) - len(cdna)) < 9,
-                    "CDS and protein sequence are too different in len: 3*{}={} vs {}".format(
-                        len(prot), 3 * len(prot), len(cdna)
-                    ),
-                )
                 self.assertTrue(self.translated_cdna_match_protein_sequence(cdna, prot))
 
     def test_increasing_offsets(self):
         entry_tab = self.db.get_hdf5_handle().get_node("/Protein/Entries")
         seq_off = -1
         cds_off = -1
         for row in entry_tab:
             self.assertLess(
                 seq_off,
                 row["SeqBufferOffset"],
-                "SeqBufferOffset decreases in row {}: {} vs {}".format(row.nrow, seq_off, row["SeqBufferOffset"]),
+                "SeqBufferOffset decreases in row {}: {} vs {}".format(
+                    row.nrow, seq_off, row["SeqBufferOffset"]
+                ),
             )
             self.assertLess(
                 cds_off,
                 row["CDNABufferOffset"],
-                "CDNABufferOffset decreases in row {}: {} vs {}".format(row.nrow, seq_off, row["CDNABufferOffset"]),
+                "CDNABufferOffset decreases in row {}: {} vs {}".format(
+                    row.nrow, seq_off, row["CDNABufferOffset"]
+                ),
             )
             seq_off = row["SeqBufferOffset"]
             cds_off = row["CDNABufferOffset"]
 
     def test_homeology_flag(self):
         genome_tab = self.db.get_hdf5_handle().get_node("/Genome")
         for g in (b"WHEAT", b"GOSHI", b"BRANA"):
@@ -86,46 +84,25 @@
                     row["IsPolyploid"],
                     "{} is recorded to be a ployploid genome".format(g),
                 )
 
     def test_synteny_scores_exist(self):
         for g in ("WHEAT", "BRANA", "GOSHI"):
             try:
-                t = self.db.get_hdf5_handle().get_node("/PairwiseRelation/{}/within".format(g))
+                t = self.db.get_hdf5_handle().get_node(
+                    "/PairwiseRelation/{}/within".format(g)
+                )
             except tables.NoSuchNodeError:
                 # if species does not exist, we skip - not all datasets will have these genomes
                 continue
             syn_col = t.col("SyntenyConservationLocal")
             computed_pairs = numpy.where(syn_col >= 0)
-            self.assertLess(0, len(computed_pairs[0]), "No synteny values computed for {}".format(g))
-
-    def test_alignment_of_pairwise_orthologs(self):
-        SAMPLES = 500
-        nr_entries = self.db.id_resolver.max_entry_nr
-        seq_search = self.db.seq_search
-        for entry_nr1 in random.sample(range(1, nr_entries + 1), 10 * SAMPLES):
-            vps = self.db.get_vpairs(entry_nr1)
-            if len(vps) == 0:
-                continue
-            pair = random.choice(vps)
-            with self.subTest(pair=pair):
-                s1 = self.db.get_sequence(pair["EntryNr1"])
-                matches = [(pair["EntryNr2"],)]
-                alignment = list(seq_search._align_entries(s1, matches, compute_distance=True))[0]
-                score = alignment[1][0]
-                dist = alignment[1][2]
-                if pair["Score"] < 1:
-                    self.assertGreaterEqual(score, 120)
-                else:
-                    # relaxed checks, as we compute only with fix PAM matrix
-                    self.assertGreaterEqual(pair["Score"], score)
-                    self.assertLessEqual(abs(pair["Distance"] - dist), 10)
-            SAMPLES -= 1
-            if SAMPLES <= 0:
-                break
+            self.assertLess(
+                0, len(computed_pairs[0]), "No synteny values computed for {}".format(g)
+            )
 
     def test_cached_orthologs_count(self):
         SAMPLES = 80
         nr_entries = self.db.id_resolver.max_entry_nr
         for entry_nr in random.sample(range(nr_entries + 1), SAMPLES):
             with self.subTest(entry_nr=entry_nr):
                 cached_ortholog_cnts = self.db.nr_ortholog_relations(entry_nr)
```

### Comparing `pyoma-0.13.2/pyoma/browser/compute_cache.py` & `pyoma-0.9.4/pyoma/browser/compute_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+import tables
+import numpy
+import numpy.lib.recfunctions
+import multiprocessing as mp
 import collections
-import functools
-import itertools
-import json
 import logging
-import multiprocessing as mp
-import os
 import signal
-import sys
+import shutil
 import time
-from os.path import commonprefix, split
-from queue import Empty
+import os
+import sys
+import functools
+import json
 
-import numpy
-import numpy.lib.recfunctions
-import tables
 from tqdm import tqdm
-
+from queue import Empty
 from .db import Database
-from .exceptions import DBConsistencyError
 from .models import ProteinEntry
 from .tablefmt import ProteinCacheInfo
+from os.path import commonprefix, split
 
 logger = logging.getLogger(__name__)
 
 Protein = collections.namedtuple("Protein", ("entry_nr", "hog_id", "group"))
 
 
 def signal_handler(signum, frame):
@@ -64,58 +62,64 @@
         timelimit_get_from_in_queue = functools.partial(self.in_queue.get, timeout=120)
 
         try:
             try:
                 for job in iter(timelimit_get_from_in_queue, None):
                     fun, params = job
                     res = getattr(self, fun)(*params)
-                    logger.debug("result for job (%s) ready", job)
+                    logger.debug('result for job ({}) ready'.format(job))
                     self.out_queue.put((job, res))
             except Empty:
-                logger.warning("No item nor termination signal received in Queue. Giving up")
+                logger.warning(
+                    "No item nor termination signal received in Queue. Giving up"
+                )
                 logger.exception("Work-queue is empty")
             self.out_queue.put("DONE")
         except KeyboardInterrupt:
             logger.info("received interrupt. Terminating")
         self.db.close()
-        logger.info("terminating worker process %s", self.name)
+        logger.info("terminating worker process {}".format(self.name))
 
     def load_fam_members(self, fam):
         members = []
-        vals = {k: self.db.format_hogid(x).encode("utf-8") for k, x in zip(("fam", "fam_next"), (fam, fam + 1))}
+        hog_range = ["HOG:{:07d}".format(x).encode("utf8") for x in (fam, fam + 1)]
         for row in self.h5.get_node("/Protein/Entries").where(
-            "(fam <= OmaHOG) & (OmaHOG < fam_next)",
-            condvars=vals,
+            "({!r} <= OmaHOG) & (OmaHOG < {!r})".format(*hog_range)
         ):
-            members.append(Protein(row["EntryNr"], row["OmaHOG"].decode(), row["OmaGroup"]))
+            members.append(
+                Protein(row["EntryNr"], row["OmaHOG"].decode(), row["OmaGroup"])
+            )
         return members
 
     def load_vps(self, entry_nr):
         return self.db.get_vpairs(entry_nr)["EntryNr2"]
 
     def load_grp_members(self, group):
-        return [row["EntryNr"] for row in self.h5.get_node("/Protein/Entries").where("OmaGroup == {:d}".format(group))]
+        return [
+            row["EntryNr"]
+            for row in self.h5.get_node("/Protein/Entries").where(
+                "OmaGroup == {:d}".format(group)
+            )
+        ]
 
-    def analyse_fam(self, fam, rng=None):
-        logger.debug("analysing family %s", fam)
+    def analyse_fam(self, fam):
+        logger.debug("analysing family {}".format(fam))
         fam_members = self.load_fam_members(fam)
-        logger.debug("family {} with {} members; doing range {}".format(fam, len(fam_members), rng))
-        grp_members = {grp: set(self.load_grp_members(grp)) for grp in set(z.group for z in fam_members if z.group > 0)}
-        nr_memb = len(fam_members)
-        fam_iter = iter(fam_members)
-        if rng is not None:
-            nr_memb = rng[1] - rng[0]
-            fam_iter = itertools.islice(fam_members, rng[0], rng[1])
-
-        counts = numpy.zeros(nr_memb, dtype=tables.dtype_from_descr(ProteinCacheInfo))
+        logger.debug("family {} with {} members".format(fam, len(fam_members)))
+        grp_members = {
+            grp: set(self.load_grp_members(grp))
+            for grp in set(z.group for z in fam_members if z.group > 0)
+        }
+        counts = numpy.zeros(
+            len(fam_members), dtype=tables.dtype_from_descr(ProteinCacheInfo)
+        )
         for i, p1 in tqdm(
-            enumerate(fam_iter),
+            enumerate(fam_members),
             disable=len(fam_members) < 500,
             desc="fam {}".format(fam),
-            total=nr_memb,
         ):
             vps = set(self.load_vps(p1.entry_nr))
             ind_orth = set(p2.entry_nr for p2 in fam_members if are_orthologous(p1, p2))
             grp = grp_members.get(p1.group, set([])) - set([p1.entry_nr])
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(
                     "entry {}: vps: {} ipw: {} grp: {} any: {}".format(
@@ -131,42 +135,42 @@
             counts[i]["NrHogInducedPWOrthologs"] = len(ind_orth)
             counts[i]["NrHogInducedPWParalogs"] = len(fam_members) - len(ind_orth) - 1
             counts[i]["NrOMAGroupOrthologs"] = len(grp)
             counts[i]["NrAnyOrthologs"] = len(vps | ind_orth | grp)
         return counts
 
     def analyse_singleton(self, entry_nr, group_nr):
-        logger.debug("analysing singleton %s (grp %s)", entry_nr, group_nr)
+        logger.debug("analysing singleton {} (grp {})".format(entry_nr, group_nr))
         vps = set(self.load_vps(entry_nr))
         grp_members = set([])
         if group_nr > 0:
             grp_members = set(self.load_grp_members(group_nr))
         counts = numpy.array(
             [(entry_nr, len(vps), 0, 0, len(grp_members), len(vps | grp_members))],
             dtype=tables.dtype_from_descr(ProteinCacheInfo),
         )
         return counts
 
     def compute_familydata_json(self, fam):
         famhog_id = self.db.format_hogid(fam)
-        logger.debug("analysing family %s", fam)
+        logger.debug("analysing family {}".format(fam))
         fam_members = self.load_fam_members(fam)
-        logger.debug("family %s with %d members", fam, len(fam_members))
+        logger.debug("family {} with {} members".format(fam, len(fam_members)))
         if len(fam_members) > 50000:
             # this will likely fail to compute the MDS for so many points
             # let's skip it for now.
             genes_null_similarity = set(p.entry_nr for p in fam_members)
         else:
             try:
                 (
                     genes_null_similarity,
                     gene_similarity_vals,
                 ) = self.db.get_gene_similarities_hog(famhog_id)
             except Exception as e:
-                logger.error("gene_similarity failed for %s: %s", fam, e)
+                print("gene_similarity failed for {}: {}".format(fam, e))
                 raise
         final_json_output = []
         for p1 in fam_members:
             to_append = {}
             protein = ProteinEntry(self.db, p1.entry_nr)
             to_append["id"] = p1.entry_nr
             to_append["protid"] = protein.omaid
@@ -180,14 +184,18 @@
             else:
                 to_append["gene_similarity"] = gene_similarity_vals[p1.entry_nr]
             final_json_output.append(to_append)
 
         return json.dumps(final_json_output)
 
 
+class ConsistenceyError(Exception):
+    pass
+
+
 class ResultHandler:
     def __init__(self, cache_file):
         self.cache_file = cache_file
         self.ortholog_count_result = []
         self.family_json_offset = []
         self.in_memory_json_buffer = []
         self.buffer_offset = 0
@@ -200,40 +208,51 @@
             try:
                 res = [h5.get_node(node).read()]
             except tables.NoSuchNodeError:
                 res = []
             return res
 
         with tables.open_file(self.cache_file) as cache:
-            self.ortholog_count_result = resilient_load_data_node(cache, "/ortholog_counts")
-            self.family_json_offset = resilient_load_data_node(cache, "/family_json/offset")
+            self.ortholog_count_result = resilient_load_data_node(
+                cache, "/ortholog_counts"
+            )
+            self.family_json_offset = resilient_load_data_node(
+                cache, "/family_json/offset"
+            )
             self.buffer_offset = len(cache.root.family_json.buffer)
             self.jobs = cache.root.pending_jobs.read(0)[0]
 
     def add_jobs(self, jobs):
         self.jobs.extend(jobs)
 
     def handle_result(self, job, result):
         if job[0] == "compute_familydata_json":
             self.store_familydata_json_result(job, result)
         elif job[0] in ("analyse_fam", "analyse_singleton"):
             self.store_ortholog_count_result(job, result)
         else:
             raise ValueError("Unexpected result type")
         self.jobs.remove(job)
-        if time.time() - self._last_cache_timestamp > 300 or sum(len(z) for z in self.in_memory_json_buffer) > 100e6:
+        if (
+            time.time() - self._last_cache_timestamp > 300
+            or sum(len(z) for z in self.in_memory_json_buffer) > 100e6
+        ):
             self.write_to_disk()
 
     def store_familydata_json_result(self, job, result):
         fam = job[1][0]
         encoded_json = result.encode("utf-8")
-        json_as_np = numpy.ndarray((len(encoded_json),), buffer=encoded_json, dtype=tables.StringAtom(1))
+        json_as_np = numpy.ndarray(
+            (len(encoded_json),), buffer=encoded_json, dtype=tables.StringAtom(1)
+        )
         self.in_memory_json_buffer.append(json_as_np)
         self.family_json_offset.append(
-            numpy.array([(fam, self.buffer_offset, len(encoded_json))], dtype=self._offset_dtype)
+            numpy.array(
+                [(fam, self.buffer_offset, len(encoded_json))], dtype=self._offset_dtype
+            )
         )
         self.buffer_offset += len(encoded_json)
 
     def store_ortholog_count_result(self, job, result):
         self.ortholog_count_result.append(result)
 
     def write_to_disk(self):
@@ -254,29 +273,37 @@
             if transfer_data:
                 with tables.open_file(self.cache_file + ".0", "r") as prev:
                     buf.append(prev.root.family_json.buffer.read())
             for el in self.in_memory_json_buffer:
                 buf.append(el)
             buf.flush()
             if len(self.family_json_offset) > 0:
-                off = numpy.lib.recfunctions.stack_arrays(self.family_json_offset, usemask=False)
+                off = numpy.lib.recfunctions.stack_arrays(
+                    self.family_json_offset, usemask=False
+                )
                 h5.create_table("/family_json", "offset", None, obj=off)
 
             if len(self.ortholog_count_result) > 0:
-                cnts = numpy.lib.recfunctions.stack_arrays(self.ortholog_count_result, usemask=False)
+                cnts = numpy.lib.recfunctions.stack_arrays(
+                    self.ortholog_count_result, usemask=False
+                )
                 h5.create_table("/", "ortholog_counts", ProteinCacheInfo, obj=cnts)
 
             a = h5.create_vlarray("/", "pending_jobs", tables.ObjectAtom())
             a.append(self.jobs)
             h5.flush()
             if len(buf) != self.buffer_offset:
-                raise DBConsistencyError("buffer has unexpeced length: {}vs{}".format(len(buf), self.buffer_offset))
+                raise ConsistenceyError(
+                    "buffer has unexpeced length: {}vs{}".format(
+                        len(buf), self.buffer_offset
+                    )
+                )
             self.in_memory_json_buffer = []
             self._last_cache_timestamp = time.time()
-            logger.info("finished writing milestone to %s", self.cache_file)
+            logger.info("finished writing milestone to {}".format(self.cache_file))
 
 
 def build_cache(db_fpath, nr_procs=None, from_cache=None):
     request_queue = mp.Queue()
     result_queue = mp.Queue()
     nr_procs = nr_procs if nr_procs else mp.cpu_count()
 
@@ -287,22 +314,32 @@
         result_handler.load_cache()
         jobs = result_handler.jobs
         logger.debug(jobs)
     else:
         nr_fams = db.get_nr_toplevel_hogs()
         singletons = [
             (int(r["EntryNr"]), int(r["OmaGroup"]))
-            for r in db.get_hdf5_handle().get_node("/Protein/Entries").where('OmaHOG == b""')
+            for r in db.get_hdf5_handle()
+            .get_node("/Protein/Entries")
+            .where('OmaHOG == b""')
         ]
 
-        logger.info("found {} hog and {} singleton jobs to be computed".format(nr_fams, len(singletons)))
+        logger.info(
+            "found {} hog and {} singleton jobs to be computed".format(
+                nr_fams, len(singletons)
+            )
+        )
         jobs = [("analyse_fam", (fam + 1,)) for fam in range(nr_fams)]
         jobs.extend([("compute_familydata_json", (fam + 1,)) for fam in range(nr_fams)])
         jobs.extend([("analyse_singleton", singleton) for singleton in singletons])
-        logger.info("nr of jobs: {} (expected {})".format(len(jobs), 2 * nr_fams + len(singletons)))
+        logger.info(
+            "nr of jobs: {} (expected {})".format(
+                len(jobs), 2 * nr_fams + len(singletons)
+            )
+        )
         result_handler.add_jobs(jobs)
     db.close()
 
     workers = []
     for i in range(nr_procs):
         w = CacheBuilderWorker(db_fpath, request_queue, result_queue, daemon=True)
         w.start()
@@ -319,57 +356,63 @@
     finished = 0
     try:
         logger.info("start to receive results")
         last_cache_timestamp = time.time()
         for reply in tqdm(iter(result_queue.get, None), total=len(jobs)):
             if reply == "DONE":
                 finished += 1
-                logger.info("%d workers finished", finished)
+                logger.info("{} workers finished".format(finished))
                 if finished == nr_procs:
                     if len(pending_jobs) > 0:
-                        logger.error("still %d pending jobs...: %s", len(pending_jobs), pending_jobs)
+                        logger.error(
+                            "still {} pending jobs...: {}".format(
+                                len(pending_jobs), pending_jobs
+                            )
+                        )
                     break
             else:
                 job, res = reply
-                logger.debug("received result for job %s", job)
+                logger.debug("received result for job {})".format(job))
                 result_handler.handle_result(job, res)
         result_handler.write_to_disk()
         logger.info("exit receiver loop. joining workers...")
         for w in workers:
             w.join()
         logger.debug("all workers joined")
     except KeyboardInterrupt as e:
         logger.info("recived interrupt. writeing out temp results")
         result_handler.write_to_disk()
         sys.exit(99)
 
-    ret = numpy.lib.recfunctions.stack_arrays(result_handler.ortholog_count_result, usemask=False)
+    ret = numpy.lib.recfunctions.stack_arrays(
+        result_handler.ortholog_count_result, usemask=False
+    )
     ret.sort(order="EntryNr")
-    logger.info("sorted results: %s", ret)
+    logger.info("sorted results: {}".format(ret))
     assert check_all_there(nr_entries, ret)
     return ret
 
 
 def check_all_there(nr_prots, cache):
     if len(cache) == nr_prots:
         return True
     missings = set(range(1, nr_prots + 1)) - set(cache["EntryNr"])
-    logger.error("Missing cache value for %s", missings)
+    logger.error("Missing cache value for {}".format(missings))
     return False
 
 
 def compute_and_store_cached_data(db_fpath, nr_procs=None, force=False, tmp_cache=None):
     ortholog_cnts_cache_path = "/Protein/OrthologsCountCache"
     if tmp_cache is None:
         tmp_cache = "/tmp/compute_cache.h5"
     with tables.open_file(db_fpath, "a") as h5:
         try:
             n = h5.get_node(ortholog_cnts_cache_path)
             if force:
-                h5.remove_node(ortholog_cnts_cache_path)
+                h5.remove_node(orthologs_cnts_cache_path)
             else:
                 return
         except tables.NoSuchNodeError:
             pass
 
     signal.signal(signal.SIGUSR2, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
@@ -377,27 +420,36 @@
     update_hdf5_from_cachefile(db_fpath, tmp_cache)
 
 
 def update_hdf5_from_cachefile(db_fpath, tmp_cache):
     ortholog_cnts_cache_path = "/Protein/OrthologsCountCache"
     path, name = split(ortholog_cnts_cache_path)
 
-    with tables.open_file(db_fpath, "a") as h5, tables.open_file(tmp_cache, "r") as cache_h5:
+    with tables.open_file(db_fpath, "a") as h5, \
+         tables.open_file(tmp_cache, "r") as cache_h5:
         cached_cnts = cache_h5.get_node("/ortholog_counts").read()
         cached_cnts.sort(order="EntryNr")
 
-        tab = h5.create_table(path, name, ProteinCacheInfo, createparents=True, obj=cached_cnts)
+        tab = h5.create_table(
+            path, name, ProteinCacheInfo, createparents=True, obj=cached_cnts
+        )
         tab.colinstances["EntryNr"].create_csindex()
 
         json_off = cache_h5.get_node("/family_json/offset").read()
         json_off.sort(order="Fam")
         tab = h5.root.RootHOG.MetaData.read()
         for fam, off, length in json_off:
             if tab[fam - 1]["FamNr"] != fam:
-                raise DBConsistencyError("table not properly ordered")
+                raise ConsistenceyError("table not properly ordered")
             tab[fam - 1]["FamDataJsonOffset"] = off
             tab[fam - 1]["FamDataJsonLength"] = length
-        h5.root.RootHOG.MetaData.modify_column(column=tab["FamDataJsonOffset"], colname="FamDataJsonOffset")
-        h5.root.RootHOG.MetaData.modify_column(column=tab["FamDataJsonLength"], colname="FamDataJsonLength")
+        h5.root.RootHOG.MetaData.modify_column(
+            column=tab["FamDataJsonOffset"], colname="FamDataJsonOffset"
+        )
+        h5.root.RootHOG.MetaData.modify_column(
+            column=tab["FamDataJsonLength"], colname="FamDataJsonLength"
+        )
 
         json_in_buf = cache_h5.root.family_json.buffer
-        json_in_buf._f_copy(h5.root.RootHOG, "JsonBuffer", expectedrows=len(json_in_buf))
+        json_in_buf._f_copy(
+            h5.root.RootHOG, "JsonBuffer", expectedrows=len(json_in_buf)
+        )
```

### Comparing `pyoma-0.13.2/pyoma/browser/convert.drw` & `pyoma-0.9.4/pyoma/browser/convert.drw`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         g := genomes[gNr];
         gs := append(gs, [parse(GS[g,TAXONID]), g, GS[g,TotEntries],
             GS[g,TotAA], Goff[gNr],
             GS[g,SCINAME], GS[g,COMMONNAME], GS[g, SYNNAME],
             GS[g,DBRELEASE], GS[g,URL], GS[g,SOURCE], GS[g,DATE], SubGenome[g]<>0]);
     od:
 
-    _parents := []: _next_new_taxid := -2:
+    _parents := []: _next_new_taxid := -1:
     linData := sort([seq([GS[g,Lineage], g], g=genomes)]):
     SpeciesTreeR(linData, 1, 0);
 
     tab := table():
     tab['GS'] := gs:
     tab['Tax'] := _parents:
     StoreResults(json(tab));
```

### Comparing `pyoma-0.13.2/pyoma/browser/convert.py` & `pyoma-0.9.4/pyoma/browser/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import collections
 import csv
 import errno
 import fileinput
 import gzip
 import hashlib
-import io
 import itertools
 import json
 import multiprocessing as mp
 import concurrent.futures
 import operator
 import os
 import re
@@ -33,71 +32,63 @@
 from tqdm import tqdm
 
 from . import locus_parser
 from . import suffixsearch
 from . import tablefmt
 from .KmerEncoder import KmerEncoder
 from .OrthoXMLSplitter import OrthoXMLSplitter
-from .geneontology import GeneOntology, OntologyParser, FreqAwareGeneOntology
+from .compute_cache import compute_and_store_cached_data
+from .geneontology import GeneOntology, OntologyParser
 from .homoeologs import HomeologsConfidenceCalculator
 from .synteny import SyntenyScorer
 from . import hoghelper
 from .. import common, version
 
 with hooks():
     import urllib.request
 
-hog_re = re.compile(rb"((?P<prefix>HOG):)?(?P<rel>[A-Z]?)(?P<fam>\d+)(\.(?P<subfamid>[0-9a-z.]+))?$")
-
 
 class DarwinException(Exception):
-    def __init__(self, stderr, stdout):
-        msg = ["Exception running darwin. End of stdout:\n"]
-        if len(stdout) > 100:
-            msg.append(" ...[{:d}]...".format(len(stdout) - 100))
-        msg.append("{!r}".format(stdout[-100:]))
-        msg.append("End of stderr:\n")
-        if len(stderr) > 100:
-            msg.append(" ...[{:d}]...".format(len(stderr) - 200))
-        msg.append("{!r}".format(stderr[-200:]))
-        super(DarwinException, self).__init__("".join(msg))
-        self.stderr = stderr
-        self.stdout = stdout
+    pass
 
 
 def callDarwinExport(func, drwfile=None):
     """Function starts a darwin session, loads convert.drw file
     and calls the darwin function passed as argument. The output
     is expected to be written by darwin in json format into the
     file specified by 'outfn'.
     This function returns the parsed json datastructure"""
 
     with NamedTemporaryFile(suffix=".dat") as tmpfile:
         if drwfile is None:
             drwfile = os.path.abspath(os.path.splitext(__file__)[0] + ".drw")
         # with open(os.devnull, 'w') as DEVNULL:
         stacksize = resource.getrlimit(resource.RLIMIT_STACK)
-        common.package_logger.debug("current stacklimit: %s", stacksize)
-        common.package_logger.debug("setting stacklimit: %s", (max(stacksize) - 1, stacksize[1]))
+        common.package_logger.debug("current stacklimit: {}".format(stacksize))
+        common.package_logger.debug(
+            "setting stacklimit: {}".format((max(stacksize) - 1, stacksize[1]))
+        )
         resource.setrlimit(resource.RLIMIT_STACK, (min(stacksize), stacksize[1]))
         p = subprocess.Popen(
             ["darwin", "-q", "-E"],
             stdin=subprocess.PIPE,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
         )
-        drw_cmd = "outfn := '{}': ReadProgram('{}'): {}; done;".format(tmpfile.name, drwfile, func).encode("utf-8")
-        common.package_logger.debug("calling darwin function: %s", func)
-        stdout, stderr = p.communicate(input=drw_cmd)
+        drw_cmd = "outfn := '{}': ReadProgram('{}'): {}; done;".format(
+            tmpfile.name, drwfile, func
+        ).encode("utf-8")
+        common.package_logger.debug("calling darwin function: {}".format(func))
+        (stdout, stderr) = p.communicate(input=drw_cmd)
         if p.returncode > 0:
-            raise DarwinException(stderr, stdout)
+            raise DarwinException(p.stderr.read())
 
         trans_tab = "".join(str(chr(x)) for x in range(128)) + " " * 128
         if not os.path.exists(tmpfile.name) or os.path.getsize(tmpfile.name) == 0:
-            raise DarwinException(stderr, stdout)
+            raise DarwinException(p.stderr.read())
         with open(tmpfile.name, "r") as jsonData:
             rawdata = jsonData.read()
             return json.loads(rawdata.translate(trans_tab))
 
 
 def uniq(seq, transform=None):
     """return uniq elements of a list, preserving order
@@ -179,23 +170,25 @@
                     names=[_[0] for _ in tsv_dtype],
                     delimiter="\t",
                     usecols=(0, 1, 2, 3, 4, 5),
                     converters={
                         "EntryNr1": lambda nr: int(nr) + off1,
                         "EntryNr2": lambda nr: int(nr) + off2,
                         "RelType": lambda rel: (
-                            relEnum[rel[::read_dir].decode()] if len(rel) <= 3 else relEnum[rel.decode()]
+                            relEnum[rel[::read_dir].decode()]
+                            if len(rel) <= 3
+                            else relEnum[rel.decode()]
                         ),
                         "Score": lambda score: float(score) / 100,
                     },
                 )
                 break
         except OSError as e:
             if curNr < 1:
-                common.package_logger.info("tried to load %s", curFn)
+                common.package_logger.info("tried to load {}".format(curFn))
                 pass
             else:
                 raise e
 
     if swap:
         reversed_cols = tuple(data.dtype.names[z] for z in (1, 0, 2, 3, 4, 5))
         data.dtype.names = reversed_cols
@@ -204,48 +197,48 @@
     full_table[common_cols] = data[common_cols]
     for col_not_in_tsv in set(full_table.dtype.names) - set(data.dtype.names):
         full_table[col_not_in_tsv] = rel_desc.columns[col_not_in_tsv].dflt
     return full_table
 
 
 def read_vps_from_tsv(gs, ref_genome, basedir=None):
-    ref_genome_idx = gs.get_where_list("(UniProtSpeciesCode==code)", condvars={"code": ref_genome})[0]
+    ref_genome_idx = gs.get_where_list("(UniProtSpeciesCode=={!r})".format(ref_genome))[
+        0
+    ]
     job_args = []
     if basedir is None:
         basedir = os.path.join(os.environ["DARWIN_OMADATA_PATH"], "Phase4")
     for g in range(len(gs)):
         if g == ref_genome_idx:
             continue
         g1, g2 = sorted((g, ref_genome_idx))
         off1, off2 = gs.read_coordinates(numpy.array((g1, g2)), "EntryOff")
         fn = os.path.join(
             basedir,
             gs.cols.UniProtSpeciesCode[g1].decode(),
             gs.cols.UniProtSpeciesCode[g2].decode() + ".orth.txt.gz",
         )
         tup = (fn, off1, off2, g1 != ref_genome_idx)
-        common.package_logger.debug("adding job: %s", tup)
+        common.package_logger.debug("adding job: {}".format(tup))
         job_args.append(tup)
 
     pool = mp.Pool(processes=min(os.cpu_count(), 12))
     all_pairs = pool.map(load_tsv_to_numpy, job_args)
     pool.close()
-    common.package_logger.info("loaded vps for %s", ref_genome.decode())
+    common.package_logger.info("loaded vps for {}".format(ref_genome.decode()))
     return numpy.lib.recfunctions.stack_arrays(all_pairs, usemask=False)
 
 
 def load_hogs_at_level(fname, level):
     with tables.open_file(fname, "r") as h5:
         lev = level.encode("utf-8") if isinstance(level, str) else level
         tab = h5.get_node("/HogLevel")
-        extended_dtype = numpy.dtype(tab.dtype.descr + [("HogLevelRowIdx", "i4")])
-        hog_it = (tuple(row.fetch_all_fields()) + (row.nrow,) for row in tab.where("Level == lev"))
-        hogs = numpy.fromiter(hog_it, dtype=extended_dtype)
+        hog_it = (row.fetch_all_fields() for row in tab.where("Level == lev"))
+        hogs = numpy.fromiter(hog_it, dtype=tab.dtype)
         hogs.sort(order="ID")
-        hogs["IdxPerLevelTable"] = numpy.arange(len(hogs))
         return hogs
 
 
 class DataImportError(Exception):
     pass
 
 
@@ -264,15 +257,18 @@
            `tablefmt.PairwiseRelationTable`
     :param genome_offs: a numpy array with the genome offsets, i.e. the entry
            numbers where the next genome starts
 
     :returns: a modified version of data
     """
     typEnum = tablefmt.PairwiseRelationTable.columns.get("RelType").enum
-    query_type = {val: "m" if cnt > 1 else "1" for val, cnt in zip(*numpy.unique(data["EntryNr2"], return_counts=True))}
+    query_type = {
+        val: "m" if cnt > 1 else "1"
+        for val, cnt in zip(*numpy.unique(data["EntryNr2"], return_counts=True))
+    }
 
     def genome_idx(enr):
         return numpy.searchsorted(genome_offs, enr - 1, side="right")
 
     g0 = genome_idx(data[0]["EntryNr2"])
     it = numpy.nditer(data, flags=["c_index"], op_flags=["readwrite"])
     while not it.finished:
@@ -343,25 +339,31 @@
         pass
     lookup = create_fast_famhoglevel_lookup(hoglevtab)
     node, name = os.path.split(array_path)
     h5.create_table(node, name, expectedrows=len(lookup), obj=lookup)
 
 
 class DarwinExporter(object):
-    DB_SCHEMA_VERSION = "3.6"
+    DB_SCHEMA_VERSION = "3.4"
     DRW_CONVERT_FILE = os.path.abspath(os.path.splitext(__file__)[0] + ".drw")
 
     def __init__(self, path, logger=None, mode=None):
         self.logger = logger if logger is not None else common.package_logger
-        fn = os.path.normpath(os.path.join(os.getenv("DARWIN_BROWSERDATA_PATH", ""), path))
+        fn = os.path.normpath(
+            os.path.join(os.getenv("DARWIN_BROWSERDATA_PATH", ""), path)
+        )
         if mode is None:
             mode = "append" if os.path.exists(fn) else "write"
         self._compr = tables.Filters(complevel=6, complib="zlib", fletcher32=True)
         self.h5 = tables.open_file(fn, mode=mode[0], filters=self._compr)
-        self.logger.info("opened {} in {} mode, options {} ; pyoma {}".format(fn, mode, str(self._compr), version()))
+        self.logger.info(
+            "opened {} in {} mode, options {} ; pyoma {}".format(
+                fn, mode, str(self._compr), version()
+            )
+        )
         if mode == "write":
             self.h5.root._f_setattr("convertion_start", time.strftime("%c"))
             self.h5.root._f_setattr("pyoma_version", version())
 
     def call_darwin_export(self, func):
         return callDarwinExport(func, self.DRW_CONVERT_FILE)
 
@@ -389,57 +391,59 @@
 
     def get_version(self):
         """return version of the dataset.
 
         Default implementation searches for 'mname' in Matrix or matrix_stats.drw files.
         """
         for fname in ("Matrix", "matrix_stats.drw"):
-            with open(os.path.join(os.environ["DARWIN_BROWSERDATA_PATH"], fname), "r") as fh:
+            with open(
+                os.path.join(os.environ["DARWIN_BROWSERDATA_PATH"], fname), "r"
+            ) as fh:
                 for i, line in enumerate(fh):
                     if line.startswith("mname :="):
                         match = re.match(r"mname := \'(?P<version>[^\']*)\'", line)
                         return match.group("version")
                     if i > 1000:
                         break
         raise DataImportError("No version information found")
 
-    def add_version(self, release_char=None):
-        if release_char is not None:
-            if not re.match(r"^[A-Z]*$", release_char):
-                raise ValueError(
-                    "Unexpected release_char argument: {}. Must be a capital ascii character".format(release_char)
-                )
-        else:
-            release_char = ""
+    def add_version(self):
         version = self.get_version()
         self.h5.set_node_attr("/", "oma_version", version)
-        self.h5.set_node_attr("/", "oma_release_char", release_char)
         self.h5.set_node_attr("/", "pytables", tables.get_pytables_version())
         self.h5.set_node_attr("/", "hdf5_version", tables.get_hdf5_version())
         self.h5.set_node_attr("/", "db_schema_version", self.DB_SCHEMA_VERSION)
 
     def add_species_data(self):
-        cache_file = os.path.join(os.getenv("DARWIN_NETWORK_SCRATCH_PATH", ""), "pyoma", "gs.json")
+        cache_file = os.path.join(
+            os.getenv("DARWIN_NETWORK_SCRATCH_PATH", ""), "pyoma", "gs.json"
+        )
         if os.path.exists(cache_file):
             with open(cache_file, "r") as fd:
                 data = json.load(fd)
         else:
             data = self.call_darwin_export("GetGenomeData();")
-        gstab = self.h5.create_table("/", "Genome", tablefmt.GenomeTable, expectedrows=len(data["GS"]))
+        gstab = self.h5.create_table(
+            "/", "Genome", tablefmt.GenomeTable, expectedrows=len(data["GS"])
+        )
         gs_data = self._parse_date_columns(data["GS"], gstab)
         self._write_to_table(gstab, gs_data)
         create_index_for_columns(gstab, "NCBITaxonId", "UniProtSpeciesCode", "EntryOff")
 
-        taxtab = self.h5.create_table("/", "Taxonomy", tablefmt.TaxonomyTable, expectedrows=len(data["Tax"]))
+        taxtab = self.h5.create_table(
+            "/", "Taxonomy", tablefmt.TaxonomyTable, expectedrows=len(data["Tax"])
+        )
         self._write_to_table(taxtab, _load_taxonomy_without_ref_to_itselfs(data["Tax"]))
         create_index_for_columns(taxtab, "NCBITaxonId")
 
     def _parse_date_columns(self, data, tab):
         """convert str values in a date column to epoch timestamps"""
-        time_cols = [i for i, col in enumerate(tab.colnames) if tab.coldescrs[col].kind == "time"]
+        time_cols = [
+            i for i, col in enumerate(tab.colnames) if tab.coldescrs[col].kind == "time"
+        ]
         dflts = [tab.coldflts[col] for col in tab.colnames]
 
         def map_data(col, data):
             try:
                 val = data[col]
                 if col in time_cols and isinstance(val, str):
                     if val == "":
@@ -472,15 +476,19 @@
     def _convert_to_numpyarray(self, data, tab):
         """convert a list of list dataset into a numpy rec array that
         corresponds to the table definition of `tab`.
 
         :param data: the data to be converted.
         :param tab: a pytables table node."""
 
-        enum_cols = {i: tab.get_enum(col) for (i, col) in enumerate(tab.colnames) if tab.coltypes[col] == "enum"}
+        enum_cols = {
+            i: tab.get_enum(col)
+            for (i, col) in enumerate(tab.colnames)
+            if tab.coltypes[col] == "enum"
+        }
         dflts = [tab.coldflts[col] for col in tab.colnames]
 
         def map_data(col, data):
             try:
                 val = data[col]
                 return enum_cols[col][val]
             except IndexError:
@@ -496,69 +504,82 @@
 
     def add_orthologs(self):
         genome_offs = self.h5.root.Genome.col("EntryOff")
         anygenome = self.h5.root.Genome[0]["UniProtSpeciesCode"].decode()
         basedir = None
         for base in ("DARWIN_OMADATA_PATH", "DARWIN_OMA_SCRATCH_PATH"):
             testdir = os.path.join(os.getenv(base, "/"), "Phase4", anygenome)
-            if os.path.isdir(testdir) and any(map(lambda x: x.endswith(".orth.txt.gz"), os.listdir(testdir))):
+            if os.path.isdir(testdir) and any(
+                map(lambda x: x.endswith(".orth.txt.gz"), os.listdir(testdir))
+            ):
                 basedir = os.path.join(os.getenv(base), "Phase4")
                 break
 
-        self.logger.info("using %s as base dir for pairwise orthology", basedir)
+        self.logger.info("using {} as base dir for pairwise orthology".format(basedir))
         for gs in self.h5.root.Genome.iterrows():
             genome = gs["UniProtSpeciesCode"].decode()
-            rel_node_for_genome = self._get_or_create_node("/PairwiseRelation/{}".format(genome))
+            rel_node_for_genome = self._get_or_create_node(
+                "/PairwiseRelation/{}".format(genome)
+            )
             if "VPairs" not in rel_node_for_genome:
                 cache_file = os.path.join(
                     os.getenv("DARWIN_NETWORK_SCRATCH_PATH", ""),
                     "pyoma",
                     "vps",
                     "{}.json".format(genome),
                 )
                 if os.path.exists(cache_file):
                     with open(cache_file, "r") as fd:
                         data = json.load(fd)
                 elif basedir is not None:
                     # we have the *.orth.txt.gz files in basedir
-                    data = read_vps_from_tsv(self.h5.root.Genome, genome.encode("utf-8"), basedir=basedir)
+                    data = read_vps_from_tsv(
+                        self.h5.root.Genome, genome.encode("utf-8"), basedir=basedir
+                    )
                 else:
                     # fallback to read from VPsDB
                     data = self.call_darwin_export("GetVPsForGenome({})".format(genome))
 
                 vp_tab = self.h5.create_table(
                     rel_node_for_genome,
                     "VPairs",
                     tablefmt.PairwiseRelationTable,
                     expectedrows=len(data),
                 )
                 if isinstance(data, list):
                     data = self._convert_to_numpyarray(data, vp_tab)
-                if numpy.any(data["RelType"] >= tablefmt.PairwiseRelationTable.columns.get("RelType").enum["n/a"]):
+                if numpy.any(
+                    data["RelType"]
+                    >= tablefmt.PairwiseRelationTable.columns.get("RelType").enum["n/a"]
+                ):
                     compute_ortholog_types(data, genome_offs)
                 self._write_to_table(vp_tab, data)
                 create_index_for_columns(vp_tab, "EntryNr1")
 
     def add_same_species_relations(self):
         for gs in self.h5.root.Genome.iterrows():
             genome = gs["UniProtSpeciesCode"].decode()
-            rel_node_for_genome = self._get_or_create_node("/PairwiseRelation/{}".format(genome))
+            rel_node_for_genome = self._get_or_create_node(
+                "/PairwiseRelation/{}".format(genome)
+            )
             if "within" not in rel_node_for_genome:
                 cache_file = os.path.join(
                     os.getenv("DARWIN_NETWORK_SCRATCH_PATH", ""),
                     "pyoma",
                     "cps",
                     "{}.json".format(genome),
                 )
                 if os.path.exists(cache_file):
                     with open(cache_file, "r") as fd:
                         data = json.load(fd)
                 else:
                     # fallback to read from VPsDB
-                    data = self.call_darwin_export("GetSameSpeciesRelations({})".format(genome))
+                    data = self.call_darwin_export(
+                        "GetSameSpeciesRelations({})".format(genome)
+                    )
 
                 ss_tab = self.h5.create_table(
                     rel_node_for_genome,
                     "within",
                     tablefmt.PairwiseRelationTable,
                     expectedrows=len(data),
                 )
@@ -578,34 +599,38 @@
         The computations of the scores are done using :mod:`synteny`
         module of this package."""
         # TODO: compute for non-homoeologs relation as well.
         self.logger.info("Adding synteny scores for polyploid genomes")
         polyploid_genomes = self.h5.root.Genome.where("IsPolyploid==True")
         for genome in polyploid_genomes:
             genome_code = genome["UniProtSpeciesCode"].decode()
-            self.logger.info("compute synteny score for %s", genome_code)
+            self.logger.info("compute synteny score for {}".format(genome_code))
             synteny_scorer = SyntenyScorer(self.h5, genome_code)
             rels = synteny_scorer.compute_scores()
-            self._callback_store_rel_data(genome_code, rels, [("SyntenyConservationLocal", "mean_synteny_score")])
+            self._callback_store_rel_data(
+                genome_code, rels, [("SyntenyConservationLocal", "mean_synteny_score")]
+            )
 
     def add_homoeology_confidence(self):
         """adds the homoeology confidence scores to the database.
 
         This method should be called only after the synteny scores have
         been computed and added to the database.
 
         The computations are done using :mod:`homoeologs` module."""
         self.logger.info("Adding homoeolog confidence scores")
         polyploid_genomes = self.h5.root.Genome.where("IsPolyploid==True")
         for genome in polyploid_genomes:
             genome_code = genome["UniProtSpeciesCode"].decode()
-            self.logger.info("compute homoeolog confidence for %s", genome_code)
+            self.logger.info("compute homoeolog confidence for {}".format(genome_code))
             homoeolg_scorer = HomeologsConfidenceCalculator(self.h5, genome_code)
             rels = homoeolg_scorer.calculate_scores()
-            self._callback_store_rel_data(genome_code, rels, [("Confidence", "fuzzy_confidence_scaled")])
+            self._callback_store_rel_data(
+                genome_code, rels, [("Confidence", "fuzzy_confidence_scaled")]
+            )
 
     def _callback_store_rel_data(self, genome, rels_df, assignments):
         tab = self.h5.get_node("/PairwiseRelation/{}/within".format(genome))
         df_all = pandas.DataFrame(tab.read())
         if "entry_nr1" in list(rels_df):
             enr_col_names = ["entry_nr1", "entry_nr2"]
         else:
@@ -645,16 +670,20 @@
             row["MD5ProteinHash"] = hashlib.md5(sequence.encode("utf-8")).hexdigest()
         return seqLen
 
     def add_proteins(self):
         gsNode = self.h5.get_node("/Genome")
         nrProt = sum(gsNode.cols.TotEntries)
         nrAA = sum(gsNode.cols.TotAA)
-        protGrp = self._get_or_create_node("/Protein", "Root node for protein (oma entries) information")
-        protTab = self.h5.create_table(protGrp, "Entries", tablefmt.ProteinTable, expectedrows=nrProt)
+        protGrp = self._get_or_create_node(
+            "/Protein", "Root node for protein (oma entries) information"
+        )
+        protTab = self.h5.create_table(
+            protGrp, "Entries", tablefmt.ProteinTable, expectedrows=nrProt
+        )
         seqArr = self.h5.create_earray(
             protGrp,
             "SequenceBuffer",
             tables.StringAtom(1),
             (0,),
             "concatenated protein sequences",
             expectedrows=nrAA + nrProt,
@@ -677,46 +706,51 @@
                 "prots",
                 "{}.json".format(genome),
             )
             if os.path.exists(cache_file):
                 with open(cache_file, "r") as fd:
                     data = json.load(fd)
             else:
-                data = self.call_darwin_export("GetProteinsForGenome({})".format(genome))
+                data = self.call_darwin_export(
+                    "GetProteinsForGenome({})".format(genome)
+                )
 
             if len(data["seqs"]) != gs["TotEntries"]:
                 raise DataImportError(
                     "number of entries ({:d}) does "
-                    "not match number of seqs ({:d}) for {}".format(len(data["seqs"]), gs["TotEntries"], genome)
+                    "not match number of seqs ({:d}) for {}".format(
+                        len(data["seqs"]), gs["TotEntries"], genome
+                    )
                 )
 
             locTab = self.h5.create_table(
                 "/Protein/Locus",
                 genome,
                 tablefmt.LocusTable,
                 createparents=True,
                 expectedrows=gs["TotEntries"] * 4,
             )
 
             cnt_missmatch_locus = 0
-            cnt_genes = 0
             for nr in range(gs["TotEntries"]):
                 eNr = data["off"] + nr + 1
                 protTab.row["EntryNr"] = eNr
                 protTab.row["OmaGroup"] = data["ogs"][nr]
 
-                seqOff += self._add_sequence(data["seqs"][nr], protTab.row, seqArr, seqOff)
-                cdnaOff += self._add_sequence(data["cdna"][nr], protTab.row, cdnaArr, cdnaOff, "CDNA")
+                seqOff += self._add_sequence(
+                    data["seqs"][nr], protTab.row, seqArr, seqOff
+                )
+                cdnaOff += self._add_sequence(
+                    data["cdna"][nr], protTab.row, cdnaArr, cdnaOff, "CDNA"
+                )
 
                 protTab.row["Chromosome"] = data["chrs"][nr]
                 protTab.row["AltSpliceVariant"] = data["alts"][nr]
                 protTab.row["OmaHOG"] = b" "  # will be assigned later
                 protTab.row["CanonicalId"] = b" "  # will be assigned later
-                if protTab.row["AltSpliceVariant"] == 0 or protTab.row["AltSpliceVariant"] == protTab.row["EntryNr"]:
-                    cnt_genes += 1  # main isoforms of gene
 
                 locus_str = data["locs"][nr]
                 try:
                     locus_tab = loc_parser.parse(locus_str, eNr)
                     locTab.append(locus_tab)
                     len_cds = sum(z["End"] - z["Start"] + 1 for z in locus_tab)
                     if len_cds != protTab.row["CDNABufferLength"] - 1:
@@ -732,69 +766,76 @@
                     protTab.row["LocusStrand"] = locus_tab[0]["Strand"]
                 except ValueError as e:
                     self.logger.warning(e)
                 protTab.row["SubGenome"] = data["subgenome"][nr].encode("ascii")
                 protTab.row.append()
             protTab.flush()
             seqArr.flush()
-            gs["TotGenes"] = cnt_genes
-            gs.update()
             if cnt_missmatch_locus > 0:
-                self.logger.warning("{} missmatches in exon-lengths compared to locus info".format(cnt_missmatch_locus))
+                self.logger.warning(
+                    "{} missmatches in exon-lengths compared to locus info".format(
+                        cnt_missmatch_locus
+                    )
+                )
             for n in (protTab, seqArr, locTab):
                 if n.size_in_memory != 0:
                     self.logger.info(
-                        "worte %s: compression ratio %3f%%" % (n._v_pathname, 100 * n.size_on_disk / n.size_in_memory)
+                        "worte %s: compression ratio %3f%%"
+                        % (n._v_pathname, 100 * n.size_on_disk / n.size_in_memory)
                     )
         create_index_for_columns(protTab, "EntryNr", "MD5ProteinHash")
 
     def _write_to_table(self, tab, data):
         if len(data) > 0:
             tab.append(data)
             self.logger.info(
-                "wrote %s : compression ratio %.3f%%" % (tab._v_pathname, 100 * tab.size_on_disk / tab.size_in_memory)
+                "wrote %s : compression ratio %.3f%%"
+                % (tab._v_pathname, 100 * tab.size_on_disk / tab.size_in_memory)
             )
         else:
-            self.logger.info("no data written for %s", tab._v_pathname)
+            self.logger.info("no data written for {}".format(tab._v_pathname))
 
     def add_hogs(self, hog_path=None, hog_file=None, tree_filename=None):
         """adds the HOGs to the database
 
         :param str hog_path: optional, directory where the split HOG files are stored or
                              should be stored. If directory does not exist, the hog_file
                              is split automatically into individual files and stored there.
 
         :param str hog_file: File containing all HOGs. if hog_path does not
                              exist, this file is split and stored in hog_path.
 
         :param str tree_filename: newick species tree file."""
         if hog_path is None:
-            hog_path = os.path.normpath(os.path.join(os.environ["DARWIN_NETWORK_SCRATCH_PATH"], "pyoma", "split_hogs"))
+            hog_path = os.path.normpath(
+                os.path.join(
+                    os.environ["DARWIN_NETWORK_SCRATCH_PATH"], "pyoma", "split_hogs"
+                )
+            )
         entryTab = self.h5.get_node("/Protein/Entries")
-        try:
-            release = self.h5.get_node_attr("/", "oma_release_char")
-        except AttributeError:
-            release = ""
         if tree_filename is None:
-            tree_filename = os.path.join(os.environ["DARWIN_BROWSERDATA_PATH"], "speciestree.nwk")
+            tree_filename = os.path.join(
+                os.environ["DARWIN_BROWSERDATA_PATH"], "speciestree.nwk"
+            )
         if not os.path.exists(hog_path):
             if hog_file is None:
                 hog_file = os.path.join(
                     os.environ["DARWIN_BROWSERDATA_PATH"],
                     "..",
                     "downloads",
                     "oma-hogs.orthoXML.gz",
                 )
-            splitter = OrthoXMLSplitter(hog_file, cache_dir=hog_path, release_char=release)
+            splitter = OrthoXMLSplitter(hog_file, cache_dir=hog_path)
             splitter()
         tax_tab = self.h5.get_node("/Taxonomy")
         tax_2_code = {
-            int(row["NCBITaxonId"]): row["UniProtSpeciesCode"].decode() for row in self.h5.get_node("/Genome")
+            int(row["NCBITaxonId"]): row["UniProtSpeciesCode"].decode()
+            for row in self.h5.get_node("/Genome")
         }
-        hog_converter = HogConverter(entryTab, release, tax_tab, tax_2_code)
+        hog_converter = HogConverter(entryTab, tax_tab, tax_2_code)
         hog_converter.attach_newick_taxonomy(tree_filename)
         hogTab = self.h5.create_table(
             "/",
             "HogLevel",
             tablefmt.HOGsTable,
             "nesting structure for each HOG",
             expectedrows=1e8,
@@ -822,97 +863,115 @@
             "Index",
             tablefmt.OrthoXmlHogTable,
             "Range index per HOG into OrthoXML Buffer",
             expectedrows=5e6,
         )
         for root, dirs, filenames in os.walk(hog_path):
             for fn in filenames:
-                if fn.endswith(".augmented"):
-                    continue
                 try:
                     input_file = os.path.join(root, fn)
                     out_orthoxml = input_file + ".augmented"
                     levels = hog_converter.convert_file(input_file, store=out_orthoxml)
                     hogTab.append(levels)
                     fam_nrs = set([z[0] for z in levels])
                     self.add_orthoxml(input_file, out_orthoxml, fam_nrs)
                 except Exception as e:
                     self.logger.error("an error occured while processing " + fn + ":")
                     self.logger.exception(e)
-        # flushing index table
-        self.orthoxml_index.flush()
+
         hog_converter.write_hogs()
 
     def add_orthoxml(self, orthoxml_path, augmented_orthoxml_path, fam_nrs):
         """append orthoxml file content to orthoxml_buffer array and add index for the HOG family"""
         if len(fam_nrs) > 1:
-            self.logger.warning("expected only one family per HOG file, but found {}: {}".format(len(fam_nrs), fam_nrs))
+            self.logger.warning(
+                "expected only one family per HOG file, but found {}: {}".format(
+                    len(fam_nrs), fam_nrs
+                )
+            )
             self.logger.warning(
                 " --> the orthoxml files per family will be not correct, "
                 "i.e. they will contain all families of this file."
             )
         offset = {}
         length = {}
-        for typ, fpath in zip(("base", "augmented"), (orthoxml_path, augmented_orthoxml_path)):
-            buffer = self.orthoxml_buffer if typ == "base" else self.orthoxml_buffer_augmented
+        for typ, fpath in zip(
+            ("base", "augmented"), (orthoxml_path, augmented_orthoxml_path)
+        ):
+            buffer = (
+                self.orthoxml_buffer
+                if typ == "base"
+                else self.orthoxml_buffer_augmented
+            )
             offset[typ] = len(buffer)
             try:
                 with open(fpath, "r") as fh:
                     orthoxml = fh.read().encode("utf-8")
                     length[typ] = len(orthoxml)
-                    buffer.append(numpy.ndarray((length[typ],), buffer=orthoxml, dtype=tables.StringAtom(1)))
+                    buffer.append(
+                        numpy.ndarray(
+                            (length[typ],), buffer=orthoxml, dtype=tables.StringAtom(1)
+                        )
+                    )
             except IOError:
                 length[typ] = 0
         for fam in fam_nrs:
             row = self.orthoxml_index.row
             row["Fam"] = fam
             row["HogBufferOffset"] = offset["base"]
             row["HogBufferLength"] = length["base"]
             row["HogAugmentedBufferOffset"] = offset["augmented"]
             row["HogAugmentedBufferLength"] = length["augmented"]
             row.append()
 
     def add_cache_of_hogs_by_level(self, nr_procs=None):
         self.logger.info("createing cached HogLevel table per level")
         hl_tab = self.h5.get_node("/HogLevel")
-        temp_hoglevel_file = os.path.join(os.getenv("DARWIN_NETWORK_SCRATCH_PATH"), "tmp-hoglevel.h5")
+        temp_hoglevel_file = os.path.join(
+            os.getenv("DARWIN_NETWORK_SCRATCH_PATH"), "tmp-hoglevel.h5"
+        )
         with tables.open_file(temp_hoglevel_file, "w") as hlfh:
             hl_tab._f_copy(hlfh.root)
             create_index_for_columns(hlfh.get_node("/HogLevel"), "Level")
 
         rel_levels = set(hl_tab.read(field="Level"))
-        self.logger.info("found {} levels, start extracting hogs in parallel".format(len(rel_levels)))
-        lev2tax = {row["Name"]: int(row["NCBITaxonId"]) for row in self.h5.get_node("/Taxonomy").read()}
+        self.logger.info(
+            "found {} levels, start extracting hogs in parallel".format(len(rel_levels))
+        )
+        lev2tax = {
+            row["Name"]: int(row["NCBITaxonId"])
+            for row in self.h5.get_node("/Taxonomy").read()
+        }
         lev2tax[b"LUCA"] = 0
-        idx_per_level = numpy.zeros(len(hl_tab), "i4")
         with concurrent.futures.ProcessPoolExecutor(max_workers=nr_procs) as pool:
             future_to_level = {
-                pool.submit(load_hogs_at_level, fname=temp_hoglevel_file, level=level): level for level in rel_levels
+                pool.submit(
+                    load_hogs_at_level, fname=temp_hoglevel_file, level=level
+                ): level
+                for level in rel_levels
             }
             for future in concurrent.futures.as_completed(future_to_level):
                 level = future_to_level[future]
                 try:
                     hogs = future.result()
-                    # fallback to level if taxid is not known
-                    tab_name = "tax{}".format(lev2tax.get(level, level.decode()))
                     tab = self.h5.create_table(
-                        where=f"/AncestralGenomes/{tab_name}",
-                        name="Hogs",
+                        "/Hogs_per_Level",
+                        "tax{}".format(lev2tax[level]),
                         title="cached HogLevel data for {}".format(level.decode()),
                         obj=hogs,
                         createparents=True,
                         expectedrows=len(hogs),
                     )
-                    create_index_for_columns(tab, "Fam", "IsRoot", "NrMemberGenes", "CompletenessScore")
-                    idx_per_level[hogs["HogLevelRowIdx"]] = hogs["IdxPerLevelTable"]
+                    create_index_for_columns(
+                        tab, "Fam", "IsRoot", "NrMemberGenes", "CompletenessScore"
+                    )
                 except Exception as exc:
                     msg = "cannot store cached hogs for {}".format(level)
                     self.logger.exception(msg)
                     pass
-        hl_tab.modify_column(column=idx_per_level, colname="IdxPerLevelTable")
 
     def xref_databases(self):
         return os.path.join(os.environ["DARWIN_BROWSERDATA_PATH"], "ServerIndexed.db")
 
     def add_xrefs(self):
         self.logger.info("start extracting XRefs, EC and GO annotations")
         db_parser = DarwinDbEntryParser()
@@ -930,25 +989,29 @@
             tablefmt.ECTable,
             "Enzyme Commission annotations",
             expectedrows=1e7,
             createparents=True,
         )
         gs = self.h5.get_node("/Genome").read()
         approx_adder = ApproximateXRefImporter(
-            os.path.join(os.getenv("DARWIN_NETWORK_SCRATCH_PATH"), "approximate_xrefs.tsv")
+            os.path.join(
+                os.getenv("DARWIN_NETWORK_SCRATCH_PATH"), "approximate_xrefs.tsv"
+            )
         )
         up_mapped_xrefs = UniProtAdditionalXRefImporter(
             *(
                 os.path.join(os.getenv("DARWIN_NETWORK_SCRATCH_PATH"), z)
                 for z in ("uniprot_xrefs.tsv", "swissprot_xrefs.tsv")
             )
         )
         with DescriptionManager(
             self.h5, "/Protein/Entries", "/Protein/DescriptionBuffer"
-        ) as de_man, GeneOntologyManager(self.h5, "/Annotations/GeneOntology", "/Ontologies/GO") as go_man:
+        ) as de_man, GeneOntologyManager(
+            self.h5, "/Annotations/GeneOntology", "/Ontologies/GO"
+        ) as go_man:
             xref_importer = XRefImporter(
                 db_parser,
                 gs,
                 xref_tab,
                 ec_tab,
                 go_man,
                 de_man,
@@ -956,53 +1019,46 @@
                 up_mapped_xrefs,
             )
             files = self.xref_databases()
             dbs_iter = fileinput.input(files=files)
             db_parser.parse_entrytags(dbs_iter)
             xref_importer.flush_buffers()
 
-        # create /XRef_EntryNr_offset array
-        enr_col = xref_tab.col("EntryNr")
-        if not (enr_col[:-1] <= enr_col[1:]).all():
-            raise DataImportError("EntryNr column is not sorted in /XRef")
-        enrs = numpy.arange(enr_col[-1] + 2)
-        idx = numpy.searchsorted(enr_col, enrs).astype("i4")
-        self.h5.create_carray(
-            "/",
-            "XRef_EntryNr_offset",
-            obj=idx,
-            title="Array containing the row index in the XRef table at entry_nr: XRef[a[enr]] = first row of EntryNr",
-        )
-
     def add_group_metadata(self):
         m = OmaGroupMetadataLoader(self.h5)
         m.add_data()
 
     def add_roothog_metadata(self):
         m = RootHOGMetaDataLoader(self.h5)
         m.add_data()
 
     def close(self):
         self.h5.root._f_setattr("conversion_end", time.strftime("%c"))
         self.h5.flush()
         self.h5.close()
-        self.logger.info("closed %s", self.h5.filename)
+        self.logger.info("closed {}".format(self.h5.filename))
 
     def create_indexes(self):
         self.logger.info("creating indexes for HogLevel table")
         hogTab = self.h5.get_node("/HogLevel")
-        create_index_for_columns(hogTab, "Fam", "ID", "Level", "NrMemberGenes", "CompletenessScore", "IsRoot")
-        create_and_store_fast_famhoglevel_lookup(self.h5, hogTab, "/HogLevel_fam_lookup")
+        create_index_for_columns(
+            hogTab, "Fam", "ID", "Level", "NrMemberGenes", "CompletenessScore", "IsRoot"
+        )
+        create_and_store_fast_famhoglevel_lookup(
+            self.h5, hogTab, "/HogLevel_fam_lookup"
+        )
 
         orthoxmlTab = self.h5.get_node("/OrthoXML/Index")
         create_index_for_columns(orthoxmlTab, "Fam")
 
         self.logger.info("creating missing indexes for Entries table")
         entryTab = self.h5.get_node("/Protein/Entries")
-        create_index_for_columns(entryTab, "EntryNr", "OmaHOG", "OmaGroup", "MD5ProteinHash")
+        create_index_for_columns(
+            entryTab, "EntryNr", "OmaHOG", "OmaGroup", "MD5ProteinHash"
+        )
 
         self.logger.info("creating suffix index for Descriptions")
         desc_buffer = self.h5.get_node("/Protein/DescriptionBuffer")
         suffixsearch.create_suffix_index(entryTab, "DescriptionOffset", desc_buffer)
 
         self.logger.info("creating index for xrefs (EntryNr and XRefId)")
         xrefTab = self.h5.get_node("/XRef")
@@ -1018,15 +1074,17 @@
         ec_tab = self.h5.get_node("/Annotations/EC")
         create_index_for_columns(ec_tab, "EntryNr", "ECacc")
 
         self.logger.info("creating index for domains (EntryNr)")
         domtab = self.h5.get_node("/Annotations/Domains")
         create_index_for_columns(domtab, "EntryNr", "DomainId")
 
-        self.logger.info("creating indexes for HOG to prevalent domains " "(Fam and DomainId)")
+        self.logger.info(
+            "creating indexes for HOG to prevalent domains " "(Fam and DomainId)"
+        )
         dom2hog_tab = self.h5.get_node("/HOGAnnotations/Domains")
         create_index_for_columns(dom2hog_tab, "DomainId")
         domprev_tab = self.h5.get_node("/HOGAnnotations/DomainArchPrevalence")
         create_index_for_columns(domprev_tab, "Fam")
 
         self.logger.info("createing indexes for Domain Descriptions")
         domdesc = self.h5.get_node("/Annotations/DomainDescription")
@@ -1053,46 +1111,54 @@
         xrefs = self.h5.get_node("/XRef")
         source_enum = xrefs.get_enum("XRefSource")
         canonical_sources = [source_enum[z] for z in xrefsource_order]
         max_acceptable_verif_value = xrefs.get_enum("Verification")["unchecked"]
         current_protein = None
         past_proteins = set([])
         for xref in xrefs:
-            if xref["Verification"] > max_acceptable_verif_value:
-                continue
             if xref["EntryNr"] != current_protein:
                 if current_protein:
                     past_proteins.add(current_protein)
                     yield (current_protein, current_xref[1])
                 current_protein = xref["EntryNr"]
                 current_xref = (1000, b"")  # init with a sentinel
                 if current_protein in past_proteins:
                     raise DataImportError("Data in /XRef is not grouped w.r.t. EntryNr")
             try:
+                if xref["Verification"] > max_acceptable_verif_value:
+                    continue
                 rank = canonical_sources.index(xref["XRefSource"])
                 if rank < current_xref[0]:
                     current_xref = (rank, xref["XRefId"])
             except ValueError:
                 pass
         if current_protein:
             yield (current_protein, current_xref[1])
 
     def add_canonical_id(self):
         """add one canonical xref id to the /Protein/Entries table."""
         self.logger.info("adding canonical ids for each protein...")
         prot_tab = self.h5.get_node("/Protein/Entries")
-        canonical_ids = numpy.chararray(shape=(len(prot_tab),), itemsize=prot_tab.cols.CanonicalId.dtype.itemsize)
+        canonical_ids = numpy.chararray(
+            shape=(len(prot_tab),), itemsize=prot_tab.cols.CanonicalId.dtype.itemsize
+        )
         for eNr, canonical_id in self._iter_canonical_xref():
             row_nr = eNr - 1
             row = prot_tab[row_nr]
             if row["EntryNr"] != eNr:
-                self.logger.warn("Entries table not properly sorted: {}, expected {}".format(row["EntryNr"], eNr))
+                self.logger.warn(
+                    "Entries table not properly sorted: {}, expected {}".format(
+                        row["EntryNr"], eNr
+                    )
+                )
                 raise DataImportError("Entries table not properly sorted")
             canonical_ids[row_nr] = canonical_id
-        prot_tab.modify_column(0, len(prot_tab), 1, column=canonical_ids, colname="CanonicalId")
+        prot_tab.modify_column(
+            0, len(prot_tab), 1, column=canonical_ids, colname="CanonicalId"
+        )
         prot_tab.flush()
 
     def add_domain_info(self, domains):
         self.logger.info("adding domain information...")
         domtab = self.h5.create_table(
             "/Annotations",
             "Domains",
@@ -1109,15 +1175,15 @@
         for i, domain in enumerate(domains):
             for entry_nr in md5_to_enr[domain.md5.encode("utf-8")]:
                 buffer.append((entry_nr, domain.id, domain.coords))
                 if len(buffer) > 5000:
                     domtab.append(buffer)
                     buffer = []
             if i % 50000 == 0:
-                self.logger.info("processed %s domain annotations so far", i)
+                self.logger.info("processed {:d} domain annotations so far".format(i))
         if len(buffer) > 0:
             domtab.append(buffer)
         domtab.flush()
 
     def add_domainname_info(self, domainname_infos):
         self.logger.info("adding domain name information...")
         dom_name_tab = self.h5.create_table(
@@ -1130,28 +1196,30 @@
         buffer = []
         for i, dom_info in enumerate(domainname_infos):
             buffer.append(dom_info)
             if len(buffer) > 5000:
                 self._write_to_table(dom_name_tab, buffer)
                 buffer = []
             if i % 50000 == 0:
-                self.logger.info("processed {:d} domain name descriptions so far".format(i))
+                self.logger.info(
+                    "processed {:d} domain name descriptions so far".format(i)
+                )
         if len(buffer) > 0:
             self._write_to_table(dom_name_tab, buffer)
         dom_name_tab.flush()
 
     def update_summary_stats(self):
         """update the summary statistics of xrefs & go.
 
         The function analyses the well-known xref sources as well as
         GO annotations and computes aggregated counts for
         all / in OMA Group / in HOGs for all of them.
         """
         for tab_name, sum_fun in [
-            ("/Annotations/GeneOntology", self.count_gene_ontology_summary),
+            ("/Annotations/GeneOntology", self.count_xref_summary),
             ("/XRef", self.count_xref_summary),
         ]:
             summary = sum_fun()
             tab = self.h5.get_node(tab_name)
             for attr, val in summary.items():
                 tab.set_attr(attr, val)
 
@@ -1164,51 +1232,41 @@
                 description=tablefmt.GroupsizeHistogram,
                 drop_data=True,
             )
             data = sorted(group_sizes[group_type].items())
             grp_size_tab.append(data)
 
         cov_fracs = self.add_domain_covered_sites_counts()
-        cov_hist, bins = numpy.histogram(cov_fracs[cov_fracs > 0], bins=numpy.linspace(0, 1, 51))
+        cov_hist, bins = numpy.histogram(
+            cov_fracs[cov_fracs > 0], bins=numpy.linspace(0, 1, 51)
+        )
         cov_hist_data = numpy.zeros(50, dtype=[("BinEndValue", "f4"), ("Counts", "i4")])
         cov_hist_data["BinEndValue"] = bins[1:]
         cov_hist_data["Counts"] = cov_hist
         dom_cov_hist_tab = self.create_table_if_needed(
             summary, "Domain_coverage_hist", drop_data=True, obj=cov_hist_data
         )
-        dom_cov_hist_tab.set_attr("frac_genes_w_domain", len(cov_fracs[cov_fracs > 0]) / len(cov_fracs))
+        dom_cov_hist_tab.set_attr(
+            "frac_genes_w_domain", len(cov_fracs[cov_fracs > 0]) / len(cov_fracs)
+        )
         dom_cov_hist_tab.set_attr("mean_coverage_overall", numpy.mean(cov_fracs))
-        dom_cov_hist_tab.set_attr("mean_coverage_w_domain", numpy.mean(cov_fracs[cov_fracs > 0]))
-
-    def collect_goterm_freqs(self):
-        self.logger.info("Computing gene ontology annotations term frequencies")
-        go_tab = self.h5.get_node("/Annotations/GeneOntology")
-        fp = io.StringIO(self.h5.get_node("/Ontologies/GO").read().tobytes().decode())
-        gof = FreqAwareGeneOntology(OntologyParser(fp), rels=None)
-        gof.parse()
-
-        def iter_entry_terms(go_tab, filter=None):
-            for (enr, term), row_iter in itertools.groupby(go_tab, operator.itemgetter("EntryNr", "TermNr")):
-                if filter is not None:
-                    evid = {row["Evidence"] for row in row_iter}
-                    if evid not in filter:
-                        continue
-                yield {"TermNr": int(term)}
-
-        gof.estimate_freqs(iter_entry_terms(go_tab))
-        return gof.cnts, gof.tot_cnts
+        dom_cov_hist_tab.set_attr(
+            "mean_coverage_w_domain", numpy.mean(cov_fracs[cov_fracs > 0])
+        )
 
     def count_gene_ontology_summary(self):
         self.logger.info("Bulding gene ontology annotations summary info")
         go_tab = self.h5.get_node("/Annotations/GeneOntology")
         prot_tab = self.h5.get_node("/Protein/Entries")
         exp_codes = frozenset([b"EXP", b"IDA", b"IPI", b"IMP", b"IGI" b"IEP"])
         cnts = collections.Counter()
         cur_enr = None
-        for (enr, term), row_iter in itertools.groupby(go_tab, operator.itemgetter("EntryNr", "TermNr")):
+        for (enr, term), row_iter in itertools.groupby(
+            go_tab, operator.itemgetter("EntryNr", "TermNr")
+        ):
             evidences = {row["Evidence"] for row in row_iter}
             is_iea = b"IEA" in evidences
             evidences.discard(b"IEA")
             is_exp = not exp_codes.isdisjoint(evidences)
             is_cur = len(evidences.difference(exp_codes)) > 0
             cnts["annotations_any"] += 1
             if is_exp:
@@ -1261,19 +1319,20 @@
                     cnts["trusted_HOG"] += 1
         return cnts
 
     def collect_group_sizes(self):
         self.logger.info("Building grouping size histograms")
         groupings = ("OmaHOG", "OmaGroup")
         memb_cnts = {grp: collections.defaultdict(int) for grp in groupings}
+        fam_re = re.compile(br"([A-Z]+:)?(?P<fam>[0-9]+).*")
         prot_tab = self.h5.get_node("/Protein/Entries")
         for row in prot_tab:
             for grp in groupings:
                 if grp == "OmaHOG":
-                    m = hog_re.match(row[grp])
+                    m = fam_re.match(row[grp])
                     if m is None:
                         continue
                     grp_id = int(m.group("fam"))
                 else:
                     grp_id = int(row[grp])
                     if grp_id == 0:
                         continue
@@ -1334,53 +1393,34 @@
                 "CoveredSitesByDomains",
                 tables.UInt32Atom(),
                 (len(cov_sites),),
             )
         dom_cov_tab[0 : len(cov_sites)] = cov_sites
         return cov_sites / (prot_tab.col("SeqBufferLength") - 1)
 
-    def add_gene_ontology_term_cnts(self):
-        """
-        Stores the counts of a gene ontology annotation per term in the database.
-
-        This function also includes the implied parental terms.
-
-        :return: hdf5 Table instance with the counts
-        """
-        cnts, tot_cnts = self.collect_goterm_freqs()
-        cnts = sorted(cnts.items())
-        tab = self.create_table_if_needed(
-            "/Ontologies",
-            "GeneOntologyTermCounts",
-            description=tablefmt.GeneOntologyTermCounts,
-        )
-        tab.append(cnts)
-        self.h5.set_node_attr(tab, "total_molecular_function", tot_cnts[0])
-        self.h5.set_node_attr(tab, "total_biological_process", tot_cnts[1])
-        self.h5.set_node_attr(tab, "total_cellular_component", tot_cnts[2])
-        return tab
-
     def add_sequence_suffix_array(self, k=6, fn=None, sa=None):
         """
         Adds the sequence suffix array to the database. NOTE: this
         (obviously) requires A LOT of memory for large DBs.
         """
         # Ensure we're run in correct order...
         assert "Protein" in self.h5.root, "Add proteins before calc. SA!"
-        idx_compr = tables.Filters(complevel=6, complib="blosc")
+        idx_compr = tables.Filters(complevel=6, complib="blosc", fletcher32=True)
 
         # Add to separate file if fn is set.
         if fn is None:
             db = self.h5
         else:
-            fn = os.path.normpath(os.path.join(os.getenv("DARWIN_BROWSERDATA_PATH", ""), fn))
+            fn = os.path.normpath(
+                os.path.join(os.getenv("DARWIN_BROWSERDATA_PATH", ""), fn)
+            )
             db = tables.open_file(fn, "w", filters=idx_compr)
             db.create_group("/", "Protein")
             db.root._f_setattr("conversion_start", time.strftime("%c"))
-            self.logger.info("opened %s", db.filename)
+            self.logger.info("opened {}".format(db.filename))
 
         # Load sequence buffer to memory - this is required to calculate the SA.
         # Do it here (instead of in PySAIS) so that we can use it for computing
         # the split points later.
         seqs = self.h5.get_node("/Protein/SequenceBuffer")[:].tobytes()
         n = len(self.h5.get_node("/Protein/Entries"))
 
@@ -1396,15 +1436,15 @@
             obj=sa,
             filters=idx_compr,
         )
 
         # Create lookup table for fa2go
         dtype = numpy.uint32 if (n < numpy.iinfo(numpy.uint32).max) else numpy.uint64
         idx = numpy.zeros(sa.shape, dtype=dtype)
-        mask = numpy.zeros(sa.shape, dtype=bool)
+        mask = numpy.zeros(sa.shape, dtype=numpy.bool)
 
         # Compute mask and entry index for sequence buff
         for i in range(n):
             s = (sa[i - 1] if i > 0 else -1) + 1
             e = sa[i] + 1
             idx[s:e] = i + 1
             mask[(e - k) : e] = True  # (k-1) invalid and delim.
@@ -1453,47 +1493,49 @@
             self.h5.create_external_link(
                 "/Protein",
                 "SequenceIndex",
                 self._relative_path_to_external_node(db.root.Protein.SequenceIndex),
             )
             db.root._f_setattr("conversion_end", time.strftime("%c"))
             db.close()
-            self.logger.info("closed %s", db.filename)
+            self.logger.info("closed {}".format(db.filename))
 
     def _relative_path_to_external_node(self, node):
-        rel_path = os.path.relpath(node._v_file.filename, os.path.dirname(self.h5.filename))
+        rel_path = os.path.relpath(
+            node._v_file.filename, os.path.dirname(self.h5.filename)
+        )
         return str(rel_path + ":" + node._v_pathname)
 
     def add_hog_domain_prevalence(self):
         # Check that protein entries / domains are added already to the DB
         assert True  # TODO
 
         # Used later
         hl_tab = self.h5.get_node("/HogLevel")
         create_index_for_columns(hl_tab, "Fam", "IsRoot")
         fam_to_rootlevel = {
-            int(row["Fam"]): row["Level"].decode() for row in hl_tab.where('~contains(ID, b".") & (IsRoot == True)')
+            int(row["Fam"]): row["Level"].decode()
+            for row in hl_tab.where('~contains(ID, b".") & (IsRoot == True)')
         }
 
         # Load the HOG -> Entry table to memory
         prot_tab = self.h5.root.Protein.Entries
         # TODO: work out how to do this in a neater way
         df = pandas.DataFrame.from_records(
-            ((z["EntryNr"], z["OmaHOG"], z["SeqBufferLength"]) for z in prot_tab.iterrows()),
+            (
+                (z["EntryNr"], z["OmaHOG"], z["SeqBufferLength"])
+                for z in prot_tab.iterrows()
+            ),
             columns=["EntryNr", "OmaHOG", "SeqBufferLength"],
         )
         # Strip singletons
         df = df[~(df["OmaHOG"] == b"")]
 
         # Reformat HOG ID to plain-integer for top-level grouping only
-        def root_hog_nr(id_):
-            m = hog_re.match(id_)
-            return int(m.group("fam"))
-
-        df["OmaHOG"] = df["OmaHOG"].apply(root_hog_nr)
+        df["OmaHOG"] = df["OmaHOG"].apply(lambda i: int(i[4:].split(b".")[0]))
 
         # Load domains
         domains = pandas.DataFrame.from_records(self.h5.root.Annotations.Domains[:])
 
         # Ensure sorted by coordinate - TODO: move this to DA import function
         domains["start"] = domains["Coords"].apply(lambda c: int(c.split(b":")[0]))
         domains.sort_values(["EntryNr", "start"], inplace=True)
@@ -1502,41 +1544,35 @@
         # Merge domains / entry-hog tables. Keep entries with no domains
         # so that we can count the size of the HOGs.
         df = pandas.merge(df, domains, on="EntryNr", how="left")
 
         # Gather entry-domain for each HOG.
         hog2dom = []
         hog2info = []
-        for hog_id, hdf in tqdm(df.groupby("OmaHOG")):
+        for (hog_id, hdf) in tqdm(df.groupby("OmaHOG")):
             size = len(set(hdf["EntryNr"]))
 
             hdf = hdf[~hdf["DomainId"].isnull()]
             cov = len(set(hdf["EntryNr"]))  # Coverage with any DA
 
             if (size > 2) and (cov > 1):
                 # There are some annotations
                 da = collections.defaultdict(list)
-                for enum, edf in hdf.groupby("EntryNr"):
+                for (enum, edf) in hdf.groupby("EntryNr"):
                     d = edf["DomainId"]
                     d = tuple(d) if (type(d) != bytes) else (d,)
                     da[d].append(enum)
 
                 da = sorted(da.items(), key=lambda i: len(i[1]), reverse=True)
                 c = len(da[0][1])  # Count of prev. DA
                 if c > 1:
                     # DA exists in more than one member.
                     cons_da = da[0][0]
                     repr_entry = da[0][1][0]
-                    try:
-                        tl = hl_tab.read_where("Fam == {}".format(hog_id))[0]["Level"].decode("ascii")
-                    except IndexError as exc:
-                        self.logger.exception("cannot get level for fam {}".format(hog_id))
-                        self.warning(hl_tab.read_where("Fam == {}".format(hog_id)))
-                        raise
-
+                    tl = fam_to_rootlevel[hog_id]
                     rep_len = hdf[hdf["EntryNr"] == repr_entry]["SeqBufferLength"]
                     rep_len = int(rep_len if len(rep_len) == 1 else list(rep_len)[0])
 
                     # Save the consensus DA
                     off = len(hog2info)  # Offset in the information table.
                     hog2dom += [(off, d) for d in cons_da]
 
@@ -1589,39 +1625,43 @@
         self.logger.info("  info for HOGs written")
 
 
 def download_url_if_not_present(url, force_copy=False):
     if url.startswith("file://") and not force_copy:
         fname = url[len("file://") :]
         if os.path.exists(fname):
-            common.package_logger.info('using file "{}" directly from source without copying.'.format(url))
+            common.package_logger.info(
+                'using file "{}" directly from source without copying.'.format(url)
+            )
             return fname
-        common.package_logger.warning("file %s does not exist", fname)
+        common.package_logger.warning("file {} does not exist".format(fname))
         return None
-    tmpfolder = os.path.join(os.getenv("DARWIN_NETWORK_SCRATCH_PATH", "/tmp"), "Browser", "xref")
+    tmpfolder = os.path.join(
+        os.getenv("DARWIN_NETWORK_SCRATCH_PATH", "/tmp"), "Browser", "xref"
+    )
     basename = url.split("/")[-1]
     fname = os.path.join(tmpfolder, basename)
     if not os.path.exists(tmpfolder):
         os.makedirs(tmpfolder)
     if not os.path.exists(fname):
-        common.package_logger.info("downloading %s into %s", url, fname)
+        common.package_logger.info("downloading {} into {}".format(url, fname))
         try:
             urllib.request.urlretrieve(url, fname)
         except urllib.request.URLError:
-            common.package_logger.warn("cannot download %s", url)
+            common.package_logger.warn("cannot download {}".format(url))
     return fname
 
 
 def iter_domains(url):
     DomainTuple = collections.namedtuple("DomainTuple", ("md5", "id", "coords"))
 
     fname = download_url_if_not_present(url)
     if fname is None:
         return
-    with common.auto_open(fname, "rt") as uncompressed:
+    with gzip.open(fname, "rt") as uncompressed:
         dialect = csv.Sniffer().sniff(uncompressed.read(4096))
         uncompressed.seek(0)
         csv_reader = csv.reader(uncompressed, dialect)
         col_md5, col_id, col_coord = (None,) * 3
         coord_fromat_trans = str.maketrans("-,", "::")
 
         for lineNr, row in enumerate(csv_reader):
@@ -1630,34 +1670,50 @@
                 if len(row) >= 9:
                     # representative_proteins format. use columns 5-7
                     col_md5, col_id, col_coord = 4, 5, 6
                 elif len(row) == 3:
                     # additionally created ones, minimal format
                     col_md5, col_id, col_coord = 0, 1, 2
                 else:
-                    raise DataImportError("Unknown Domain Annotation format in {}".format(uncompressed.filename))
+                    raise DataImportError(
+                        "Unknown Domain Annotation format in {}".format(
+                            uncompressed.filename
+                        )
+                    )
             try:
                 dom = DomainTuple(
                     row[col_md5],
                     row[col_id],
                     row[col_coord].translate(coord_fromat_trans),
                 )
                 if lineNr < 10:
                     # do some sanity checks on the first few lines
                     if re.match(r"[0-9a-f]{32}$", dom.md5) is None:
-                        raise DataImportError("md5 hash of line {:d} has unexpected values: {}".format(lineNr, dom.md5))
+                        raise DataImportError(
+                            "md5 hash of line {:d} has unexpected values: {}".format(
+                                lineNr, dom.md5
+                            )
+                        )
                     if re.match(r"([1-4]\.\d+\.\d+\.\d+|PF\d+)$", dom.id) is None:
-                        raise DataImportError("Domain-ID of line {:d} has unexpected value: {}".format(lineNr, dom.id))
+                        raise DataImportError(
+                            "Domain-ID of line {:d} has unexpected value: {}".format(
+                                lineNr, dom.id
+                            )
+                        )
                     if re.match(r"\d+:\d+", dom.coords) is None:
                         raise DataImportError(
-                            "Domain coordinates in line {:d} has unexpected value: {}".format(lineNr, dom.coords)
+                            "Domain coordinates in line {:d} has unexpected value: {}".format(
+                                lineNr, dom.coords
+                            )
                         )
                 yield dom
             except Exception:
-                common.package_logger.exception("cannot create tuple from line {}".format(lineNr))
+                common.package_logger.exception(
+                    "cannot create tuple from line {}".format(lineNr)
+                )
 
 
 def only_pfam_or_cath_domains(iterable):
     cath_re = re.compile(r"[1-4]\.")
     for dom in iterable:
         if dom.id.startswith("PF") or cath_re.match(dom.id) is not None:
             yield dom
@@ -1670,15 +1726,19 @@
     ignored = 0
     for dom in iterable:
         if not dom in seen:
             seen.add(dom)
             yield dom
         else:
             ignored += 1
-    common.package_logger.info("skipped {} duplicated domains. {} distinct domains yielded".format(ignored, len(seen)))
+    common.package_logger.info(
+        "skipped {} duplicated domains. {} distinct domains yielded".format(
+            ignored, len(seen)
+        )
+    )
 
 
 class RootHOGMetaDataLoader(object):
     """RootHOG Meta data extractor.
 
     This class provides the means to import the Keywords of the RootHOGs
     into the hdf5 database. The data is stored under in the node defined
@@ -1690,49 +1750,57 @@
     tab_description = tablefmt.RootHOGMetaTable
     meta_data_path = "/RootHOG/MetaData"
 
     def __init__(self, db):
         self.db = db
 
     def add_data(self):
-        common.package_logger.info("adding %s", self.meta_data_path)
+        common.package_logger.info("adding {}".format(self.meta_data_path))
         nr_groups = self._get_nr_of_groups()
         has_meta_data = self._check_textfiles_avail()
         if has_meta_data:
             data = self._load_data()
             encoded_data = {}
             for key in self.expected_keys:
-                encoded_data[key] = [x.encode("utf-8") if isinstance(x, str) else b"-" for x in data[key]]
+                encoded_data[key] = [x.encode("utf-8") for x in data[key]]
                 if nr_groups != len(encoded_data[key]):
-                    raise DataImportError("nr of oma groups does not match the number of {}".format(key))
+                    raise DataImportError(
+                        "nr of oma groups does not match the number of {}".format(key)
+                    )
         else:
-            common.package_logger.warning("No fingerprint nor keyword information available")
+            common.package_logger.warning(
+                "No fingerprint nor keyword information available"
+            )
             encoded_data = {}
             for key in self.expected_keys:
                 if key == "Fingerprints":
                     encoded_data[key] = [b"n/a"] * nr_groups
                 else:
                     encoded_data[key] = [b""] * nr_groups
 
         grptab, keybuf = self._create_db_objects(nr_groups)
         self._fill_data_into_db(encoded_data, grptab, keybuf)
         if "NrMembers" in grptab.colnames:
-            grptab.modify_column(column=self._get_group_member_counts(), colname="NrMembers")
+            grptab.modify_column(
+                column=self._get_group_member_counts(), colname="NrMembers"
+            )
         self._create_indexes(grptab)
 
     def _create_db_objects(self, nrows):
         key_path = os.path.join(os.path.dirname(self.meta_data_path), "KeywordBuffer")
         try:
             self.db.get_node(self.meta_data_path)
             self.db.remove_node(self.meta_data_path)
             self.db.remove_node(key_path)
         except tables.NoSuchNodeError:
             pass
         root, name = self.meta_data_path.rsplit("/", 1)
-        grptab = self.db.create_table(root, name, self.tab_description, expectedrows=nrows, createparents=True)
+        grptab = self.db.create_table(
+            root, name, self.tab_description, expectedrows=nrows, createparents=True
+        )
         buffer = self.db.create_earray(
             root,
             "KeywordBuffer",
             tables.StringAtom(1),
             (0,),
             "concatenated keywords descriptions",
             expectedrows=500 * nrows,
@@ -1744,15 +1812,17 @@
         buf_pos = 0
         keywords = encoded_data["Keywords"]
         for i in range(len(keywords)):
             row["FamNr"] = i + 1
             row["KeywordOffset"] = buf_pos
             row["KeywordLength"] = len(keywords[i])
             row.append()
-            key = numpy.ndarray((len(keywords[i]),), buffer=keywords[i], dtype=tables.StringAtom(1))
+            key = numpy.ndarray(
+                (len(keywords[i]),), buffer=keywords[i], dtype=tables.StringAtom(1)
+            )
             key_buf.append(key)
             buf_pos += len(keywords[i])
         grp_tab.flush()
         key_buf.flush()
 
     def _create_indexes(self, grp_tab):
         create_index_for_columns(grp_tab, "FamNr")
@@ -1798,15 +1868,17 @@
         keywords = encoded_data["Keywords"]
         for i in range(len(stable_ids)):
             row["GroupNr"] = i + 1
             row["Fingerprint"] = stable_ids[i]
             row["KeywordOffset"] = buf_pos
             row["KeywordLength"] = len(keywords[i])
             row.append()
-            key = numpy.ndarray((len(keywords[i]),), buffer=keywords[i], dtype=tables.StringAtom(1))
+            key = numpy.ndarray(
+                (len(keywords[i]),), buffer=keywords[i], dtype=tables.StringAtom(1)
+            )
             key_buf.append(key)
             buf_pos += len(keywords[i])
         grp_tab.flush()
         key_buf.flush()
 
     def _create_indexes(self, grp_tab):
         create_index_for_columns(grp_tab, "Fingerprint", "GroupNr")
@@ -1818,15 +1890,17 @@
         etab = self.db.get_node("/Protein/Entries")
         try:
             return etab[etab.colindexes["OmaGroup"][-1]]["OmaGroup"]
         except KeyError:
             return max(etab.col("OmaGroup"))
 
     def _get_group_member_counts(self):
-        grp_nr, cnts = numpy.unique(self.db.get_node("/Protein/Entries").col("OmaGroup"), return_counts=True)
+        grp_nr, cnts = numpy.unique(
+            self.db.get_node("/Protein/Entries").col("OmaGroup"), return_counts=True
+        )
         if grp_nr[0] == 0:
             cnts = cnts[1:]
         assert len(cnts) == self._get_nr_of_groups()
         return cnts
 
     def _check_textfiles_avail(self):
         rootdir = os.getenv("DARWIN_BROWSERDATA_PATH", "")
@@ -1839,60 +1913,71 @@
     def __init__(self, db, entry_path, buffer_path):
         self.db = db
         self.entry_path = entry_path
         self.buffer_path = buffer_path
 
     def __enter__(self):
         self.entry_tab = self.db.get_node(self.entry_path)
-        if not numpy.all(numpy.equal(self.entry_tab.col("EntryNr"), numpy.arange(1, len(self.entry_tab) + 1))):
+        if not numpy.all(
+            numpy.equal(
+                self.entry_tab.col("EntryNr"), numpy.arange(1, len(self.entry_tab) + 1)
+            )
+        ):
             raise RuntimeError("entry table is not sorted")
 
         root, name = os.path.split(self.buffer_path)
         self.desc_buf = self.db.create_earray(
             root,
             name,
             tables.StringAtom(1),
             (0,),
             "concatenated protein descriptions",
             expectedrows=len(self.entry_tab) * 100,
         )
         self.cur_eNr = None
         self.cur_desc = []
         bufindex_dtype = numpy.dtype(
-            [(col, self.entry_tab.coldtypes[col]) for col in ("DescriptionOffset", "DescriptionLength")]
+            [
+                (col, self.entry_tab.coldtypes[col])
+                for col in ("DescriptionOffset", "DescriptionLength")
+            ]
         )
         # columns to be stored in entry table with buffer index data
         self.buf_index = numpy.zeros(len(self.entry_tab), dtype=bufindex_dtype)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.cur_eNr:
             self._store_description()
         self.desc_buf.flush()
-        self.entry_tab.modify_columns(columns=self.buf_index, names=self.buf_index.dtype.names)
+        self.entry_tab.modify_columns(
+            columns=self.buf_index, names=self.buf_index.dtype.names
+        )
         self.entry_tab.flush()
 
     def add_description(self, eNr, desc):
         """stages a description for addition. Note that the descriptions
         must be ordered according to the entryNr, i.e. all descriptions
         related to eNr X must be staged before changeing to another eNr."""
         if self.cur_eNr and self.cur_eNr != eNr:
             self._store_description()
             self.cur_desc = []
         self.cur_eNr = eNr
         self.cur_desc.append(desc)
 
     def _store_description(self):
         buf = "; ".join(self.cur_desc).encode("utf-8")
-        buf = buf[0 : 2**16 - 1]  # limit to max value of buffer length field
+        buf = buf[0 : 2 ** 16 - 1]  # limit to max value of buffer length field
         len_buf = len(buf)
         idx = self.cur_eNr - 1
         self.buf_index[idx]["DescriptionOffset"] = len(self.desc_buf)
         self.buf_index[idx]["DescriptionLength"] = len_buf
-        self.desc_buf.append(numpy.ndarray((len_buf,), buffer=buf, dtype=tables.StringAtom(1)))
+        self.desc_buf.append(
+            numpy.ndarray((len_buf,), buffer=buf, dtype=tables.StringAtom(1))
+        )
 
 
 class GeneOntologyManager(object):
     ontology_url = "http://purl.obolibrary.org/obo/go/go-basic.obo"
 
     def __init__(self, db, annotation_path, ontology_path):
         self.db = db
@@ -1932,15 +2017,15 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._flush_buffers()
         self.go_tab.flush()
 
     def _get_obo_version(self, obo_arr):
         header = obo_arr[0:1000].tobytes()
-        rel_info = re.search(rb"data-version:\s*(?P<version>[\w/_ -]+)", header)
+        rel_info = re.search(b"data-version:\s*(?P<version>[\w/_ -]+)", header)
         if rel_info is not None:
             rel_info = rel_info.group("version").decode()
         return rel_info
 
     def _flush_buffers(self):
         common.package_logger.info("flushing go annotations buffers")
         if len(self._go_buf) > 0:
@@ -1959,103 +2044,106 @@
                 common.package_logger.warning("cannot parse GO annotation: " + t)
                 continue
 
             try:
                 term_nr = self.go.term_by_id(term).id
             except ValueError:
                 common.package_logger.warning(
-                    "invalid GO term for entry {:d}: {:s} (likely obsolete)".format(enr, term)
+                    "invalid GO term for entry {:d}: {:s} (likely obsolete)".format(
+                        enr, term
+                    )
                 )
                 continue
             rem = rem.replace("{", "[")
             rem = rem.replace("}", "]")
-            rem = self.quote_re.sub(r'\g<1>"\g<2>"\g<3>', rem)
+            rem = self.quote_re.sub('\g<1>"\g<2>"\g<3>', rem)
             for evi, refs in eval(rem):
                 for ref in refs:
                     self._go_buf.append((enr, term_nr, evi, ref.encode("utf-8")))
             if len(self._go_buf) > 2e6:
                 self._flush_buffers()
 
 
 class GroupAnnotatorInclGeneRefs(familyanalyzer.GroupAnnotator):
     def _annotateGroupR(self, node, og, idx=0):
         is_geneRef = familyanalyzer.OrthoXMLQuery.is_geneRef_node(node)
         is_og = self.parser.is_ortholog_group(node)
         if is_og or is_geneRef:
-            if self.parser.is_paralog_group(node.getparent()) or node.getparent().tag == "{{{ns0}}}groups".format(
-                **self.parser.ns
-            ):
+            if self.parser.is_paralog_group(
+                node.getparent()
+            ) or node.getparent().tag == "{{{ns0}}}groups".format(**self.parser.ns):
                 # direct children of a paralogGroup. set IsRoot to true in most general TaxRange property tag
                 prop_tag = "{{{ns0}}}property".format(**self.parser.ns)
                 for child in node[::-1]:
                     if child.tag == prop_tag and child.attrib["name"] == "TaxRange":
                         child.attrib["IsRoot"] = str(True)
                         break
 
         if is_geneRef:
             node.set("LOFT", og)
         else:
             super()._annotateGroupR(node, og, idx)
 
 
 class HogConverter(object):
-    def __init__(self, entry_tab, release_char=None, tax_tab=None, tax_2_code=None):
-        self.fam_re = re.compile(r"HOG:(?P<release>[A-Z]+)?(?P<fam_nr>\d+)")
-        self.hogs = numpy.zeros(shape=(len(entry_tab) + 1,), dtype=entry_tab.cols.OmaHOG.dtype)
+    def __init__(self, entry_tab, tax_tab=None, tax_2_code=None):
+        self.fam_re = re.compile(r"HOG:(?P<fam_nr>\d+)")
+        self.hogs = numpy.zeros(
+            shape=(len(entry_tab) + 1,), dtype=entry_tab.cols.OmaHOG.dtype
+        )
         self.entry_tab = entry_tab
-        self.taxrange_2_taxid = self._extract_taxrange_2_taxid_map(tax_tab) if tax_tab else None
+        self.taxrange_2_taxid = (
+            self._extract_taxrange_2_taxid_map(tax_tab) if tax_tab else None
+        )
         self.taxid_2_code = tax_2_code
-        if release_char is None:
-            self.release_char = ""
-        elif re.match(r"^[A-Z]?$", release_char):
-            self.release_char = release_char
-        else:
-            raise ValueError(
-                "invalid release_char value: {}. Expected is a single capital ascii character".format(release_char)
-            )
 
     def _extract_taxrange_2_taxid_map(self, tax_tab):
         return {row["Name"].decode(): int(row["NCBITaxonId"]) for row in tax_tab}
 
     def attach_newick_taxonomy(self, tree):
         self.taxonomy = familyanalyzer.NewickTaxonomy(tree)
 
     def _assert_hogid_has_correct_prefix(self, fa_parser):
         for grp in fa_parser.getToplevelGroups():
-            if not grp.get("id").startswith("HOG:{:s}".format(self.release_char)):
-                grp.set("id", "HOG:{:s}{:07d}".format(self.release_char, int(grp.get("id"))))
+            if not grp.get("id").startswith("HOG:"):
+                grp.set("id", "HOG:{:07d}".format(int(grp.get("id"))))
 
     def convert_file(self, fn, store=None):
         p = familyanalyzer.OrthoXMLParser(fn)
         self._assert_hogid_has_correct_prefix(p)
         if hasattr(self, "taxonomy"):
             tax = self.taxonomy
         else:
             tax = familyanalyzer.TaxonomyFactory.newTaxonomy(p)
-        annotator = GroupAnnotatorInclGeneRefs(p, self.taxrange_2_taxid, self.taxid_2_code)
+        annotator = GroupAnnotatorInclGeneRefs(
+            p, self.taxrange_2_taxid, self.taxid_2_code
+        )
         annotator.annotateMissingTaxRanges(tax)
         annotator.annotateDoc()
 
         levs = []
         for fam in p.getToplevelGroups():
             m = self.fam_re.match(self.get_hog_id(fam))
             fam_nr = int(m.group("fam_nr"))
-            for taxnode in familyanalyzer.OrthoXMLQuery.getTaxRangeNodes(fam, recursively=True):
+            for taxnode in familyanalyzer.OrthoXMLQuery.getTaxRangeNodes(
+                fam, recursively=True
+            ):
                 ognode = taxnode.getparent()
                 levs.append(
                     (fam_nr, self.get_hog_id(ognode), taxnode.get("value"))
                     + self.get_hog_scores(ognode, taxnode)
                     + (
                         self.get_nr_member_genes(ognode),
                         bool(taxnode.get("IsRoot", False)),
-                        -1,
                     )
                 )
 
-        geneNodes = p.root.findall(".//{{{ns0}}}geneRef".format(**familyanalyzer.OrthoXMLParser.ns))
+        geneNodes = p.root.findall(
+            ".//{{{ns0}}}geneRef".format(**familyanalyzer.OrthoXMLParser.ns)
+        )
         for x in geneNodes:
             self.hogs[int(x.get("id"))] = x.get("LOFT")
         if store is not None:
             p.write(store, pretty_print=True)
         return levs
 
     def write_hogs(self):
@@ -2077,33 +2165,38 @@
     def get_hog_scores(self, og_node, tax_node):
         """extract the scores associated with an orthologGroup node
 
         only scores that are defined in HOGsTable are extract. The method
         returns a tuple with the scores in the order of the score fields."""
         all_score_ids = ("CompletenessScore", "ImpliedLosses")
         parse_fun = {"CompletenessScore": float, "ImpliedLosses": int}
-        scores = collections.OrderedDict([(score, tablefmt.HOGsTable.columns[score].dflt) for score in all_score_ids])
+        scores = collections.OrderedDict(
+            [(score, tablefmt.HOGsTable.columns[score].dflt) for score in all_score_ids]
+        )
         for score in og_node.iterfind("{*}score"):
             score_id = score.get("id")
             scores[score_id] = parse_fun[score_id](score.get("value"))
         # might be overwritten in tax_node (more specific if available)
         for score_id in all_score_ids:
             val = tax_node.get(score_id)
             if val is not None:
                 scores[score_id] = parse_fun[score_id](val)
         return tuple(scores.values())
 
     def get_nr_member_genes(self, og_node):
         for child in og_node:
             if (
-                child.tag == "{{{ns0}}}property".format(**familyanalyzer.OrthoXMLParser.ns)
+                child.tag
+                == "{{{ns0}}}property".format(**familyanalyzer.OrthoXMLParser.ns)
                 and child.get("name") == "NrMemberGenes"
             ):
                 return int(child.get("value"))
-        common.package_logger.warning("couldn't find NrMemberGenes property. scanning xml file for geneRefs")
+        common.package_logger.warning(
+            "couldn't find NrMemberGenes property. scanning xml file for geneRefs"
+        )
         return len(familyanalyzer.OrthoXMLQuery.getGeneRefNodes(og_node))
 
 
 class XRefImporter(object):
     """Object to import various types of crossreferences into hdf5.
 
     The XRefImporter registers at a db_parser object various handlers
@@ -2150,53 +2243,67 @@
             "EMBL": (xrefEnum["EMBL"], "unchecked"),
             "ID": (xrefEnum["SourceID"], "exact"),
             "AC": (xrefEnum["SourceAC"], "exact"),
         }
         for tag, enumval in tag_to_enums.items():
             db_parser.add_tag_handler(
                 tag,
-                lambda key, enr, typ=enumval: self.multi_key_handler(key, enr, typ[0], typ[1]),
+                lambda key, enr, typ=enumval: self.multi_key_handler(
+                    key, enr, typ[0], typ[1]
+                ),
             )
-        db_parser.add_tag_handler("DE", lambda key, enr: self.description_handler(key, enr))
+        db_parser.add_tag_handler(
+            "DE", lambda key, enr: self.description_handler(key, enr)
+        )
         db_parser.add_tag_handler("GO", self.go_handler)
         db_parser.add_tag_handler("ID", self.assign_source_handler)
         db_parser.add_tag_handler("AC", self.assign_source_handler)
         db_parser.add_tag_handler("EC", self.ec_handler)
 
         for tag in ["SwissProt_AC", "UniProt"]:  # UniProt/TrEMBL tag is cut to UniProt!
             db_parser.add_tag_handler(
                 tag,
-                lambda key, enr, typ=xrefEnum["UniProtKB/TrEMBL"]: self.remove_uniprot_code_handler(key, enr, typ),
+                lambda key, enr, typ=xrefEnum[
+                    "UniProtKB/TrEMBL"
+                ]: self.remove_uniprot_code_handler(key, enr, typ),
             )
 
         db_parser.add_post_entry_handler(self.add_approx_xrefs)
         # register the potential_flush as end_of_entry_notifier
         db_parser.add_post_entry_handler(self.potential_flush)
 
         self.db_parser = db_parser
         self.xrefEnum = xrefEnum
-        self.ENS_RE = re.compile(r"ENS(?P<species>[A-Z]{0,3})(?P<typ>[GTP])(?P<num>\d{11})")
+        self.ENS_RE = re.compile(
+            r"ENS(?P<species>[A-Z]{0,3})(?P<typ>[GTP])(?P<num>\d{11})"
+        )
         self.FB_RE = re.compile(r"FB(?P<typ>[gnptr]{2})(?P<num>\d{7})")
         self.NCBI_RE = re.compile(r"[A-Z]{3}\d{5}\.\d$")
         self.WB_RE = re.compile(r"WBGene\d{8}$")
         self.EC_RE = re.compile(r"\d+\.(\d+|-)\.(\d+|-)\.(\d+|-)")
-        self.ENSGENOME_RE = re.compile(b"Ensembl (Metazoa|Plant|Fungi|Protist|Bacteria)", re.IGNORECASE)
+        self.ENSGENOME_RE = re.compile(
+            b"Ensembl (Metazoa|Plant|Fungi|Protist|Bacteria)", re.IGNORECASE
+        )
 
         self.FLUSH_SIZE = 5e6
 
         # info about current genome
         self.genomes_tab = genomes_tab
         self._cur_genome = None
 
     def _get_genome_info(self, entry_nr):
         if not (
             self._cur_genome is not None
-            and self._cur_genome["EntryOff"] < entry_nr <= self._cur_genome["EntryOff"] + self._cur_genome["TotEntries"]
+            and self._cur_genome["EntryOff"]
+            < entry_nr
+            <= self._cur_genome["EntryOff"] + self._cur_genome["TotEntries"]
         ):
-            self._cur_genome = self.genomes_tab[self.genomes_tab["EntryOff"].searchsorted(entry_nr + 1) - 1]
+            self._cur_genome = self.genomes_tab[
+                self.genomes_tab["EntryOff"].searchsorted(entry_nr + 1) - 1
+            ]
         return self._cur_genome
 
     def from_EnsemblGenome(self, entry_nr):
         genome_info = self._get_genome_info(entry_nr)
         return self.ENSGENOME_RE.search(genome_info["Release"]) is not None
 
     def flush_buffers(self):
@@ -2242,15 +2349,17 @@
                 typ = ens_match.group("typ")
                 if typ == "P":
                     enum_nr = self.xrefEnum["Ensembl Protein"]
                 elif typ == "G":
                     enum_nr = self.xrefEnum["Ensembl Gene"]
                 elif typ == "T":
                     enum_nr = self.xrefEnum["Ensembl Transcript"]
-                common.package_logger.debug("ensembl: ({}, {}, {})".format(key, typ, enum_nr))
+                common.package_logger.debug(
+                    "ensembl: ({}, {}, {})".format(key, typ, enum_nr)
+                )
                 self._add_to_xrefs(eNr, enum_nr, key, "exact")
 
             for enum, regex in {
                 "FlyBase": self.FB_RE,
                 "NCBI": self.NCBI_RE,
                 "WormBase": self.WB_RE,
             }.items():
@@ -2272,25 +2381,69 @@
                 self.ec.append((enr, acc_match.group(0)))
 
     def description_handler(self, de, eNr):
         self.desc_manager.add_description(eNr, de)
 
     def remove_uniprot_code_handler(self, multikey, eNr, enum_nr):
         """remove the species part (sep by '_') of a uniprot long accession to the short acc"""
-        common.package_logger.debug("remove_uniprot_code_handler called ({}, {},{})".format(multikey, eNr, enum_nr))
+        common.package_logger.debug(
+            "remove_uniprot_code_handler called ({}, {},{})".format(
+                multikey, eNr, enum_nr
+            )
+        )
         for key in multikey.split("; "):
             pos = key.find("_")
             store_key = key if pos < 0 else key[:pos]
             self._add_to_xrefs(eNr, enum_nr, store_key, "exact")
             for tup in self.uniprot_xref_adder.iter_xreftuples_for_up(store_key, eNr):
                 self.xrefs.append(tup)
 
     def add_approx_xrefs(self, enr):
         self.xrefs.extend(self.approx_adder.iter_approx_xrefs_for(enr))
 
+    def build_suffix_index(self, force=False):
+        parent, name = os.path.split(self.xref_tab._v_pathname)
+        file_ = self.xref_tab._v_file
+        idx_node = get_or_create_tables_node(
+            file_, os.path.join(parent, "{}_Index".format(name))
+        )
+        for arr_name, typ in (
+            ("buffer", tables.StringAtom(1)),
+            ("offset", tables.UInt32Atom()),
+        ):
+            try:
+                n = idx_node._f_get_child(arr_name)
+                if not force:
+                    raise tables.NodeError(
+                        "Suffix index for xrefs does already exist. Use 'force' to overwrite"
+                    )
+                n.remove()
+            except tables.NoSuchNodeError:
+                pass
+            file_.create_earray(idx_node, arr_name, typ, (0,), expectedrows=100e6)
+        buf, off = (idx_node._f_get_child(node) for node in ("buffer", "offset"))
+        self._build_lowercase_xref_buffer(buf, off)
+        sa = sais(buf)
+        try:
+            idx_node._f_get_child("suffix").remove()
+        except tables.NoSuchNodeError:
+            pass
+        file_.create_carray(idx_node, "suffix", obj=sa)
+
+    def _build_lowercase_xref_buffer(self, buf, off):
+        cur_pos = 0
+        for xref_row in tqdm(self.xref_tab):
+            lc_ref = xref_row["XRefId"].lower()
+            ref = numpy.ndarray(
+                (len(lc_ref),), buffer=lc_ref, dtype=tables.StringAtom(1)
+            )
+            buf.append(ref)
+            off.append([cur_pos])
+            cur_pos += len(lc_ref)
+
 
 class UniProtAdditionalXRefImporter(object):
     def __init__(self, *args):
         self.verify_enum = tablefmt.XRefTable.columns.get("Verification").enum
         xref_enum = tablefmt.XRefTable.columns.get("XRefSource").enum
         self.mapping = {
             x: xref_enum[x]
@@ -2315,15 +2468,19 @@
             }
         )
         self._lookup = collections.defaultdict(list)
         for fpath in args:
             if os.path.exists(fpath):
                 self._load_projected_xrefs(fpath)
             else:
-                common.package_logger.warning('UniProt projected XRef file "{}" does not exist. Skipping'.format(fpath))
+                common.package_logger.warning(
+                    'UniProt projected XRef file "{}" does not exist. Skipping'.format(
+                        fpath
+                    )
+                )
 
     def _load_projected_xrefs(self, fpath):
         with open(fpath, "rt", newline="", encoding="utf-8", errors="ignore") as fh:
             csv_reader = csv.reader(fh, delimiter="\t")
             for row in csv_reader:
                 try:
                     source = self.mapping[row[1]]
@@ -2353,15 +2510,17 @@
             "GeneName": xref_enum["Gene Name"],
         }
         self.xrefs = []
         for fpath in args:
             if os.path.exists(fpath):
                 self.load_approx_xref_file(fpath)
             else:
-                common.package_logger.warning('Approximate XRef file "{}" does not exist. Skipping'.format(fpath))
+                common.package_logger.warning(
+                    'Approximate XRef file "{}" does not exist. Skipping'.format(fpath)
+                )
         self._pos = 0
         self._last_enr = 0
 
     def load_approx_xref_file(self, fpath):
         with open(fpath, "rt", newline="", encoding="utf-8", errors="ignore") as fh:
             for row in csv.reader(fh, delimiter="\t"):
                 if row[1] in self.mapping:
@@ -2395,15 +2554,17 @@
         """Initializes a Parser for SGML formatted darwin database file"""
         self.tag_handlers = collections.defaultdict(list)
         self.end_of_entry_notifier = []
 
     def add_tag_handler(self, tag, handler):
         """add a callback handler for a certain tag"""
         self.tag_handlers[tag].append(handler)
-        common.package_logger.debug("# handlers for {}: {}".format(tag, len(self.tag_handlers[tag])))
+        common.package_logger.debug(
+            "# handlers for {}: {}".format(tag, len(self.tag_handlers[tag]))
+        )
 
     def add_post_entry_handler(self, handler):
         self.end_of_entry_notifier.append(handler)
 
     def parse_entrytags(self, fh):
         """AC, CHR, DE, E, EMBL, EntrezGene, GI, GO, HGNC_Name, HGNC_Sym,
         ID, InterPro, LOC, NR , OG, OS, PMP, Refseq_AC, Refseq_ID, SEQ,
@@ -2415,24 +2576,31 @@
         for line in fh:
             line = line.strip()
             if not line.startswith("<E>"):
                 common.package_logger.debug("skipping line:" + line)
                 continue
 
             eNr += 1
-            common.package_logger.debug("entry {}: {}".format(eNr, line.encode("utf-8")))
+            common.package_logger.debug(
+                "entry {}: {}".format(eNr, line.encode("utf-8"))
+            )
             entry = lxml.html.fragment_fromstring(line)
             for tag, handlers in self.tag_handlers.items():
-                common.package_logger.debug("tag {} ({} handlers)".format(tag, len(handlers)))
+                common.package_logger.debug(
+                    "tag {} ({} handlers)".format(tag, len(handlers))
+                )
                 tag_text = [t.text for t in entry.findall("./" + tag.lower())]
                 for value in tag_text:
+                    # common.package_logger.debug('value of tag: {}'.format(value.encode('utf-8')))
                     if value is None:
                         continue
                     for handler in handlers:
                         handler(value, eNr)
+                        # common.package_logger.debug('called handler {} with ({},{})'.format(
+                        #    handler, value.encode('utf-8'), eNr))
             for notifier in self.end_of_entry_notifier:
                 notifier(eNr)
 
 
 DomainDescription = collections.namedtuple(
     "DomainDescription", tables.dtype_from_descr(tablefmt.DomainDescriptionTable).names
 )
@@ -2442,15 +2610,16 @@
     re_pattern = re.compile(r"(?P<id>[0-9.]*)\s{3,}\w{7}\s{3,}:\s*(?P<desc>.*)")
     source = b"CATH/Gene3D"
 
     def __init__(self, url):
         self.fname = download_url_if_not_present(url)
 
     def parse(self):
-        with common.auto_open(self.fname, "rt") as fh:
+        open_lib = gzip.open if self.fname.endswith(".gz") else open
+        with open_lib(self.fname, "rt") as fh:
             for line in fh:
                 match = self.re_pattern.match(line)
                 if match is not None:
                     yield DomainDescription(
                         DomainId=match.group("id").encode("utf-8"),
                         Source=self.source,
                         Description=match.group("desc").encode("utf-8"),
@@ -2486,15 +2655,17 @@
             gnrs = collections.Counter(map(enr_to_gnr, memb))
             for gn, cnts in gnrs.items():
                 in_groups[gn] += cnts
             for g1, g2 in itertools.combinations(gnrs, 2):
                 shared_ogs[g1, g2] += 1
                 shared_ogs[g2, g1] += 1
             common.package_logger.info(
-                "grp {} with {} members took {:.1f}msec".format(grp, len(memb), 1000 * (time.time() - t0))
+                "grp {} with {} members took {:.1f}msec".format(
+                    grp, len(memb), 1000 * (time.time() - t0)
+                )
             )
         self.shared_ogs = shared_ogs
         self.in_groups = in_groups
 
     def write(self, node=None):
         root = "/Summary" if node is None else node
         for label, data in (
@@ -2516,16 +2687,17 @@
 
 
 class PerGenomeHOGAuxAdder(PerGenomeOMAGroupAuxDataAdder):
     node_postfix = "hog"
 
     def get_group_members(self, etab):
         grp_members = collections.defaultdict(list)
+        fam_re = re.compile(rb"HOG:(?P<fam_nr>\d+)")
         for row in etab.where('OmaHOG != b""'):
-            fam = int(hog_re.match(row["OmaHOG"]).group("fam"))
+            fam = int(fam_re.match(row["OmaHOG"]).group("fam_nr"))
             grp_members[fam].append(row["EntryNr"])
         return grp_members
 
 
 class InvarianceException(Exception):
     pass
 
@@ -2539,82 +2711,50 @@
     :param fpath: path to genomes.json file
     :param h5: hdf5 database handle."""
     common.package_logger.info("Augmenting genomes.json file with Nr of HOGs per level")
 
     # load taxonomy and sorter by Name
     tax = h5.get_node("/Taxonomy").read()
     sorter = numpy.argsort(tax["Name"])
-    gs = h5.get_node("/Genome").read()
-    pe = h5.get_node("/Protein/Entries")
     with open(fpath, "rt") as fh:
         genomes = json.load(fh)
     os.rename(fpath, fpath + ".bak")
 
-    def traverse(node, parent_hogs=None, parent_hogs_support=None):
+    def traverse(node, parent_hogs=None):
+        if "children" not in node:
+            return
+
         if parent_hogs is None:
             parent_hogs = numpy.array([], dtype=h5.get_node("/HogLevel").dtype)
-        if parent_hogs_support is None:
-            parent_hogs_support = numpy.array([], dtype=h5.get_node("/HogLevel").dtype)
-
         try:
             n = node["name"].encode("utf-8")
             idx = numpy.searchsorted(tax["Name"], n, sorter=sorter)
             if tax["Name"][sorter[idx]] == n:
                 node["taxid"] = taxid = int(tax["NCBITaxonId"][sorter[idx]])
             elif n == b"LUCA":
                 taxid = 0
-            elif b"(disambiguate" in n:
-                # this is a special case to deal with internal species
-                # hoginfo is stored at tax[UniProtSpeciesCode]
-                taxid = node["id"]
             else:
                 node["nr_hogs"] = 0
                 raise ValueError("not in taxonomy: {}".format(n))
-
-            for modif, completeness, parent in zip(["", "_support"], [0.0, 0.2], [parent_hogs, parent_hogs_support]):
-                hogs = h5.get_node(f"/AncestralGenomes/tax{taxid}/Hogs").read_where("CompletenessScore > completeness")
-                if modif == "":
-                    hog_level = hogs
-                else:
-                    hog_level_support = hogs
-                node["nr_hogs{}".format(modif)] = len(hogs)
-                diff_parent, dupl_events = hoghelper.compare_levels(parent, hogs, return_duplication_events=True)
-                changes = collections.defaultdict(int)
-                for x in diff_parent["Event"]:
-                    changes[x.decode()] += 1
-                changes["duplications"] = dupl_events
-                if "children" not in node and modif != "_support":
-                    # dealing with an extend species, special way to assess gains, based on
-                    # HOG singletons that are main isoforms
-                    assert changes["gained"] == 0
-                    g = numpy.extract(gs["UniProtSpeciesCode"] == node["id"].encode("utf-8"), gs)[0]
-                    query_main_iso_of_genome = "(EntryNr > {}) & (EntryNr <= {}) & ((AltSpliceVariant == 0) | (AltSpliceVariant == EntryNr))".format(
-                        g["EntryOff"], g["EntryOff"] + g["TotEntries"]
-                    )
-                    nr_genes, nr_gains = 0, 0
-                    for p in pe.where(query_main_iso_of_genome):
-                        nr_genes += 1
-                        if p["OmaHOG"] == b"":
-                            nr_gains += 1
-                    changes["gained"] = nr_gains
-                    node["nr_genes{}".format(modif)] = nr_genes
-                node["evolutionaryEvents{}".format(modif)] = changes
-            common.package_logger.info(
-                "node: {}: events: {}; events_support: {}".format(
-                    n, node["evolutionaryEvents"], node["evolutionaryEvents_support"]
-                )
+            hog_level = h5.get_node("/Hogs_per_Level/tax{}".format(taxid)).read()
+            node["nr_hogs"] = len(hog_level)
+            diff_parent, dupl_events = hoghelper.compare_levels(
+                parent_hogs, hog_level, return_duplication_events=True
             )
+            changes = collections.defaultdict(int)
+            for x in diff_parent["Event"]:
+                changes[x.decode()] += 1
+            changes["duplications"] = dupl_events
+            node["evolutionaryEvents"] = changes
         except Exception:
             common.package_logger.exception("Cannot identify taxonomy id")
             hog_level = parent_hogs.copy()
-            hog_level_support = parent_hogs_support.copy()
 
-        if "children" in node:
-            for child in node["children"]:
-                traverse(child, parent_hogs=hog_level, parent_hogs_support=hog_level_support)
+        for child in node["children"]:
+            traverse(child, parent_hogs=hog_level)
 
     traverse(genomes)
     with open(fpath, "wt") as fh:
         json.dump(genomes, fh)
 
 
 def getLogger(level="DEBUG"):
@@ -2624,99 +2764,78 @@
     if isinstance(level, str):
         level = logging.getLevelName(level.upper())
         if not isinstance(level, int):
             level = logging.DEBUG
     log.setLevel(level)
     logHandler = logging.StreamHandler()
     logHandler.setLevel(level)
-    logHandler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
+    logHandler.setFormatter(
+        logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+    )
     log.addHandler(logHandler)
     return log
 
 
-def main(
-    name="OmaServer.h5",
-    k=6,
-    idx_name=None,
-    domains=None,
-    log_level="INFO",
-    release=None,
-    phases=None,
-):
+def main(name="OmaServer.h5", k=6, idx_name=None, domains=None, log_level="INFO"):
     idx_name = (name + ".idx") if idx_name is None else idx_name
-    if phases is None:
-        phases = list(range(1, 10))
-    if not all((isinstance(z, int) for z in phases)) or min(phases) < 1 or max(phases) > 9:
-        raise ValueError("phases argument must be integers between 1 and 9")
-    phases = uniq(sorted(phases))
-
-    def phase1():
-        x.add_version(release_char=release)
-        x.add_species_data()
-        x.add_orthologs()
-        x.add_same_species_relations()
-        x.add_proteins()
-
-    def phase2():
-        x.add_sequence_suffix_array(k=k, fn=idx_name)
-
-    def phase3():
-        x.add_hogs()
-        x.add_xrefs()
-
-    def phase4():
-        x.add_synteny_scores()
-        x.add_homoeology_confidence()
-
-    def phase5():
-        if domains is None:
-            domainFiles = ["file:///dev/null"]
-        else:
-            domainFiles = list(map(lambda url: "file://" + url if url.startswith("/") else url, domains))
-        log.info("loading domain annotations from {}".format(domainFiles))
-        x.add_domain_info(
-            filter_duplicated_domains(
-                only_pfam_or_cath_domains(itertools.chain.from_iterable(map(iter_domains, domainFiles)))
-            )
-        )
-        x.add_domainname_info(
-            itertools.chain(
-                CathDomainNameParser(
-                    "http://download.cathdb.info/cath/releases/latest-release/"
-                    "cath-classification-data/cath-names.txt"
-                ).parse(),
-                PfamDomainNameParser(
-                    "ftp://ftp.ebi.ac.uk/pub/databases/Pfam/current_release/Pfam-A.clans.tsv.gz"
-                ).parse(),
-            )
-        )
 
-    def phase6():
-        x.add_canonical_id()
-        x.add_group_metadata()
-        x.add_hog_domain_prevalence()
-        x.add_roothog_metadata()
-        x.add_gene_ontology_term_cnts()
-
-    def phase7():
-        x.create_indexes()
-        x.update_summary_stats()
-        x.add_per_species_aux_groupdata()
-
-    def phase8():
-        x.add_cache_of_hogs_by_level(min(os.cpu_count(), 32))
-
-    def phase9():
-        genomes_json_fname = os.path.normpath(
-            os.path.join(os.path.dirname(x.h5.filename), "..", "downloads", "genomes.json")
+    log = getLogger(log_level)
+    x = DarwinExporter(name, logger=log)
+    x.add_version()
+    x.add_species_data()
+    x.add_orthologs()
+    x.add_same_species_relations()
+    x.add_proteins()
+    x.add_hogs()
+    x.add_xrefs()
+    x.add_synteny_scores()
+    x.add_homoeology_confidence()
+    if domains is None:
+        domains = ["file://dev/null"]
+    else:
+        domains = list(
+            map(lambda url: "file://" + url if url.startswith("/") else url, domains)
+        )
+    log.info("loading domain annotations from {}".format(domains))
+    x.add_domain_info(
+        filter_duplicated_domains(
+            only_pfam_or_cath_domains(
+                itertools.chain.from_iterable(map(iter_domains, domains))
+            )
         )
-        augment_genomes_json_download_file(genomes_json_fname, x.h5)
+    )
+    # iter_domains('file:///scratch/beegfs/monthly/aaltenho/Browser/cath/all_domains.csv.gz'),
+    # iter_domains('file:///scratch/beegfs/monthly/aaltenho/Browser/cath/additional_domains.mdas.csv.gz')
+    #    ))))
+    x.add_domainname_info(
+        itertools.chain(
+            CathDomainNameParser(
+                "http://download.cathdb.info/cath/releases/latest-release/"
+                "cath-classification-data/cath-names.txt"
+            ).parse(),
+            PfamDomainNameParser(
+                "ftp://ftp.ebi.ac.uk/pub/databases/Pfam/current_release/Pfam-A.clans.tsv.gz"
+            ).parse(),
+        )
+    )
+    x.add_canonical_id()
+    x.add_group_metadata()
+    x.add_hog_domain_prevalence()
+    x.add_roothog_metadata()
+    x.close()
 
-    log = getLogger(log_level)
-    log.info("Running the following phases: {}".format(phases))
     x = DarwinExporter(name, logger=log)
-    for phase_nr in phases:
-        phase_func = locals()["phase{}".format(phase_nr)]
-        log.info("calling phase{}".format(phase_nr))
-        phase_func()
-        log.info("done with phase{}".format(phase_nr))
+    x.create_indexes()
+    x.add_sequence_suffix_array(k=k, fn=idx_name)
+    x.update_summary_stats()
+    x.add_per_species_aux_groupdata()
+    x.add_cache_of_hogs_by_level(min(os.cpu_count(), 32))
+    genomes_json_fname = os.path.normpath(
+        os.path.join(os.path.dirname(x.h5.filename), "..", "downloads", "genomes.json")
+    )
+    augment_genomes_json_download_file(genomes_json_fname, x.h5)
     x.close()
+
+    # compute cached orthology counts
+    compute_and_store_cached_data(
+        x.h5.filename, "/Protein/OrthologsCountCache", min(os.cpu_count(), 12)
+    )
```

### Comparing `pyoma-0.13.2/pyoma/browser/convert_omastandalone.drw` & `pyoma-0.9.4/pyoma/browser/convert_omastandalone.drw`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     tab := table():
     tab['GS'] := gs:
     _parents := []:
     if lowercase(SpeciesTree)='lineage' then
         linData := sort([seq([GS[g,Lineage], g], g=genomes)]):
         SpeciesTreeR(linData, 1, 0);
         if sum(If(z[2]=0,1,0), z=_parents) > 1 then
-            _parents := append(_parents, [0,0, 'LUCA']);
+            _parents = append(_parents, [0,0, 'LUCA']);
         fi:
     else
         stree := SpeciesTree;
         if lowercase(SpeciesTree)='estimate' then
             stree := ReadRawFile(root_dir.'/'.OutputFolder.'/EstimatedSpeciesTree.nwk');
         fi:
         TreeToParentTable(ParseNewickTree(stree), 0):
@@ -297,15 +297,28 @@
             vptab := append(vptab, [i, vp, 'n/a'])
         od:
     od:
     StoreResults(json(vptab)):
 end:
 
 GetSameSpeciesRelations := proc(g)
+    global DB;
+    ReadDb(ddir.'/ServerVPs.db');
+    gNr := SearchArray(g, genomes);
     ssTab :=  []:
+    for i from Goff[gNr]+1 to Goff[gNr+1] do
+        e := Entry(i);
+        for cp in parse(SearchTag('CP', e)) do
+            ssTab := append(ssTab, [i, cp, 'close paralog', -1, -1, -1, -1]);
+        od:
+        hpTag := SearchTag('HP', e);
+        if hpTag<>'' then for hp in parse(hpTag) do
+            ssTab := append(ssTab, [i, hp[1], 'homeolog', -1, hp[2], -1, -1, -1]);
+        od fi:
+    od:
     StoreResults(json(ssTab));
 end:
 
 StoreProteinsForGenome := proc(g, grps, fname)
     global DB, Splicings;
     tab:= table():
     gNr := SearchArray(g, genomes);
```

### Comparing `pyoma-0.13.2/pyoma/browser/db.py` & `pyoma-0.9.4/pyoma/browser/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,73 +6,41 @@
 import itertools
 import json
 import logging
 import os
 import re
 import threading
 import time
-import warnings
 from bisect import bisect_left
 from builtins import chr, range, object, zip, bytes, str
 from xml.etree import ElementTree as et
-from typing import Union, Tuple, Optional, AnyStr, Set, Generator, Mapping
 
 import dateutil
 import fuzzyset
 import networkx as nx
 import numpy
 import numpy.lib.recfunctions
-import pandas
 import pandas as pd
 import pyopa
 import tables
 import tables.file as _tables_file
 from Bio.UniProt import GOA
 from datasketch import MinHash
 from tqdm import tqdm
 
 from .KmerEncoder import KmerEncoder
-from .decorators import timethis, outdated_database_warning
-from .exceptions import (
-    InvalidTaxonId,
-    DBVersionError,
-    DBConsistencyError,
-    DBOutdatedError,
-    InvalidId,
-    InvalidOmaId,
-    UnknownIdType,
-    UnknownSpecies,
-    OutdatedHogId,
-    Singleton,
-    NoReprEntry,
-    AmbiguousID,
-    TooUnspecificQuery,
-)
-from .geneontology import GeneOntology, OntologyParser, GOAspect, FreqAwareGeneOntology
-from .hoghelper import compare_levels, are_orthologous
+from .decorators import timethis
+from .geneontology import GeneOntology, OntologyParser, GOAspect
+from .hoghelper import compare_levels
 from .hogprofile import Profiler
 from .models import LazyProperty, KeyWrapper, ProteinEntry, Genome, HOG
 from .suffixsearch import SuffixSearcher, SuffixIndexError
-from .idmapper import (
-    XRefNoApproximateIdMapper,
-    XrefIdMapper,
-    LinkoutIdMapper,
-    GeneNameOrSymbolIdMapper,
-    GeneNameAndMainDbIdMapper,
-    UniProtIdMapper,
-    DomainNameIdMapper,
-)
 from .. import version
 
 logger = logging.getLogger(__name__)
-warnings.filterwarnings(
-    "ignore",
-    category=tables.PerformanceWarning,
-    message=r".*maximum recommended rowsize.*",
-)
 
 # Raise stack limit for PyOPA ~400MB
 threading.stack_size(4096 * 100000)
 
 # Global initialisations
 GAF_VERSION = "2.1"
 
@@ -147,210 +115,105 @@
 _tables_file._open_files = ThreadsafeFileRegistry()
 
 
 # end monkey patch pytables
 ####
 
 
-def count_rows_of_index_column_with_value(tab: Union[str, tables.Table], col: str, start, end=None):
-    idx = tab.colindexes[col]
-    stop = end if end is not None else start
-    return idx.search((start, stop))
-
-
-def _get_limited_synteny_graph(
-    edges_data: Generator[Tuple[int, int, dict], None, None],
-    hog_tab: Union[tables.Table, numpy.ndarray, dict],
-    ref_hog_idx: Optional[int],
-    steps: Optional[int],
-):
-    G = nx.Graph()
-    G.add_edges_from(edges_data)
-    if ref_hog_idx is not None:
-        try:
-            neighbors = [ref_hog_idx] + [v for u, v in nx.bfs_edges(G, source=ref_hog_idx, depth_limit=steps)]
-        except nx.exception.NetworkXError as e:
-            logger.error(
-                "Trying to access a non-stored HOG in the ancestral synteny graph: "
-                "hog_row: {}, Size of Graph: N={}, E={}".format(ref_hog_idx, len(G), len(G.edges))
-            )
-            raise DBConsistencyError("Cannot find HogIdx {}  in Ancestral synteny graph".format(ref_hog_idx))
-        S = G.subgraph(neighbors)
-    else:
-        if isinstance(hog_tab, dict):
-            G.add_nodes_from(hog_tab.keys())
-        else:
-            G.add_nodes_from(range(len(hog_tab)))
-        S = G
-    for n in S.nodes:
-        hog = hog_tab[n]
-        S.nodes[n].update(
-            {
-                "nr_members": int(hog["NrMemberGenes"]),
-                "completeness_score": float(hog["CompletenessScore"]),
-            }
-        )
-    return nx.relabel_nodes(S, lambda x: hog_tab[x]["ID"].decode())
-
-
-def read_table_where(
-    tab: tables.Table, query: str, condvars: Optional[Mapping] = None, field: str = None
-) -> numpy.ndarray:
-    """Reads data of a pytables table fulfilling the query as a numpy array.
-
-    This is a more efficient implementation of the :py:method:`tables.Table.read_where`
-    method.
-
-    :param tab: The table to be read from
-    :param query: the query
-    :param condvars: mapping of condition variables of the query
-    :param field: which column to be read.
-                  If set to None, all columns are read, if set to 'nrow',
-                  the row number is returned
-    :return the data as a numpy array
-    """
-    it = tab.where(query, condvars=condvars)
-    try:
-        first = next(it)
-    except StopIteration:
-        return numpy.array([], dtype=tab.dtype)
-    if field is None:
-        fun = lambda row: row.fetch_all_fields()
-        dtyp = tab.dtype
-    elif field.lower == "nrow":
-        fun = lambda row: row.nrow
-        dtyp = numpy.int64
-    else:
-        fun = lambda row: row[field]
-        dtyp = tab.dtype[field]
-
-    data = numpy.fromiter(
-        map(fun, itertools.chain([first], it)),
-        dtype=dtyp,
-    )
-    return data
+class DBOutdatedError(Exception):
+    pass
 
 
 class Database(object):
     """This is the main interface to the oma database. Queries
-    will typically be issued by methods of this object. Typically,
+    will typically be issued by methods of this object. Typically
     the result of queries will be :py:class:`numpy.recarray` objects."""
 
-    EXPECTED_DB_SCHEMA = "3.6"
+    EXPECTED_DB_SCHEMA = "3.4"
 
     def __init__(self, db):
         if isinstance(db, str):
-            logger.info("opening %s for read-only", db)
+            logger.info("opening {} for read-only".format(db))
             self.db = tables.open_file(db, "r")
             self._close_fh = True
-        elif isinstance(db, (tables.File, tables.file.File)):
+        elif isinstance(db, tables.File):
             self.db = db
             self._close_fh = False
         else:
             raise ValueError(str(db) + " is not a valid database type")
 
         try:
             lib_version = self.db.get_node_attr("/", "pyoma_version")
         except AttributeError:
             lib_version = "<=0.7.0"
-        logger.info("pyoma library version: {}; db written with {}".format(version(), lib_version))
+        logger.info(
+            "pyoma library version: {}; db written with {}".format(
+                version(), lib_version
+            )
+        )
 
         try:
             db_version = self.db.get_node_attr("/", "db_schema_version")
         except AttributeError:
             db_version = "1.0"
 
-        logger.info("database version: %s", db_version)
-        logger.info("release: %s; release_char in HOG-IDs: '%s'", self.get_release_name(), self.release_char)
+        logger.info("database version: {}".format(db_version))
         if db_version != self.EXPECTED_DB_SCHEMA:
             exp_tup = self.EXPECTED_DB_SCHEMA.split(".")
             db_tup = db_version.split(".")
             if db_tup[0] != exp_tup[0]:
                 raise DBVersionError(
                     "Unsupported database version: {} != {} ({})".format(
                         db_version, self.EXPECTED_DB_SCHEMA, self.db.filename
                     )
                 )
             else:
                 logger.warning(
-                    "outdated database version, but only minor version change: %s != %s. Some functions might fail",
-                    db_version,
-                    self.EXPECTED_DB_SCHEMA,
+                    "outdated database version, but only minor version change: "
+                    "{} != {}. Some functions might fail".format(
+                        db_version, self.EXPECTED_DB_SCHEMA
+                    )
                 )
         self.db_schema_version = tuple(int(z) for z in db_version.split("."))
-        self._on_close_notify = []
 
         try:
             self.seq_search = SequenceSearch(self)
         except DBConsistencyError as e:
-            logger.exception("Cannot load SequenceSearch. Any future call to seq_search will fail!")
-            self.seq_search = None
+            logger.exception(
+                "Cannot load SequenceSearch. Any future call to seq_search will fail!"
+            )
+            self.seq_search = object()
         self.id_resolver = IDResolver(self)
         self.id_mapper = IdMapperFactory(self)
         genomes = [Genome(self, g) for g in self.db.root.Genome.read()]
-        self.tax = Taxonomy(self.db.root.Taxonomy.read(), genomes={g.ncbi_taxon_id: g for g in genomes})
+        self.tax = Taxonomy(
+            self.db.root.Taxonomy.read(), genomes={g.ncbi_taxon_id: g for g in genomes}
+        )
         try:
             self.desc_searcher = DescriptionSearcher(self)
         except SuffixIndexError:
             self.desc_searcher = None
         self.hog_profiler = None
         self._re_fam = None
         self.format_hogid = None
         self.mds = None
         self._set_hogid_schema()
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-    def register_on_close(self, callback):
-        self._on_close_notify.append(callback)
-        logger.debug("registered call to %s on close", callback)
-
-    def unregister_on_close(self, callback):
-        try:
-            self._on_close_notify.remove(callback)
-            logger.debug("un-register %s on close", callback)
-        except ValueError:
-            logger.debug("could not un-register %s", callback)
-
     def close(self):
-        for listener in self._on_close_notify:
-            listener()
         if self._close_fh:
             self.get_hdf5_handle().close()
 
     @LazyProperty
     def gene_ontology(self):
         """returns GeneOntology object containing hierarchy
         of terms using the is_a and part_of relations. See
         :meth:`load_gene_ontology` to parametrize the
         creation of GeneOntology object."""
         return self.load_gene_ontology(GeneOntology)
 
-    @LazyProperty
-    def freq_aware_gene_ontology(self):
-        gof = self.load_gene_ontology(factory=FreqAwareGeneOntology)
-        try:
-            go_count_tab = self.db.get_node("/Ontologies/GeneOntologyTermCounts")
-            gof.cnts = {int(row["TermNr"]): int(row["Counts"]) for row in go_count_tab}
-            gof.tot_cnts = [
-                go_count_tab.attrs[z]
-                for z in (
-                    "total_molecular_function",
-                    "total_biological_process",
-                    "total_cellular_component",
-                )
-            ]
-        except tables.NoSuchNodeError:
-            pass
-        return gof
-
     def load_gene_ontology(self, factory=None, rels=None):
         """Instantiate GeneOntology object
 
         By default, a GeneOntology object is returned based on
         the default relations (which are defined in :mod:`.gene_ontology`)
 
         The factory parameter allows to specify an subtype of
@@ -360,15 +223,17 @@
         should be used as parents relations.
 
         :param factory: GeneOntology factory
         :param rels: list of rels for parent relations
 
         :returns: GeneOntology object"""
         try:
-            fp = io.StringIO(self.db.root.Ontologies.GO.read().tobytes().decode("utf-8"))
+            fp = io.StringIO(
+                self.db.root.Ontologies.GO.read().tobytes().decode("utf-8")
+            )
         except tables.NoSuchNodeError:
             p = os.path.join(os.path.dirname(self.db.filename), "go-basic.obo")
             fp = open(p, "rt")
         if factory is None:
             factory = GeneOntology
         go = factory(OntologyParser(fp), rels=rels)
         go.parse()
@@ -405,192 +270,119 @@
         """Returns the entry from the /Protein/Entries table
         corresponding to entry_nr.
 
         :param int entry_nr: a numeric identifier for the protein
             entry"""
         entry = self.db.root.Protein.Entries[entry_nr - 1]
         if entry["EntryNr"] != entry_nr:
-            logger.warning("EntryNr {} not at position {}. Using index instead".format(entry_nr, entry_nr - 1))
-            entry = self.db.root.Protein.Entries.read_where("EntryNr == {:d}".format(entry_nr))
+            logger.warning(
+                "EntryNr {} not at position {}. Using index instead".format(
+                    entry_nr, entry_nr - 1
+                )
+            )
+            entry = self.db.root.Protein.Entries.read_where(
+                "EntryNr == {:d}".format(entry_nr)
+            )
             if len(entry) != 1:
-                raise ValueError("there are {} entries with entry_nr {}".format(len(entry), entry_nr))
+                raise ValueError(
+                    "there are {} entries with entry_nr {}".format(len(entry), entry_nr)
+                )
             entry = entry[0]
         return entry
 
     def _set_hogid_schema(self):
         """Determines the used HOG ID schema
 
         Some versions of the database have HOG IDs of the form
         "HOG:0000001" and others without the prefix (e.g. standalone)
         or with the prefix, but without padding. This method checks
         which schema is used and sets the appropriate member vars
         """
-        re_id = re.compile(rb"(?P<prefix>HOG:)(?P<rel>[A-Z]+)?(?P<nr>\d+)")
+        re_id = re.compile(b"(?P<prefix>HOG:)(?P<nr>\d+)")
         for entry in self.db.root.Protein.Entries:
             m = re_id.match(entry["OmaHOG"])
             if m is None:
                 continue
             nr = m.group("nr")
             if len(nr) >= 7 and not nr.startswith(b"0"):
                 continue  # a case where we cannot determine if padded nr
             is_padded = nr.startswith(b"0")
             prefix = m.group("prefix").decode()
             if prefix is None:
                 prefix = ""
-            rel = m.group("rel").decode() if m.group("rel") else ""
-            if rel != self.release_char:
-                raise DBConsistencyError("release_char does not match HOG-ids: {} vs {}".format(self.release_char, rel))
-            fmt = "{}{}{{:{}d}}".format(prefix, rel, "07" if is_padded else "")
-            self._re_fam = re.compile(r"{}(?P<rel>[A-Z]+)?(?P<fam>\d+)".format(prefix).encode("ascii"))
+            fmt = "{}{{:{}d}}".format(prefix, "07" if is_padded else "")
+            self._re_fam = re.compile("{}(?P<fam>\d+)".format(prefix).encode("ascii"))
             self.format_hogid = lambda fam: fmt.format(fam)
-            logger.info("setting HOG ID schema: re_fam: {}, hog_fmt: {}".format(self._re_fam, fmt))
+            logger.info(
+                "setting HOG ID schema: re_fam: {}, hog_fmt: {}".format(
+                    self._re_fam, fmt
+                )
+            )
             return
         raise DBConsistencyError("no protein in a hog")
 
     def all_proteins_of_genome(self, genome):
         """return all protein entries of a genome"""
         rng = self.id_mapper["OMA"].genome_range(genome)
         prot_tab = self.get_hdf5_handle().get_node("/Protein/Entries")
-        return read_table_where(prot_tab, "(EntryNr >= {}) & (EntryNr <= {})".format(rng[0], rng[1]))
+        return prot_tab.read_where(
+            "(EntryNr >= {}) & (EntryNr <= {})".format(rng[0], rng[1])
+        )
 
     def main_isoforms(self, genome):
         """returns the proteins that are the main isoforms of a genome.
 
         The main isoform is in this context the isoform that we used in OMA to
         infer the orthologs. It is the one variant that has the most alignment
         matches to all other gnomes.
 
-        The `genome` parameter should be the UniProtSpeciesCode of the species of
+        The genome parameter should be the UniProtSpeciesCode of the species of
         interest. If it is a numeric value, the genome parameter is interpreted
         as the protein entrynr. The method returns then the main isoforms for
         the species to which this protein belongs.
 
         :Note: OMA only predicts orthologs for the main isoform, so there is no
             difference if you work with only the main isoforms or all proteins of
             a genome in terms of orthologs.
 
         :param genome: UniProtSpeciesCode of the genome of interest, or a gene
                        number (EntryNr) from the genome of interest.
         """
         rng = self.id_mapper["OMA"].genome_range(genome)
-        it = self._main_isoform_iter(rng[0], rng[1])
-        try:
-            first = next(it)
-        except StopIteration:
-            return numpy.array([], dtype=self.get_hdf5_handle().get_node("/Protein/Entries").dtype)
-        return numpy.fromiter(
-            map(lambda x: x.fetch_all_fields(), itertools.chain([first], it)),
-            dtype=first.table.dtype,
-        )
-
-    def _main_isoform_iter(self, entry_nr_low=None, entry_nr_high=None):
-        query = []
-        if entry_nr_low is not None:
-            query.append("(EntryNr >= {})".format(entry_nr_low))
-        if entry_nr_high is not None:
-            query.append("(EntryNr <= {})".format(entry_nr_high))
-        query.append("((AltSpliceVariant == EntryNr) | (AltSpliceVariant == 0))")
-        query = " & ".join(query)
         prot_tab = self.get_hdf5_handle().get_node("/Protein/Entries")
-        res_iter = prot_tab.where(query)
-        return res_iter
-
-    def count_main_isoforms(self, genome=None):
-        """returns the number of main isoforms (i.e. the number
-        of genes).
-
-        If `genome` parameter is not `None`, the count is limited to the specified
-        genome, otherwise all genomes in the database are used.
-
-        The `genome` parameter should be the UniProtSpeciesCode of the species of
-        interest. If it is a numeric value, the genome parameter is interpreted
-        as the protein entrynr. The method returns then the main isoforms for
-        the species to which this protein belongs.
-
-        :param genome: UniProtSpeciesCode of the genome of interest, or a gene
-                       number (EntryNr) from the genome of interest.
-        """
-        low, high = None, None
-        if genome is not None:
-            low, high = self.id_mapper["OMA"].genome_range(genome)
-        return count_elements(self._main_isoform_iter(low, high))
+        return prot_tab.read_where(
+            "(EntryNr >= {}) & (EntryNr <= {}) & ((AltSpliceVariant == EntryNr) | (AltSpliceVariant == 0))".format(
+                rng[0], rng[1]
+            )
+        )
 
     def get_splicing_variants(self, entry):
         e = self.ensure_entry(entry)
         if e["AltSpliceVariant"] == 0:
             return numpy.array([e], dtype=e.dtype)
         # TODO: create index on AltSpliceVariant column?!
-        return read_table_where(
-            self.get_hdf5_handle().get_node("/Protein/Entries"),
-            "(EntryNr >= {:d}) & (EntryNr < {:d}) & (AltSpliceVariant == {:d})".format(
-                e["EntryNr"] - 100, e["EntryNr"] + 100, e["AltSpliceVariant"]
-            ),
-        )
-
-    def get_extant_synteny_graph(
-        self,
-        genome,
-        center_entry: Optional[Union[int, str]] = None,
-        window: Optional[int] = None,
-    ):
-        all_genes = self.main_isoforms(genome)
-        all_genes.sort(order=["Chromosome", "LocusStart"])
-        gs = self.id_mapper["OMA"].genome_of_entry_nr(all_genes[0]["EntryNr"])
-        if center_entry is not None:
-            if window is None:
-                window = 7
-            if isinstance(center_entry, str) and center_entry.startswith("HOG:"):
-                k = numpy.where(all_genes["OmaHOG"] == center_entry.encode("utf-8"))[0]
-                if len(k) == 1:
-                    en = all_genes[k]
-                else:
-                    raise InvalidId(f"{center_entry} unknown for {gs['UniProtSpeciesCode']}")
-            else:
-                en = self.ensure_entry(self.id_resolver.resolve(center_entry))
-                if en["AltSpliceVariant"] > 0 and en["AltSpliceVariant"] != en["EntryNr"]:
-                    en = self.ensure_entry(en["AltSpliceVariant"])
-            try:
-                idx = numpy.where(all_genes["EntryNr"] == en["EntryNr"])[0][0]
-                ref = all_genes[idx]
-            except IndexError:
-                identified_genome = gs["UniProtSpeciesCode"].decode()
-                raise InvalidId(f"Center gene {center_entry} is not a valid for genome {identified_genome}")
-            all_genes = all_genes[idx - window : idx + window + 1]
-            all_genes = all_genes[numpy.where(all_genes["Chromosome"] == ref["Chromosome"])]
-        oma_ids = list(
-            map(
-                lambda x: f"{gs['UniProtSpeciesCode'].decode()}{x - gs['EntryOff']:05d}",
-                all_genes["EntryNr"],
+        return (
+            self.get_hdf5_handle()
+            .get_node("/Protein/Entries")
+            .read_where(
+                "(EntryNr >= {:d}) & (EntryNr < {:d}) & (AltSpliceVariant == {:d})".format(
+                    e["EntryNr"] - 100, e["EntryNr"] + 100, e["AltSpliceVariant"]
+                )
             )
         )
 
-        def node_data_generator(genes):
-            for id_, g in zip(oma_ids, genes):
-                yield (
-                    id_,
-                    {
-                        "chromosome": g["Chromosome"].decode(),
-                        "start": int(g["LocusStart"]),
-                        "strand": "+" if g["LocusStrand"] > 0 else "-",
-                        "hog_id": g["OmaHOG"].decode(),
-                    },
-                )
-
-        G = nx.Graph()
-        G.add_nodes_from(node_data_generator(all_genes))
-        for i in range(len(all_genes) - 1):
-            if all_genes[i]["Chromosome"] == all_genes[i + 1]["Chromosome"]:
-                G.add_edge(oma_ids[i], oma_ids[i + 1], weight=1)
-        return G
-
     def _get_vptab(self, entry_nr):
         return self._get_pw_tab(entry_nr, "VPairs")
 
     def _get_pw_tab(self, entry_nr, subtab):
-        genome = self.id_mapper["OMA"].genome_of_entry_nr(entry_nr)["UniProtSpeciesCode"].decode()
+        genome = (
+            self.id_mapper["OMA"]
+            .genome_of_entry_nr(entry_nr)["UniProtSpeciesCode"]
+            .decode()
+        )
         return self.db.get_node("/PairwiseRelation/{}/{}".format(genome, subtab))
 
     def nr_ortholog_relations(self, entry_nr):
         """returns the number of orthologous relations for a given entry.
 
         The return value is a numpy.void tuple with all the gene centric orthology/paralogy
         counts. The named fields are:
@@ -624,29 +416,30 @@
             return cnt
 
     def count_homoeologs(self, entry_nr):
         """number of homoeologs of a given protein entry"""
         pwtab = self._get_pw_tab(entry_nr, "within")
         homolog_typ_nr = pwtab.get_enum("RelType")["homeolog"]
         try:
-            cnt = count_elements(pwtab.where("(EntryNr1=={:d}) & (RelType == {:d})".format(entry_nr, homolog_typ_nr)))
+            cnt = count_elements(
+                pwtab.where(
+                    "(EntryNr1=={:d}) & (RelType == {:d})".format(
+                        entry_nr, homolog_typ_nr
+                    )
+                )
+            )
         except (TypeError, ValueError):
             cnt = 0
         return cnt
 
-    def _get_pw_data(self, entry_nr, tab, target_range=None, typ_filter=None, extra_cols=None):
-        if isinstance(entry_nr, tuple):
-            query = "(EntryNr1 >= {:d}) & (EntryNr1 <= {:d})".format(*entry_nr)
-        else:
-            query = "(EntryNr1 == {:d})".format(entry_nr)
-        if target_range is not None:
-            query += " & (EntryNr2 >= {:d}) & (EntryNr2 <= {:d})".format(*target_range)
+    def _get_pw_data(self, entry_nr, tab, typ_filter=None, extra_cols=None):
+        query = "(EntryNr1 == {:d})".format(entry_nr)
         if typ_filter is not None:
             query += " & (RelType == {:d})".format(typ_filter)
-        dat = read_table_where(tab, query)
+        dat = tab.read_where(query)
         typ = tab.get_enum("RelType")
         cols = ["EntryNr1", "EntryNr2", "Score", "Distance"]
         if extra_cols is not None:
             cols.extend(extra_cols)
         res = numpy.lib.recfunctions.append_fields(
             dat[cols],
             names="RelType",
@@ -665,48 +458,14 @@
         orthology), the alignment score and the distance. The score and
         distance will be set to -1 if unknown.
 
         :param int entry_nr: the numeric entry_nr of the query protein."""
         vp_tab = self._get_vptab(entry_nr)
         return self._get_pw_data(entry_nr, vp_tab)
 
-    def get_vpairs_between_species_pair(self, genome1, genome2):
-        """Returns all the pairwise orthologs between two species.
-
-        This method returns a numpy array of the same dtype as
-        :meth:`get_vpairs` does. As input, two genomes present in the
-        OMA database need to be passed, either as rows from from the
-        GenomeTable or with the UniProt mnemonic species code.
-        The pairwise orthologs are symetric, so the order of genome1
-        and genome2 does not have any impact (except of the order of
-        EntryNr1 and EntryNr2)
-
-        :param genome1: first genome
-        :type genome1: :class:`numpy.void`, :class:`pyoma.browser.models.Genome`, str
-        :param genome2: second genome
-        :type genome2: :class:`numpy.void`, :class:`pyoma.browser.models.Genome`, str
-        :returns array with pairwise orthologs between genome1 and genome2
-        :rtype: `numpy.ndarray` of dtype :class:`.tablefmt.PairwiseRelationTable`
-
-        """
-
-        def to_genome(g) -> Genome:
-            if isinstance(g, Genome):
-                return g
-            else:
-                return Genome(self, g)
-
-        g1, g2 = map(to_genome, (genome1, genome2))
-        vptab = self._get_vptab(g1.entry_nr_offset + 1)
-        return self._get_pw_data(
-            entry_nr=(g1.entry_nr_offset + 1, g1.entry_nr_offset + g1.nr_entries),
-            target_range=(g2.entry_nr_offset + 1, g2.entry_nr_offset + g2.nr_entries),
-            tab=vptab,
-        )
-
     def get_within_species_paralogs(self, entry_nr):
         """returns the within species paralogs of a given entry
 
         This method returns a :class:`numpy.recarray` instance
         containing the close paralogs. Close paralogs are within
         species paralogs that are inparalogs to at least one
         ortholog of the query gene in OMA.
@@ -748,42 +507,48 @@
             for details on encoding."""
             if a["EntryNr"] == b["EntryNr"]:
                 return False
             prefix = os.path.commonprefix((a["OmaHOG"], b["OmaHOG"])).decode()
             if "." in prefix and prefix[-1].isdigit():
                 return False
             # count number of genes in query genome that are co-orthologs (== having the prefix)
-            cnts = numpy.char.startswith(hogids_of_genes_in_query_genome, prefix.encode("utf-8")).sum()
+            cnts = numpy.char.startswith(
+                hogids_of_genes_in_query_genome, prefix.encode("utf-8")
+            ).sum()
             return cnts
 
         try:
             fam = self.hog_family(entry)
             hog_member = self.member_of_fam(fam)
         except Singleton:
             # an empty fetch
             hog_member = self.db.root.Protein.Entries[0:0]
         hogids_of_genes_in_query_genome = hog_member[
             numpy.where(
-                (hog_member["EntryNr"] >= genome_entry_range[0]) & (hog_member["EntryNr"] < genome_entry_range[1])
+                (hog_member["EntryNr"] >= genome_entry_range[0])
+                & (hog_member["EntryNr"] < genome_entry_range[1])
             )
         ]["OmaHOG"]
         query_genome_genes_cnt = numpy.array(
             [is_orthologous(entry, hog_member[i]) for i in range(len(hog_member))],
             dtype="i4",
         )
-        mask = numpy.asarray(query_genome_genes_cnt, bool)
+        mask = numpy.asarray(query_genome_genes_cnt, numpy.bool)
         target_genomes = [
-            self.id_mapper["OMA"].genome_of_entry_nr(o["EntryNr"])["NCBITaxonId"] for o in hog_member[mask]
+            self.id_mapper["OMA"].genome_of_entry_nr(o["EntryNr"])["NCBITaxonId"]
+            for o in hog_member[mask]
         ]
         targ_genome_genes_cnt = collections.Counter(target_genomes)
         induced_orthologs = numpy.lib.recfunctions.append_fields(
             hog_member[mask],
             names="RelType",
             data=[
-                "{}:{}".format("m" if cnt_a > 1 else 1, "n" if targ_genome_genes_cnt[b] > 1 else 1).encode("utf-8")
+                "{}:{}".format(
+                    "m" if cnt_a > 1 else 1, "n" if targ_genome_genes_cnt[b] > 1 else 1
+                ).encode("utf-8")
                 for cnt_a, b in zip(query_genome_genes_cnt[mask], target_genomes)
             ],
         )
         return induced_orthologs
 
     def get_hog_induced_pairwise_paralogs(self, entry, start=0, stop=None):
         """This method retrieves the hog induced pairwise paralogs
@@ -793,15 +558,14 @@
         ProteinEntry, the array contains an additional column with the
         taxonomic level when the duplication occurred.
 
         :param entry: entry or entry_nr of the query protein"""
         entry = self.ensure_entry(entry)
         genome = self.id_mapper["OMA"].genome_of_entry_nr(entry["EntryNr"])
         lineage = self.tax.get_parent_taxa(genome["NCBITaxonId"])["Name"]
-        lineage = numpy.fromiter(filter(lambda x: x in self.tax.all_hog_levels, lineage), dtype=lineage.dtype)
         lineage_sorter = numpy.argsort(lineage)
         try:
             fam = self.hog_family(entry)
         except Singleton:
             # an empty fetch
             hog_member = self.db.root.Protein.Entries[0:0]
         else:
@@ -819,15 +583,17 @@
                 return False
             prefix = os.path.commonprefix((a["OmaHOG"], b["OmaHOG"])).decode()
             if "." in prefix and prefix[-1].isdigit():
                 # gene is paralog. find MRCA in taxonomy of common HOGid prefix
                 k = prefix.rfind(".")
                 hog_id = prefix[:k].encode("ascii")
                 cand_levels = levels[numpy.where(levels["ID"] == hog_id)]
-                sortidx = lineage.searchsorted(cand_levels["Level"], sorter=lineage_sorter)
+                sortidx = lineage.searchsorted(
+                    cand_levels["Level"], sorter=lineage_sorter
+                )
                 lin_idx = numpy.take(lineage_sorter, sortidx, mode="clip")
                 mask = lineage[lin_idx] == cand_levels["Level"]
                 # we take the first diverged lineage, meaning the duplication happened
                 # on the branch to that level.
                 return lineage[lin_idx[mask].min() - 1]
             return None
 
@@ -840,75 +606,14 @@
         ext_prot_dtype = numpy.dtype(entry.dtype.descr + [("DivergenceLevel", "S255")])
         paralogs = numpy.fromiter(
             itertools.islice(filter_candidates(entry, hog_member), start, stop),
             dtype=ext_prot_dtype,
         )
         return paralogs
 
-    def get_hog_induced_orthologs_between_genome_pair(self, g1, g2, return_cardinality=False, return_omagroup=False):
-        """Returns the HOG-induced pairwise orthologs between two genomes.
-
-        The method returns a numpy structured array with EntryNr1, EntryNr2 and HogID columns.
-        If `return_cardinaltiy` is set to True, a `RelType` column is added which returns the
-        cardinality of the relation (1:1, 1:n, m:1, m:1).
-        If `return_omagroup` is set to True, the returned array also has a column `OmaGroup` the
-        contains the numeric oma group if the two proteins belong to the same oma group. Otherwise,
-        the value is set to NaN.
-
-        :param g1: first genome
-        :type g1: :class:`numpy.void`, :class:`pyoma.browser.models.Genome`, str
-        :param g2: second genome
-        :type g2: :class:`numpy.void`, :class:`pyoma.browser.models.Genome`, str
-        :param return_cardinality: whether or not to return the cardinality, i.e. 1:1, 1:n, m:1, m:n
-        :type return_cardinality: bool
-        :param return_omagroup: whether or not to return the oma group nr in case both proteins
-                                belong to the same oma group. If not, NaNs will be returned.
-        :type return_omagroup: bool
-        :returns: array with hog induced pairwise orthologs between genome1 and genome2
-        """
-
-        def load_prot_dataframe(g):
-            genome = g if isinstance(g, Genome) else Genome(self, g)
-            prots = pandas.DataFrame(numpy.sort(self.main_isoforms(genome.uniprot_species_code), order="OmaHOG"))
-            col_keep = {"EntryNr", "OmaHOG", "OmaGroup", "CanonicalId"}
-            prots.drop(columns=set(prots.columns) - col_keep, inplace=True)
-            prots["Fam"] = prots["OmaHOG"].apply(lambda x: 0 if x == b"" else self.parse_hog_id(x))
-            prots.drop(prots[prots.Fam == 0].index, inplace=True)  # remove prots that don't belong to a hog
-            return prots
-
-        prots1 = load_prot_dataframe(g1)
-        prots2 = load_prot_dataframe(g2)
-        joined_fam = prots1.join(prots2.set_index("Fam"), on="Fam", how="inner", lsuffix="1", rsuffix="2")
-        joined_fam["HogID"] = joined_fam.apply(
-            lambda row: are_orthologous(row["OmaHOG1"], row["OmaHOG2"], return_group=True),
-            axis=1,
-        )
-        orthologs = joined_fam[joined_fam["HogID"] != False].copy()
-        orthologs["HogID"] = orthologs["HogID"].str.encode("ascii")
-        return_cols = ["EntryNr1", "EntryNr2", "HogID"]
-        if return_cardinality:
-            e1_cnts = orthologs["EntryNr1"].value_counts()
-            e2_cnts = orthologs["EntryNr2"].value_counts()
-            orthologs.loc[:, "RelType"] = orthologs.apply(
-                lambda r: (
-                    ("1" if e2_cnts[r.EntryNr2] == 1 else "m") + ":" + ("1" if e1_cnts[r.EntryNr1] == 1 else "n")
-                ).encode("ascii"),
-                axis=1,
-            )
-            return_cols.append("RelType")
-        if return_omagroup:
-            orthologs.loc[:, "OmaGroup"] = orthologs.apply(
-                lambda r: r.OmaGroup1 if r.OmaGroup1 == r.OmaGroup2 else numpy.nan,
-                axis=1,
-            )
-            return_cols.append("OmaGroup")
-        orthologs = orthologs[return_cols]
-        typ = orthologs.dtypes
-        return numpy.array([tuple(x) for x in orthologs.values], dtype=list(zip(typ.index, typ)))
-
     def neighbour_genes(self, entry_nr, window=1):
         """Returns neighbor genes around a query gene.
 
         This method returns a tuple containing a numpy recarray with
         gene entries located around the query gene, and an index
         pointing to the query gene. The genes are sorted according to
         their position on the chromosome.
@@ -924,42 +629,34 @@
         if window <= 0 or not isinstance(window, int):
             raise ValueError("windows parameters must be a positive integer value")
 
         dat = self.entry_by_entry_nr(entry_nr)
         target_chr = dat["Chromosome"]
         genome_range = self.id_mapper["OMA"].genome_range(entry_nr)
         f = 5
-        condvars = {
-            "enr_max": min(genome_range[1], entry_nr + f * window),
-            "enr_min": max(genome_range[0], entry_nr - f * window),
-            "chr": target_chr,
-        }
-        data = read_table_where(
-            self.db.root.Protein.Entries,
-            "(EntryNr >= enr_min) & (EntryNr <= enr_max) & "
-            "(Chromosome == chr) & "
+        data = self.db.root.Protein.Entries.read_where(
+            "(EntryNr >= {:d}) & (EntryNr <= {:d}) & "
+            "(Chromosome == {!r}) & "
             "((AltSpliceVariant == 0) |"
-            " (AltSpliceVariant == EntryNr))",
-            condvars=condvars,
+            " (AltSpliceVariant == EntryNr))".format(
+                max(genome_range[0], entry_nr - f * window),
+                min(genome_range[1], entry_nr + f * window),
+                target_chr,
+            )
         )
         data.sort(order=["LocusStart"])
         idx = int((data["EntryNr"] == entry_nr).nonzero()[0])
         res = data[max(0, idx - window) : idx + window + 1]
         idx = int((res["EntryNr"] == entry_nr).nonzero()[0])
         return res, idx
 
     def parse_hog_id(self, hog_id):
         hog_id = hog_id if isinstance(hog_id, bytes) else hog_id.encode("ascii")
         m = self._re_fam.match(hog_id)
         if m is not None:
-            rel = m.group("rel")
-            if rel is None:
-                rel = b""
-            if rel.decode() != self.release_char:
-                raise OutdatedHogId(hog_id)
             return int(m.group("fam"))
         else:
             raise ValueError("invalid hog id format")
 
     def hog_family(self, entry):
         entry = self.ensure_entry(entry)
         m = self._re_fam.match(entry["OmaHOG"])
@@ -994,81 +691,87 @@
             fam_idx = self.db.get_node("/HogLevel_fam_lookup")
             levels = hoglevel_tab.read(*fam_idx[fam_nr], field=field)
         except IndexError:
             # dummy read that returns empty list of same dtype
             levels = hoglevel_tab.read(0, 0, field=field)
         except tables.NoSuchNodeError:
             # fall back to index based search
-            levels = self.db.root.HogLevel.read_where("(Fam=={})".format(fam_nr), field=field)
-        logger.debug("retrieving levels for family {:d} took {:.7f} sec".format(fam_nr, time.time() - t0))
+            levels = self.db.root.HogLevel.read_where(
+                "(Fam=={})".format(fam_nr), field=field
+            )
+        logger.debug(
+            "retrieving levels for family {:d} took {:.7f} sec".format(
+                fam_nr, time.time() - t0
+            )
+        )
         return levels
 
-    def get_subhogs(self, hog_id, level=None, include_subids=False, include_leaf_levels=True):
+    def get_subhogs(
+        self, hog_id, level=None, include_subids=False, include_leaf_levels=True
+    ):
         """Get all the (sub)hogs for a given hog_id
 
         This method returns an generator of :class:`models.HOG` instances,
         that have a certain (sub)hog id. If `include_subids` is set to
         False (default), only the (sub)HOGs with exactly the query
         hog_id will be returned, i.e. a set of taxonomic ranges for
         which no duplication occurred in between for this HOG.
 
-        The method returns a generator of :class:`models.HOG` instances.
+        The method returns an generator of :class:`models.HOG` instances.
 
         :param (bytes, str) hog_id: the hog_id of interest
 
         :param str level: the root level, defaults to the root of the subhog
 
-        :param bool include_subids: whether to include suhogs
+        :param bool include_subids: whether or not to include suhogs
                                     that originated after a duplication
                                     in the query (sub)HOG. defaults to False
 
-        :param bool include_leaf_levels: whether to include the level
+        :param bool include_leaf_levels: whether or not to include the level
                                     of the extant species. defaults to True.
                                     Leaf levels have by definition only one
                                     member and are thus not of limited interest
                                     in most situations
 
-        :returns: generator of HOG instances
-        :rtype: :class:`models.HOG`
+        :returns generator of HOG instances
+        :rtype :class:`models.HOG`
 
         :see_also: :meth:`get_hog` that returns a single HOG instance
             for a specific level or the root level one for a specific HOG id.
         """
         if level is not None and level not in ("LUCA", b"LUCA"):
             try:
                 subtax = self.tax.get_subtaxonomy_rooted_at(level, collapse=False)
                 if not include_leaf_levels:
-                    idx = subtax.tax_table["NCBITaxonId"].searchsorted(
+                    internal_node_idx = subtax.tax_table["NCBITaxonId"].searchsorted(
                         subtax.tax_table["ParentTaxonId"], sorter=subtax.taxid_key
                     )
-                    internal_node_idx = set(
-                        pos
-                        for i, pos in enumerate(idx)
-                        if 0 <= pos < len(subtax.tax_table)
-                        and subtax.tax_table["NCBITaxonId"][pos] == subtax.tax_table["ParentTaxonId"][i]
-                    )
-                    internal_node_idx = numpy.fromiter(internal_node_idx, dtype="i4", count=len(internal_node_idx))
                     subtax.tax_table = subtax.tax_table[internal_node_idx]
                 children = set(n["Name"] for n in subtax.tax_table)
-                children.remove(level.encode("utf-8") if isinstance(level, str) else level)
+                children.remove(
+                    level.encode("utf-8") if isinstance(level, str) else level
+                )
             except KeyError as e:
-                raise ValueError(f"invalid level: {level}") from e
+                raise ValueError("invalid level: {}".format(level))
         elif not include_leaf_levels:
             children = self.tax.all_hog_levels
 
         if include_subids:
-            condvars = {v: k for v, k in zip(("hogid_low", "hogid_high"), self._hog_lex_range(hog_id))}
-            query = "(ID >= hogid_low) & (ID < hogid_high)"
+            query = "(ID >= {!r}) & (ID < {!r})".format(*self._hog_lex_range(hog_id))
         else:
-            query = "ID == hogid"
-            condvars = {"hogid": hog_id}
+            hog_id_ascii = (
+                hog_id if isinstance(hog_id, bytes) else hog_id.encode("ascii")
+            )
+            query = "ID == {!r}".format(hog_id_ascii)
 
-        for row in self.db.root.HogLevel.where(query, condvars=condvars):
+        for row in self.db.root.HogLevel.where(query):
             hog = row.fetch_all_fields()
-            if ((level is None or level in ("LUCA", b"LUCA")) and include_leaf_levels) or hog["Level"] in children:
+            if (
+                (level is None or level in ("LUCA", b"LUCA")) and include_leaf_levels
+            ) or hog["Level"] in children:
                 yield HOG(self, hog)
 
     def get_subhogids_at_level(self, fam_nr, level):
         """get all the hog ids within a given family at a given taxonomic
         level of interest.
 
         After a duplication in an ancestor lineage, there exists multiple
@@ -1077,19 +780,20 @@
 
         E.g. assume in family 1 (HOG:0000001) there has been a duplication
         between Eukaryota and Metazoa. this method would return for
         get_subhogids_at_level(1, 'Eukaryota') --> ['HOG:0000001']
         and for
         get_subhogids_at_level(1, 'Metazoa') --> ['HOG:0000001.1a', 'HOG:0000001.1b']
 
-        :note::
-        There is also the method :meth:`get_subhogs_at_level` which returns all
+        :note:
+        There is also the method :method:`get_subhogs_at_level` which returns all
         information stored in the HogLevel table, not only the HOG id.
 
-        :see_also:: :meth:`get_subhogs_at_level`
+        :see_also:
+        get_subhogs_at_level
 
         :param fam_nr: the numeric family id
         :param level: the taxonomic level of interest"""
         return self.get_subhogs_at_level(fam_nr, level, field="ID")
 
     def get_subhogs_at_level(self, fam_nr, level, field=None):
         """get all the hogs within a given family at a given taxonomic
@@ -1104,19 +808,16 @@
         the hogids for the chosen level, not all information on the HOGs.
 
         :param fam_nr: the numeric family id
         :param level: the taxonomic level of interest
         :param field: name of the column to be returned. If not set, all columns
             will be returned."""
         lev = level if isinstance(level, bytes) else level.encode("ascii")
-        return read_table_where(
-            self.db.root.HogLevel,
-            query="(Fam==fam) & (Level == lev)",
-            condvars={"fam": fam_nr, "lev": lev},
-            field=field,
+        return self.db.root.HogLevel.read_where(
+            "(Fam=={}) & (Level == {!r})".format(fam_nr, lev), field=field
         )
 
     def get_parent_hogs(self, hog_id, level=None):
         """return an array of parent (deeper) HOGs.
 
         The returned array is sorted from deepest to shallowest parent
         HOG of the query HOG. The query HOG can be either defined just
@@ -1132,42 +833,47 @@
         :param str level: optional level of reference HOG"""
         if isinstance(hog_id, str):
             hog_id = hog_id.encode("ascii")
         ref_hog = self.get_hog(hog_id, level=level)
         parent_pos = {b"LUCA": -1}
         if ref_hog["Level"] != b"LUCA":
             taxnode_of_level = self.tax.get_taxnode_from_name_or_taxid(ref_hog["Level"])
-            parent_taxnodes = self.tax.get_parent_taxa(taxnode_of_level[0]["NCBITaxonId"])
-            parent_pos.update({lev: pos for pos, lev in enumerate(parent_taxnodes["Name"][::-1])})
-        query = "(Fam == fam) & (ID <= hogid)"
-        condvars = {"fam": ref_hog["Fam"], "hogid": hog_id}
+            parent_taxnodes = self.tax.get_parent_taxa(
+                taxnode_of_level[0]["NCBITaxonId"]
+            )
+            parent_pos.update(
+                {lev: pos for pos, lev in enumerate(parent_taxnodes["Name"][::-1])}
+            )
+        query = "(Fam == {}) & (ID <= {!r})".format(ref_hog["Fam"], hog_id)
         parent_hogs = [] * len(parent_pos)
-        for row in self.db.root.HogLevel.where(query, condvars=condvars):
+        for row in self.db.root.HogLevel.where(query):
             hog = row.fetch_all_fields()
             if not hog_id.startswith(hog["ID"]):
                 continue
             if len(hog_id) > len(hog["ID"]) and hog_id[len(hog["ID"])] != ord("."):
                 continue
             if hog["Level"] in parent_pos:
                 parent_hogs.append(HOG(self, hog))
         parent_hogs.sort(key=lambda x: parent_pos[x._hog["Level"]])
         return parent_hogs
 
     def _members_of_hog_id(self, hog_id):
         hog_range = self._hog_lex_range(hog_id)
         it = self.db.root.Protein.Entries.where(
-            "(low <= OmaHOG) & (OmaHOG < high)",
-            condvars={k: v for k, v in zip(("low", "high"), hog_range)},
+            "({!r} <= OmaHOG) & (OmaHOG < {!r})".format(*hog_range)
         )
         # we need to filter them in case there are many (>26) paralog clusters,
         # in which case the hog_id need to be followed by a '.'
         hog_id_len = len(hog_range[0])
 
         def is_same_subhog(row):
-            return len(row["OmaHOG"]) == hog_id_len or chr(row["OmaHOG"][hog_id_len]) == "."
+            return (
+                len(row["OmaHOG"]) == hog_id_len
+                or chr(row["OmaHOG"][hog_id_len]) == "."
+            )
 
         for row in it:
             if is_same_subhog(row):
                 yield row.fetch_all_fields()
 
     def member_of_hog_id(self, hog_id, level=None):
         """return an array of protein entries which belong to a given hog_id.
@@ -1202,18 +908,20 @@
             return numpy.array([], dtype=self.db.root.Protein.Entries.dtype)
 
         members = numpy.fromiter(itertools.chain([first], it), dtype=first.dtype)
         if level is not None and level != "LUCA":
             keep = numpy.array(
                 [
                     level.encode("ascii")
-                    in self.tax.get_parent_taxa(self.id_mapper["OMA"].genome_of_entry_nr(enr)["NCBITaxonId"])["Name"]
+                    in self.tax.get_parent_taxa(
+                        self.id_mapper["OMA"].genome_of_entry_nr(enr)["NCBITaxonId"]
+                    )["Name"]
                     for enr in members["EntryNr"]
                 ],
-                dtype=bool,
+                dtype=numpy.bool,
             )
             members = members[keep]
         return members
 
     def iter_members_of_hog_id(self, hog_id, start=0, stop=None, step=1):
         """iterates over all proteins that belong to a specific hog_id.
 
@@ -1259,22 +967,22 @@
         The method will return a list of protein entries that are all
         member of the same hog with respect to the taxonomic range
         of interest.
 
         :param bytes hog_id: the query hog id
         :param str level: the taxonomic level of interest"""
         try:
-            hog = next(self.iter_hogs_at_level(hog_id, level))
+            hog = next(self.iter_hog_at_level(hog_id, level))
         except StopIteration:
             raise ValueError('Level "{0:s}" undefined for query gene'.format(level))
         # get the entries which have this hogid (or a sub-hog)
         members = self.member_of_hog_id(hog["ID"], level=level)
         return members
 
-    def iter_hogs_at_level(self, hog_id, level):
+    def iter_hog_at_level(self, hog_id, level):
         """yields the (sub- or parent-) hogs for a given level.
 
         This method yields the hogs as numpy.array instances that
         match the requested level exactly and match the hog_id as
         closely as possible:
 
         For a more general hog_id, the method returns all the subhogs
@@ -1290,105 +998,77 @@
         If the hog_id is known to match the level, the method
         :meth:`get_hog` can be used as it is a bit faster.
 
         :see_also: :meth:`get_subhogs_at_level`, :meth:`get_hog`
         """
         if isinstance(hog_id, str):
             hog_id = hog_id.encode("ascii")
-
-        condvars = {"fam": self.parse_hog_id(hog_id)}
-        query = "(Fam == fam)"
-        try:
-            anc_node = self._ancestral_node(level)
-            hog_tab = anc_node.Hogs
-        except DBConsistencyError:
-            hog_tab = self.db.root.HogLevel
-            query += " & (Level == lev)"
-            condvars["lev"] = level.encode("utf-8")
-
-        for hog in hog_tab.where(query, condvars=condvars):
+        query_fam = self.parse_hog_id(hog_id)
+        for hog in self.db.root.HogLevel.where(
+            "(Fam == {:d}) & (Level == {!r})".format(query_fam, level.encode("ascii"))
+        ):
             if hog_id.startswith(hog["ID"]):
                 if hog_id == hog["ID"] or chr(hog_id[len(hog["ID"])]) == ".":
                     yield hog.fetch_all_fields()
             elif hog["ID"].startswith(hog_id):
                 yield hog.fetch_all_fields()
 
-    def iter_hog_at_level(self, hog_id, level):
-        """deprecated method. use iter_hogs_at_level"""
-        yield from self.iter_hogs_at_level(hog_id=hog_id, level=level)
-
-    def get_hog(self, hog_id, level=None, field=None, tab=None):
+    def get_hog(self, hog_id, level=None, field=None):
         """Retrieve the one relevant HOG for a certain hog-id.
 
         If a level is provided, returns the (sub)hog at this level, otherwise
         it will return the deepest (sub)hog for that ID. Note that for this
         method the hog_id must match the expected subhog exactly. That means
         the method does not try to identify the correct hog_id for the requested
         level. In case the hog_id needs to be potentially adjusted given a level
         of interest, you should use :meth:`iter_hogs_at_level`.
 
         :see_also: :meth:`iter_hogs_at_level`, :meth:`get_subhogs_at_level`
 
-        :param hog_id: the query hog id
-        :type hog_id: (bytes, str)
+        :param (bytes,str) hog_id: the query hog id
         :param str level: the taxonomic level of interest, defaults to None
         :param field: the attribute of the HogLevel table to be returned. Defaults
                       to all attributes of the table.
         """
 
         if isinstance(hog_id, str):
             hog_id = hog_id.encode("ascii")
-        condvars = {"query_fam": self.parse_hog_id(hog_id), "hogid": hog_id}
-        query = "(Fam == query_fam) & (ID == hogid)"
-        if tab is None:
-            tab = self.db.get_node("/HogLevel")
-            if level is None:
-                query += " & (IsRoot == is_root)"
-                condvars["is_root"] = True
-            else:
-                query += " & (Level == lev)"
-                condvars["lev"] = level.encode("ascii")
+        query_fam = self.parse_hog_id(hog_id)
+        if level is None:
+            query = "(Fam == {}) & (ID == {!r}) & (IsRoot == True)".format(
+                query_fam, hog_id
+            )
+        else:
+            query = "(Fam == {:d}) & (ID == {!r}) & (Level == {!r})".format(
+                query_fam, hog_id, level.encode("ascii")
+            )
         try:
-            row = next(tab.where(query, condvars=condvars))
+            row = next(self.db.root.HogLevel.where(query))
             if field is not None:
                 if field == "_NROW":
                     return row.nrow
                 return row[field]
             return row.fetch_all_fields()
         except StopIteration:
             raise ValueError(
                 'HOG-ID/Level combination "{}/{:s}" unknown'.format(
-                    hog_id.decode(), level if level is not None else "Root"
+                    hog_id.decode(), level
                 )
             )
 
-    def count_hogs_at_level(self, level):
-        """returns the number of HOGs at the requested taxonomic level"""
-        try:
-            anc_node = self._ancestral_node(level)
-            return len(anc_node.Hogs)
-        except DBConsistencyError:
-            try:
-                taxid = self.taxid_from_level(level)
-                return len(self.db.get_node("/Hogs_per_Level/tax{}".format(taxid)))
-            except tables.NoSuchNodeError:
-                return len(self.get_all_hogs_at_level(level))
-
     def get_all_hogs_at_level(self, level, compare_with=None):
         """returns a :class:`numpy.array` instance with all hogs at the requested level"""
+        taxid = self.taxid_from_level(level)
         try:
-            anc_node = self._ancestral_node(level)
-            hog_data = anc_node.Hogs.read()
-        except DBConsistencyError:
-            try:
-                taxid = self.taxid_from_level(level)
-                hog_data = self.db.get_node("/Hogs_per_Level/tax{}".format(taxid)).read()
-            except tables.NoSuchNodeError:
-                logger.warning("Cannot load AncestralGenome nor Hogs_per_Level. extracting from main table. SLOW!")
-                hog_data = self.db.get_node("/HogLevel").read_where("Level == level")
+            hog_data = self.db.get_node("/Hogs_per_Level/tax{}".format(taxid)).read()
+        except tables.NoSuchNodeError:
+            logger.warning(
+                "Cannot load Hogs_per_Level. extracting from main table. SLOW!"
+            )
+            hog_data = self.db.get_node("/HogLevel").read_where("Level == level")
         if compare_with is None:
             return hog_data
         compare_hog = self.get_all_hogs_at_level(compare_with)
         diff = compare_levels(compare_hog, hog_data)
         return diff
 
     def get_roothog_keywords(self, fam) -> str:
@@ -1407,15 +1087,18 @@
             if fam <= 0 or fam > len(metadata):
                 raise KeyError("family {} does not exist".format(fam))
             fam_data = metadata[fam - 1]
             if fam_data["FamNr"] != fam:
                 logger.warning("/RootHOG/MetaData is not ordered")
                 fam_data = metadata.read_where("FamNr == {:d}".format(fam))
             keyword = (
-                buffer[fam_data["KeywordOffset"] : fam_data["KeywordOffset"] + fam_data["KeywordLength"]]
+                buffer[
+                    fam_data["KeywordOffset"] : fam_data["KeywordOffset"]
+                    + fam_data["KeywordLength"]
+                ]
                 .tobytes()
                 .decode()
             )
         return keyword
 
     def count_hog_members(self, hog_id, level=None):
         """Count the number of members in a (sub)hog.
@@ -1428,29 +1111,31 @@
         """
         return self.get_hog(hog_id, level, field="NrMemberGenes")
 
     def get_orthoxml(self, fam, augmented=False):
         """returns the orthoxml of a given toplevel HOG family
 
         :param fam: numeric id of requested toplevel hog
-        :param augmented: boolean flag to indicated whether to return
+        :param augmented: boolean flag to indicated whether or not to return
                           the augmented orthoxml or not. (defaults to not)"""
-        idx = read_table_where(self.db.root.OrthoXML.Index, "Fam == {:d}".format(fam))
+        idx = self.db.root.OrthoXML.Index.read_where("Fam == {:d}".format(fam))
         if len(idx) < 1:
             raise ValueError("cannot retrieve orthoxml for {}".format(fam))
         idx = idx[0]
         if augmented:
             buf = self.db.root.OrthoXML.BufferAugmented
             rng = slice(
                 idx["HogAugmentedBufferOffset"],
                 idx["HogAugmentedBufferOffset"] + idx["HogAugmentedBufferLength"],
             )
         else:
             buf = self.db.root.OrthoXML.Buffer
-            rng = slice(idx["HogBufferOffset"], idx["HogBufferOffset"] + idx["HogBufferLength"])
+            rng = slice(
+                idx["HogBufferOffset"], idx["HogBufferOffset"] + idx["HogBufferLength"]
+            )
         return buf[rng].tobytes()
 
     def get_cached_family_json(self, fam) -> str:
         """returns a json encoded list for protein infos of a family
 
         This is data contains the protein attributes needed for iHam
         visualization. For older databases that function might raise
@@ -1467,15 +1152,18 @@
         if fam < 0 or fam > len(metadata):
             raise KeyError("family {} does not exist".format(fam))
         fam_data = metadata[fam - 1]
         if fam_data["FamNr"] != fam:
             logger.warning("/RootHOG/MetaData is not ordered")
             fam_data = metadata.read_where("FamNr == {:d}".format(fam))
         json_str = (
-            json_buffer[fam_data["FamDataJsonOffset"] : fam_data["FamDataJsonOffset"] + fam_data["FamDataJsonLength"]]
+            json_buffer[
+                fam_data["FamDataJsonOffset"] : fam_data["FamDataJsonOffset"]
+                + fam_data["FamDataJsonLength"]
+            ]
             .tobytes()
             .decode()
         )
         return json_str
 
     def _hog_lex_range(self, hog):
         """return the lexographic range of a hog.
@@ -1487,89 +1175,46 @@
         query hog."""
         hog_str = hog.decode() if isinstance(hog, bytes) else hog
         return (
             hog_str.encode("ascii"),
             (hog_str[0:-1] + chr(1 + ord(hog_str[-1]))).encode("ascii"),
         )
 
-    def _ancestral_node(self, level):
-        taxid_of_level = self.taxid_from_level(level)
-        try:
-            return self.db.get_node("/AncestralGenomes/tax{}".format(taxid_of_level))
-        except tables.NoSuchNodeError as e:
-            logger.exception("cannot find ancestral genome node for taxid:{} ({})".format(taxid_of_level, level))
-            raise DBConsistencyError(f"Ancestral genome node not found: {taxid_of_level}")
-
-    def get_syntentic_hogs(self, level, hog_id, steps=2):
-        import warnings
-
-        warnings.warn(
-            f"{__name__} is deprecated. please use `get_syntenic_hogs` instead",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.get_syntenic_hogs(level, hog_id, steps=steps)
-
-    def get_syntenic_hogs(self, level, hog_id=None, evidence=None, steps=None):
+    def get_syntentic_hogs(self, hog_id, level, steps=2):
         """Returns a graph of the ancestral synteny
 
         This method returns a networkx.Graph object with HOGs as nodes
         and weighted edges representing ancestral synteny.
 
-        The evidence is a filter which can be one of `linearized`, `parsimonious` or `any`.
-        It defaults to `parsimonious`.
-
         :param str hog_id: the hog_id of the query HOG
         :param str level: the taxonomic level of the ancestral genome
-        :param str evidence: include only edges with evidences up to this level
-        :param int steps: number of breadth-first steps to take to get the local
+        :param int step: number of breadth-first steps to take to get the local
                          neighborhood of the query HOG.
         """
-        if self.db_schema_version < (3, 5):
-            logger.warning("ancestral synteny: ignoring evidence as outdated database")
-            return self._get_syntenic_hogs_obsolete_data(hog_id, level, steps=steps)
-        ancestral_node = self._ancestral_node(level)
-        if evidence is None:
-            evidence = "parsimonious"
-        try:
-            evidence_enum = ancestral_node.Synteny.get_enum("Evidence")
-            evidence = evidence_enum[evidence]
-        except KeyError:
-            raise ValueError(f"Invalid evidence value {evidence}")
-        edge_data = read_table_where(ancestral_node.Synteny, "Evidence <= {}".format(evidence))
-        edges = ((e[0], e[1], {"weight": int(e[2]), "evidence": evidence_enum(e[3])}) for e in edge_data)
-        if hog_id is not None:
-            hog_row = self.get_hog(hog_id, tab=ancestral_node.Hogs, field="_NROW")
-            hogs = ancestral_node.Hogs
-        else:
-            hog_row = None
-            hogs = ancestral_node.Hogs.read()
-        return _get_limited_synteny_graph(edges, hogs, hog_row, steps)
-
-    @outdated_database_warning()
-    def _get_syntenic_hogs_obsolete_data(self, hog_id, level, steps=2):
+        hl_tab = self.db.get_node("/HogLevel")
+        hog_row = self.get_hog(hog_id, level, "_NROW")
         taxid_of_level = self.taxid_from_level(level)
         try:
-            edge_data = self.db.get_node("/AncestralSynteny/tax{}".format(taxid_of_level)).read()
+            edge_data = self.db.get_node(
+                "/AncestralSynteny/tax{}".format(taxid_of_level)
+            ).read()
         except tables.NoSuchNodeError as e:
-            logger.exception("cannot find ancestral synteny data for taxid:{} ({})".format(taxid_of_level, level))
+            logger.exception(
+                "cannot find ancestral synteny data for taxid:{} ({})".format(
+                    taxid_of_level, level
+                )
+            )
             edge_data = []
-        edges = ((e[0], e[1], {"weight": e[2], "evidence": "any"}) for e in edge_data)
-
-        hl_tab = self.db.get_node("/HogLevel")
-        hogs = hl_tab
-        if hog_id is None:
-            all_hogs = {}
-            for row in hl_tab.where("Level == lev", {"lev": level.encode("utf-8")}):
-                all_hogs[row.nrow] = row.fetch_all_fields()
-            hog_row = None
-            hogs = all_hogs
-        else:
-            hog_row = self.get_hog(hog_id, level, "_NROW")
-        return _get_limited_synteny_graph(edges, hogs, hog_row, steps)
+        G = nx.Graph()
+        G.add_weighted_edges_from(edge_data)
+        neighbors = [hog_row] + [
+            v for u, v in nx.bfs_edges(G, source=hog_row, depth_limit=steps)
+        ]
+        S = G.subgraph(neighbors)
+        return nx.relabel_nodes(S, lambda x: hl_tab[x]["ID"].decode())
 
     def taxid_from_level(self, level):
         try:
             taxnodes = self.tax.get_taxnode_from_name_or_taxid(level)
             taxid_of_level = int(taxnodes[0]["NCBITaxonId"])
         except KeyError:
             if level == b"LUCA" or level == "LUCA":
@@ -1584,202 +1229,120 @@
         This method returns just the adjacent HOGs from the ancestral
         synteny graph of that level
 
         :param hog_id: the reference HOG.
         :param level: the taxonomic level of the ancestral genome
         :returns dict: hog_id -> edge_weight of the neighboring hogs
         """
-        G = self.get_syntentic_hogs(hog_id=hog_id, level=level, steps=1)
+        G = self.get_syntentic_hogs(hog_id, level, 1)
         try:
             neighbors = {nbr: edg["weight"] for nbr, edg in G[hog_id]}
         except KeyError:
             neighbors = {}
         return neighbors
 
-    def get_ancestral_gene_ontology_annotations(
-        self,
-        level: Union[str, bytes, int],
-        hog_id: Union[str, bytes, None] = None,
-        as_dataframe: bool = False,
-        as_gaf: bool = False,
-    ):
-        """
-        Retrieve the ancestral gene ontology annotations for a hog / all hogs at a taxonomic level
-
-        The method returns the gene ontology annotations stored in the database
-        for a given hog_id at a given taxonomic level or for all the hogs at the given
-        taxonomic level.
-
-        By default, the result are returned as numpy arrays of type
-        :class:`tablefmt.AncestralGeneOntologyTable`, augemtned with a HogID column.
-        If `as_dataframe` is set to true, the result will be a pandas dataframe,
-        and if `as_gaf` is set to true, a gaf formatted text file with the
-        annotations is returned.
-
-        :param level: the taxonomic level for the ancestral data
-        :type level: str | bytes | int
-        :param hog_id: the hog_id for which the annotations should be retrieved.
-                       if not specified, information for all hogs will be used.
-        :type hog_id: str | bytes
-        :param as_dataframe: return as a pandas dataframe.
-        :type as_dataframe: bool
-        :param as_gaf: return annotations in GAF format
-        :type as_gaf: bool
-        """
-        ancestral_node = self._ancestral_node(level)
-        if hog_id is not None:
-            hog = self.get_hog(hog_id, tab=ancestral_node.Hogs)
-            query = f"(HogRow == {hog['IdxPerLevelTable']})"
-            annots = read_table_where(ancestral_node.GeneOntology, query)
-            hog_ids = {hog["IdxPerLevelTable"]: hog["ID"]}
-        else:
-            annots = ancestral_node.GeneOntology.read()
-            hog_ids = ancestral_node.Hogs.read(field="ID")
-        annots = numpy.lib.recfunctions.append_fields(
-            annots,
-            names="HogID",
-            data=[hog_ids[row] for row in annots["HogRow"]],
-            usemask=False,
-        )
-        if not as_dataframe and not as_gaf:
-            return annots
-        # early return if no annotations available
-        if len(annots) == 0:
-            return "!gaf-version: {}\n".format(GAF_VERSION) if as_gaf else None
-
-        df = pd.DataFrame(annots)
-        df["DB"] = "OMA"
-        df["DB_Object_ID"] = df["HogID"]
-        # 3R DB Object Symbol
-        df["DB_Object_Symbol"] = df["DB_Object_ID"]
-        # 4O Qualifier
-        df["Qualifier"] = ""
-        # 5R GO ID
-        df["GO_ID"] = df["TermNr"].apply(lambda t: "GO:{:07d}".format(t))
-        # 6R DB:Reference
-        df["DB:Reference"] = "OMA HogProp"
-        # 7R Evidence code
-        df["Evidence"] = "IEA"
-        # 8O With (or) From
-        df["With"] = ""
-        # 9R Aspect
-        df["Aspect"] = df["GO_ID"].apply(lambda t: GOAspect.to_char(self.gene_ontology.term_by_id(t).aspect))
-        # 10O DB Object Name
-        df["DB_Object_Name"] = ""
-        # 11O DB Object Synonym (|Synonym)
-        df["Synonym"] = ""
-        # 12R DB Object Type
-        df["DB_Object_Type"] = "ancestral protein"
-        # 13R Taxon (|taxon)
-        df["Taxon_ID"] = level
-        # 14R Date
-        df["Date"] = self.get_conversion_date().strftime("%Y%m%d")
-        # 15R Assigned by
-        df["Assigned_By"] = df["DB"]
-        # 16O Annotation Extension
-        df["Annotation_Extension"] = ""
-        # 17O Gene Product Form ID
-        df["Gene_Product_Form_ID"] = ""
-
-        df = df[GOA.GAF20FIELDS]
-        return (
-            df
-            if not as_gaf
-            else (
-                "!gaf-version: {}\n".format(GAF_VERSION)
-                + "\n".join(df.apply(lambda e: "\t".join(map(str, e)), axis=1))
-                + "\n"
-            )
-        )
-
     def oma_group_members(self, group_id):
         """get the member entries of an oma group.
 
         This method returns a numpy array of protein entries that form
         an oma group. If the group id is invalid (not positive
         integer value or a valid Fingerprint), an `InvalidId` Exception
         is raised.
 
         :param group_id: numeric oma group id or Fingerprint"""
         group_nr = self.resolve_oma_group(group_id)
-        pe_tab = self.db.get_node("/Protein/Entries")
-        return read_table_where(pe_tab, "OmaGroup == {:d}".format(group_nr))
+        members = self.db.root.Protein.Entries.read_where(
+            "OmaGroup=={:d}".format(group_nr)
+        )
+        return members
 
     def resolve_oma_group(self, group_id):
-        if isinstance(group_id, int) and 0 < group_id <= self._nr_oma_groups:
+        if isinstance(group_id, int) and 0 < group_id <= self.get_nr_oma_groups():
             return group_id
         elif isinstance(group_id, numpy.integer):
             return self.resolve_oma_group(int(group_id))
         elif isinstance(group_id, (bytes, str)):
             if group_id.isdigit():
                 return self.resolve_oma_group(int(group_id))
             if isinstance(group_id, str):
                 group_id = group_id.encode("utf-8")
             if group_id == b"n/a":
                 raise InvalidId("Invalid ID (n/a) for an OMA Group")
             if not self.seq_search.contains_only_valid_chars(group_id):
-                raise InvalidId("Invalid ID: non-amino-accids characters in Fingerprint or sequence pattern")
+                raise InvalidId(
+                    "Invalid ID: non-amino-accids characters in Fingerprint or sequence pattern"
+                )
             if len(group_id) == 7:
                 # most likely a fingerprint. let's check that first
                 group_meta_tab = self.db.get_node("/OmaGroups/MetaData")
                 try:
-                    e = next(group_meta_tab.where("(Fingerprint == og)", {"og": group_id}))
+                    e = next(
+                        group_meta_tab.where("(Fingerprint == {!r})".format(group_id))
+                    )
                     return int(e["GroupNr"])
                 except StopIteration:
                     pass
             # search in suffix array
-            entry_nrs = self.seq_search.exact_search(group_id.decode(), only_full_length=False)
+            entry_nrs = self.seq_search.exact_search(
+                group_id.decode(), only_full_length=False
+            )
             if len(entry_nrs) == 0:
                 raise InvalidId("No sequence contains search pattern")
             group_nrs = {self.entry_by_entry_nr(nr)["OmaGroup"] for nr in entry_nrs}
             group_nrs.discard(0)
             if len(group_nrs) == 1:
                 return int(group_nrs.pop())
             elif len(group_nrs) == 0:
-                raise InvalidId("Sequence with pattern '{}' does not belong to any group".format(group_id.decode()))
+                raise InvalidId(
+                    "Sequence with pattern '{}' does not belong to any group".format(
+                        group_id.decode()
+                    )
+                )
             else:
-                raise AmbiguousID("sequence pattern matches several oma groups", candidates=group_nrs)
-        raise InvalidId("Invalid type to determine OMA Group: {} (type: {})".format(group_id, type(group_id)))
+                raise AmbiguousID(
+                    "sequence pattern matches several oma groups", candidates=group_nrs
+                )
+        raise InvalidId(
+            "Invalid type to determine OMA Group: {} (type: {})".format(
+                group_id, type(group_id)
+            )
+        )
 
     def oma_group_metadata(self, group_nr):
-        """get the metadata associated with an OMA Group
+        """get the meta data associated with a OMA Group
 
-        The metadata contains the fingerprint and the keywords inferred for this group.
-        The method returns this information as a dictionary. The parameter must be
+        The meta data contains the fingerprint and the keywords infered for this group.
+        The method retuns this information as a dictionary. The parameter must be
         the numeric oma group nr.
 
         :param int group_nr: a numeric oma group id."""
         if not isinstance(group_nr, (int, numpy.integer)) or group_nr < 0:
-            raise InvalidId("Invalid group nr: {} (type: {})".format(group_nr, type(group_nr)))
+            raise InvalidId(
+                "Invalid group nr: {} (type: {})".format(group_nr, type(group_nr))
+            )
         meta_tab = self.db.get_node("/OmaGroups/MetaData")
         try:
             e = next(meta_tab.where("GroupNr == {:d}".format(group_nr)))
             kw_buf = self.db.get_node("/OmaGroups/KeywordBuffer")
-            try:
-                grp_size = int(e["NrMembers"])
-            except KeyError:
-                # fallback if not stored in DB yet
-                grp_size = -1
-
             res = {
                 "fingerprint": e["Fingerprint"].decode(),
                 "group_nr": int(e["GroupNr"]),
-                "keywords": kw_buf[e["KeywordOffset"] : e["KeywordOffset"] + e["KeywordLength"]].tobytes().decode(),
-                "size": grp_size,
+                "keywords": kw_buf[
+                    e["KeywordOffset"] : e["KeywordOffset"] + e["KeywordLength"]
+                ]
+                .tobytes()
+                .decode(),
+                "size": int(e["NrMembers"]) if "NrMembers" in e else -1,
             }
             return res
         except StopIteration:
             raise InvalidId("invalid group nr")
 
     def get_nr_oma_groups(self):
         """returns the number of OMA Groups in the database"""
-        return self._nr_oma_groups
-
-    @LazyProperty
-    def _nr_oma_groups(self):
         tab = self.db.get_node("/Protein/Entries")
         try:
             idx = tab.colindexes["OmaGroup"][-1]
             return int(tab[idx]["OmaGroup"])
         except KeyError:
             hist = self.group_size_histogram("oma")
             return int(hist["Count"].sum())
@@ -1814,53 +1377,65 @@
 
     def get_sequence(self, entry):
         """get the protein sequence of a given entry as a string
 
         :param entry: the entry or entry_nr for which the sequence is requested"""
         entry = self.ensure_entry(entry)
         seqArr = self.db.get_node("/Protein/SequenceBuffer")
-        seq = seqArr[entry["SeqBufferOffset"] : entry["SeqBufferOffset"] + entry["SeqBufferLength"] - 1]
+        seq = seqArr[
+            entry["SeqBufferOffset"] : entry["SeqBufferOffset"]
+            + entry["SeqBufferLength"]
+            - 1
+        ]
         return seq.tobytes()
 
     def get_cdna(self, entry):
         """get the protein sequence of a given entry as a string"""
         entry = self.ensure_entry(entry)
         seqArr = self.db.get_node("/Protein/CDNABuffer")
-        seq = seqArr[entry["CDNABufferOffset"] : entry["CDNABufferOffset"] + entry["CDNABufferLength"] - 1]
+        seq = seqArr[
+            entry["CDNABufferOffset"] : entry["CDNABufferOffset"]
+            + entry["CDNABufferLength"]
+            - 1
+        ]
         return seq.tobytes()
 
     def get_description(self, entry):
         entry = self.ensure_entry(entry)
         descArr = self.db.get_node("/Protein/DescriptionBuffer")
-        desc = descArr[entry["DescriptionOffset"] : entry["DescriptionOffset"] + entry["DescriptionLength"]]
+        desc = descArr[
+            entry["DescriptionOffset"] : entry["DescriptionOffset"]
+            + entry["DescriptionLength"]
+        ]
         return desc.tobytes()
 
     def get_ec_annotations(self, entry_nr):
         ec_tab = self.db.get_node("/Annotations/EC")
-        return [row["ECacc"].decode() for row in ec_tab.where("EntryNr == {}".format(entry_nr))]
+        return [
+            row["ECacc"].decode()
+            for row in ec_tab.where("EntryNr == {}".format(entry_nr))
+        ]
 
     def get_release_name(self):
         return str(self.db.get_node_attr("/", "oma_version"))
 
-    @LazyProperty
-    def release_char(self):
-        try:
-            release = self.db.get_node_attr("/", "oma_release_char")
-        except AttributeError:
-            release = ""
-        return release
-
     def get_exons(self, entry_nr):
-        genome = self.id_mapper["OMA"].genome_of_entry_nr(entry_nr)["UniProtSpeciesCode"].decode()
+        genome = (
+            self.id_mapper["OMA"]
+            .genome_of_entry_nr(entry_nr)["UniProtSpeciesCode"]
+            .decode()
+        )
         locus_tab = self.db.get_node("/Protein/Locus/{}".format(genome))
-        return read_table_where(locus_tab, "EntryNr == {}".format(entry_nr))
+        return locus_tab.read_where("EntryNr == {}".format(entry_nr))
 
     def get_domains(self, entry_nr):
         try:
-            return read_table_where(self.db.root.Annotations.Domains, "EntryNr == {:d}".format(entry_nr))
+            return self.db.root.Annotations.Domains.read_where(
+                "EntryNr == {:d}".format(entry_nr)
+            )
         except ValueError as e:
             raise InvalidId("require a numeric entry id, got {}".format(entry_nr))
 
     def get_representative_entry_of_hog(self, fam):
         """Get the information of the representative entry for a given family (roothog).
 
         For each family we select a represenative entry that has the most prevalent
@@ -1903,22 +1478,26 @@
                 sim_fams[hog_with_domain["Offset"]][d] += 1
 
         if len(sim_fams) == 0:
             return fam_row, None
 
         # Now get similar families and order them by similarity
         sim_fams_df = pd.DataFrame(domprev_tab[list(sim_fams.keys())])
-        sim_fams_df["sim"] = list(map(lambda i: sum((sim_fams[i] & fam_da).values()), sim_fams.keys()))
+        sim_fams_df["sim"] = list(
+            map(lambda i: sum((sim_fams[i] & fam_da).values()), sim_fams.keys())
+        )
 
         # Sort by similarity & family size
         sim_fams_df.sort_values(["sim", "FamSize"], inplace=True, ascending=False)
         sim_fams_df.reset_index(drop=True, inplace=True)
 
         # Prevalence
-        sim_fams_df["Prev"] = 100.0 * (sim_fams_df["PrevCount"] / sim_fams_df["FamSize"])
+        sim_fams_df["Prev"] = 100.0 * (
+            sim_fams_df["PrevCount"] / sim_fams_df["FamSize"]
+        )
 
         return fam_row, sim_fams_df
 
     def get_families_with_similar_hog_profile(self, fam, max_nr_similar_fams=50):
         """Retrieves the family nr of families that have a similar
         presence/loss/gain pattern of genes, i.e. potentially
         co-evolving families.
@@ -1938,196 +1517,62 @@
                 # create and cache Profiler instance. Not done in constructor
                 # as otherwise building of profiles fails.
                 self.hog_profiler = Profiler(self)
             return self.hog_profiler.query(fam, k=max_nr_similar_fams)
         except KeyError:
             return None
 
-    def entrynrs_with_ec_annotation(
-        self,
-        ec: AnyStr,
-        limit: Optional[int] = None,
-        entrynr_filter: Union[Tuple[int, int], Set[int], None] = None,
-    ) -> Set[int]:
-        """Search for protein entries with a certain EC annotation.
-
-        The option arguments limit and entrynr_filter can be used to
-        limit the amount of entries that are returned and to speed
-        up the search time.
-
-        :param ec: EC identifier to be searched
-        :type ec: (str, bytes)
-        :param limit: maximum number of entries to be returned.
-        :type limit: int
-        :param entrynr_filter: range (low, high) or set of entry numbers that should be considered
-        :type entrynr_filter: Union[Tuple[int, int], Set[int], None]
-        :return: Entry numbers of proteins that contain the domain id.
-        :rtype: set[int]
-        """
+    def entrynrs_with_ec_annotation(self, ec):
         if isinstance(ec, str):
             ec = ec.encode("utf-8")
-        query = "(ECacc == ec)"
         ectab = self.get_hdf5_handle().get_node("/Annotations/EC")
-        return self._fetch_entry_nrs(
-            self._iter_rows_with_entrynr_filter(ectab, query, condvars={"ec", ec}, entrynr_filter=entrynr_filter),
-            limit,
-        )
-
-    def count_ec_annotations(self, ec: AnyStr) -> int:
-        """
-        Count the number of EC annoations of a certain term in the database.
-
-        :param ec: EC identifier, e.g. "GO:0003676", 50, b"GO:0003674"
-        :type ec: (str, bytes)
-        :return number of annotations
-        :rtype int
-        """
-        if isinstance(ec, str):
-            ec = ec.encode("utf-8")
-        ecTab = self.get_hdf5_handle().get_node("/Annotations/EC")
-        return count_rows_of_index_column_with_value(ecTab, "ECacc", ec)
-
-    def entrynrs_with_domain_id(
-        self,
-        domain_id: AnyStr,
-        limit: Optional[int] = None,
-        entrynr_filter: Union[Tuple[int, int], Set[int], None] = None,
-    ) -> Set[int]:
-        """Search for protein entries with a certain domain_id.
-
-        The option arguments limit and entrynr_filter can be used to
-        limit the amount of entries that are returned and to speed
-        up the search time.
-
-        :param domain_id: domain identifier to be searched
-        :type domain_id: (str, bytes)
-        :param limit: maximum number of entries to be returned.
-        :type limit: int
-        :param entrynr_filter: range (low, high) or set of entry numbers that should be considered
-        :type entrynr_filter:  Union[Tuple[int, int], Set[int], None]
-        :return: Entry numbers of proteins that contain the domain id.
-        :rtype: set[int]"""
-
-        vars = {"dom": domain_id.encode("utf-8") if isinstance(domain_id, str) else domain_id}
-        query = "(DomainId == dom)"
-        domtab = self.get_hdf5_handle().get_node("/Annotations/Domains")
-        return self._fetch_entry_nrs(
-            self._iter_rows_with_entrynr_filter(domtab, query, vars, entrynr_filter),
-            limit,
-        )
-
-    def count_domain_id_annotations(self, domain_id: AnyStr) -> int:
-        """
-        Count the number of Domain annoations of a certain id in the database.
+        entrynrs = {row["EntryNr"] for row in ectab.where("(ECacc == {!r})".format(ec))}
+        return entrynrs
 
-        :param domain_id: Domain identifier, e.g. "2.60.10.60"
-        :type domain_id: (str, bytes)
-        :return number of annotations
-        :rtype int
-        """
+    def entrynrs_with_domain_id(self, domain_id):
         if isinstance(domain_id, str):
             domain_id = domain_id.encode("utf-8")
-        ecTab = self.get_hdf5_handle().get_node("/Annotations/Domains")
-        return count_rows_of_index_column_with_value(ecTab, "DomainId", domain_id)
+        domtab = self.get_hdf5_handle().get_node("/Annotations/Domains")
+        entrynrs = {
+            row["EntryNr"] for row in domtab.where("DomainId =={!r}".format(domain_id))
+        }
+        return entrynrs
 
-    def entrynrs_with_go_annotation(
-        self,
-        term: Union[AnyStr, int],
-        evidence: Optional[AnyStr] = None,
-        limit: Optional[int] = None,
-        entrynr_filter: Union[Tuple[int, int], Set[int], None] = None,
-    ) -> Set[int]:
+    def entrynrs_with_go_annotation(self, term, evidence=None):
         """Retrieve protein entry numbers that have a certain GO annotation term
 
-        :param term: numeric term or GO-identifier
-        :type term: (int, str, bytes)
-        :param evidence: evidence code which is required
-        :type evidence: (str, bytes)
-        :param limit: maximum number of entries to be returned.
-        :type limit: int
-        :param entrynr_filter: range (low, high) or set of entry numbers that should be considered
-        :type entrynr_filter: Union[Tuple[int, int], Set[int], None]
-        :return: Entry numbers of proteins that contain the domain id.
-        :rtype: set[int]
-        """
-        if (isinstance(term, str) and term.startswith("GO:")) or (isinstance(term, bytes) and term.startswith(b"GO:")):
+        :param term: numeric term or GO-identifier"""
+        if (isinstance(term, str) and term.startswith("GO:")) or (
+            isinstance(term, bytes) and term.startswith(b"GO:")
+        ):
             term = term[3:]
 
         try:
-            vars = {"term_nr": int(term)}
+            term = int(term)
         except ValueError:
             raise InvalidId("Invalid GO ID: {}".format(term))
 
         gotab = self.get_hdf5_handle().get_node("/Annotations/GeneOntology")
-        query = "(TermNr == term_nr)"
+        query = "(TermNr == {})".format(term)
         if evidence is not None:
-            vars["ev"] = evidence.encode("utf-8")
-            query += " & (Evidence == ev)"
-
-        return self._fetch_entry_nrs(
-            self._iter_rows_with_entrynr_filter(gotab, query, condvars=vars, entrynr_filter=entrynr_filter),
-            limit,
-        )
-
-    def count_go_annotations(self, term: Union[AnyStr, int]) -> int:
-        """
-        Count the number of GeneOntology annoations of a certain term in the database.
-        Annotations are counted multiple time if several evidences or references are
-        recorded.
-
-        :param term: numeric term or GO-identifier, e.g. "GO:0003676", 50, b"GO:0003674"
-        :type term: (int, str, bytes)
-        :return number of annotations
-        :rtype int
-        """
-        if (isinstance(term, str) and term.startswith("GO:")) or (isinstance(term, bytes) and term.startswith(b"GO:")):
-            term = term[3:]
-
-        try:
-            term = int(term)
-        except ValueError:
-            raise InvalidId("Invalid GO ID: {}".format(term))
-        gotab = self.get_hdf5_handle().get_node("/Annotations/GeneOntology")
-        return count_rows_of_index_column_with_value(gotab, "TermNr", term)
-
-    def _fetch_entry_nrs(self, row_iter, limit: Optional[int] = None) -> Set[int]:
-        entrynrs = set([])
-        for row in row_iter:
-            entrynrs.add(int(row["EntryNr"]))
-            if limit is not None and len(entrynrs) >= limit:
-                break
+            query += "& (Evidence == {!r})".format(evidence.encode("utf-8"))
+        entrynrs = {row["EntryNr"] for row in gotab.where(query)}
         return entrynrs
 
-    def _iter_rows_with_entrynr_filter(
-        self,
-        tab: tables.Table,
-        query_stub: str,
-        condvars: Optional[Mapping] = None,
-        entrynr_filter: Union[Tuple[int, int], Set[int], None] = None,
-    ) -> Generator:
-        query = query_stub
-        cond = lambda row: True
-        if entrynr_filter is not None:
-            rng = min(entrynr_filter), max(entrynr_filter)
-            query += " & (EntryNr >= {}) & (EntryNr <= {})".format(*rng)
-            if isinstance(entrynr_filter, set):
-                cond = lambda row: row["EntryNr"] in entrynr_filter
-        for row in tab.where(query, condvars=condvars):
-            if cond(row):
-                yield row
-
-    def get_gene_ontology_annotations(self, entry_nr, stop=None, as_dataframe=False, as_gaf=False):
+    def get_gene_ontology_annotations(
+        self, entry_nr, stop=None, as_dataframe=False, as_gaf=False
+    ):
         """Retrieve the gene ontology annotations for an entry or entry_range
 
         The method returns the gene ontology annotations stored in the database
         for a given entry (if `stop` parameter is not provided) or for all the
         entries between [entry_nr, stop). Like in slices, the stop entry_nr is
-        not inclusive, whereas the entry_nr - the start of the slice - is.
+        not inclusive, where as the entry_nr - the start of the slice - is.
 
-        By default, the result are returned as numpy arrays of type
+        By default the result are returned as numpy arrays of type
         :class:`tablefmt.GeneOntologyTable`. If as_dataframe is set to true, the
         result will be a pandas dataframe, and if as_gaf is set to true, a gaf
         formatted text file with the annotations is returned.
 
         :param int entry_nr: numeric protein entry
         """
 
@@ -2140,17 +1585,19 @@
                 return False
 
         try:
             if stop is None:
                 query = "EntryNr == {:d}".format(entry_nr)
             else:
                 if not isinstance(stop, (numpy.integer, int)) or stop < entry_nr:
-                    raise TypeError("stop argument needs to be a entry number that is larger than 'entry_nr'")
+                    raise TypeError(
+                        "stop argument needs to be a entry number that is larger than 'entry_nr'"
+                    )
                 query = "(EntryNr >= {:d}) & (EntryNr < {:d})".format(entry_nr, stop)
-            annots = read_table_where(self.db.root.Annotations.GeneOntology, query)
+            annots = self.db.root.Annotations.GeneOntology.read_where(query)
 
             # for test database we also have some obsolete terms. we need to filter those
             if len(annots) > 0:
                 not_obsolete = numpy.vectorize(filter_obsolete_terms)(annots["TermNr"])
                 annots = annots[not_obsolete]
         except ValueError as e:
             raise InvalidId("require a numeric entry id, got {}".format(entry_nr))
@@ -2176,24 +1623,28 @@
         # 6R DB:Reference
         df["DB:Reference"] = df["Reference"].apply(lambda x: x.decode("ascii"))
         # 7R Evidence code
         df["Evidence"] = df["Evidence"].apply(lambda x: x.decode("ascii"))
         # 8O With (or) From
         df["With"] = ""
         # 9R Aspect
-        df["Aspect"] = df["GO_ID"].apply(lambda t: GOAspect.to_char(self.gene_ontology.term_by_id(t).aspect))
+        df["Aspect"] = df["GO_ID"].apply(
+            lambda t: GOAspect.to_char(self.gene_ontology.term_by_id(t).aspect)
+        )
         # 10O DB Object Name
         df["DB_Object_Name"] = ""
         # 11O DB Object Synonym (|Synonym)
         df["Synonym"] = ""
         # 12R DB Object Type
         df["DB_Object_Type"] = "protein"
         # 13R Taxon (|taxon)
         df["Taxon_ID"] = df["EntryNr"].apply(
-            lambda e: "taxon:{:d}".format(self.id_mapper["Oma"].genome_of_entry_nr(e)["NCBITaxonId"])
+            lambda e: "taxon:{:d}".format(
+                self.id_mapper["Oma"].genome_of_entry_nr(e)["NCBITaxonId"]
+            )
         )
         # 14R Date
         df["Date"] = self.get_conversion_date().strftime("%Y%m%d")
         # 15R Assigned by - TODO: FIX FOR NON OMA!!!
         df["Assigned_By"] = df["DB"]
         # 16O Annotation Extension
         df["Annotation_Extension"] = ""
@@ -2233,15 +1684,17 @@
         i = 0
         for member in tqdm(
             hog_members,
             disable=len(hog_members) < 500,
             desc="GO-loading {}".format(hog_id),
         ):
             curr_prot_entrynr = member["EntryNr"]
-            annos = self.get_gene_ontology_annotations(entry_nr=curr_prot_entrynr, as_dataframe=False)
+            annos = self.get_gene_ontology_annotations(
+                entry_nr=curr_prot_entrynr, as_dataframe=False
+            )
 
             if len(annos) == 0:
                 go_annots_not_fetched.append(curr_prot_entrynr)
             else:
                 idx_map[i] = curr_prot_entrynr
                 h = MinHash()
                 for d in annos["TermNr"].astype("unicode"):
@@ -2254,15 +1707,17 @@
             dist_matrix = numpy.zeros((n, n))
             for p1, p2 in tqdm(
                 itertools.combinations(range(n), 2),
                 disable=n < 50,
                 total=n * (n - 1) / 2,
                 desc="sim-matrix {}".format(hog_id),
             ):
-                score = minhash_signatures[idx_map[p1]].jaccard(minhash_signatures[idx_map[p2]])
+                score = minhash_signatures[idx_map[p1]].jaccard(
+                    minhash_signatures[idx_map[p2]]
+                )
                 dist_matrix[p1][p2] = 1 - score
                 dist_matrix[p2][p1] = 1 - score
 
             if dist_matrix.max() == 0:
                 # all values the same
                 positions = numpy.zeros((n, 1))
             else:
@@ -2288,28 +1743,38 @@
         genome = genome if isinstance(genome, bytes) else genome.encode("ascii")
         try:
             self.genome_idx = numpy.where(self.genomes == genome)[0][0]
         except IndexError:
             raise UnknownSpecies("UniProtSpeciesCode '{}' not known".format(genome))
 
     def get_most_similar_species(self, limit=None, group_type="OMAGroup", reverse=True):
-        overlap_groups = self.h5.get_node("/Summary/shared_{}".format(group_type.lower()))[self.genome_idx, :]
+        overlap_groups = self.h5.get_node(
+            "/Summary/shared_{}".format(group_type.lower())
+        )[self.genome_idx, :]
         key = numpy.argsort(overlap_groups)
         if reverse:
             limit = limit if limit is None else -limit - 1
             s = slice(None, limit, -1)
         else:
             s = slice(0, limit, None)
-        return [(self.genomes[k].decode(), int(overlap_groups[k])) for k in key[s] if k != self.genome_idx]
+        return [
+            (self.genomes[k].decode(), int(overlap_groups[k]))
+            for k in key[s]
+            if k != self.genome_idx
+        ]
 
     def get_least_similar_species(self, **kwargs):
         return self.get_most_similar_species(reverse=False, **kwargs)
 
     def get_nr_genes_in_group(self, group_type="OMAGroup"):
-        return int(self.h5.get_node("/Summary/prots_in_{}".format(group_type.lower()))[self.genome_idx])
+        return int(
+            self.h5.get_node("/Summary/prots_in_{}".format(group_type.lower()))[
+                self.genome_idx
+            ]
+        )
 
 
 class SequenceSearch(object):
     """
     Contains all the methods for searching the sequence
 
     TODO: implement taxonomic filtering.
@@ -2337,22 +1802,24 @@
             self.seq_idx = self.db_idx.root.Protein.SequenceIndex
             if isinstance(self.seq_idx, tables.link.ExternalLink):
                 self.seq_idx = self.seq_idx()
             self.kmer_lookup = self.db_idx.root.Protein.KmerLookup
             if isinstance(self.kmer_lookup, tables.link.ExternalLink):
                 self.kmer_lookup = self.kmer_lookup()
         except (AttributeError, OSError) as e:
-            raise DBConsistencyError("Suffix index for protein sequences is not available: " + str(e))
+            raise DBConsistencyError(
+                "Suffix index for protein sequences is not available: " + str(e)
+            )
         self.seq_buff = self.db.root.Protein.SequenceBuffer
         self.n_entries = len(self.db.root.Protein.Entries)
 
         # Kmer lookup arrays / kmer setup
         self.k = self.kmer_lookup._f_getattr("k")
         self.encoder = KmerEncoder(self.k)
-        logger.info("KmerLookup of size k=%s loaded", self.k)
+        logger.info("KmerLookup of size k={} loaded".format(self.k))
         self.multienv_align = None
 
     def get_entry_length(self, ii):
         """Get length of a particular entry."""
         return self.db.root.Protein.Entries[ii - 1]["SeqBufferLength"] - 1
 
     @LazyProperty
@@ -2384,21 +1851,17 @@
 
     def _sanitise_seq(self, seq):
         """
         Sanitise a string protein sequence. Deletes "invalid" characters.
         TODO: add functionality for biopython sequence / skbio sequence.
         """
         assert type(seq) == str
-        return "".join(filter(lambda c: c in self.PROTEIN_CHARS, seq.upper())).encode("ascii")
-
-    def _tax_filter_range(self, en, rng):
-        return rng[0] <= en <= rng[1]
-
-    def _tax_filter_set(self, en, taxset):
-        return en in taxset
+        return "".join(filter(lambda c: c in self.PROTEIN_CHARS, seq.upper())).encode(
+            "ascii"
+        )
 
     def search(
         self,
         seq,
         n=None,
         coverage=None,
         is_sanitised=None,
@@ -2407,15 +1870,18 @@
     ):
         """
         Searches the database for entries that match. If can't find an exact
         match performs a kmer + local alignment approach to approximate
         search.
         """
         seq = self._sanitise_seq(seq) if not is_sanitised else seq
-        m = self.exact_search(seq, is_sanitised=True, entrynr_range=entrynr_range)
+        m = self.exact_search(seq, is_sanitised=True)
+        # TODO: taxonomic filtering.
+        if entrynr_range is not None:
+            m = [x for x in m if entrynr_range[0] <= x <= entrynr_range[1]]
         if len(m) == 0:
             # Do approximate search
             m = self.approx_search(
                 seq,
                 n=n,
                 is_sanitised=True,
                 coverage=coverage,
@@ -2423,127 +1889,88 @@
                 entrynr_range=entrynr_range,
             )
             # TODO: taxonomic filtering.
             return ("approx", m) if m is not [] else None
         else:
             return "exact", m
 
-    def exact_search(self, seq, only_full_length=True, is_sanitised=None, entrynr_range=None):
+    def exact_search(self, seq, only_full_length=True, is_sanitised=None):
         """
         Performs an exact match search using the suffix array.
         """
+        # TODO: work out whether to just use the approximate search and then
+        # check if any are actually exact matches. Do the counting and then
+        # do an equality checking on any of the sequences that have the correct
+        # number of kmer matches.
         seq = seq if is_sanitised else self._sanitise_seq(seq)
-        filt = self._tax_filter_range if isinstance(entrynr_range, tuple) else self._tax_filter_set
         nn = len(seq)
         if nn > 0:
-            z = KeyWrapper(self.seq_idx, key=lambda i: self.seq_buff[i : (i + nn)].tobytes())
+            z = KeyWrapper(
+                self.seq_idx, key=lambda i: self.seq_buff[i : (i + nn)].tobytes()
+            )
             ii = bisect_left(z, seq, lo=self.n_entries)
 
             if ii and ii < len(self.seq_idx) and (z[ii] == seq):
                 # Left most found.
                 seq_after = seq[:-1] + chr(seq[-1] + 1).encode("utf-8")
                 jj = bisect_left(z, seq_after, lo=ii)
                 if (jj < len(self.seq_idx) and z[jj] == seq) or z[jj - 1] != seq:
                     raise RuntimeError("suffix index broken. should not happen")
 
-                # Find entry numbers and enr_filter to remove incorrect entries
+                # Find entry numbers and filter to remove incorrect entries
                 return list(
                     filter(
-                        lambda e: (
-                            ((not only_full_length) or self.get_entry_length(e) == nn)
-                            and (entrynr_range is None or filt(e, entrynr_range))
-                        ),
+                        lambda e: (not only_full_length)
+                        or self.get_entry_length(e) == nn,
                         self.get_entrynr(self.seq_idx[ii:jj]),
                     )
                 )
 
         # Nothing found.
         return []
 
-    def approx_search_no_align(self, seq, is_sanitised=False, coverage=0.0, entrynr_range=None):
-        """Performs a quick ranking of the best matches based on kmer index.
-        The method does not compute an alignment, but just reports the
-        entry number with the fraction of kmer matching better than the set coverage
-
-        :param seq: the sequence to be searched
-        :type seq: str, bytes
-        :param is_sanitised: whether or not the sequence is already sanitised. defaults to false.
-        :type is_sanitised: bool
-        :param coverage: the minimum fraction of covered kmers by the target sequence
-        :type coverage: float
-        :param entrynr_range: target entry number range as a tuple (min, max) or set for filtering
-        :type entrynr_range: set[int], tuple[int, int]
-        :returns: A list of tuples with (entry_nr, fraction_of_matched_kmers)
+    def approx_search(
+        self,
+        seq,
+        n=None,
+        is_sanitised=None,
+        coverage=None,
+        compute_distance=False,
+        entrynr_range=None,
+    ):
+        """
+        Performs an exact match search using the suffix array.
+        :param entrynr_range:
         """
         seq = seq if is_sanitised else self._sanitise_seq(seq)
-        tax_filt = self._tax_filter_range if isinstance(entrynr_range, tuple) else self._tax_filter_set
+        n = n if n is not None else 50
+        coverage = 0.0 if coverage is None else coverage
 
         # 1. Do kmer counting vs entry numbers TODO: switch to np.unique?
         c = collections.Counter()
         for z in map(
             lambda kmer: numpy.unique(self.kmer_lookup[int(kmer)]),
             self.encoder.decompose(seq),
         ):
             c.update(z)
 
         # 2. Filter to top n if necessary
         z = len(seq) - self.k + 1
         cut_off = coverage * z
-        entries = [
+        c = [
             (enr, (cnts / z))
             for enr, cnts in c.items()
-            if cnts >= cut_off and (entrynr_range is None or tax_filt(enr, entrynr_range))
+            if cnts >= cut_off
+            and (entrynr_range is None or entrynr_range[0] <= enr <= entrynr_range[1])
         ]
-        return entries
-
-    def approx_search(
-        self,
-        seq,
-        n=None,
-        is_sanitised=None,
-        coverage=None,
-        compute_distance=False,
-        entrynr_range=None,
-        return_kmer_hits=False,
-    ):
-        """
-        Performs an approximate match search using the kmer index.
-        For the n best matching candidates based on kmer lookup, a
-        Smith-Waterman alignment is computed.
-
-        If compute_distance is set to True, an ML distance estimate
-        of the alignment is returned as part of the resulting dictionary
-
-        :param seq: the query sequence to be searched
-        :type seq: str, bytes
-        :param int n: number of maximum returned entries that match query
-        :param bool is_sanitised: whether or not the sequence is already sanitised. defaults to false.
-        :param float coverage: the minimum fraction of covered kmers by the target sequence
-        :param entrynr_range: target entry number range as a tuple (min, max) or set for filtering
-        :type entrynr_range: set[int], tuple[int, int]
-        :param bool return_kmer_hits: whether or not the full list of matched kmer entries should be
-        returned. if set to True, the return value will be a tuple instead of a single list
-
-        :returns: list of matched entries, each element is a tuple with the entry_nr and a dictionary
-        containing the score, alignment and distance estimates.
-        If return_kmer_hits is set to True, also the full list of matching entries is returned.
-        """
-        seq = seq if is_sanitised else self._sanitise_seq(seq)
-        n = n if n is not None else 50
-        coverage = 0.0 if coverage is None else coverage
-
-        kmer_hits = self.approx_search_no_align(seq, is_sanitised=True, coverage=coverage, entrynr_range=entrynr_range)
-        c = sorted(kmer_hits, reverse=True, key=lambda x: x[1])
-        if n > 0:
-            c = c[:n]
+        c = sorted(c, reverse=True, key=lambda x: x[1])[:n] if n > 0 else c
 
         # 3. Do local alignments and return count / score / alignment
-        res = []
         if len(c) > 0:
-            res = sorted(
+            return sorted(
                 [
                     (
                         m[0],
                         {
                             "kmer_coverage": m[1],
                             "score": a[0],
                             "alignment": a[1],
@@ -2552,18 +1979,15 @@
                         },
                     )
                     for (m, a) in self._align_entries(seq, c, compute_distance)
                 ],
                 key=lambda q: q[1]["score"],
                 reverse=True,
             )
-        if return_kmer_hits:
-            return res, kmer_hits
-        else:
-            return res
+        return []
 
     def _align_entries(self, seq, matches, compute_distance=False):
         # Does the alignment for the approximate search
         def align(s1, s2s, env, aligned):
             for s2 in s2s:
                 z = pyopa.align_double(s1, s2, env, False, False, True)
                 a = pyopa.align_strings(s1, s2, env, False, z)
@@ -2587,15 +2011,17 @@
                         ),
                     )
                 aligned.append(res_ds)
 
         if compute_distance and self.multienv_align is None:
             # lazy loading of MultipleAlEnv datastructure
             envs = pyopa.load_default_environments()
-            self.multienv_align = pyopa.MutipleAlEnv(envs["environments"], envs["log_pam1"])
+            self.multienv_align = pyopa.MutipleAlEnv(
+                envs["environments"], envs["log_pam1"]
+            )
 
         aligned = []
         query = pyopa.Sequence(seq.decode("ascii"))
         entries = list(
             map(
                 lambda m: pyopa.Sequence(self.get_sequence(int(m[0])).decode("ascii")),
                 matches,
@@ -2634,24 +2060,30 @@
                 if len(val) > 0:
                     values.append(val)
                     maps_to.append(row)
         return FuzzyMatcher(values, maps_to, rel_sim_cutoff=0.6)
 
     def genome_of_entry_nr(self, e_nr):
         """returns the genome code belonging to a given entry_nr"""
-        idx = self.genome_table["EntryOff"].searchsorted(e_nr - 1, side="right", sorter=self._entry_off_keys)
+        idx = self.genome_table["EntryOff"].searchsorted(
+            e_nr - 1, side="right", sorter=self._entry_off_keys
+        )
         return self.genome_table[self._entry_off_keys[idx - 1]]
 
     def map_entry_nr(self, entry_nr):
         genome = self.genome_of_entry_nr(entry_nr)
-        return "{0:s}{1:05d}".format(genome["UniProtSpeciesCode"].decode(), entry_nr - genome["EntryOff"])
+        return "{0:s}{1:05d}".format(
+            genome["UniProtSpeciesCode"].decode(), entry_nr - genome["EntryOff"]
+        )
 
     def genome_from_UniProtCode(self, code):
         code = code.encode("ascii")
-        idx = self.genome_table["UniProtSpeciesCode"].searchsorted(code, sorter=self._genome_keys)
+        idx = self.genome_table["UniProtSpeciesCode"].searchsorted(
+            code, sorter=self._genome_keys
+        )
         try:
             genome = self.genome_table[self._genome_keys[idx]]
         except IndexError:
             raise UnknownSpecies("{} is unknown".format(code))
 
         if genome["UniProtSpeciesCode"] != code:
             raise UnknownSpecies("{} is unknown".format(code))
@@ -2668,43 +2100,40 @@
         if genome["SciName"] != name:
             raise UnknownSpecies("{} is unknown".format(name))
         return genome
 
     def genome_from_taxid(self, taxid):
         try:
             taxid = int(taxid)
-            idx = self.genome_table["NCBITaxonId"].searchsorted(taxid, sorter=self._taxid_keys)
+            idx = self.genome_table["NCBITaxonId"].searchsorted(
+                taxid, sorter=self._taxid_keys
+            )
             genome = self.genome_table[self._taxid_keys[idx]]
         except (IndexError, ValueError):
             raise UnknownSpecies('TaxonId "{}" is unknown'.format(taxid))
         if genome["NCBITaxonId"] != taxid:
             raise UnknownSpecies('TaxonId "{}" is unknown'.format(taxid))
         return genome
 
     def identify_genome(self, code):
         """identify genome based on either a UniProtSpeciesCode,
         NCBI Taxonomy Id or species name"""
-        try:
-            code = int(code)
-        except ValueError:
+        if isinstance(code, int) or code.isdigit():
+            return self.genome_from_taxid(code)
+        else:
             if len(code) == 5:
                 try:
-                    return self.genome_from_UniProtCode(code.upper())
+                    return self.genome_from_UniProtCode(code)
                 except UnknownSpecies:
                     pass
             return self.genome_from_SciName(code)
-        return self.genome_from_taxid(code)
 
-    def approx_search_genomes(self, pattern, scores=False):
+    def approx_search_genomes(self, pattern):
         candidates = self._approx_genome_matcher.search_approx(pattern)
-        genomes = [Genome(self._db, self.genome_table[z[2]]) for z in candidates]
-        if scores:
-            return genomes, [z[0] for z in candidates]
-        else:
-            return genomes
+        return [Genome(self._db, self.genome_table[z[2]]) for z in candidates]
 
     def omaid_to_entry_nr(self, omaid):
         """returns the internal numeric entrynr from a
         UniProtSpeciesCode+nr id. this is the inverse
         function of 'map_entry_nr'."""
         match = self._omaid_re.match(omaid)
         if match is None:
@@ -2746,56 +2175,31 @@
 
         :param root: UniProtSpeciesCode of the root genome.
         :returns: a list of species codes in the correct order."""
         if root is None:
             root = self.genome_table[0]["UniProtSpeciesCode"]
         root_genome = self.genome_from_UniProtCode(root)
         lins = {
-            g["UniProtSpeciesCode"]: [lev["Name"] for lev in self._db.tax.get_parent_taxa(g["NCBITaxonId"])][::-1]
+            g["UniProtSpeciesCode"]: [
+                lev["Name"] for lev in self._db.tax.get_parent_taxa(g["NCBITaxonId"])
+            ][::-1]
             for g in self.genome_table
         }
         root_lin = lins[root_genome["UniProtSpeciesCode"]]
         sort_key = {}
         for g, lin_g in lins.items():
             for k in range(min(len(root_lin), len(lin_g))):
                 if root_lin[k] != lin_g[k]:
                     k -= 1
                     break
             sort_key[g] = (-k, lin_g)
         sorted_genomes = sorted(list(sort_key.keys()), key=lambda g: sort_key[g])
         return {g.decode(): v for v, g in enumerate(sorted_genomes)}
 
 
-class HogIdForwardMapper(object):
-    def __init__(self, db: Database, hogmap_filename=None):
-        if hogmap_filename is None:
-            hogmap_filename = db.get_hdf5_handle().filename.replace(".h5", ".hogmap.h5")
-        self.h5_hogmap = tables.open_file(hogmap_filename, mode="r")
-        self.db = db
-        self.db.register_on_close(self.close)
-
-    def close(self):
-        self.h5_hogmap.close()
-        self.db.unregister_on_close(self.close)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-    def map_hogid(self, hogid):
-        hogid = hogid.encode("utf-8") if isinstance(hogid, str) else hogid
-        cand_iter = self.h5_hogmap.get_node("/hogmap").where(
-            "Old == hogid",
-            {"hogid": hogid},
-        )
-        return {c["New"].decode(): float(c["Jaccard"]) for c in cand_iter}
-
-
 class FuzzyMatcher(object):
     def __init__(
         self,
         values,
         maps_to=None,
         rel_sim_cutoff=0.8,
         gram_size_lower=3,
@@ -2840,14 +2244,20 @@
                 for src in sources:
                     if src not in bests or score > bests[src][0]:
                         bests[src] = (score, val, src)
             matches = list(bests.values())
         return matches
 
 
+class AmbiguousID(Exception):
+    def __init__(self, message, candidates):
+        super(AmbiguousID, self).__init__(message, candidates)
+        self.candidates = candidates
+
+
 class IDResolver(object):
     def __init__(self, db):
         entry_nr_col = db.get_hdf5_handle().root.Protein.Entries.cols.EntryNr
         self.max_entry_nr = entry_nr_col[int(entry_nr_col.index[-1])]
         self._db = db
 
     def _from_numeric(self, e_id):
@@ -2861,22 +2271,33 @@
 
     def search_xrefs(self, e_id, return_seq_modified=False):
         """search for all xrefs. TODO: what happens if xref is ambiguous?"""
         xref_res = self._db.id_mapper["XRef"].search_xref(e_id)
         res = set([x["EntryNr"] for x in xref_res])
         if len(res) == 0:
             # let's try to mach as substring using suffix array case insensitive
-            xref_res = self._db.id_mapper["XRef"].search_xref(e_id, match_any_substring=True)
+            xref_res = self._db.id_mapper["XRef"].search_xref(
+                e_id, match_any_substring=True
+            )
             res = set([x["EntryNr"] for x in xref_res])
             if len(res) == 0:
                 raise InvalidId(e_id)
         if len(res) > 1:
             # check whether its only different isoforms, then return canonical isoform
-            splice_variants = set([x["AltSpliceVariant"] for x in (self._db.entry_by_entry_nr(eNr) for eNr in res)])
-            logger.info("xref {} has {} entries, {} splice variants".format(e_id, len(res), len(splice_variants)))
+            splice_variants = set(
+                [
+                    x["AltSpliceVariant"]
+                    for x in (self._db.entry_by_entry_nr(eNr) for eNr in res)
+                ]
+            )
+            logger.info(
+                "xref {} has {} entries, {} splice variants".format(
+                    e_id, len(res), len(splice_variants)
+                )
+            )
             if len(splice_variants) > 1 or 0 in splice_variants:
                 raise AmbiguousID('Cross-ref "{}" is ambiguous'.format(e_id), res)
             else:
                 res = splice_variants
         return_val = int(res.pop())
         if return_seq_modified:
             idx = numpy.where(xref_res["EntryNr"] == return_val)
@@ -2892,43 +2313,37 @@
                 nr = self._from_omaid(e_id)
             except (InvalidOmaId, UnknownSpecies) as e:
                 nr = self.search_xrefs(e_id, return_seq_modified=check_if_modified)
         if check_if_modified and not isinstance(nr, tuple):
             nr = (nr, False)
         return nr
 
-    @timethis(logging.DEBUG)
-    def search_protein(self, query: str, limit=None, entrynr_range=None):
+    def search_protein(self, query: str, limit=None):
         candidates = collections.defaultdict(dict)
         try:
             nr = self._from_numeric(query)
-            if entrynr_range is None or entrynr_range[0] <= nr <= entrynr_range[1]:
-                candidates[nr]["numeric_id"] = [query]
+            candidates[nr]["numeric_id"] = [query]
         except ValueError:
             pass
         try:
             nr = self._from_omaid(query)
-            if entrynr_range is None or entrynr_range[0] <= nr <= entrynr_range[1]:
-                candidates[nr]["omaid"] = [query]
+            candidates[nr]["omaid"] = [query]
         except (InvalidOmaId, UnknownSpecies) as e:
             pass
-        id_res = self._db.id_mapper["XRef"].search_id(query, limit=limit, entrynr_range=entrynr_range)
+        id_res = self._db.id_mapper["XRef"].search_id(query, limit)
         for nr, res_dict in id_res.items():
             candidates[nr].update(res_dict)
-        if len(id_res) < 5 and self._db.desc_searcher is not None:
-            try:
-                desc_res = self._db.desc_searcher.search_term(query, limit)
-                desc_res.sort()
-                for row_nr in desc_res[:limit]:
-                    nr = row_nr + 1
-                    if entrynr_range is None or entrynr_range[0] <= nr <= entrynr_range[1]:
-                        candidates[nr]["Description"] = [self._db.get_description(nr).decode()]
-            except SuffixIndexError as e:
-                logger.warning(e)
-                logger.warning("No Descriptions searched")
+        try:
+            desc_res = DescriptionSearcher(self._db).search_term(query)
+            for row_nr in desc_res[:limit]:
+                nr = row_nr + 1
+                candidates[nr]["Description"] = [self._db.get_description(nr).decode()]
+        except SuffixIndexError as e:
+            logger.warning(e)
+            logger.warning("No Descriptions searched")
         return candidates
 
 
 class Taxonomy(object):
     """Taxonomy provides an interface to navigate the taxonomy data.
 
     The input data is the same as what is stored in the Database in
@@ -2937,102 +2352,108 @@
     def __init__(self, data, genomes=None, _valid_levels=None):
         if not isinstance(data, numpy.ndarray):
             raise ValueError("Taxonomy expects a numpy table.")
         self.genomes = genomes if genomes is not None else {}
         self.tax_table = data
         self.taxid_key = self.tax_table.argsort(order=("NCBITaxonId"))
         self.parent_key = self.tax_table.argsort(order=("ParentTaxonId"))
-        self._add_luca_if_needed()
         self.all_hog_levels = _valid_levels
         self._approx_matcher = None
         if _valid_levels is None:
             self._load_valid_taxlevels()
 
     def _load_valid_taxlevels(self):
-        forbidden_chars = re.compile(r"[^A-Za-z0-9()/_,.: -]")
+        forbidden_chars = re.compile(r"[^A-Za-z0-9()/,.: -]")
         try:
             with open(os.environ["DARWIN_BROWSERDATA_PATH"] + "/TaxLevels.drw") as f:
                 taxStr = f.read()
             tax_json = json.loads(("[" + taxStr[14:-3] + "]").replace("'", '"'))
-            self.all_hog_levels = frozenset([t.encode("ascii") for t in tax_json if forbidden_chars.search(t) is None])
+            self.all_hog_levels = frozenset(
+                [
+                    t.encode("ascii")
+                    for t in tax_json
+                    if forbidden_chars.search(t) is None
+                ]
+            )
         except (IOError, KeyError):
             self.all_hog_levels = frozenset(
-                [l for l in self.tax_table["Name"] if forbidden_chars.search(l.decode()) is None]
+                [
+                    l
+                    for l in self.tax_table["Name"]
+                    if forbidden_chars.search(l.decode()) is None
+                ]
             )
 
     def _table_idx_from_numeric(self, tids):
         i = self.tax_table["NCBITaxonId"].searchsorted(tids, sorter=self.taxid_key)
         idx = self.taxid_key[i]
         if (self.tax_table[idx]["NCBITaxonId"] != tids).any():
             unkn = tids[self.tax_table[idx]["NCBITaxonId"] != tids]
             raise InvalidTaxonId("{} are invalid/unknown taxonomy ids".format(unkn))
         return idx
 
     def _get_root_taxon(self):
         i1 = self.tax_table["ParentTaxonId"].searchsorted(0, sorter=self.parent_key)
-        i2 = self.tax_table["ParentTaxonId"].searchsorted(0, sorter=self.parent_key, side="right")
+        i2 = self.tax_table["ParentTaxonId"].searchsorted(
+            0, sorter=self.parent_key, side="right"
+        )
         if i2 - i1 == 0:
-            raise DBConsistencyError("Not a single root in Taxonomy: {}".format(self.tax_table[self.parent_key[i1]]))
+            raise DBConsistencyError(
+                "Not a single root in Taxonomy: {}".format(
+                    self.tax_table[self.parent_key[i1]]
+                )
+            )
         elif i2 - i1 == 1:
             res = self.tax_table[self.parent_key[i1]]
         else:
             res = numpy.array([(0, -1, b"LUCA")], dtype=self.tax_table.dtype)[0]
         return res
 
-    def _add_luca_if_needed(self):
-        i1 = self.tax_table["ParentTaxonId"].searchsorted(0, sorter=self.parent_key)
-        i2 = self.tax_table["ParentTaxonId"].searchsorted(0, sorter=self.parent_key, side="right")
-        if i2 - i1 > 1:
-            self.tax_table = numpy.append(
-                self.tax_table,
-                numpy.array([(0, -1, b"LUCA")], dtype=self.tax_table.dtype),
-            )
-            self.taxid_key = self.tax_table.argsort(order=("NCBITaxonId"))
-            self.parent_key = self.tax_table.argsort(order=("ParentTaxonId"))
-
     def _taxon_from_numeric(self, tid):
         idx = self._table_idx_from_numeric(tid)
         return self.tax_table[idx]
 
     def _direct_children_taxa(self, tid):
         i = self.tax_table["ParentTaxonId"].searchsorted(tid, sorter=self.parent_key)
         idx = []
-        while i < len(self.parent_key) and self.tax_table[self.parent_key[i]]["ParentTaxonId"] == tid:
+        while (
+            i < len(self.parent_key)
+            and self.tax_table[self.parent_key[i]]["ParentTaxonId"] == tid
+        ):
             idx.append(self.parent_key[i])
             i += 1
         return self.tax_table.take(idx)
 
     def approx_search(self, pattern):
         if self._approx_matcher is None:
             valid_levels_as_str = (l.decode() for l in self.all_hog_levels)
             self._approx_matcher = FuzzyMatcher(values=valid_levels_as_str)
         candidates = self._approx_matcher.search_approx(pattern)
         return candidates
 
-    def get_parent_taxa(self, query, root=0):
+    def get_parent_taxa(self, query):
         """Get array of taxonomy entries leading towards the
         root of the taxonomy.
 
-        :param query: the starting taxonomy level
-        :param root: parameter to identify the root-taxid. defaults to 0.
-                     if set to -1, LUCA will be included into the list.
-        """
+        :param query: the starting taxonomy level"""
         idx = []
         parent = query
         count = 0
-        while parent != root:
+        while parent != 0:
             i = self._table_idx_from_numeric(parent)
             idx.append(i)
             tmp = self.tax_table[i]["ParentTaxonId"]
             if tmp == parent:
                 raise InvalidTaxonId("{0:d} has itself as parent".format(tmp))
             parent = tmp
             count += 1
             if count > 100:
-                raise InvalidTaxonId("{0:d} exceeds max depth of 100. Infinite recursion?".format(query))
+                raise InvalidTaxonId(
+                    "{0:d} exceeds max depth of 100. Infinite recursion?".format(query)
+                )
         return self.tax_table.take(idx)
 
     def _get_taxids_from_any(self, it, skip_missing=True):
         if not isinstance(it, numpy.ndarray):
             try:
                 it = numpy.fromiter(it, dtype="i4")
             except ValueError:
@@ -3114,23 +2535,27 @@
 
         taxids_to_keep = numpy.sort(self._get_taxids_from_any(members))
         if augment_parents:
             # find all the parents of all the members, add them to taxids_to_keep
             additional_levels = set([])
             for cur_tax in taxids_to_keep:
                 try:
-                    additional_levels.update(set(self.get_parent_taxa(cur_tax)["NCBITaxonId"]))
+                    additional_levels.update(
+                        set(self.get_parent_taxa(cur_tax)["NCBITaxonId"])
+                    )
                 except KeyError:
-                    logger.info("%s seems not to exist in Taxonomy", cur_tax)
+                    logger.info("{} seems not to exist in Taxonomy".format(cur_tax))
                     pass
             # add and remove duplicates
             all_levels = numpy.append(taxids_to_keep, list(additional_levels))
             taxids_to_keep = numpy.unique(all_levels)
 
-        idxs = numpy.searchsorted(self.tax_table["NCBITaxonId"], taxids_to_keep, sorter=self.taxid_key)
+        idxs = numpy.searchsorted(
+            self.tax_table["NCBITaxonId"], taxids_to_keep, sorter=self.taxid_key
+        )
         idxs = numpy.clip(idxs, 0, len(self.taxid_key) - 1)
         subtaxdata = self.tax_table[self.taxid_key[idxs]]
         if not numpy.alltrue(subtaxdata["NCBITaxonId"] == taxids_to_keep):
             raise KeyError("not all levels in members exists in this taxonomy")
 
         updated_parent = numpy.zeros(len(subtaxdata), "bool")
         for i, cur_tax in enumerate(taxids_to_keep):
@@ -3149,19 +2574,25 @@
             subtaxdata["ParentTaxonId"][new_idx] = parents
             updated_parent[new_idx] = True
 
         if collapse:
             nr_children = collections.defaultdict(int)
             for p in subtaxdata["ParentTaxonId"]:
                 nr_children[p] += 1
-            rem = [p for (p, cnt) in nr_children.items() if cnt == 1 and p != 0 and p not in self.genomes]
+            rem = [
+                p
+                for (p, cnt) in nr_children.items()
+                if cnt == 1 and p != 0 and p not in self.genomes
+            ]
             if len(rem) > 0:
                 idx = taxids_to_keep.searchsorted(rem)
                 return self.get_induced_taxonomy(numpy.delete(taxids_to_keep, idx))
-        return Taxonomy(subtaxdata, genomes=self.genomes, _valid_levels=self.all_hog_levels)
+        return Taxonomy(
+            subtaxdata, genomes=self.genomes, _valid_levels=self.all_hog_levels
+        )
 
     def newick(self):
         """Get a Newick representation of the Taxonomy
 
         Note: as many newick parsers do not support quoted labels,
         the method instead replaces spaces with underscores."""
 
@@ -3180,15 +2611,17 @@
                     # this is a special case where the current internal level is also
                     # an extant species in OMA. we resolve this by adding the current
                     # level also as an extra child
                     children.append(
                         newick_enc(
                             "{:s} (disambiguate {:s})".format(
                                 node["Name"].decode(),
-                                self.genomes[int(node["NCBITaxonId"])].uniprot_species_code,
+                                self.genomes[
+                                    int(node["NCBITaxonId"])
+                                ].uniprot_species_code,
                             )
                         )
                     )
 
                 t = ",".join(children)
                 return "(" + t + ")" + newick_enc(node["Name"].decode())
 
@@ -3245,17 +2678,21 @@
                 # an extant species in OMA. we resolve this by adding the current
                 # level also as an extra child
                 cp_n = et.Element("clade")
                 cp_tax = et.SubElement(cp_n, "taxonomy")
                 cp_id = et.SubElement(cp_tax, "id", provider="uniprot")
                 cp_id.text = str(node["NCBITaxonId"])
                 cp_code = et.SubElement(cp_tax, "code")
-                cp_code.text = self.genomes[int(node["NCBITaxonId"])].uniprot_species_code
+                cp_code.text = self.genomes[
+                    int(node["NCBITaxonId"])
+                ].uniprot_species_code
                 cp_sci = et.SubElement(cp_tax, "scientific_name")
-                cp_sci.text = "{:s} (disambiguate {:s})".format(node["Name"].decode(), cp_code.text)
+                cp_sci.text = "{:s} (disambiguate {:s})".format(
+                    node["Name"].decode(), cp_code.text
+                )
                 children.append(cp_n)
 
             if len(children) == 0:
                 try:
                     g = self.genomes[int(node["NCBITaxonId"])]
                     code = et.SubElement(tax, "code")
                     code.text = g.uniprot_species_code
@@ -3271,128 +2708,440 @@
         name = et.SubElement(phylo, "name")
         name.text = "(Partial) species phylogeny from OMA Browser"
         phylo.append(_rec_phyloxml(self._get_root_taxon()))
 
         return et.tostring(root, encoding="utf-8")
 
 
+class InvalidTaxonId(Exception):
+    pass
+
+
+class DBVersionError(Exception):
+    pass
+
+
+class DBConsistencyError(Exception):
+    pass
+
+
+class InvalidId(Exception):
+    pass
+
+
+class InvalidOmaId(InvalidId):
+    pass
+
+
+class UnknownIdType(Exception):
+    pass
+
+
+class UnknownSpecies(Exception):
+    pass
+
+
+class Singleton(Exception):
+    def __init__(self, entry, msg=None):
+        super(Singleton, self).__init__(msg)
+        self.entry = entry
+
+
+class NoReprEntry(Exception):
+    pass
+
+
 class IdMapperFactory(object):
     def __init__(self, db_obj):
         self.db = db_obj
         self.mappers = {}
 
     def __getitem__(self, idtype):
         return self.get_mapper(idtype)
 
     def get_mapper(self, idtype):
         try:
             mapper = self.mappers[idtype]
         except KeyError:
-            mapper = None
-            for inst in (str(idtype).title() + "IdMapper", str(idtype)):
-                try:
-                    mapper = globals()[inst](self.db)
-                    self.mappers[idtype] = mapper
-                    break
-                except KeyError:
-                    pass
-            if mapper is None:
+            try:
+                mapper = globals()[str(idtype).title() + "IdMapper"](self.db)
+                self.mappers[idtype] = mapper
+            except KeyError:
                 raise UnknownIdType("{} is unknown".format(str(idtype)))
         return mapper
 
 
-class BestIdPerEntryOnlyMixin:
-    def filter_best_id(self, arr):
-        df = pd.DataFrame(arr)
-        order = self.canonical_source_order()
-        df["ord"] = df["XRefSource"].apply(lambda x: order.index(self.xrefEnum(x)))
-        df = df.sort_values(by=["EntryNr", "ord"]).drop_duplicates(subset="EntryNr", keep="first")
-        return df.drop(columns="ord").to_records(index=False, column_dtypes=dict(arr.dtype.descr))
+class XrefIdMapper(object):
+    def __init__(self, db):
+        self._db = db
+        self.xref_tab = db.get_hdf5_handle().get_node("/XRef")
+        self.xrefEnum = self.xref_tab.get_enum("XRefSource")
+        self.idtype = frozenset(list(self.xrefEnum._values.keys()))
+        self.verif_enum = self.xref_tab.get_enum("Verification")
+        self._max_verif_for_mapping_entrynrs = 1000  # allow all verification values
+        try:
+            self.xref_index = SuffixSearcher.from_tablecolumn(self.xref_tab, "XRefId")
+        except SuffixIndexError:
+            # compability mode
+            idx_node = db.get_hdf5_handle().get_node("/XRef_Index")
+            self.xref_index = SuffixSearcher.from_index_node(idx_node)
+
+    def map_entry_nr(self, entry_nr):
+        """returns the XRef entries associated with the query protein.
+
+        The types of XRefs that are returned depends on the idtype
+        class member variable. In the base-class, idtype contains
+        all valid xref types. Typically, subclasses of XrefIdMapper
+        will change this set.
+
+        :param entry_nr: the numeric id of the query protein.
+        :returns: list of dicts with 'source' and 'xref' keys."""
+        res = [
+            {
+                "source": self.xrefEnum(row["XRefSource"]),
+                "xref": row["XRefId"].decode(),
+                "seq_match": self.verif_enum(row["Verification"]),
+            }
+            for row in self.xref_tab.where(
+                "(EntryNr=={:d}) & (Verification <= {:d})".format(
+                    entry_nr, self._max_verif_for_mapping_entrynrs
+                )
+            )
+            if row["XRefSource"] in self.idtype
+        ]
+        return res
+
+    def canonical_source_order(self):
+        """returns the list of xref sources in order of their importance.
+
+        Most important source - in the base class for example UniProtKB/SwissProt
+        are first. The canonical order is defined in the enum definition.
+
+        :returns: list of source strings"""
+        return [self.xrefEnum(z) for z in sorted(self.idtype)]
+
+    def iter_xrefs_for_entry_nr(self, entry_nr):
+        """Iterate over the xrefs of a given entry number.
+
+        This method returns a dict with 'source' and 'xref' fields
+        (both str) holding the information of the xref record.
+
+        :param entry_nr: the numeric id of the query protein"""
+        for row in self.xref_tab.where(
+            "(EntryNr=={:d}) & (Verification <= {:d})".format(
+                entry_nr, self._max_verif_for_mapping_entrynrs
+            )
+        ):
+            if row["XRefSource"] in self.idtype:
+                yield {
+                    "source": self.xrefEnum._values[row["XRefSource"]],
+                    "xref": row["XRefId"].decode(),
+                }
+
+    def _combine_query_values(self, field, values):
+        parts = ["({}=={})".format(field, z) for z in values]
+        return "(" + "|".join(parts) + ")"
+
+    def map_many_entry_nrs(self, entry_nrs):
+        """map several entry_nrs with as few db queries as possible
+        to their cross-references. The function returns a
+        :class:`numpy.recarray` containing all fields as defined in
+        the table.
+
+        :param entry_nrs: a list with numeric protein entry ids"""
+        mapped_junks = []
+        chunk_size = 32
+        source_condition = None
+        verif_condition = None
+        if len(self.idtype) < len(self.xrefEnum):
+            chunk_size -= len(self.idtype)  # respect max number of condition variables.
+            source_condition = self._combine_query_values("XRefSource", self.idtype)
+        if self._max_verif_for_mapping_entrynrs < max(x[1] for x in self.verif_enum):
+            chunk_size -= 1
+            verif_condition = "(Verification <= {:d})".format(
+                self._max_verif_for_mapping_entrynrs
+            )
+        for start in range(0, len(entry_nrs), chunk_size):
+            condition_list = [
+                self._combine_query_values(
+                    "EntryNr", entry_nrs[start : start + chunk_size]
+                )
+            ]
+            if source_condition:
+                condition_list.append(source_condition)
+            if verif_condition:
+                condition_list.append(verif_condition)
+            condition = " & ".join(condition_list)
+            mapped_junks.append(self.xref_tab.read_where(condition))
+        return numpy.lib.recfunctions.stack_arrays(mapped_junks, usemask=False)
+
+    @timethis(logging.DEBUG)
+    def search_xref(self, xref, is_prefix=False, match_any_substring=False):
+        """identify proteins associcated with `xref`.
+
+        The crossreferences are limited to the types in the class
+        member `idtype`. In the base class, all types are valid
+        xrefs. The method returns a :class:`numpy.recarry` defined
+        for the XRef table with all entries pointing to `xref`.
+
+        The method by default returns only exact matches. By setting
+        `is_prefix` to True, one can indicated that the requested xref
+        should be interpreted as a prefix and all entries matching this
+        prefix should be returned.
+
+        :param str xref: an xref to be located
+        :param bool is_prefix: treat xref as a prefix and return
+                     potentially several matching xrefs"""
+        if match_any_substring:
+            query = xref.encode("utf-8").lower()
+            res = self.xref_tab[self.xref_index.find(query)]
+        else:
+            if is_prefix:
+                up = xref[:-1] + chr(ord(xref[-1]) + 1)
+                cond = "(XRefId >= {!r}) & (XRefId < {!r})".format(
+                    xref.encode("utf-8"), up.encode("utf-8")
+                )
+            else:
+                cond = "XRefId=={!r}".format(xref.encode("utf-8"))
+            res = self.xref_tab.read_where(cond)
+        if len(res) > 0 and len(self.idtype) < len(self.xrefEnum):
+            res = res[numpy.in1d(res["XRefSource"], list(self.idtype))]
+
+        return res
+
+    def search_id(self, query, limit=None):
+        source_filter = None
+        try:
+            prefix, term = query.split(":", maxsplit=1)
+            if prefix in self.xrefEnum:
+                source_filter = self.xrefEnum[prefix]
+            else:
+                term = query
+        except ValueError:
+            term = query
+
+        result = collections.defaultdict(dict)
+        for xref_row in self.xref_index.find(term):
+            xref = self.xref_tab[xref_row]
+            if not source_filter or xref["XRefSource"] == source_filter:
+                source = self.xrefEnum(xref["XRefSource"])
+                try:
+                    result[xref["EntryNr"]][source].append(xref["XRefId"].decode())
+                except KeyError:
+                    result[xref["EntryNr"]][source] = [xref["XRefId"].decode()]
+            if limit is not None and len(result) >= limit:
+                break
+        return result
+
+    def source_as_string(self, source):
+        """string representation of xref source enum value
+
+        this auxiliary method converts the numeric value of
+        a xref source into a string representation.
+
+        :param int source: numeric value of xref source"""
+        try:
+            return self.xrefEnum._values[source]
+        except KeyError:
+            raise ValueError("'{}' is not a valid xref source value".format(source))
+
+    def verification_as_string(self, verif):
+        """string representation of xref verifiction enum value"""
+        return self.verif_enum(verif)
+
+    def xreftab_to_dict(self, tab):
+        """convert a xreftable to a dictionary per entry_nr.
+
+        All rows in `tab` are converted into a nested dictionary
+        where the outer key is a protein entry number and the
+        inner key the xref source type.
+
+        :param tab: a :class:`numpy.recarray` corresponding to XRef
+            table definition to be converted"""
+        xrefdict = collections.defaultdict(dict)
+        for row in tab:
+            try:
+                typ = self.xrefEnum(row["XRefSource"])
+            except IndexError:
+                logger.warning("invalid XRefSource value in {}".format(row))
+                continue
+            if typ not in xrefdict[row["EntryNr"]]:
+                xrefdict[row["EntryNr"]][typ] = {
+                    "id": row["XRefId"],
+                    "seq_match": self.verif_enum(row["Verification"]),
+                }
+        return xrefdict
+
+
+class XRefNoApproximateIdMapper(XrefIdMapper):
+    def __init__(self, db):
+        super(XRefNoApproximateIdMapper, self).__init__(db)
+        self._max_verif_for_mapping_entrynrs = self.verif_enum["unchecked"]
+
+
+class UniProtIdMapper(XrefIdMapper):
+    def __init__(self, db):
+        super(UniProtIdMapper, self).__init__(db)
+        self.idtype = frozenset(
+            [self.xrefEnum[z] for z in ["UniProtKB/SwissProt", "UniProtKB/TrEMBL"]]
+        )
+
+
+class LinkoutIdMapper(XrefIdMapper):
+    def __init__(self, db):
+        super(LinkoutIdMapper, self).__init__(db)
+        self.idtype = frozenset(
+            [
+                self.xrefEnum[z]
+                for z in [
+                    "UniProtKB/SwissProt",
+                    "UniProtKB/TrEMBL",
+                    "Ensembl Protein",
+                    "Ensembl Gene",
+                    "EntrezGene",
+                ]
+            ]
+        )
+
+    def url(self, typ, id_):
+        # TODO: improve url generator in external module with all xrefs
+        url = None
+        try:
+            id_ = id_.decode()
+        except AttributeError:
+            pass
+
+        if typ.startswith("UniProtKB"):
+            url = "http://uniprot.org/uniprot/{}".format(id_)
+        elif typ == "EntrezGene":
+            url = "http://www.ncbi.nlm.nih.gov/gene/{}".format(id_)
+        elif typ.startswith("Ensembl"):
+            url = "http://ensembl.org/id/{}".format(id_)
+        return url
+
+    def xreftab_to_dict(self, tab):
+        xref = super(LinkoutIdMapper, self).xreftab_to_dict(tab)
+        for d in list(xref.values()):
+            for typ, elem in list(d.items()):
+                elem["url"] = self.url(typ, elem["id"])
+        return xref
+
+    def iter_xrefs_for_entry_nr(self, entry_nr):
+        """same as base clase but includes also the url as a field"""
+        for xref in super(LinkoutIdMapper, self).iter_xrefs_for_entry_nr(entry_nr):
+            xref["url"] = self.url(xref["source"], xref["xref"])
+            yield xref
+
+
+class DomainNameIdMapper(object):
+    def __init__(self, db):
+        self.domain_src = db.get_hdf5_handle().root.Annotations.DomainDescription.read()
+        self.domain_src.sort(order="DomainId")
+
+    def _get_dominfo(self, domain_id):
+        idx = self.domain_src["DomainId"].searchsorted(domain_id)
+        if self.domain_src[idx]["DomainId"] != domain_id:
+            raise KeyError("no domain info available for {}".format(domain_id))
+        return self.domain_src[idx]
+
+    def get_info_dict_from_domainid(self, domain_id):
+        info = self._get_dominfo(domain_id)
+        return {
+            "name": info["Description"].decode(),
+            "source": info["Source"].decode(),
+            "domainid": domain_id.decode(),
+        }
 
 
 class DescriptionSearcher(object):
     def __init__(self, db):
         self.entry_tab = db.get_hdf5_handle().get_node("/Protein/Entries")
-        self.desc_index = SuffixSearcher.from_tablecolumn(self.entry_tab, "DescriptionOffset")
+        self.desc_index = SuffixSearcher.from_tablecolumn(
+            self.entry_tab, "DescriptionOffset"
+        )
 
     @timethis(logging.DEBUG)
-    def search_term(self, term, limit=None):
-        return self.desc_index.find(term, limit=limit)
+    def search_term(self, term):
+        return self.desc_index.find(term)
 
 
 class FastMapper(object):
     """GO Function projection to sequences from OMA hdf5 file"""
 
     def __init__(self, db):
         self.db = db
 
-    def iter_projected_goannotations(self, records, target_species=None):
+    def iter_projected_goannotations(self, records):
         # gene ontology fast mapping, uses exact / approximate search.
         # todo: implement taxonomic restriction.
         # Input: iterable of biopython SeqRecords
 
-        entrynr_range = None
-        if target_species is not None:
-            entrynr_range = self.db.id_mapper["OMA"].genome_range(target_species)
-
         for rec in records:
-            logger.debug("projecting function to %s", rec)
+            logger.debug("projecting function to {}".format(rec))
             if len(rec) < 25:
-                logger.warning("Skipping short sequence (len=%s AA)", len(rec))
+                logger.warning("Skipping short sequence (len={} AA)".format(len(rec)))
                 continue
             t0 = time.time()
-            r = self.db.seq_search.search(str(rec.seq), entrynr_range=entrynr_range)
-            logger.info("sequence matching of %s (%d AA) took %fsec", rec.id, len(rec), time.time() - t0)
+            r = self.db.seq_search.search(str(rec.seq))
+            logger.info(
+                "sequence matching of {} ({} AA) took {:.3f}sec".format(
+                    rec.id, len(rec), time.time() - t0
+                )
+            )
             if r is not None:
                 logger.debug(str(r))
                 go_df = None
                 if r[0] == "exact":
                     tdfs1 = []
                     for enum in r[1]:
-                        df = self.db.get_gene_ontology_annotations(enum, as_dataframe=True)
+                        df = self.db.get_gene_ontology_annotations(
+                            enum, as_dataframe=True
+                        )
                         if df is not None:
-                            df["With"] = "Exact:{}".format(self.db.id_mapper["Oma"].map_entry_nr(enum))
+                            df["With"] = "Exact:{}".format(
+                                self.db.id_mapper["Oma"].map_entry_nr(enum)
+                            )
                             tdfs1.append(df)
                     if len(tdfs1) > 0:
                         go_df = pd.concat(tdfs1, ignore_index=True)
 
                 else:
-                    # Take best match, that has go-annotations unless it's alignment score
-                    # is less than 80% of the highest scoring match.
-                    max_score = r[1][0][1]["score"]
-                    for enr, match_res in r[1]:
-                        score = match_res["score"]
-                        if score < 70 or score < 0.8 * max_score:
-                            break
-
-                        go_df = self.db.get_gene_ontology_annotations(enr, as_dataframe=True)
-                        cnt = len(go_df) if go_df is not None else 0
-                        logger.debug("match: enr: {}, score:{}, go_anno: {}".format(enr, score, cnt))
-
-                        if go_df is not None:
-                            go_df["With"] = "Approx:{}:{}".format(
-                                self.db.id_mapper["Oma"].map_entry_nr(enr),
-                                score,
-                            )
-                            break
+                    # Take best match. TODO: remove those below some level of match.
+                    match_enum = r[1][0][0]
+                    match_score = r[1][0][1]["score"]
+                    logger.debug(
+                        "match: enum: {}, score:{}".format(match_enum, match_score)
+                    )
+                    go_df = self.db.get_gene_ontology_annotations(
+                        match_enum, as_dataframe=True
+                    )
+                    if go_df is not None:
+                        go_df["With"] = "Approx:{}:{}".format(
+                            self.db.id_mapper["Oma"].map_entry_nr(match_enum),
+                            match_score,
+                        )
                 if go_df is not None:
                     go_df["DB"] = "OMA_FastMap"
                     go_df["Assigned_By"] = go_df["DB"]
                     go_df["DB_Object_ID"] = rec.id
                     go_df["DB_Object_Symbol"] = go_df["DB_Object_ID"]
                     go_df["Evidence"] = "IEA"
                     go_df["DB:Reference"] = "OMA_Fun:002"
                     go_df["Taxon_ID"] = "taxon:-1"
                     len_with_dupl = len(go_df)
                     go_df.drop_duplicates(inplace=True)
-                    logger.debug("cleaning duplicates: from {} to {} annotations".format(len_with_dupl, len(go_df)))
+                    logger.debug(
+                        "cleaning duplicates: from {} to {} annotations".format(
+                            len_with_dupl, len(go_df)
+                        )
+                    )
                     for row in go_df.to_dict("records"):
                         yield row
 
-    def write_annotations(self, file, seqrecords, target_species=None):
+    def write_annotations(self, file, seqrecords):
         """Project annotations and write them to file
 
         This method takes a filehandle and an iterable of BioPython
         SeqRecords objects as input. The function computes the
         projected annotations and writes them to the file in gaf
         format.
 
@@ -3400,78 +3149,62 @@
         :param seqrecords: input sequencs to project functions to
         """
 
         file.write("!gaf-version: {}\n".format(GAF_VERSION))
         file.write("!Project Name: OMA Fast Function Projection\n")
         file.write("!Date created: {}\n".format(time.strftime("%c")))
         file.write("!Contact Email: contact@omabrowser.org\n")
-        for anno in self.iter_projected_goannotations(seqrecords, target_species):
+        for anno in self.iter_projected_goannotations(seqrecords):
             GOA.writerec(anno, file, GOA.GAF20FIELDS)
 
 
-HogMapperTuple = collections.namedtuple("HogMapperTuple", "query, closest_entry_nr, target, distance, score")
+HogMapperTuple = collections.namedtuple(
+    "HogMapperTuple", "query, closest_entry_nr, target, distance, score"
+)
 
 
 class ClosestSeqMapper(object):
     """Fast mapper of sequeces to closest sequence and taken their HOG annotation"""
 
-    def __init__(self, db, threaded=False, nr_approx_alignments=50):
+    def __init__(self, db, threaded=False):
         self.db = Database(db.get_hdf5_handle().filename) if threaded else db
-        self.nr_approx_alignments = nr_approx_alignments
-        self._times = []
 
     def _get_main_protein_from_entrynr(self, enr):
         entry = ProteinEntry(self.db, self.db.entry_by_entry_nr(enr))
         return entry.get_main_isoform()
 
-    def _search_seq_with_time_stats(self, rec, entrynr_range=None):
-        t_start = time.time()
-        search_res = self.db.seq_search.search(
-            str(rec.seq), n=self.nr_approx_alignments, compute_distance=True, entrynr_range=entrynr_range
-        )
-        t_search = time.time() - t_start
-        self._times.append(t_search)
-        logger.debug("mapping of %s took %f sec", rec.id, t_search)
-        return search_res
-
-    def _log_time_stat(self, runtime):
-        self._times
-        quantiles = numpy.quantile(self._times, [0, 0.1, 0.5, 0.9, 1])
-        logger.info(
-            "Mapped %d sequences. Total mapping time %f (tot time %f)", len(self._times), sum(self._times), runtime
-        )
-        logger.info(" min_time: %f, 10%% time: %f, avg_time: %f, 90%% time: %f, max_time: %f", *quantiles)
-
     def imap_sequences(self, seqrecords, target_species=None):
         """maps an iterator of Bio.Seq.SeqRecords to database and
         yields the mappings."""
         entrynr_range = None
         if target_species is not None:
             entrynr_range = self.db.id_mapper["OMA"].genome_range(target_species)
 
-        t_start = t_last = time.time()
         for rec in seqrecords:
-            logger.debug("projecting %s (%d AA) to closest sequence", rec.id, len(rec.seq))
-            search_res = self._search_seq_with_time_stats(rec, entrynr_range=entrynr_range)
-            if search_res is not None:
-                if search_res[0] == "exact":
+            logger.debug("projecting {} to closest sequence".format(rec))
+            r = self.db.seq_search.search(
+                str(rec.seq), compute_distance=True, entrynr_range=entrynr_range
+            )
+            if r is not None:
+                if r[0] == "exact":
                     # r[1] contains list of entry nr with exact sequence match (full length)
-                    for enr in search_res[1]:
+                    for enr in r[1]:
                         p = self._get_main_protein_from_entrynr(enr)
-                        # score is set to expected score for a matching AAs: sum(AF[k]*sim[k,k])=12.61
-                        yield HogMapperTuple(rec.id, enr, p, 0.01, len(rec.seq) * 12.61)
+                        # TODO: good score for identical sequences
+                        yield HogMapperTuple(rec.id, enr, p, 0, 0)
                 else:
-                    candidate_matches = search_res[1]
+                    candidate_matches = r[1]
                     if len(candidate_matches) <= 0:
                         continue
                     # Take best matches, up to score>80 & score_i > .5*score_max
                     score_max = candidate_matches[0][1]["score"]
                     for enr, match_res in candidate_matches:
-                        if match_res["score"] < 80 or match_res["score"] < 0.5 * score_max:
+                        if (
+                            match_res["score"] < 80
+                            or match_res["score"] < 0.5 * score_max
+                        ):
                             break
                         p = self._get_main_protein_from_entrynr(enr)
                         # score, distance, distvar = pyopa.MutipleAlEnv
-                        yield HogMapperTuple(rec.id, enr, p, match_res["distance"], match_res["score"])
-            if time.time() - t_last > 60:
-                t_last = time.time()
-                self._log_time_stat(t_last - t_start)
-        self._log_time_stat(time.time() - t_start)
+                        yield HogMapperTuple(
+                            rec.id, enr, p, match_res["distance"], match_res["score"]
+                        )
```

### Comparing `pyoma-0.13.2/pyoma/browser/decorators.py` & `pyoma-0.9.4/pyoma/browser/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,22 +29,7 @@
             end = time()
             log.log(level, "time for {}: {}sec".format(func.__name__, end - start))
             return result
 
         return wrapper
 
     return decorate
-
-
-def outdated_database_warning():
-    def decorate(func):
-        log = logging.getLogger(func.__module__)
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            log.warning("outdated database warning in {}".format(func.__name__))
-            result = func(*args, **kwargs)
-            return result
-
-        return wrapper
-
-    return decorate
```

### Comparing `pyoma-0.13.2/pyoma/browser/geneontology.py` & `pyoma-0.9.4/pyoma/browser/geneontology.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from builtins import int, bytes, str
 import collections
 import csv
 import logging
 import math
 import re
-from functools import lru_cache
-from collections import deque
-
 import numpy
 
 
 """
 IMPORTANT NOTE:
 ---------------
 This module has been copied from the dessimoz zoo library
@@ -75,23 +72,22 @@
         return cls.aspect2char[aspectnr]
 
 
 class GOterm(object):
     """A class representing a single Gene Ontology term.
 
     This class can serve as a factory for the OntologyParser. For that,
-    pass it as a factory on 'Term'."""
+    pass it as a factory on 'Term'. """
 
     def __init__(self, stanza):
         self.id = validate_go_id(stanza["id"][0])
         self.name = " ".join(stanza["name"])
         self.definition = " ".join(stanza["def"])
         self.aspect = GOAspect.from_string(" ".join(stanza["namespace"]))
         self.is_a = [validate_go_id(parent) for parent in stanza["is_a"]]
-        self.min_depth = 100000
         for rel in stanza["relationship"]:
             reltype, partner = rel.strip().split()
             if not reltype in self.__dict__.keys():
                 self.__dict__[reltype] = list()
             self.__dict__[reltype].append(validate_go_id(partner))
 
     def replace_parentnames_by_refs(self, ont):
@@ -207,15 +203,17 @@
         if stanza is not None:
             try:
                 factory = self.factories[stanza["_name"]]
             except KeyError:
                 # no factory for this stanza type. ignore
                 pass
             else:
-                if (not "is_obsolete" in stanza) or (not "true" in stanza["is_obsolete"]):
+                if (not "is_obsolete" in stanza) or (
+                    not "true" in stanza["is_obsolete"]
+                ):
                     res = factory(stanza)
         return res
 
     def __iter__(self):
         return self.stanzas()
 
 
@@ -241,26 +239,14 @@
             self.terms[cur_term.id] = cur_term
 
         # replace parents nrs by the references to the GO terms objects
         # this can be only done once all the terms have been created
         for term in self.terms.values():
             term.replace_parentnames_by_refs(self.terms)
 
-        # compute mindepth of terms in a bfg traversal
-        self._compute_min_depths()
-
-    def _compute_min_depths(self):
-        root_terms = [t for t in self.terms.values() if not any((len(getattr(t, rel, [])) > 0 for rel in self.up_rels))]
-        bfg_queue = deque(((t, 0) for t in root_terms))
-        while len(bfg_queue) > 0:
-            term, depth = bfg_queue.popleft()
-            if depth < term.min_depth:
-                term.min_depth = depth
-                bfg_queue.extend((child, depth + 1) for rel in self.down_rels for child in getattr(term, rel, []))
-
     def ensure_term(self, term):
         """returns the term object associated with term. if term is already
         a GOterm object, it is simply return. term_ids can be either numeric
         ids of existing GO-terms or propper GO-terms ids, i.e. GO:000002
 
         :param term: a term_id or a GOterm object"""
         if isinstance(term, GOterm):
@@ -287,15 +273,14 @@
         term = self.ensure_term(term)
         return self._traverseGraph(term, max_steps, self.up_rels)
 
     def get_subterms(self, term, max_steps=-1):
         term = self.ensure_term(term)
         return self._traverseGraph(term, max_steps, self.down_rels)
 
-    @lru_cache(maxsize=4048)
     def _traverseGraph(self, node, max_steps, rels):
         """_traverseGraph traverses the graph in a breath first manner
         and reports all the nodes reachable within max_steps."""
         remain = set([node])
         found = set()
         while len(remain) > 0 and max_steps != 0:
             novel = set()
@@ -330,15 +315,17 @@
         self.tot_cnts = [0] * NUM_ONT
 
     def estimate_freqs(self, annotations):
         for anno in annotations:
             try:
                 self._update_counts(self.term_by_id(anno["TermNr"]))
             except ValueError:
-                logging.info("invalid annotation term_id in freq estim:" + str(anno["TermNr"]))
+                logging.info(
+                    "invalid annotation term_id in freq estim:" + str(anno.term_id)
+                )
 
     def _update_counts(self, term):
         for cur_term in self.get_superterms_incl_queryterm(term):
             self.cnts[cur_term.id] = self.cnts.get(cur_term.id, 0) + 1
         self.tot_cnts[cur_term.aspect] += 1
 
     def get_term_frequency(self, term):
@@ -352,65 +339,34 @@
     def last_common_ancestor(self, *terms):
         cand = self.get_superterms_incl_queryterm(terms[0])
         for t in terms[1:]:
             cand.intersection_update(self.get_superterms_incl_queryterm(t))
         lca = min(cand, key=self.get_term_frequency)
         return lca
 
-    def ic(self, term):
-        """returns the information content of the term based on the number of annotations in the OMA database
-
-        .. math::
-            ic(GO_i) = -\log_{10}(term_freq)
-        """
-        term = self.ensure_term(term)
-        return abs(-math.log(self.get_term_frequency(term)))
-
-    def _resolve_lca_term(self, *terms):
-        goterms = list(map(self.ensure_term, terms))
-        if not all(map(lambda t: goterms[0].aspect == t.aspect, goterms)):
-            raise DifferentAspectError()
-        lca = self.last_common_ancestor(*goterms)
-        return lca, *goterms
-
-    def lin_similarity(self, term1, term2) -> float:
-        """computes the Lin similarity between two GO terms:
-
-        .. math::
-            sim(GO_i, GO_j) = \frac{2 \log_{10}(IC(GO_{LCA}}{\log_{10}(IC(GO_i) + \log_{10}(IC(GO_j))}
-
-        """
-        try:
-            lca, term1, term2 = self._resolve_lca_term(term1, term2)
+    def lin_similarity(self, term1, term2):
+        term1 = self.ensure_term(term1)
+        term2 = self.ensure_term(term2)
+        if term1.aspect != term2.aspect:
+            # early abort, since the two terms will be by
+            # definition not similar
+            sim = 0
+        else:
+            lca = self.last_common_ancestor(term1, term2)
             sim = (
                 2
                 * math.log(self.get_term_frequency(lca))
-                / (math.log(self.get_term_frequency(term1)) + math.log(self.get_term_frequency(term2)))
+                / (
+                    math.log(self.get_term_frequency(term1))
+                    + math.log(self.get_term_frequency(term2))
+                )
             )
-            return sim
-        except DifferentAspectError:
-            return 0
-
-    def semantic_similarity(self, term1, term2):
-        try:
-            lca, term1, term2 = self._resolve_lca_term(term1, term2)
-        except DifferentAspectError:
-            return 0
-        p_lca = self.get_term_frequency(lca)
-        sim = (1 - p_lca) * (
-            (2 * numpy.log2(p_lca))
-            / (numpy.log2(self.get_term_frequency(term1)) + numpy.log2(self.get_term_frequency(term2)))
-        )
         return sim
 
 
-class DifferentAspectError(Exception):
-    pass
-
-
 class AnnotationFilter(object):
     EXP_CODES = frozenset(["EXP", "IDA", "IPI", "IMP", "IGI", "IEP"])
     TRUST_IEA_REFS = frozenset(
         [
             "GO_REF:0000002",
             "GOA:interpro",
             "GOA:interpro|GO_REF:0000002",  # InterPro
@@ -434,15 +390,19 @@
 
     @classmethod
     def is_exp_annotation(cls, a):
         return a.evidence in cls.EXP_CODES and not cls.is_negated(a)
 
     @classmethod
     def is_trusted_electronic(cls, a):
-        return a.evidence == "IEA" and a.db_ref in cls.TRUST_IEA_REFS and not cls.is_negated(a)
+        return (
+            a.evidence == "IEA"
+            and a.db_ref in cls.TRUST_IEA_REFS
+            and not cls.is_negated(a)
+        )
 
     @classmethod
     def is_exp_or_trusted_electronic(cls, a):
         return cls.is_exp_annotation(a) or cls.is_trusted_electronic(a)
 
 
 # definition of the GOA Annotations. for performance reasons, we
@@ -490,15 +450,17 @@
     def _read_headers(self):
         pass
 
     def annotations(self):
         """Iterates over the annotations in the file yielding objects
         constructed by the factory argument passed to the constructor
         of this class for each annotation."""
-        csv_reader = csv.reader((l for l in self.fp if not l.startswith("!")), delimiter="\t")
+        csv_reader = csv.reader(
+            (l for l in self.fp if not l.startswith("!")), delimiter="\t"
+        )
         for row in csv_reader:
             yield self.factory(row)
         if self._needs_close:
             self.fp.close()
 
     def __iter__(self):
         return self.annotations()
```

### Comparing `pyoma-0.13.2/pyoma/browser/hoghelper.py` & `pyoma-0.9.4/pyoma/browser/hoghelper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import collections
 import logging
-import os.path
-import re
 import numpy
-from typing import Union
 
 logger = logging.getLogger(__name__)
 
 
 class HogLevelFilter(object):
     """Filter sub-hogs at given level (or below)
 
@@ -15,23 +11,30 @@
     does not go deep enough to cover the desired level, the whole hog will be returned.
     """
 
     def __init__(self, db, level):
         self.db = db
         self.level = level
         tax_below_level = self.db.tax.get_subtaxonomy_rooted_at(level)
-        self.sub_level_distances = self._build_distance_to_query_level_lookup(tax_below_level)
+        self.sub_level_distances = self._build_distance_to_query_level_lookup(
+            tax_below_level
+        )
         self.parent_levels = set(
-            db.tax.get_parent_taxa(db.tax.get_taxnode_from_name_or_taxid(level)[0]["NCBITaxonId"])["Name"]
+            db.tax.get_parent_taxa(
+                db.tax.get_taxnode_from_name_or_taxid(level)[0]["NCBITaxonId"]
+            )["Name"]
         )
         # cache all the families nrs that are defined in the clade of interest
         self.fams_in_clade = set(
             int(roothog["Fam"])
-            for roothog in db.get_hdf5_handle().root.HogLevel.where('~contains(ID, b".") & (IsRoot == True)')
-            if roothog["Level"] in self.sub_level_distances or roothog["Level"] in self.parent_levels
+            for roothog in db.get_hdf5_handle().root.HogLevel.where(
+                '~contains(ID, b".") & (IsRoot == True)'
+            )
+            if roothog["Level"] in self.sub_level_distances
+            or roothog["Level"] in self.parent_levels
         )
 
     def _build_distance_to_query_level_lookup(self, tax):
         nodes = {}
 
         def traverse(node, dist=0):
             nodes[node["name"].encode("utf-8")] = dist
@@ -51,15 +54,15 @@
         for lev in levs:
             try:
                 if self.sub_level_distances[lev] < min_dist:
                     closest = lev.item().decode()
                     min_dist = self.sub_level_distances[lev]
             except KeyError:
                 pass
-        logger.debug("closest level %s at %s", closest, min_dist)
+        logger.debug("closest level {} at {}".format(closest, min_dist))
         return closest
 
     def analyse_families(self, it):
         for fam in it:
             if fam not in self.fams_in_clade:
                 continue
             subhog_ids = self.db.get_subhogids_at_level(fam_nr=fam, level=self.level)
@@ -70,28 +73,14 @@
                 if closest_level is not None:
                     yield (self.db.format_hogid(fam), closest_level)
             else:
                 for subhog_id in subhog_ids:
                     yield (subhog_id, self.level)
 
 
-def build_hog_to_og_map(db):
-    hog_to_og_cnts = collections.defaultdict(collections.Counter)
-    entries = db.get_hdf5_handle().get_node("/Protein/Entries")
-    for protein in entries.where("(OmaHOG != b'') & (OmaGroup > 0)"):
-        hog_id = protein["OmaHOG"]
-        og = int(protein["OmaGroup"])
-        for p in re.finditer(rb"\.", hog_id):
-            cur_id = hog_id[: p.start()]
-            hog_to_og_cnts[cur_id].update((og,))
-        hog_to_og_cnts[hog_id].update((og,))
-    for hog_id, cnts in hog_to_og_cnts.items():
-        yield hog_id, cnts.most_common(1)
-
-
 def compare_levels(
     parent_level_hogs: numpy.array,
     children_level_hogs: numpy.array,
     return_duplication_events=False,
 ):
     """compares hogs at two levels and returns duplicated/lost/gained/identical states
 
@@ -109,17 +98,17 @@
         else:
             if parent_level_hogs[i]["ID"] == children_level_hogs[j]["ID"]:
                 annotated.append(tuple(children_level_hogs[j]) + (b"retained",))
                 i += 1
                 j += 1
             else:
                 dupl_fnd = 0
-                while j < len(children_level_hogs) and children_level_hogs[j]["ID"].startswith(
-                    parent_level_hogs[i]["ID"]
-                ):
+                while j < len(children_level_hogs) and children_level_hogs[j][
+                    "ID"
+                ].startswith(parent_level_hogs[i]["ID"]):
                     annotated.append(tuple(children_level_hogs[j]) + (b"duplicated",))
                     j += 1
                     dupl_fnd += 1
                 if dupl_fnd > 0:
                     # parent duplicated into at least one subhog
                     dups += 1
                 else:
@@ -134,42 +123,7 @@
         annotated.append(tuple(children_level_hogs[j]) + (b"gained",))
         j += 1
     dt = children_level_hogs.dtype.descr + [("Event", "S10")]
     diff = numpy.array(annotated, dtype=dt)
     if return_duplication_events:
         return diff, dups
     return diff
-
-
-hog_re = re.compile(r"(?P<id>HOG:(?P<rel>[A-Z]+)?(?P<fam>\d+)(?P<sub>[a-z0-9.]*))(?:_(?P<taxid>\d+))?")
-sub_re = re.compile(r"^(?P<nr>\d+)(?P<char>[a-z]+)$")
-
-
-def are_orthologous(
-    hogid1: Union[bytes, str], hogid2: Union[bytes, str], return_group: bool = False
-) -> Union[bool, str]:
-    h1 = hogid1 if isinstance(hogid1, str) else hogid1.decode()
-    h2 = hogid2 if isinstance(hogid2, str) else hogid2.decode()
-
-    m1 = hog_re.match(h1)
-    m2 = hog_re.match(h2)
-    if m1.group("fam") != m2.group("fam") or m1.group("rel") != m2.group("rel"):
-        return False
-    common_group = ["HOG:{}{}".format(m1.group("rel"), m1.group("fam"))]
-    for sub_i, sub_j in zip(m1.group("sub").split("."), m2.group("sub").split(".")):
-        if sub_i == sub_j:
-            if len(sub_i) > 0:
-                common_group.append(sub_i)
-            continue
-        m_sub_i = sub_re.match(sub_i)
-        m_sub_j = sub_re.match(sub_j)
-        if m_sub_i.group("nr") != m_sub_j.group("nr"):
-            if return_group:
-                return ".".join(common_group)
-            else:
-                return True
-        elif m_sub_i.group("char") != m_sub_j.group("char"):
-            return False
-    if return_group:
-        return ".".join(common_group)
-    else:
-        return True
```

### Comparing `pyoma-0.13.2/pyoma/browser/hogidmap.py` & `pyoma-0.9.4/tests/browser/test_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,297 +1,339 @@
-import collections
-import itertools
-import logging
-import multiprocessing
+from __future__ import absolute_import, print_function, division
+
+import csv
+import gzip
+import io
+import json
 import os
-import re
-import time
-from functools import partial
-from tqdm import tqdm
+import shutil
+import tempfile
+import unittest
+from hashlib import md5
 
 import numpy
 import tables
-from datasketch import MinHash, MinHashLSH, LeanMinHash
+import pyoma.browser.tablefmt as tablefmt
+from pyoma.browser.convert import (
+    callDarwinExport,
+    DarwinExporter,
+    compute_ortholog_types,
+    load_tsv_to_numpy,
+    HogConverter,
+)
+
+
+def store_in_json(data, fn):
+    os.mkdir(os.path.dirname(fn))
+    with open(fn, "w") as fd:
+        json.dump(data, fd)
+
+
+class ImportDummyBase(unittest.TestCase):
+    """This base class makes sure that the environment vars
+    `DARWIN_BROWSERDATA_PATH` and `DARWIN_NETWORK_SCRATCH_PATH`
+    are set to a temporary path at the beginning of the test cases
+    and get restored to the initial value after a test cases
+    finished.
+
+    At the beginning of each testcase, a new DarwinExporter is
+    created at the location of $DARWIN_BROWSERDATA_PATH and removed
+    after the testcase.
+
+    Subclasses can therefor overwrite the $DARWIN_BROWSERDATA_PATH
+    in the setUpClass method if needed.
+    """
+
+    @classmethod
+    def setUpClass(cls):
+        cls.tmpdir = tempfile.mkdtemp()
+        cls.old_env = {
+            (z, os.getenv(z, None))
+            for z in ("DARWIN_NETWORK_SCRATCH_PATH", "DARWIN_BROWSERDATA_PATH")
+        }
+        os.environ["DARWIN_NETWORK_SCRATCH_PATH"] = cls.tmpdir
+        os.environ["DARWIN_BROWSERDATA_PATH"] = cls.tmpdir
+
+    @classmethod
+    def tearDownClass(cls):
+        shutil.rmtree(cls.tmpdir)
+        for var, val in cls.old_env:
+            if val is None:
+                os.unsetenv(var)
+            else:
+                os.environ[var] = val
+
+    def setUp(self):
+        fname = tempfile.mktemp(".h5", "OmaServer-", self.tmpdir)
+        self.darwin_exporter = DarwinExporter(fname)
+
+    def tearDown(self):
+        fn = self.darwin_exporter.h5.filename
+        self.darwin_exporter.close()
+        os.remove(fn)
+
+
+class ImportIntegrationBase(ImportDummyBase):
+    """This base class checks if the Test-case data
+    is available on any of the groups shared directories
+    and uses this directory for the DARWIN_BROWSERDATA_PATH.
+    If none of the shares is available, the tests are skipped.
+    """
+
+    @classmethod
+    def setUpClass(cls):
+        super(ImportIntegrationBase, cls).setUpClass()
+        test_data_available = False
+        for folder in (
+            "/pub/projects/cbrg-oma-browser",
+            "/cs/research/biosciences/oma/oma-server",
+            "/scratch/ul/projects/cdessimo/oma-browser",
+        ):
+            if os.path.isdir(folder):
+                test_data_available = True
+                break
+        if not test_data_available:
+            raise unittest.SkipTest("data not available")
+        os.environ["DARWIN_BROWSERDATA_PATH"] = os.path.join(
+            folder, "Test.Jul2014", "data"
+        )
 
-from .db import Database
-from .hogprofile.build import BaseProfileBuilderProcess, SourceProcess, Pipeline, Stage
 
-logger = logging.getLogger(__name__)
-MinHash256 = partial(MinHash, seed=1, num_perm=256)
-LeanMinHash256 = partial(LeanMinHash, seed=1)
-
-
-class HogHasher(object):
-    def __init__(self, db: Database):
-        self.db = db
-        self.xrefs = db.id_mapper["XRef"]
-
-    def analyze_fam(self, fam_nr):
-        members = self.db.member_of_fam(fam_nr)
-        minhashes = collections.defaultdict(MinHash256)
-        t_start = t0 = time.time()
-        for i, e in enumerate(members):
-            hog_id = e["OmaHOG"]
-            prot_id = e["CanonicalId"]
-            if len(prot_id) == e.dtype["CanonicalId"].itemsize:
-                # probably overflow, get full id from xref
-                for ref in self.xrefs.iter_xrefs_for_entry_nr(e["EntryNr"]):
-                    if ref["xref"].encode("utf-8").startswith(prot_id):
-                        prot_id = ref["xref"].encode("utf-8")
-                        break
-            for p in re.finditer(rb"\.", hog_id):
-                minhashes[hog_id[: p.start()]].update(prot_id)
-            minhashes[hog_id].update(prot_id)
-            if time.time() - t0 > 10:
-                logger.debug(
-                    f"working since {time.time()-t_start}sec on fam {fam_nr}. Done {i} out of {len(members)} proteins"
+class GenomeDirectImportTest(ImportIntegrationBase):
+    def compare_genomes_tab(self, data):
+        self.darwin_exporter.add_species_data()
+        gstab = self.darwin_exporter.h5.get_node("/Genome")
+        self.assertEqual(len(gstab), len(data["GS"]), "unexpected number of genomes")
+        for genome in data["GS"]:
+            gs = gstab.read_where(
+                "UniProtSpeciesCode == {!r}".format(genome[1].encode("utf-8"))
+            )
+            for key in (
+                (2, "TotEntries"),
+                (3, "TotAA"),
+                (0, "NCBITaxonId"),
+                (5, "SciName"),
+            ):
+                expected = genome[key[0]]
+                if isinstance(expected, str):
+                    expected = expected.encode("utf-8")
+                self.assertEqual(
+                    gs[key[1]],
+                    expected,
+                    "data doesn't match for {}: {} vs {}".format(
+                        key[0], gs[key[1]], expected
+                    ),
                 )
-                t0 = time.time()
-        return minhashes
+        taxtab = self.darwin_exporter.h5.get_node("/Taxonomy")
+        all_taxlevels = taxtab[:]
+        self.assertFalse(
+            numpy.where(all_taxlevels["NCBITaxonId"] == all_taxlevels["ParentTaxonId"])[
+                0
+            ].any(),
+            "must not have taxlevel pointing to itself",
+        )
 
+    def test_load_species_from_json(self):
+        data = self.darwin_exporter.call_darwin_export("GetGenomeData();")
+        json_fname = os.path.join(self.tmpdir, "pyoma", "gs.json")
+        store_in_json(data, json_fname)
+        self.compare_genomes_tab(data)
+        os.remove(json_fname)
+
+    def test_load_species_from_darwin(self):
+        data = self.darwin_exporter.call_darwin_export("GetGenomeData();")
+        self.compare_genomes_tab(data)
+
+
+class ProteinImportViaJson(ImportIntegrationBase):
+    @classmethod
+    def setUpClass(cls):
+        super(ProteinImportViaJson, cls).setUpClass()
+        data = callDarwinExport("GetGenomeData();")
+        json_fname = os.path.join(cls.tmpdir, "pyoma", "gs.json")
+        store_in_json(data, json_fname)
+
+    def test_add_proteins(self):
+        self.darwin_exporter.add_species_data()
+        self.darwin_exporter.add_proteins()
+
+        entry_tab = self.darwin_exporter.h5.get_node("/Protein/Entries")
+        sequence_tab = self.darwin_exporter.h5.get_node("/Protein/SequenceBuffer")
+        for i, e in enumerate(entry_tab):
+            self.assertEqual(
+                i + 1,
+                e["EntryNr"],
+                "entries are not ordered: {} - {}".format(i, e["EntryNr"]),
+            )
+            seq = sequence_tab[
+                e["SeqBufferOffset"] : e["SeqBufferOffset"] + e["SeqBufferLength"] - 1
+            ].tostring()
+            self.assertEqual(
+                md5(seq).hexdigest(),
+                e["MD5ProteinHash"].decode(),
+                "sequence hashes disagree for {}".format(e["EntryNr"]),
+            )
+
+    def test_get_version(self):
+        version = self.darwin_exporter.get_version()
+        self.assertIn("Test", version)
+        self.darwin_exporter.add_version()
+        self.assertEqual(
+            version, self.darwin_exporter.h5.get_node_attr("/", "oma_version")
+        )
 
-class LSHBuilder(object):
-    def __init__(self, hash_file, mode="r", threshold=0.7):
-        if mode not in ("r", "a", "w"):
-            raise ValueError("invalid mode string ``%s``. Allowed modes are: " "'r', 'a' and 'w'" % mode)
-        if mode == "r":
-            if not os.path.exists(hash_file):
-                raise IOError('file "{}" does not exist'.format(hash_file))
-            self.h5, self.lsh, self.hogid2row = self._load_hash_file(hash_file, mode)
-        elif mode == "a" and os.path.exists(hash_file):
-            self.h5, self.lsh, self.hogid2row = self._load_hash_file(hash_file, mode)
-        elif mode == "w" or mode == "a" and not os.path.exists(hash_file):
-            self.lsh = MinHashLSH(threshold=threshold, num_perm=256)
-            self.hogid2row = {}
-            self.h5 = self.init_hash_table_file(hash_file)
-        self.hashes = self.h5.get_node("/hashes")
-        self.hogids = self.h5.get_node("/hogids")
-        self.threshold = threshold
-        self._readonly = mode == "r"
-
-    def _open_hdf5(self, filename, mode="w"):
-        filters = None
-        if mode == "w":
-            filters = tables.Filters(complevel=1, complib="blosc", shuffle=True)
-        return tables.open_file(filename, mode=mode, filters=filters)
-
-    def init_hash_table_file(self, hash_file):
-        h5 = self._open_hdf5(hash_file, mode="w")
-        h5.create_earray("/", "hashes", atom=tables.Int64Atom(), shape=(0, 256), expectedrows=1e6)
-        h5.create_earray(
-            "/",
-            "hogids",
-            atom=tables.StringAtom(itemsize=255),
-            shape=(0,),
-            expectedrows=1e6,
-        )
-        h5.create_vlarray("/", "lsh_obj", atom=tables.ObjectAtom())
-        return h5
-
-    def _load_hash_file(self, hash_file, mode="r"):
-        h5 = self._open_hdf5(hash_file, mode=mode)
-        lsh_obj_arr = h5.get_node("/lsh_obj")
-        lsh = lsh_obj_arr[-2]
-        hogid2row = lsh_obj_arr[-1]
-        return h5, lsh, hogid2row
-
-    def close(self):
-        if self.h5.mode != "r":
-            lsh_obj_arr = self.h5.get_node("/lsh_obj")
-            lsh_obj_arr.append(self.lsh)
-            lsh_obj_arr.append(self.hogid2row)
-            self.hashes.flush()
-            self.hogids.flush()
-        self.h5.close()
-
-    def add_minhashes(self, it):
-        for hogid, minhash in it:
-            self.hashes.append([minhash.digest()])
-            self.hogids.append([hogid])
-        self.hashes.flush()
-        self.hogids.flush()
-
-    def compute_lsh(self):
-        lsh = MinHashLSH(threshold=self.threshold, num_perm=256)
-        hog2row = {}
-        for row, (hogid, hashvals) in enumerate(itertools.zip_longest(self.hogids, self.hashes)):
-            hog2row[hogid] = row
-            lsh.insert(hogid, LeanMinHash256(hashvalues=hashvals))
-        self.lsh = lsh
-        self.hogid2row = hog2row
-
-    def query(self, key, minhash):
-        """query with a minhash, returns a list of tuples of
-        (query-key, target-key, jaccard)"""
-        candidates = self.lsh.query(minhash)
-        for c in candidates:
-            hashvals = self.hashes[self.hogid2row[c]]
-            h = MinHash256(hashvalues=hashvals)
-            yield key, c, minhash.jaccard(h)
-
-
-class FamGenerator(SourceProcess):
-    def __init__(self, fam_generator=None, **kwargs):
-        super().__init__(**kwargs)
-        self.fams_to_process = fam_generator
-
-    def generate_data(self):
-        for fam in self.fams_to_process:
-            yield fam
-        logger.info("all families put to queue")
-
-
-class HashWorker(BaseProfileBuilderProcess):
-    def __init__(self, db_path, **kwargs):
-        super().__init__(**kwargs)
-        self.db_path = db_path
-        self.db = None
-        self.hasher = None
-        self.handled_queries = None
-
-    def setup(self):
-        self.db = Database(self.db_path)
-        self.hasher = HogHasher(self.db)
-        self.handled_queries = 0
-
-    def handle_input(self, fam):
-        logger.info("computing hashes for family %s", fam)
-        if self.handled_queries > 10000:
-            self.db.close()
-            logger.info("resetting database handle")
-            self.setup()
-        logger.info("start chewing on fam %s...", fam)
-        t0 = time.time()
-        hashes = self.hasher.analyze_fam(fam)
-        logger.info("... done with fam %s. Took %f sec", fam, time.time() - t0)
-        self.handled_queries += 1
-        return hashes
-
-    def finalize(self):
-        self.db.close()
-
-
-class Collector(BaseProfileBuilderProcess):
-    def __init__(self, output_path, **kwargs):
-        super().__init__(**kwargs)
-        self.output_path = output_path
-
-    def setup(self):
-        self.lsh_builder = LSHBuilder(self.output_path, mode="a")
-
-    def handle_input(self, hashes):
-        logger.info("build lsh for {} hashes ({})".format(len(hashes), next(iter(hashes))))
-        self.lsh_builder.add_minhashes(hashes.items())
-
-    def finalize(self):
-        self.lsh_builder.close()
-
-
-def generator_of_unprocessed_fams(db_path, lsh_path=None):
-    def _get_nr_families(db_path):
-        db = Database(db_path)
-        nr_hogs = db.get_nr_toplevel_hogs()
-        db.close()
-        logger.info("Found %d families to process", nr_hogs)
-        return nr_hogs
-
-    def _load_unprocessed_fams(db_path, lsh_path):
-        db = Database(db_path)
-        with tables.open_file(lsh_path, "r") as lsh_h5:
-            processed_fams = set(db.parse_hog_id(x) for x in lsh_h5.get_node("/hogids"))
-        remaining = set(range(1, db.get_nr_toplevel_hogs() + 1)) - processed_fams
-        db.close()
-        logger.info("Found %d unprocessed families", len(remaining))
-        return remaining
-
-    if lsh_path is None or not os.path.exists(lsh_path):
-        fams_to_process = range(1, _get_nr_families(db_path) + 1)
-    else:
-        fams_to_process = _load_unprocessed_fams(db_path, lsh_path)
-    return fams_to_process
-
-
-def compute_minhashes_for_db(db_path, output_path, nr_procs=None):
-    if nr_procs is None:
-        nr_procs = multiprocessing.cpu_count()
-
-    fams_to_process = generator_of_unprocessed_fams(db_path, output_path)
-    while True:
-        pipeline = Pipeline()
-        pipeline.add_stage(Stage(FamGenerator, nr_procs=1, fam_generator=fams_to_process))
-        pipeline.add_stage(Stage(HashWorker, nr_procs=nr_procs, db_path=db_path))
-        pipeline.add_stage(Stage(Collector, nr_procs=1, output_path=output_path))
-        print("setup pipeline, about to start it.")
-        pipeline.run()
-        print("finished with computing the MinHashLSH for {}".format(db_path))
-
-        fams_to_process = set(generator_of_unprocessed_fams(db_path, output_path))
-        if len(fams_to_process) == 0:
-            break
-    print("for sure all families processes. we're done!")
-
-
-def compare_versions(output_file, target_path, *old_path):
-    lsh = LSHBuilder(target_path, mode="r")
-    lsh.compute_lsh()
-    with tables.open_file(
-        output_file,
-        "w",
-        filters=tables.Filters(complevel=1, complib="blosc", shuffle=True),
-    ) as h5_map:
-        tab = h5_map.create_table(
-            "/",
-            "hogmap",
-            description=numpy.dtype([("Old", "S255"), ("New", "S255"), ("Jaccard", "f4")]),
+    def test_add_orthologs_from_darwin(self):
+        pass
+
+
+class OrthologyTypeTester(unittest.TestCase):
+    def setUp(self):
+        self._tmpdir = tempfile.mkdtemp()
+        self.exp = DarwinExporter(os.path.join(self._tmpdir, "test.h5"))
+        self.pw = self.exp.h5.create_table(
+            "/", "VPairs", tablefmt.PairwiseRelationTable
+        )
+
+    def test_convert_to_numpytable(self):
+        rels = [[1, 5], (2, 6)]
+        tab = self.exp._convert_to_numpyarray(rels, self.pw)
+        self.assertEqual(len(tab), 2)
+        # test that default value are used
+        self.assertTrue(numpy.all(tab["Distance"] == -1))
+
+    def test_orthology_type_inference(self):
+        genome_offs = numpy.array([0, 4, 9, 19])
+        rels = [
+            [1, 5],
+            [1, 6],
+            [1, 10],
+            [1, 20],
+            [2, 5],
+            [2, 6],
+            [2, 10],
+            [2, 11],
+            [3, 12],
+            [3, 21],
+            [3, 22],
+        ]
+        expected_rel_type = numpy.array([3, 3, 2, 0, 3, 3, 3, 1, 0, 1, 1])
+
+        reltab = self.exp._convert_to_numpyarray(rels, self.pw)
+        compute_ortholog_types(reltab, genome_offs)
+        self.assertTrue(numpy.array_equal(reltab["RelType"], expected_rel_type))
+
+    def tearDown(self):
+        self.exp.close()
+        shutil.rmtree(self._tmpdir)
+
+
+class TSVOrthologyFileTester(unittest.TestCase):
+    def setUp(self):
+        with tempfile.NamedTemporaryFile(suffix=".gz", delete=False) as fh:
+            self.datafile = fh.name
+
+    def tearDown(self):
+        try:
+            os.remove(self.datafile)
+        except OSError:
+            pass
+
+    def put_data_in_file(self, data):
+        with gzip.open(self.datafile, mode="wt", compresslevel=6) as cmp:
+            writer = csv.writer(cmp, delimiter=str("\t"))
+            for row in data:
+                writer.writerow(row)
+
+    def test_regular_example(self):
+        data = [
+            (1, 1, 12421, "1:1", 0.99, 1.523),
+            (2, 5, 21214, "n:1", 0.94, 12.14),
+            (3, 5, 23552, "n:1", 0.91, 21.2),
+        ]
+        self.put_data_in_file(data)
+        res = load_tsv_to_numpy((self.datafile, 0, 100, False))
+        self.assertEqual(3, res.size)
+        self.assertTrue((numpy.arange(1, 4) == res["EntryNr1"]).all())
+        self.assertTrue((numpy.array((101, 105, 105)) == res["EntryNr2"]).all())
+        self.assertTrue((numpy.array((0, 2, 2)) == res["RelType"]).all())
+        self.assertTrue(((res["Distance"] > 0) & (res["Distance"] < 22)).all())
+        self.assertTrue(
+            ((res["AlignmentOverlap"] > 0.9) & (res["AlignmentOverlap"] <= 1)).all()
+        )
+
+    def test_empty_file(self):
+        self.put_data_in_file([])
+        res = load_tsv_to_numpy((self.datafile, 0, 0, False))
+        self.assertEqual(0, res.size)
+
+
+class H5HelpersTests(ImportDummyBase):
+    @staticmethod
+    def get_table_data():
+        return numpy.array([(1, 9), (2, 11), (5, 21)], dtype=[("X", "i4"), ("Y", "u2")])
+
+    def setUp(self):
+        super(H5HelpersTests, self).setUp()
+        data = self.get_table_data()
+        self.darwin_exporter.h5.create_table("/", "Example", obj=data)
+
+    def test_create_table_if_needed_without_existing_table(self):
+        self.darwin_exporter.create_table_if_needed(
+            "/", "XRef2", description=self.get_table_data().dtype
         )
-        dubious = h5_map.create_earray(
+        self.assertEqual(0, len(self.darwin_exporter.h5.get_node("/XRef2")))
+
+    def test_create_table_if_needed_not_needed(self):
+        self.darwin_exporter.create_table_if_needed("/", "Example")
+        self.assertEqual(3, len(self.darwin_exporter.h5.get_node("/Example")))
+
+    def test_create_table_if_needed_replace_data(self):
+        data = self.get_table_data()
+        data["X"] *= 2
+        self.darwin_exporter.create_table_if_needed(
+            "/", "Example", obj=data, drop_data=True
+        )
+        res = self.darwin_exporter.h5.get_node("/Example").read()
+        numpy.testing.assert_equal(res, data)
+
+    def test_create_table_if_needed_append_data(self):
+        data = self.get_table_data()
+        data["X"] *= 2
+        expected = numpy.hstack((self.get_table_data(), data))
+        self.darwin_exporter.create_table_if_needed(
+            "/", "Example", obj=data, dump_data=False
+        )
+        res = self.darwin_exporter.h5.get_node("/Example").read()
+        numpy.testing.assert_equal(res, expected)
+
+
+class HogConverterTest(unittest.TestCase):
+    orthoxml_file = os.path.join(os.path.dirname(__file__), "hog-example.orthoXML")
+
+    def setUp(self):
+        self.h5 = tables.open_file(
+            "test", "w", driver="H5FD_CORE", driver_core_backing_store=0
+        )
+        self.h5.create_table(
             "/",
-            "dubious",
-            atom=tables.StringAtom(itemsize=255),
-            shape=(0,),
-            expectedrows=1e5,
-        )
-        for old in old_path:
-            old = LSHBuilder(old, mode="r")
-            for old_id, old_hashvals in tqdm(itertools.zip_longest(old.hogids, old.hashes), total=len(old.hogids)):
-                minhash = LeanMinHash256(hashvalues=old_hashvals)
-                candidates = sorted(lsh.query(old_id, minhash), key=lambda x: -x[2])
-                logger.debug("old_id: %s: candidates: %s", old_id, candidates)
-                if len(candidates) > 10 and candidates[6][2] > 0.9:
-                    # this is a dubious node, store it for now, maybe try to recover later.
-                    # it seems that this happens if the CanonicalId is truncated and hence maps to several ids.
-                    dubious.append([old_id])
-                    continue
-                if len(candidates) > 0 and candidates[0][2] > 0.6:
-                    tab.append([(old_id, candidates[0][1], candidates[0][2])])
-                    if candidates[0][2] < 1:
-                        other_cands = [(old_id, c[1], c[2]) for c in candidates[1:]]
-                        if len(other_cands) > 0:
-                            tab.append(other_cands)
-            tab.flush()
-            dubious.flush()
-            old.close()
-        # build index of Old ids
-        tab.colinstances["Old"].create_csindex()
-
-
-def build_lookup(target_db, old_dbs, nr_procs=None):
-    def lsh_fn_from_db_path(dbpath, modif=None):
-        dbname = os.path.splitext(os.path.basename(dbpath))[0]
-        modif_str = "-{}".format(modif) if modif is not None else ""
-        lsh_fn = "{}{}.hog-lsh.h5".format(dbname, modif_str)
-        return lsh_fn
-
-    target_lsh_fn = lsh_fn_from_db_path(target_db)
-    compute_minhashes_for_db(target_db, target_lsh_fn, nr_procs=nr_procs)
-
-    old_lsh_paths = []
-    for k, dbpath in enumerate(old_dbs):
-        cached_lsh_fn = dbpath.replace(".h5", ".hog-lsh.h5")
-        if not os.path.exists(cached_lsh_fn):
-            cached_lsh_fn = lsh_fn_from_db_path(dbpath, modif=k)
-            print("computing lsh for {} - storing in {}".format(dbpath, cached_lsh_fn))
-            compute_minhashes_for_db(dbpath, cached_lsh_fn, nr_procs=nr_procs)
-        old_lsh_paths.append(cached_lsh_fn)
+            "Entries",
+            tablefmt.ProteinTable,
+            obj=numpy.zeros(6, tables.dtype_from_descr(tablefmt.ProteinTable)),
+        )
 
-    hogmap_name = os.path.splitext(os.path.basename(target_db))[0] + ".hogmap.h5"
-    compare_versions(hogmap_name, target_lsh_fn, old_lsh_paths)
+    def test_extract_levels(self):
+        conv = HogConverter(self.h5.root.Entries)
+        levels = conv.convert_file(self.orthoxml_file)
+        self.assertEqual(9, len(levels), "levels is broken: {}".format(levels))
+        self.assertEqual(
+            len(tables.dtype_from_descr(tablefmt.HOGsTable)), len(levels[0])
+        )
+        mammalia = next((x for x in levels if x[2] == "Mammalia"), None)
+        self.assertAlmostEqual(
+            1, mammalia[3], msg="CompletenessScore not what is expected"
+        )
+        self.assertEqual(1, mammalia[4], "ImpliedLosses was not read from input xml")
+        rodents = [x for x in levels if x[2] == "Rodents"]
+        self.assertEqual(2, len(rodents), "expect 2 subhogs at level of Rodents")
+        self.assertEqual(
+            [1, 0.5], [z[3] for z in rodents], "CompletenessScore does not match"
+        )
```

### Comparing `pyoma-0.13.2/pyoma/browser/hogprofile/build.py` & `pyoma-0.9.4/pyoma/browser/hogprofile/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import functools
 import queue
-import signal
-import threading
-import uuid
-
 import tables
 import ete3
 import multiprocessing as mp
 import time
 import tempfile
 import pandas as pd
 from datasketch import WeightedMinHashGenerator, MinHashLSHForest
@@ -32,115 +28,73 @@
         full_tree = ete3.PhyloTree(tree_newick, format=1)
         self.tree = filter_tree(full_tree, root_node=taxmask, taxfilter=taxfilter)
         self.tree_newick = self.tree.write(format=1)
         self.taxa_index = taxa_index(self.tree)
         self.leaf_index = leaf_index(self.tree)
         self.tree_weights = generate_treeweights(self.tree, self.taxa_index)
         self.numperm = numperm
-        self.wmg = WeightedMinHashGenerator(3 * len(self.taxa_index), sample_size=numperm, seed=1)
+        self.wmg = WeightedMinHashGenerator(
+            3 * len(self.taxa_index), sample_size=numperm, seed=1
+        )
 
 
 class BaseProfileBuilderProcess(mp.Process):
     def __init__(
         self,
         in_queue: mp.Queue,
         out_queue: mp.Queue,
         nr_workers_pre_step: mp.Value,
         log_queue: mp.Queue,
-        control_queue: mp.Queue,
-        **kwargs,
+        **kwargs
     ):
         super().__init__(**kwargs)
         self.in_queue = in_queue
         self.out_queue = out_queue
         self.log_queue = log_queue
         self.outstanding_dones = nr_workers_pre_step
-        self.control_queue = control_queue
-        self.quit_req = False
-        self.proc_id = str(uuid.uuid4())
 
     def setup(self):
         pass
 
     def finalize(self):
         pass
 
-    def _handle_signal(self, signum, frame):
-        print("Stopping worker (pid: {}; name: {}): received signal {}".format(self.pid, self.name, signum))
-        self.quit_req = True
-
     def run(self):
         self.setup()
-        # Set signals for worker process
-        signal.signal(signal.SIGINT, self._handle_signal)
-        signal.signal(signal.SIGUSR2, self._handle_signal)
-        signal.signal(signal.SIGTERM, self._handle_signal)
-
-        nr_empty_cnt = 0
-        while not self.quit_req and self.outstanding_dones.value > 0:
+        while self.outstanding_dones.value > 0:
             try:
                 item = self.in_queue.get(timeout=1)
-                nr_empty_cnt = 0
             except queue.Empty:
-                nr_empty_cnt += 1
-                if nr_empty_cnt > 10:
-                    logger.info(
-                        "input queue seems to be empty ({}x), but expecting still some chunks".format(nr_empty_cnt)
-                    )
-                self.control_queue.put((self.proc_id, "NO WORK"))
                 continue
 
             if item is None:
-                logger.info("received sentinel from previous pipeline step")
                 with self.outstanding_dones.get_lock():
                     self.outstanding_dones.value -= 1
-                logger.info("outstanding_dones: %s", self.outstanding_dones)
-                self.control_queue.put((self.proc_id, "DONE"))
-                logger.debug("sent DONE info to control queue (%s)", self.proc_id)
             else:
                 result = self.handle_input(item)
                 if result is not None:
                     self.out_queue.put(result)
-                self.control_queue.put((self.proc_id, "JOB_HANDELED"))
-        if not self.quit_req:
-            self.out_queue.put(None)  # signal end of work for this worker
-            logger.info("sent sentinel to next stage")
-        else:
-            logger.info("received termination signal")
+        self.out_queue.put(None)  # signal end of work for this worker
         self.finalize()
 
     def handle_input(self, item):
         raise NotImplementedError("This method must be overwritten")
 
 
 class SourceProcess(BaseProfileBuilderProcess):
     def __init__(self, out_queue, **kwargs):
-        super().__init__(in_queue=None, out_queue=out_queue, nr_workers_pre_step=None, **kwargs)
-
-    def _put_in_queue_with_status(self, input):
-        while True:
-            try:
-                self.out_queue.put(input, timeout=5)
-                break
-            except queue.Full:
-                qsize = "?"
-                try:
-                    qsize = self.out_queue.qsize()
-                except NotImplementedError:
-                    pass
-                logger.info("Queue full. (approx size: {}) Cannot put item {} into output queue".format(qsize, input))
-            self.control_queue.put((self.proc_id, "ALIVE"))
+        super().__init__(
+            in_queue=None, out_queue=out_queue, nr_workers_pre_step=None, **kwargs
+        )
 
     def run(self):
         self.setup()
         for input in self.generate_data():
-            self._put_in_queue_with_status(input)
+            self.out_queue.put(input)
         self.out_queue.put(None)
-        self.control_queue.put((self.proc_id, "DONE"))
-        logger.info("sent sentinel to next stage")
         self.finalize()
 
     def generate_data(self):
         raise NotImplementedError("SourceProcess should implement this method")
 
 
 class ProfileBuilder(BaseProfileBuilderProcess):
@@ -151,15 +105,17 @@
         self.ham_pipeline = None
         self.hash_pipeline = None
 
     def setup(self):
         from ..db import Database
 
         self.builder = LSHBuilderBase(db=Database(self.db_path))
-        self.ham_pipeline = functools.partial(get_ham_treemap_from_row, tree=self.builder.tree_newick)
+        self.ham_pipeline = functools.partial(
+            get_ham_treemap_from_row, tree=self.builder.tree_newick
+        )
         self.hash_pipeline = functools.partial(
             row2hash,
             taxa_index=self.builder.taxa_index,
             species_index=self.builder.leaf_index,
             treeweights=self.builder.tree_weights,
             wmg=self.builder.wmg,
         )
@@ -167,15 +123,17 @@
 
     def finalize(self):
         self.builder.db.close()
 
     def handle_input(self, df):
         print("handling df: {}".format(df))
         df["tree"] = df[["Fam", "ortho"]].apply(self.ham_pipeline, axis=1)
-        df[["hash", "rows", "species"]] = df[["Fam", "tree"]].apply(self.hash_pipeline, axis=1)
+        df[["hash", "rows", "species"]] = df[["Fam", "tree"]].apply(
+            self.hash_pipeline, axis=1
+        )
         return df[["Fam", "hash", "species"]]
 
 
 class Collector(BaseProfileBuilderProcess):
     def __init__(self, db_path, tmp_file, **kwargs):
         super().__init__(**kwargs)
         self.tmp_file = tmp_file
@@ -188,40 +146,40 @@
             "hashes",
             createparents=True,
             atom=tables.Int64Atom(),
             shape=(
                 self.builder.db.get_nr_toplevel_hogs() + 1,
                 self.builder.numperm * 2,
             ),
-            filters=tables.Filters(complevel=3, complib="blosc"),
+            filters=tables.Filters(complevel=3, complib="blosc", fletcher32=True),
         )
         species = self.h5.create_carray(
             root,
             "species_profile",
             createparents=True,
             atom=tables.Int8Atom(),
             shape=(
                 self.builder.db.get_nr_toplevel_hogs() + 1,
                 len(self.builder.leaf_index),
             ),
-            filters=tables.Filters(complevel=3, complib="blosc"),
+            filters=tables.Filters(complevel=3, complib="blosc", fletcher32=True),
         )
         lsh_forest = self.h5.create_vlarray(
             root,
             "min_hash_lsh_forest",
             createparents=True,
             atom=tables.ObjectAtom(),
-            filters=tables.Filters(complevel=3, complib="blosc"),
+            filters=tables.Filters(complevel=3, complib="blosc", fletcher32=True),
         )
         lsh_tree = self.h5.create_vlarray(
             root,
             "species_tree",
             createparents=True,
             atom=tables.ObjectAtom(),
-            filters=tables.Filters(complevel=3, complib="blosc"),
+            filters=tables.Filters(complevel=3, complib="blosc", fletcher32=True),
         )
         lsh_tree.append(self.builder.tree)
         self.h5.set_node_attr(root, "num_perm", self.builder.numperm)
         return hashes, species, lsh_forest
 
     def setup(self):
         from ..db import Database
@@ -233,29 +191,33 @@
         self.forest = MinHashLSHForest(num_perm=self.builder.numperm)
         self.h5 = tables.open_file(self.tmp_file, "w")
         root = "/HOGProfile/ALL"
         # if self.builder.tree.name != "0":
         #     root = "/HOGProfile/{}".format(self.builder.tree.name)
         print("storing results in {}:{}".format(self.tmp_file, root))
 
-        self.hashes_matrix, self.species_matrix, self.forest_arr = self._init_tmp_h5(root)
+        self.hashes_matrix, self.species_matrix, self.forest_arr = self._init_tmp_h5(
+            root
+        )
         print("Collector process initialized")
 
     def handle_input(self, df: pd.DataFrame):
         print("handling hash df: {}".format(df))
         if not df.empty:
             hashes = df["hash"].to_dict()
             hashes = {fam: hashes[fam] for fam in hashes if hashes[fam]}
             for fam, hashvals in hashes.items():
                 self.forest.add(str(fam), hashvals)
                 self.hashes_matrix[fam, :] = hashvals.hashvalues.ravel()
                 self.species_matrix[fam, :] = df["species"][fam]
                 self.count += 1
             if time.time() - self.save_start > 200:
-                print("Saving current results: {}".format(time.time() - self.global_time))
+                print(
+                    "Saving current results: {}".format(time.time() - self.global_time)
+                )
                 self.forest.index()
                 print(
                     "Checking consistency of search index. Fam {} --> {}".format(
                         fam, self.forest.query(hashes[fam], k=10)
                     )
                 )
                 self.save_start = time.time()
@@ -271,28 +233,30 @@
         self.h5.flush()
         self.h5.close()
         self.builder.db.close()
         print("stored all data in temporary file")
 
 
 class HogGenerator(SourceProcess):
-    def __init__(self, db_path, max_hogsize=None, min_hogsize=100, chunk_size=100, **kwargs):
+    def __init__(
+        self, db_path, max_hogsize=None, min_hogsize=100, chunk_size=100, **kwargs
+    ):
         super().__init__(**kwargs)
         self.db_path = db_path
         self.max_hogsize = max_hogsize
         self.min_hogsize = min_hogsize
         self.chunk_size = chunk_size
 
     def generate_data(self):
         from ..db import Database
 
         db = Database(self.db_path)
         nr_groups = db.get_nr_toplevel_hogs()
         chunk = {}
-        logger.debug("nr of toplevel hogs: %d", nr_groups)
+        logger.debug("nr of toplevel hogs: {}".format(nr_groups))
         for fam in range(1, nr_groups + 1):
             try:
                 orthoxml = db.get_orthoxml(fam).decode()
             except ValueError as e:
                 continue
             nr_species = orthoxml.count("<species name=")
             if (self.max_hogsize is None or nr_species < self.max_hogsize) and (
@@ -320,83 +284,25 @@
     root.addHandler(h)
     root.setLevel(logging.DEBUG)
 
 
 def logger_listener(log_queue):
     root = logging.getLogger()
     console_handler = logging.StreamHandler()
-    formatter = logging.Formatter("%(asctime)s %(processName)-10s %(name)s %(levelname)-8s %(message)s")
+    formatter = logging.Formatter(
+        "%(asctime)s %(processName)-10s %(name)s %(levelname)-8s %(message)s"
+    )
     console_handler.setFormatter(formatter)
     root.addHandler(console_handler)
     root.setLevel(logging.DEBUG)
     for record in iter(log_queue.get, None):
         logger = logging.getLogger(record.name)
         logger.handle(record)
 
 
-class PipelineControllerThread(threading.Thread):
-    def __init__(self, control_queue, log_queue, processes, time_until_kill=1800, **kwargs):
-        super().__init__(**kwargs)
-        self.control_queue = control_queue
-        self.log_queue = log_queue
-        self.processes = {p.proc_id: [0, p] for p in processes}
-        self.time_until_kill = time_until_kill
-        self._last_timeout_check = time.time()
-
-    def _process_alive_info(self, item):
-        proc_id, flag = item
-        logger.debug(item)
-        if flag == "DONE":
-            self.processes.pop(proc_id)
-        else:
-            self.processes[proc_id][0] = time.time()
-
-    def _kill_orphan_procs(self):
-        to_rem = []
-        for proc_id, proc_info in self.processes.items():
-            last_seen, proc = proc_info[0], proc_info[1]
-            if last_seen == 0:
-                logger.info("process %s[%s] not yet started?", proc.name, proc.proc_id)
-            elif time.time() - last_seen > self.time_until_kill:
-                logger.warning(
-                    "process %s[%s] seems to be dead. No alive signal since %fsec.",
-                    proc.name,
-                    proc.proc_id,
-                    time.time() - last_seen,
-                )
-                proc.terminate()
-                proc.out_queue.put(None)
-                to_rem.append(proc_id)
-        for proc_id in to_rem:
-            self.processes.pop(proc_id)
-        logger.info("killed %d orphan processes", len(to_rem))
-
-    def run(self):
-        logger.info("starting controler thread")
-        nr_empty_cnt = 0
-        while len(self.processes) > 0:
-            try:
-                item = self.control_queue.get(timeout=30)
-                nr_empty_cnt = 0
-                if item is None:
-                    break  # None indicates end of pipeline
-                self._process_alive_info(item)
-            except queue.Empty:
-                nr_empty_cnt += 1
-                if nr_empty_cnt > 10:
-                    logger.info(
-                        "control queue seems to be empty ({}x), but expecting still some running jobs".format(
-                            nr_empty_cnt
-                        )
-                    )
-            if time.time() - self._last_timeout_check > 10:
-                self._kill_orphan_procs()
-                self._last_timeout_check = time.time()
-
-
 class Stage(object):
     def __init__(self, process, nr_procs, **kwargs):
         self.process = process
         self.nr_procs = nr_procs
         self.kwargs = kwargs
         self.outstanding_dones = None
         self.in_queue = None
@@ -412,60 +318,48 @@
 
     def run(self):
         log_queue = mp.Queue()
         logger_process = mp.Process(target=logger_listener, args=(log_queue,))
         logger_process.start()
         rootlogger_configurer(log_queue)
         print("setting up pipeline")
-        control_queue = mp.Queue()
 
         procs = []
         for i in range(len(self.stages) - 1, 0, -1):
             stage = self.stages[i]
             stage.outstanding_dones = mp.Value("d", self.stages[i - 1].nr_procs)
             stage.in_queue = mp.Queue(maxsize=10 * mp.cpu_count())
-            stage.out_queue = self.stages[i + 1].in_queue if i < len(self.stages) - 1 else mp.Queue()
+            stage.out_queue = (
+                self.stages[i + 1].in_queue if i < len(self.stages) - 1 else mp.Queue()
+            )
             for k in range(stage.nr_procs):
                 p = stage.process(
                     in_queue=stage.in_queue,
                     out_queue=stage.out_queue,
                     nr_workers_pre_step=stage.outstanding_dones,
                     log_queue=log_queue,
-                    control_queue=control_queue,
                     daemon=True,
-                    **stage.kwargs,
+                    **stage.kwargs
                 )
                 procs.append(p)
                 p.start()
         # add source process
         stage = self.stages[0]
         stage.out_queue = self.stages[1].in_queue
         for k in range(stage.nr_procs):
             p = stage.process(
-                out_queue=stage.out_queue,
-                log_queue=log_queue,
-                control_queue=control_queue,
-                **stage.kwargs,
+                out_queue=stage.out_queue, log_queue=log_queue, **stage.kwargs
             )
             procs.append(p)
             p.start()
-        control_thread = PipelineControllerThread(control_queue=control_queue, log_queue=log_queue, processes=procs)
-        control_thread.start()
         print("all processes started")
-        try:
-            for p in procs:
-                p.join()
-        except KeyboardInterrupt:
-            print("keyboard interupt in main loop")
-            time.sleep(20)
+        for p in procs:
+            p.join()
         log_queue.put(None)
-        control_queue.put(None)
         logger_process.join()
-        control_thread.join()
-
         print("successfully joined all processes")
 
 
 def compute_profiles(db_path, min_hogsize=100, max_hogsize=None, nr_procs=None):
     pipeline = Pipeline()
     with tempfile.NamedTemporaryFile(suffix=".h5", delete=False) as h5_tmp:
         tmp_file = h5_tmp.name
```

### Comparing `pyoma-0.13.2/pyoma/browser/hogprofile/hashutils.py` & `pyoma-0.9.4/pyoma/browser/hogprofile/hashutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,30 @@
     :param treeweights: a vector of weights for each tax levels
     :param wmg: Datasketch weighted minhash generator
     :return hog_matrix: a vector of weights for each tax level
     :return weighted_hash: a weighted minhash of a HOG
 
     """
 
-    losses = [taxa_index[n.name] for n in tp.traverse() if n.lost and n.name in taxa_index]
-    dupl = [taxa_index[n.name] for n in tp.traverse() if n.dupl and n.name in taxa_index]
-    presence = [taxa_index[n.name] for n in tp.traverse() if n.nbr_genes > 0 and n.name in taxa_index]
-    covered_species = [species_index[n.name] for n in tp.iter_leaves() if n.nbr_genes > 0 and n.name in species_index]
+    losses = [
+        taxa_index[n.name] for n in tp.traverse() if n.lost and n.name in taxa_index
+    ]
+    dupl = [
+        taxa_index[n.name] for n in tp.traverse() if n.dupl and n.name in taxa_index
+    ]
+    presence = [
+        taxa_index[n.name]
+        for n in tp.traverse()
+        if n.nbr_genes > 0 and n.name in taxa_index
+    ]
+    covered_species = [
+        species_index[n.name]
+        for n in tp.iter_leaves()
+        if n.nbr_genes > 0 and n.name in species_index
+    ]
     indices = dict(zip(["presence", "loss", "dup"], [presence, losses, dupl]))
     hog_matrix_weighted = np.zeros((1, 3 * len(taxa_index)))
     hog_matrix_binary = np.zeros((1, 3 * len(taxa_index)))
     species_matrix = np.zeros(len(species_index))
     species_matrix[covered_species] = 1
     for i, event in enumerate(indices):
         if len(indices[event]) > 0:
@@ -59,9 +71,13 @@
     :param treeweights: a vector of weights for each tax levels
     :param wmg: Datasketch weighted minhash generator
     :return: hog_matrix: a vector of weights for each tax level
     :return: weighted_hash: a weighted minhash of a HOG
     """
     # convert a dataframe row to a weighted minhash
     fam, treemap = row.tolist()
-    hog_matrix, weighted_hash, species_matrix = hash_tree_profile(treemap, taxa_index, species_index, treeweights, wmg)
-    return pd.Series([weighted_hash, hog_matrix, species_matrix], index=["hash", "rows", "species"])
+    hog_matrix, weighted_hash, species_matrix = hash_tree_profile(
+        treemap, taxa_index, species_index, treeweights, wmg
+    )
+    return pd.Series(
+        [weighted_hash, hog_matrix, species_matrix], index=["hash", "rows", "species"]
+    )
```

### Comparing `pyoma-0.13.2/pyoma/browser/hogprofile/pyhamutils.py` & `pyoma-0.9.4/pyoma/browser/hogprofile/pyhamutils.py`

 * *Files identical despite different names*

### Comparing `pyoma-0.13.2/pyoma/browser/hogprofile/query.py` & `pyoma-0.9.4/pyoma/browser/hogprofile/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     def __init__(self, db):
         root_level_data = db.get_hdf5_handle().get_node("/HOGProfile/ALL")
         self.db = db  # backref
         self.forest = root_level_data.min_hash_lsh_forest[0]
         self.hashes = root_level_data.hashes
         self.species_profile = root_level_data.species_profile
         self.species_tree = root_level_data.species_tree[0]
-        self.num_perm = db.get_hdf5_handle().get_node_attr("/HOGProfile/ALL", "num_perm")
+        self.num_perm = db.get_hdf5_handle().get_node_attr(
+            "/HOGProfile/ALL", "num_perm"
+        )
         self.species_names = self._build_tree_range_lookup()
         self.tax_range_index = self._select_key_levels_and_ranges()
 
     def _map_taxid_to_name(self, taxid):
         if int(taxid) == 0:
             return "LUCA"
         tax_row = self.db.tax._taxon_from_numeric(int(taxid))
@@ -48,28 +50,32 @@
                 for child in node.children:
                     idx_map(child)
                     if child.range[0] < min_range:
                         min_range = child.range[0]
                     if child.range[1] > max_range:
                         max_range = child.range[1]
                     size += child.size
-                node.add_features(range=(min_range, max_range), size=size, sciname=sciname)
+                node.add_features(
+                    range=(min_range, max_range), size=size, sciname=sciname
+                )
 
         # annotate speciestree with range features
         idx_map(self.species_tree)
         return species_names
 
     def _select_key_levels_and_ranges(self):
         def nodes_of_size(node, size):
             for n in node.iter_leaves(is_leaf_fn=lambda n: size >= n.size > 0.1 * size):
                 yield n
 
         indexes = {}
         for size in (50, 200):
-            indexes[size] = {n.sciname: n.range for n in nodes_of_size(self.species_tree, size)}
+            indexes[size] = {
+                n.sciname: n.range for n in nodes_of_size(self.species_tree, size)
+            }
         indexes["root"] = {n.sciname: n.range for n in self.species_tree.children}
         return indexes
 
     def query(self, fam_nr, k=50):
         """Query the database for similar hogs than fam_nr.
 
         :param int fam_nr: numeric root family
```

### Comparing `pyoma-0.13.2/pyoma/browser/hogprofile/tree_helper.py` & `pyoma-0.9.4/pyoma/browser/hogprofile/tree_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         children = []
         for child in node["children"]:
             children.append(rec(child))
         return "({}){}".format(",".join(children), node["id"])
 
     def get_duplicates(node):
         c = collections.Counter(x["id"] for x in traverse(node))
-        return list(item[0] for item in itertools.takewhile(lambda x: x[1] > 1, c.most_common()))
+        return list(
+            item[0] for item in itertools.takewhile(lambda x: x[1] > 1, c.most_common())
+        )
 
     def rename_internal_duplicates(node, duplicates):
         for n in traverse(node):
             if n["id"] in duplicates and "children" in n:
                 n["id"] = "{}Rep".format(n["id"])
 
     taxdict = tax.as_dict()
```

### Comparing `pyoma-0.13.2/pyoma/browser/homoeologs.py` & `pyoma-0.9.4/pyoma/browser/homoeologs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import pandas
 import logging
 import collections
 import numpy as np
+import matplotlib
+
+matplotlib.use("agg")
 from skfuzzy import control as ctrl
 from skfuzzy import gaussmf
 import sklearn
 import sklearn.preprocessing
 import tables
 
 try:
@@ -13,26 +16,32 @@
 except ImportError:
     tqdm = lambda x, **kwargs: x
 logger = logging.getLogger(__name__)
 
 
 def define_universe(df):
     # New Antecedent/Consequent objects hold universe variables and membership functions
-    distance = ctrl.Antecedent(np.arange(0, df["Distance"].max() + 0.01, 0.01), "distance")
+    distance = ctrl.Antecedent(
+        np.arange(0, df["Distance"].max() + 0.01, 0.01), "distance"
+    )
     synteny = ctrl.Antecedent(np.arange(0, 1.01, 0.01), "synteny_score")
-    total_nb_hom = ctrl.Antecedent(np.arange(2, df["TotalCopyNr"].max() + 1, 1), "total_nb_homoeologs")
+    total_nb_hom = ctrl.Antecedent(
+        np.arange(2, df["TotalCopyNr"].max() + 1, 1), "total_nb_homoeologs"
+    )
     conf = ctrl.Consequent(np.arange(0, 101, 1), "conf")
     return distance, synteny, total_nb_hom, conf
 
 
 def create_fuzzy_rules(distance, synteny, total_nb_hom, conf):
     """Takes the antecedent and consequent objects as input"""
 
     # very low confidence
-    rule1 = ctrl.Rule(synteny["low"] & distance["high"] & total_nb_hom["high"], conf["very_low"])
+    rule1 = ctrl.Rule(
+        synteny["low"] & distance["high"] & total_nb_hom["high"], conf["very_low"]
+    )
 
     # low confidence
     rule2 = ctrl.Rule(
         (synteny["low"] & distance["high"] & total_nb_hom["low"])
         | (synteny["low"] & distance["high"] & total_nb_hom["med"])
         | (synteny["low"] & distance["med"] & total_nb_hom["high"])
         | (synteny["med"] & distance["high"] & total_nb_hom["high"]),
@@ -67,25 +76,31 @@
         | (synteny["med"] & distance["low"] & total_nb_hom["high"])
         | (synteny["med"] & distance["low"] & total_nb_hom["med"])
         | (synteny["med"] & distance["low"] & total_nb_hom["low"]),
         conf["high"],
     )
 
     # very high confidence
-    rule5 = ctrl.Rule(synteny["high"] & distance["low"] & total_nb_hom["low"], conf["very_high"])
+    rule5 = ctrl.Rule(
+        synteny["high"] & distance["low"] & total_nb_hom["low"], conf["very_high"]
+    )
     return [rule1, rule2, rule3, rule4, rule5]
 
 
 def get_distance_mf(df, distance):
     # here, the first numnber is the universe, second number the central point, third the standard deviation
     distance["low"] = gaussmf(distance.universe, 0, (df["Distance"].max() / 10))
 
-    distance["med"] = gaussmf(distance.universe, (df["Distance"].max() / 4), (df["Distance"].max() / 10))
+    distance["med"] = gaussmf(
+        distance.universe, (df["Distance"].max() / 4), (df["Distance"].max() / 10)
+    )
 
-    distance["high"] = gaussmf(distance.universe, df["Distance"].max(), (df["Distance"].max() / 2.5))
+    distance["high"] = gaussmf(
+        distance.universe, df["Distance"].max(), (df["Distance"].max() / 2.5)
+    )
     return distance
 
 
 def get_synteny_mf(df, synteny, view=False):
     # synteny (gaussian)
     synteny["low"] = gaussmf(synteny.universe, 0, 0.15)
     synteny["med"] = gaussmf(synteny.universe, 0.3, 0.15)
@@ -93,17 +108,21 @@
     return synteny
 
 
 def get_total_nb_hom_mf(df, total_nb_hom):
     copy_nr_median = df["TotalCopyNr"].median()
     total_nb_hom["low"] = gaussmf(total_nb_hom.universe, copy_nr_median, copy_nr_median)
 
-    total_nb_hom["med"] = gaussmf(total_nb_hom.universe, 4 * copy_nr_median, 1.5 * copy_nr_median)
+    total_nb_hom["med"] = gaussmf(
+        total_nb_hom.universe, 4 * copy_nr_median, 1.5 * copy_nr_median
+    )
 
-    total_nb_hom["high"] = gaussmf(total_nb_hom.universe, df["TotalCopyNr"].max(), df["TotalCopyNr"].max() / 2.5)
+    total_nb_hom["high"] = gaussmf(
+        total_nb_hom.universe, df["TotalCopyNr"].max(), df["TotalCopyNr"].max() / 2.5
+    )
     return total_nb_hom
 
 
 def get_conf_mf(df, conf):
     # confidence (gaussian)
     conf["very_low"] = gaussmf(conf.universe, 0, 20)
     conf["low"] = gaussmf(conf.universe, 50, 10)
@@ -129,47 +148,59 @@
         self.h5_handle = h5_handle
         self.genome = genome
         if isinstance(h5_handle, tables.File):
             self.h5_handle = h5_handle
         elif isinstance(h5_handle, (str, bytes)):
             self.h5_handle = tables.open_file(h5_handle, "r")
         else:
-            raise TypeError("expected h5_handle to be either h5-file handle or a path to file")
+            raise TypeError(
+                "expected h5_handle to be either h5-file handle or a path to file"
+            )
 
-        genome_row = next(self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome"))
+        genome_row = next(
+            self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome")
+        )
         self.genome_range = (
             int(genome_row["EntryOff"]) + 1,
             int(genome_row["EntryOff"] + genome_row["TotEntries"]),
         )
         genome_df = pandas.DataFrame(
             self.h5_handle.root.Protein.Entries.read_where(
                 "(EntryNr >= {}) & (EntryNr <= {})".format(*self.genome_range)
             )
         )
         self.genome_df = genome_df[
-            (genome_df["AltSpliceVariant"] == 0) | (genome_df["AltSpliceVariant"] == genome_df["EntryNr"])
+            (genome_df["AltSpliceVariant"] == 0)
+            | (genome_df["AltSpliceVariant"] == genome_df["EntryNr"])
         ]
         self.genome_df.reset_index(inplace=True)
         self.relations_df = self._load_pairwise_relations()
 
     def _load_pairwise_relations(self):
         """load the homoeologous relations of the cannonical splice variants only
         The method returns a pandas dataframe with the relations."""
         df = pandas.DataFrame(
-            self.h5_handle.get_node("/PairwiseRelation/{}/within".format(self.genome)).read_where("RelType == 5")
-        )
-        df = df[df["EntryNr1"].isin(self.genome_df["EntryNr"]) & df["EntryNr2"].isin(self.genome_df["EntryNr"])]
+            self.h5_handle.get_node(
+                "/PairwiseRelation/{}/within".format(self.genome)
+            ).read_where("RelType == 5")
+        )
+        df = df[
+            df["EntryNr1"].isin(self.genome_df["EntryNr"])
+            & df["EntryNr2"].isin(self.genome_df["EntryNr"])
+        ]
         return df[self.fields_to_load]
 
     def _count_homeologs_per_entry(self, df):
         return collections.Counter(df["EntryNr1"])
 
     def _augment_dataframe_with_all_features(self, df):
         counts = self._count_homeologs_per_entry(df)
-        df["TotalCopyNr"] = df.apply(lambda x: counts[x["EntryNr1"]] + counts[x["EntryNr2"]], axis=1)
+        df["TotalCopyNr"] = df.apply(
+            lambda x: counts[x["EntryNr1"]] + counts[x["EntryNr2"]], axis=1
+        )
         df.loc[df.SyntenyConservationLocal < 0, "SyntenyConservationLocal"] = 0
         return df
 
     def calculate_scores(self):
         # load dataframe
         df = self.relations_df
         df = self._augment_dataframe_with_all_features(df)
@@ -194,16 +225,20 @@
                     "total_nb_homoeologs": row["TotalCopyNr"],
                 },
             )
 
         df["fuzzy_confidence"] = df.apply(defuzzify, axis=1)
 
         # scale the confidence between minimum value and 100
-        min_max_scaler = sklearn.preprocessing.MinMaxScaler(feature_range=(df["fuzzy_confidence"].min(), 100))
-        df["fuzzy_confidence_scaled"] = min_max_scaler.fit_transform(df["fuzzy_confidence"].values.reshape(-1, 1))
+        min_max_scaler = sklearn.preprocessing.MinMaxScaler(
+            feature_range=(df["fuzzy_confidence"].min(), 100)
+        )
+        df["fuzzy_confidence_scaled"] = min_max_scaler.fit_transform(
+            df["fuzzy_confidence"].values.reshape(-1, 1)
+        )
         return df
 
     def augment_ids(self, df, keep=None):
         xref_tab = self.h5_handle.root.XRef
         xrefs = pandas.DataFrame(
             xref_tab.read_where(
                 "(EntryNr >= {}) & (EntryNr <= {}) & (XRefSource == {})".format(
@@ -215,26 +250,34 @@
         )
         xrefs.drop(columns=["XRefSource", "Verification"], inplace=True)
         xrefs["XRefId"] = xrefs["XRefId"].str.decode("utf-8")
 
         if keep is None or keep == "first":
             xrefs_one_ref = xrefs.drop_duplicates(subset="EntryNr", keep="first")
         elif keep == "agg":
-            xrefs_one_ref = xrefs.groupby("EntryNr")["XRefId"].agg(lambda x: "; ".join(x.values)).to_frame()
+            xrefs_one_ref = (
+                xrefs.groupby("EntryNr")["XRefId"]
+                .agg(lambda x: "; ".join(x.values))
+                .to_frame()
+            )
         else:
             raise ValueError('argument "keep" must be either "first" or "agg"')
         new_df = pandas.merge(
-            pandas.merge(df, xrefs_one_ref, how="left", left_on="EntryNr1", right_on="EntryNr"),
+            pandas.merge(
+                df, xrefs_one_ref, how="left", left_on="EntryNr1", right_on="EntryNr"
+            ),
             xrefs_one_ref,
             how="left",
             left_on="EntryNr2",
             right_on="EntryNr",
         )
         new_df.drop(columns=["EntryNr_x", "EntryNr_y"], inplace=True, errors="ignore")
-        new_df.rename(columns={"XRefId_x": "SourceID1", "XRefId_y": "SourceID2"}, inplace=True)
+        new_df.rename(
+            columns={"XRefId_x": "SourceID1", "XRefId_y": "SourceID2"}, inplace=True
+        )
         return new_df
 
 
 class HomeologsConfidenceCalculatorFromTSV(HomeologsConfidenceCalculator):
     def __init__(self, infile):
         self.relations_df = pandas.read_csv(infile, sep="\t")
         expected_columns = [
@@ -261,16 +304,20 @@
         self.genome = genome
         self.kwargs = kwargs
         if isinstance(h5_handle, tables.File):
             self.h5_handle = h5_handle
         elif isinstance(h5_handle, (str, bytes)):
             self.h5_handle = tables.open_file(h5_handle, "r")
         else:
-            raise TypeError("expected h5_handle to be either h5-file handle or a path to file")
-        self.genome_row = next(self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome"))
+            raise TypeError(
+                "expected h5_handle to be either h5-file handle or a path to file"
+            )
+        self.genome_row = next(
+            self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome")
+        )
         self.genome_range = (
             int(self.genome_row["EntryOff"]) + 1,
             int(self.genome_row["EntryOff"] + self.genome_row["TotEntries"]),
         )
 
     def dedup_homoeolog_df(self, df):
         """Removes the double (inverse) homoeolog pairs from the table"""
@@ -294,36 +341,41 @@
         # Get all the entries of our genome and remove alternative splice variants
         entries_df = pandas.DataFrame(
             self.h5_handle.root.Protein.Entries.read_where(
                 "(EntryNr >= {}) & (EntryNr <= {})".format(*self.genome_range)
             )
         )
         entries_df = entries_df[
-            (entries_df["AltSpliceVariant"] == 0) | (entries_df["AltSpliceVariant"] == entries_df["EntryNr"])
+            (entries_df["AltSpliceVariant"] == 0)
+            | (entries_df["AltSpliceVariant"] == entries_df["EntryNr"])
         ]
 
         return entries_df
 
     def get_homoeolog_pairs_df(self, genome):
         # Create a dataframe containing only the homoeologs
         df = pandas.DataFrame(
-            self.h5_handle.get_node("/PairwiseRelation/{}/within".format(self.genome)).read_where("RelType == 5")
+            self.h5_handle.get_node(
+                "/PairwiseRelation/{}/within".format(self.genome)
+            ).read_where("RelType == 5")
         )
         return df
 
     def get_gene_info_for_homeologs(self, entries_df, homoeolog_pairs_df):
         # Merge with entries_df to get protein lengths, chromosomes, subgenomes for each entry
         df = pandas.merge(
             homoeolog_pairs_df,
             entries_df,
             how="left",
             left_on=["EntryNr1"],
             right_on=["EntryNr"],
         )
-        df = pandas.merge(df, entries_df, how="left", left_on=["EntryNr2"], right_on=["EntryNr"])
+        df = pandas.merge(
+            df, entries_df, how="left", left_on=["EntryNr2"], right_on=["EntryNr"]
+        )
         return df
 
     def decode_df(self, df):
         columns = df.columns
         for column in columns:
             try:
                 df[column] = df[column].str.decode("utf-8")
@@ -377,22 +429,27 @@
             right_on=["entrynr1", "entrynr2"],
         )
         df.drop(["entrynr1", "entrynr2"], 1, inplace=True)
         return df
 
     def add_copynr(self, df):
         counts = collections.Counter(df["EntryNr1"])
-        df["TotalCopyNr"] = df.apply(lambda x: counts[x["EntryNr1"]] + counts[x["EntryNr2"]], axis=1)
+        df["TotalCopyNr"] = df.apply(
+            lambda x: counts[x["EntryNr1"]] + counts[x["EntryNr2"]], axis=1
+        )
         return df
 
     def get_final_homoeolog_df(self):
         entries_df = self.get_entries_df()
         hom_df = self.get_homoeolog_pairs_df(self.genome)
         # remove ASVs
-        df = hom_df[hom_df["EntryNr1"].isin(entries_df["EntryNr"]) & hom_df["EntryNr2"].isin(entries_df["EntryNr"])]
+        df = hom_df[
+            hom_df["EntryNr1"].isin(entries_df["EntryNr"])
+            & hom_df["EntryNr2"].isin(entries_df["EntryNr"])
+        ]
         # add number of duplications
         homObj = HomeologsConfidenceCalculator(self.h5_handle, self.genome)
         df = self.add_copynr(df)
         # Merge with entries_df to get protein lengths, chromosomes, subgenomes for each entry
         df = self.get_gene_info_for_homeologs(entries_df, df)
         df = self._rename_and_remove_columns(df)
         df = self.decode_df(df)
@@ -406,35 +463,42 @@
             return df
 
 
 if __name__ == "__main__":
     import argparse
 
     # Get arguments from command line
-    parser = argparse.ArgumentParser(description="Computes homoeology confidence score using fuzzy logic")
+    parser = argparse.ArgumentParser(
+        description="Computes homoeology confidence score using fuzzy logic"
+    )
     grp = parser.add_mutually_exclusive_group(required=True)
     grp.add_argument("--h5", help="name of hdf5 file, full path")
-    grp.add_argument("--csv", help="tab-separated file with input data as alternative to hdf5 file")
+    grp.add_argument(
+        "--csv", help="tab-separated file with input data as alternative to hdf5 file"
+    )
     parser.add_argument(
         "--genome",
-        help="5 letter code of polyploid genome to analyze. " "Must be specified if used with --h5 option.",
+        help="5 letter code of polyploid genome to analyze. "
+        "Must be specified if used with --h5 option.",
     )
     parser.add_argument(
         "--outfile",
         help="name where results will be stored (file name created to include parameters)",
         default="homoeolog_confidence.tsv",
     )
 
     args = parser.parse_args()
     logging.basicConfig(level=logging.INFO)
 
     if args.h5 is not None and args.genome is None:
         import sys
 
-        sys.stderr.write("genomes argument required if using with an hdf5 file as input")
+        sys.stderr.write(
+            "genomes argument required if using with an hdf5 file as input"
+        )
         sys.exit(1)
 
     if args.h5:
         import tables
 
         scorer = HomeologsConfidenceCalculator(tables.open_file(args.h5), args.genome)
     else:
```

### Comparing `pyoma-0.13.2/pyoma/browser/linkout.py` & `pyoma-0.9.4/pyoma/browser/linkout.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,29 @@
         self._add_doctype()
 
     def root_children(self):
         return {}
 
     def _add_doctype(self):
         self.tree.docinfo.public_id = "-//NLM//DTD LinkOut 1.0//EN"
-        self.tree.docinfo.system_url = "https://www.ncbi.nlm.nih.gov/projects/linkout/doc/LinkOut.dtd"
+        self.tree.docinfo.system_url = (
+            "https://www.ncbi.nlm.nih.gov/projects/linkout/doc/LinkOut.dtd"
+        )
 
     def text_elemement(self, tag, text):
         el = etree.Element(tag)
         el.text = text
         return el
 
     def write(self, fh):
-        fh.write(etree.tostring(self.tree, pretty_print=True, xml_declaration=True, encoding="utf-8"))
+        fh.write(
+            etree.tostring(
+                self.tree, pretty_print=True, xml_declaration=True, encoding="utf-8"
+            )
+        )
 
 
 class Provider(NCBILinkOutXML):
     root_node = "Provider"
 
     def root_children(self):
         elements = collections.OrderedDict(
@@ -176,16 +182,20 @@
 
     @classmethod
     def set_link_offset(cls, off):
         cls.link_id = off
 
 
 class LinkoutBuffer(object):
-    def __init__(self, resource, outdir="/tmp", bulk_add=True, max_file_size=20 * 2**20):
-        self.max_records = math.floor((max_file_size - resource.DISKSIZE_HEADER) / resource.DISKSIZE_PER_LINK)
+    def __init__(
+        self, resource, outdir="/tmp", bulk_add=True, max_file_size=20 * 2 ** 20
+    ):
+        self.max_records = math.floor(
+            (max_file_size - resource.DISKSIZE_HEADER) / resource.DISKSIZE_PER_LINK
+        )
         self.cur_nr = 0
         self.buf = []
         self.bulk_add = bulk_add
         self.resource_type = resource
         self.outdir = outdir
         logger.info(
             "Setup Linkout buffer for {} with max {} records ({}bytes) per file, bulk_add={}".format(
@@ -201,28 +211,32 @@
     def flush(self):
         res = self.resource_type()
         if self.bulk_add:
             res.add_link(self.buf)
         else:
             for obj in self.buf:
                 res.add_link(obj)
-        fn = os.path.join(self.outdir, "{}_{:02d}.xml".format(res.base_name, self.cur_nr))
+        fn = os.path.join(
+            self.outdir, "{}_{:02d}.xml".format(res.base_name, self.cur_nr)
+        )
         with open(fn, "wb") as fh:
             res.write(fh)
         self.cur_nr += 1
         self.buf = []
 
 
 class GenesPriorizationHandler(object):
     """Adapter to LinkoutBuffer to select only a limited number of crossrefs.
     NCBI linkout caps at 10%"""
 
     def __init__(self, max_linkouts=None, db=None, **kwargs):
-        self.max_links = int(max_linkouts) if max_linkouts else 20357436 // 10  # obtained in Jan2018
-        logger.info("Limiting Genes to %d links max", self.max_links)
+        self.max_links = (
+            int(max_linkouts) if max_linkouts else 20357436 // 10
+        )  # obtained in Jan2018
+        logger.info("Limiting Genes to {} links max".format(self.max_links))
         self.genes_buffer = LinkoutBuffer(GenesResource, **kwargs)
         self.genes = []
         self.db = db
 
     def add(self, key, value):
         self.genes.append((key, value))
 
@@ -275,20 +289,20 @@
         for link_acc, link_target in self.genes[0 : self.max_links]:
             self.genes_buffer.add({link_acc: link_target})
         self.genes_buffer.flush()
 
         c = collections.defaultdict(int)
         for acc, target in self.genes[self.max_links :]:
             c[target[0:5]] += 1
-        logger.info("Skipping genes link in the following species: %s", c)
+        logger.info("Skipping genes link in the following species: {}".format(c))
 
 
 def prepare_linkout_files(outdir="/tmp", infile="../pyomabrowser/OmaServer.h5"):
     prov = Provider()
-    with open(os.path.join(outdir, "providerinfo.xml"), "wb") as fh:
+    with open(os.path.join(outdir, "provider.xml"), "wb") as fh:
         prov.write(fh)
 
     db = Database(infile)
     xrefs = db.get_hdf5_handle().get_node("/XRef")
     xref_source_enum = xrefs.get_enum("XRefSource")
 
     protein_buffer = LinkoutBuffer(ProteinResource, outdir=outdir, bulk_add=True)
```

### Comparing `pyoma-0.13.2/pyoma/browser/locus_parser.py` & `pyoma-0.9.4/pyoma/browser/locus_parser.py`

 * *Files identical despite different names*

### Comparing `pyoma-0.13.2/pyoma/browser/sanitychecks.py` & `pyoma-0.9.4/pyoma/browser/sanitychecks.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         genomes = [x.decode("utf-8") for x in genomes]
         return genomes
 
     def get_omagroups(self):
         """get the number of genes in each oma group and returns a dictionary/Counter
         object that key: oma group id, value: number of genes in this oma group
         """
-        omagroups = Counter((x["OmaGroup"] for x in self.entries_table.where("OmaGroup!=0")))
+        omagroups = Counter(
+            (x["OmaGroup"] for x in self.entries_table.where("OmaGroup!=0"))
+        )
         return omagroups
 
     def get_all_lvls(self):
         """get all taxonomic levels"""
         return [x["Level"] for x in self.hoglevel_table.iterrows()]
 
     def get_all_hogs(self):
@@ -94,32 +96,43 @@
         result["release"] = self.release
         return result
 
     def num_hogs_per_level(self):
         """get the number of hogs for a list of taxa levels"""
         result = ""
         for taxa in self.all_lvls:
-            result += str(taxa.decode("utf-8")) + "\t" + self.release + "\t" + str(self.all_hog_lvls.get(taxa)) + "\n"
+            result += (
+                str(taxa.decode("utf-8"))
+                + "\t"
+                + self.release
+                + "\t"
+                + str(self.all_hog_lvls.get(taxa))
+                + "\n"
+            )
             result = re.sub(r"None", "", result)
         return result
 
     def get_number_of_xrefs_per_species(self):
         """load all the xrefs we have of each type and species"""
         xreftab = self.h5_handle.root.XRef
         enum = xreftab.get_enum("XRefSource")
         genomes = self.h5_handle.root.Genome.read()
         sorter = genomes.argsort(order=("EntryOff"))
 
         def map_to_species(entry_nrs):
-            idx = genomes["EntryOff"].searchsorted(entry_nrs - 1, side="right", sorter=sorter)
+            idx = genomes["EntryOff"].searchsorted(
+                entry_nrs - 1, side="right", sorter=sorter
+            )
             return genomes[idx - 1]["UniProtSpeciesCode"]
 
         cnts = Counter()
         chunksize = xreftab.chunkshape[0]
-        for start in tqdm(range(0, len(xreftab), chunksize), desc="processing xref-chunks"):
+        for start in tqdm(
+            range(0, len(xreftab), chunksize), desc="processing xref-chunks"
+        ):
             chunk = xreftab.read(start, start + chunksize)
             orgs = map_to_species(chunk["EntryNr"])
             for org, xref_instance in zip(orgs, chunk):
                 cnts[(org, enum(xref_instance["XRefSource"]))] += 1
         df = pd.DataFrame(
             [(org.decode(), source, counts) for (org, source), counts in cnts.items()],
             columns=["Species", "Source", "Counts"],
```

### Comparing `pyoma-0.13.2/pyoma/browser/suffixsearch.py` & `pyoma-0.9.4/pyoma/browser/suffixsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 from __future__ import division, print_function, absolute_import, unicode_literals
 
-import functools
 import time
 from builtins import bytes, str, range, str
 from bisect import bisect_left
 import os
 import numpy
 import tables
 from .models import KeyWrapper
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class SuffixIndexBuilderStringCol(object):
-    MEM_PER_CHUNK = 50 * 2**20
+    MEM_PER_CHUNK = 50 * 2 ** 20
 
     def __init__(self, tab, col, index_group, ignore_case):
         if not isinstance(tab, tables.Table):
             raise ValueError("tab argument must be a tables.Table object")
         if col not in tab.colnames:
             raise ValueError("column '{}' does not exist in {}".format(col, tab))
         self.h5 = tab._v_file
         self.tab = tab
         self.col = col
-        self.index_group = index_group if isinstance(index_group, tables.Group) else self.h5.get_node(index_group)
+        self.index_group = (
+            index_group
+            if isinstance(index_group, tables.Group)
+            else self.h5.get_node(index_group)
+        )
         self.ignore_case = ignore_case
 
     def check_column_types_or_raise(self):
         if not numpy.issubdtype(self.tab.coldtypes[self.col].type, numpy.bytes_):
-            raise TypeError("column '{}' must be a character type column".format(self.col))
+            raise TypeError(
+                "column '{}' must be a character type column".format(self.col)
+            )
 
     def get_expected_index_length(self):
         return self.tab.coldtypes[self.col].itemsize * len(self.tab)
 
     def _arrayname(self, kind):
         return self.col + "_" + kind
 
     def _remove_aux_arrays(self):
         for kind in ("suffix", "buffer", "offset"):
             try:
                 n = self.get_aux_array_handle(kind)
                 index_group_path = self.index_group._v_pathname
-                if os.path.commonprefix([index_group_path, n._v_pathname]) == index_group_path:
+                if (
+                    os.path.commonprefix([index_group_path, n._v_pathname])
+                    == index_group_path
+                ):
                     # auxilary buffer hangs on the index_group. we can remove it
-                    logger.info("removing existing auxillary node: {}".format(n._v_pathname))
+                    logger.info(
+                        "removing existing auxillary node: {}".format(n._v_pathname)
+                    )
                     n.remove()
                     try:
                         self.h5.del_node_attr(self.index_group, self._arrayname(kind))
                     except AttributeError:
                         pass
             except tables.NoSuchNodeError:
                 pass
 
     def create_aux_arrays(self):
         for kind, typ in (
             ("buffer", tables.StringAtom(1)),
             ("offset", tables.UInt32Atom()),
         ):
             arr_name = self._arrayname(kind)
-            exp_rows = self.get_expected_index_length() if kind == "buffer" else len(self.tab)
-            arr = self.h5.create_earray(self.index_group, arr_name, typ, (0,), expectedrows=exp_rows)
+            exp_rows = (
+                self.get_expected_index_length() if kind == "buffer" else len(self.tab)
+            )
+            arr = self.h5.create_earray(
+                self.index_group, arr_name, typ, (0,), expectedrows=exp_rows
+            )
             self.h5.set_node_attr(self.index_group, arr_name, arr._v_pathname)
 
     def get_aux_array_handle(self, kind):
         if kind not in ("buffer", "offset", "suffix"):
             raise ValueError("Not a valid handle for suffix index")
         attr = self._arrayname(kind)
         try:
@@ -72,126 +86,151 @@
         except AttributeError:
             raise tables.NoSuchNodeError("'{}' does not exist".format(attr))
         return self.h5.get_node(path)
 
     def build_index_buffer(self):
         chunksize = int(self.MEM_PER_CHUNK / self.tab.coldtypes[self.col].itemsize)
         total_offset = 0
-        buffer, offset = (self.get_aux_array_handle(kind) for kind in ("buffer", "offset"))
+        buffer, offset = (
+            self.get_aux_array_handle(kind) for kind in ("buffer", "offset")
+        )
         for chunk_start in range(0, len(self.tab), chunksize):
             # load fixed width string col in numpy array, compute actual string lengths and build
             # a \x00 delimited buffer of all values
-            col_data = self.tab.read(start=chunk_start, stop=chunk_start + chunksize, field=self.col)
+            col_data = self.tab.read(
+                start=chunk_start, stop=chunk_start + chunksize, field=self.col
+            )
             data_lens = numpy.char.str_len(col_data)
             data_as_long_arr = col_data.view("S1")
             tot_len = (data_lens + 1).sum()
             buf = numpy.zeros(tot_len, dtype="S1")
             t = (data_lens + 1).cumsum()
             starts = numpy.roll(t, 1)
             starts[0] = 0
             ends = t - 1
             stride = col_data.strides[0]
             for i in range(len(col_data)):
-                buf[starts[i] : ends[i]] = data_as_long_arr[(stride * i) : (stride * i + data_lens[i])]
+                buf[starts[i] : ends[i]] = data_as_long_arr[
+                    (stride * i) : (stride * i + data_lens[i])
+                ]
             if self.ignore_case:
                 buf = numpy.char.lower(buf)
             # update global offset and append chunked buffer
             starts += total_offset
             buffer.append(buf)
             offset.append(starts)
             total_offset += tot_len
 
     def build_suffix_array(self):
         from PySAIS import sais
 
         data = self.get_aux_array_handle("buffer")[:]
-        suffix = sais(data) if len(data) > 0 else data
-        arr = self.h5.create_earray(self.index_group, self._arrayname("suffix"), obj=suffix)
-        self.h5.set_node_attr(self.index_group, self._arrayname("suffix"), arr._v_pathname)
-        self.h5.set_node_attr(self.index_group, self.col + "_ignore_case", self.ignore_case)
-        self.h5.set_node_attr(self.tab, self.col + "_suffixindexnode", self.index_group._v_pathname)
+        suffix = sais(data)
+        arr = self.h5.create_carray(
+            self.index_group, self._arrayname("suffix"), obj=suffix
+        )
+        self.h5.set_node_attr(
+            self.index_group, self._arrayname("suffix"), arr._v_pathname
+        )
+        self.h5.set_node_attr(
+            self.index_group, self.col + "_ignore_case", self.ignore_case
+        )
+        self.h5.set_node_attr(
+            self.tab, self.col + "_suffixindexnode", self.index_group._v_pathname
+        )
 
     def __call__(self, force=True):
         self.check_column_types_or_raise()
         if force:
             self._remove_aux_arrays()
         self.create_aux_arrays()
         self.build_index_buffer()
         self.build_suffix_array()
 
 
 class SuffixIndexBuilderVarStringCol(SuffixIndexBuilderStringCol):
     def __init__(self, tab, col, buffer, index_group, ignore_case):
         if not isinstance(buffer, tables.CArray):
             raise TypeError("buffer argument must be a tables.CArray instance")
-        super(SuffixIndexBuilderVarStringCol, self).__init__(tab, col, index_group, ignore_case)
+        super(SuffixIndexBuilderVarStringCol, self).__init__(
+            tab, col, index_group, ignore_case
+        )
         self.orig_buffer = buffer
 
     def check_column_types_or_raise(self):
         if not numpy.issubdtype(self.orig_buffer.dtype.type, numpy.bytes_):
-            raise TypeError("buffer '{}' must be a character type column".format(self.orig_buffer._v_pathname))
+            raise TypeError(
+                "buffer '{}' must be a character type column".format(
+                    self.orig_buffer._v_pathname
+                )
+            )
         if not numpy.issubdtype(self.tab.coldtypes[self.col].type, numpy.integer):
             raise TypeError(
                 "column '{}' must be an integer argument with offsets into the '{}' buffer array".format(
                     self.col, self.orig_buffer._v_pathname
                 )
             )
 
     def get_expected_index_length(self):
-        return len(self.orig_buffer) + len(self.tab)  # extra char per row for delimiting
+        return len(self.orig_buffer) + len(
+            self.tab
+        )  # extra char per row for delimiting
 
     def create_aux_arrays(self):
         for kind, typ in (
             ("buffer", tables.StringAtom(1)),
             ("offset", tables.UInt32Atom()),
         ):
             arr_name = self._arrayname(kind)
             if not self.ignore_case and kind == "buffer":
-                self.h5.set_node_attr(self.index_group, arr_name, self.orig_buffer._v_pathname)
+                self.h5.set_node_attr(
+                    self.index_group, arr_name, self.orig_buffer._v_pathname
+                )
             else:
-                exp_rows = self.get_expected_index_length() if kind == "buffer" else len(self.tab)
-                arr = self.h5.create_earray(self.index_group, arr_name, typ, (0,), expectedrows=exp_rows)
+                exp_rows = (
+                    self.get_expected_index_length()
+                    if kind == "buffer"
+                    else len(self.tab)
+                )
+                arr = self.h5.create_earray(
+                    self.index_group, arr_name, typ, (0,), expectedrows=exp_rows
+                )
                 self.h5.set_node_attr(self.index_group, arr_name, arr._v_pathname)
 
     def build_index_buffer(self):
         off_data = self.h5.get_node(self.tab).read(field=self.col)
-        # first, we need to fix cases where off_data is 0 in the middle of an array,
-        # simply because it has not been set as its length is also 0. We do this
-        # by setting the offsets to the next starting offset of a non-zero length
-        # entry (by copying the next value from the back)
-        # set every zero position except [0] to the one following in the buffer,
-        # in case the buffer ends with an uninitialized value, set it to the
-        # length of the entire buffer.
-        if off_data[-1] == 0:
-            off_data[-1] = len(self.orig_buffer)
-            # if now off_data[-1] is still 0, then there is actually no buffer data at all
-            if off_data[-1] == 0:
-                off_arr = self.get_aux_array_handle("offset")
-                off_arr.append(off_data)
-                return
-        zero_positions = numpy.where(off_data == 0)[0]
-        for idx in zero_positions[:0:-1]:
-            off_data[idx] = off_data[idx + 1]
-
         if self.ignore_case:
             starts = off_data
+            # first, we need to fix cases where starts is 0 in the middle of an array,
+            # simply because it has not been set as its length is also 0. We do this
+            # by setting the offsets to the next starting offset of a non-zero length
+            # entry (by copying the next value from the back)
+            zero_positions = numpy.where(starts == 0)[0]
+            for idx in zero_positions[
+                :0:-1
+            ]:  # skip position 0, as this is the true value there
+                starts[idx] = starts[idx + 1]
             # now, set the stop position by using the next start postion (shift array by 1)
             stops = numpy.roll(off_data, -1)
             stops[-1] = len(self.orig_buffer)
             buf_arr = self.get_aux_array_handle("buffer")
-            CHUNKSIZE = 2**22  # 4MB
+            CHUNKSIZE = 2 ** 22  # 4MB
             tmp_buf = numpy.zeros(CHUNKSIZE, dtype="S1")
             tmp_buf_idx = 0
             for i in range(len(off_data)):
                 if stops[i] - starts[i] + tmp_buf_idx >= CHUNKSIZE:
                     buf_arr.append(numpy.char.lower(tmp_buf[0:tmp_buf_idx]))
                     tmp_buf = numpy.zeros(CHUNKSIZE, dtype="S1")
                     tmp_buf_idx = 0
-                tmp_buf[tmp_buf_idx : (tmp_buf_idx + stops[i] - starts[i])] = self.orig_buffer[starts[i] : stops[i]]
-                tmp_buf_idx += stops[i] - starts[i] + 1  # keep one extra '\x00' as separator
+                tmp_buf[
+                    tmp_buf_idx : (tmp_buf_idx + stops[i] - starts[i])
+                ] = self.orig_buffer[starts[i] : stops[i]]
+                tmp_buf_idx += (
+                    stops[i] - starts[i] + 1
+                )  # keep one extra '\x00' as separator
             if tmp_buf_idx > 0:
                 buf_arr.append(numpy.char.lower(tmp_buf[0:tmp_buf_idx]))
             # add one extra position to each string that contains a '\x00'
             off_data += numpy.arange(0, len(off_data), 1, dtype=off_data.dtype)
 
         off_arr = self.get_aux_array_handle("offset")
         off_arr.append(off_data)
@@ -206,15 +245,17 @@
 
     try:
         return f.get_node(idx_prefix, name=idx_name)
     except tables.NoSuchNodeError:
         return f.create_group(idx_prefix, idx_name)
 
 
-def create_suffix_index(tab, col, buffer=None, index_group=None, ignore_case=True, force=False):
+def create_suffix_index(
+    tab, col, buffer=None, index_group=None, ignore_case=True, force=False
+):
     """Create a suffix array from the given table column (or buffer).
 
     This function creates for a given fix-width char column a suffix array for
     fast lookup of (partial) matches. In this case, the `buffer` argument
     should be None. Alternatively, if a index should be build from a variable
     length column, i.e. a buffer array with offset and length attributes in
     the table, one should pass the offset column as `col` argument and the
@@ -234,36 +275,44 @@
     :param str col: the name the column to be indexed
     :param buffer: handle to buffer array
     :param str index_group: path to existing or non-existing group node
         where index data will be stored.
     :param bool ignore_case: case insensitive lookup
     :param force: overwrite existing suffix array data"""
     if not isinstance(tab, tables.Table):
-        raise TypeError("tab arguments must be a tables.Table (is a {})".format(type(tab)))
+        raise TypeError(
+            "tab arguments must be a tables.Table (is a {})".format(type(tab))
+        )
     if not isinstance(col, str) or col not in tab.colnames:
         raise ValueError("table {} does not have a column named '{}'".format(tab, col))
     typ = tab.coldtypes[col]
     if numpy.issubdtype(typ.type, numpy.bytes_):
         if typ.itemsize < 3:
-            raise TypeError("suffix arrays should be created for longer string columns only")
+            raise TypeError(
+                "suffix arrays should be created for longer string columns only"
+            )
         suffixbuilder = SuffixIndexBuilderStringCol(
             tab,
             col,
             create_or_load_index_group(tab, index_group),
             ignore_case=ignore_case,
         )
     elif numpy.issubdtype(typ.type, numpy.integer):
         if buffer is None:
             raise ValueError("buffer array must be specified for numeric table columns")
         if isinstance(buffer, str):
             buffer = tab._v_file.get_node(buffer)
         if not (
-            isinstance(buffer, tables.CArray) and numpy.issubdtype(buffer, numpy.bytes_) and buffer.dtype.itemsize == 1
+            isinstance(buffer, tables.CArray)
+            and numpy.issubdtype(buffer, numpy.bytes_)
+            and buffer.dtype.itemsize == 1
         ):
-            raise TypeError("buffer array must by a character tables.CArray instance (itemsize == 1)")
+            raise TypeError(
+                "buffer array must by a character tables.CArray instance (itemsize == 1)"
+            )
         suffixbuilder = SuffixIndexBuilderVarStringCol(
             tab,
             col,
             buffer,
             create_or_load_index_group(tab, index_group),
             ignore_case=ignore_case,
         )
@@ -276,21 +325,27 @@
     @classmethod
     def from_tablecolumn(cls, table, column, ignore_case=False):
         h5 = table._v_file
         try:
             idx_node = h5.get_node_attr(table, column + "_suffixindexnode")
             idx_node = h5.get_node(idx_node)
         except (AttributeError, tables.NoSuchNodeError) as e:
-            raise SuffixIndexError("Column {} of table {} does not seem to have a suffix index".format(column, table))
+            raise SuffixIndexError(
+                "Column {} of table {} does not seem to have a suffix index".format(
+                    column, table
+                )
+            )
         try:
             suffix_arr = h5.get_node(idx_node, column + "_suffix")
             buffer_arr = h5.get_node(h5.get_node_attr(idx_node, column + "_buffer"))
             offset_arr = h5.get_node(h5.get_node_attr(idx_node, column + "_offset"))
         except (tables.NoSuchNodeError, AttributeError) as e:
-            raise SuffixIndexInconsitency("not all suffix index elements available: {}".format(e))
+            raise SuffixIndexInconsitency(
+                "not all suffix index elements available: {}".format(e)
+            )
         try:
             ignore_case = bool(h5.get_node_attr(idx_node, column + "_ignore_case"))
         except AttributeError:
             ignore_case = False
         return cls(suffix_arr, buffer_arr, offset_arr, ignore_case)
 
     @classmethod
@@ -304,55 +359,55 @@
             raise TypeError("expected a tables.Group node pointing to the index")
         try:
             buffer_arr = buffer if buffer else index_node._f_get_child("buffer")
             suffix_arr = index_node._f_get_child("suffix")
             offset_arr = offset if offset else index_node._f_get_child("offset")
             return cls(suffix_arr, buffer_arr, offset_arr, ignore_case=True)
         except tables.NoSuchNodeError as e:
-            raise SuffixIndexInconsitency("suffix array data missing: {}".format(e))
+            raise SuffixIndexInconsitency("suffix array data missing: {}".formate(e))
 
     def __init__(self, suffix, buffer, offset, ignore_case):
         self.suffix_arr = suffix
         self.buffer_arr = buffer
         self.offset_arr = offset[:]
         self.ignore_case = bool(ignore_case)
 
-    @functools.lru_cache(maxsize=16)
-    def _get_index_range(self, query):
+    def find(self, query):
         if isinstance(query, str):
             query = query.encode("utf-8")
         if self.ignore_case:
             query = query.lower()
         n = len(query)
         if n > 0:
-            slicer = KeyWrapper(self.suffix_arr, key=lambda i: self.buffer_arr[i : (i + n)].tobytes())
+            slicer = KeyWrapper(
+                self.suffix_arr, key=lambda i: self.buffer_arr[i : (i + n)].tobytes()
+            )
+            t0 = time.time()
             ii = bisect_left(slicer, query)
+            t1 = time.time()
             if ii and ii < len(self.suffix_arr) and (slicer[ii] == query):
                 query_after = query[:-1] + chr(query[-1] + 1).encode("utf-8")
                 jj = bisect_left(slicer, query_after)
-                if (jj < len(self.suffix_arr) and slicer[jj] == query) or (slicer[jj - 1] != query):
+                if (jj < len(self.suffix_arr) and slicer[jj] == query) or slicer[
+                    jj - 1
+                ] != query:
                     raise RuntimeError("index broken, should not happen")
-                return slice(ii, jj)
-        return slice(0, 0)
-
-    def count(self, query):
-        index_range = self._get_index_range(query)
-        return index_range.stop - index_range.start
-
-    def find(self, query, limit=None):
-        index_range = self._get_index_range(query)
-        if index_range.stop - index_range.start == 0:
-            return numpy.array([], self.offset_arr.dtype)
-
-        if limit is not None:
-            index_range = slice(index_range.start, min(index_range.stop, index_range.start + limit))
-
-        # Find row numbers
-        res = numpy.searchsorted(self.offset_arr, self.suffix_arr[index_range] + 1) - 1
-        return res
+                t2 = time.time()
+                # Find row numbers
+                res = (
+                    numpy.searchsorted(self.offset_arr, self.suffix_arr[ii:jj] + 1) - 1
+                )
+                t3 = time.time()
+                logger.debug(
+                    "SuffixIndex.find({}) bisect: {}, zoom: {}, extract: {} --> {}rows".format(
+                        query, t1 - t0, t2 - t1, t3 - t2, len(res)
+                    )
+                )
+                return res
+        return []
 
 
 class SuffixIndexError(Exception):
     pass
 
 
 class SuffixIndexInconsitency(SuffixIndexError):
```

### Comparing `pyoma-0.13.2/pyoma/browser/synteny.py` & `pyoma-0.9.4/pyoma/browser/synteny.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,54 +15,69 @@
         self.genome = genome
         self.windowsize = windowsize
         if isinstance(h5_handle, tables.File):
             self.h5_handle = h5_handle
         elif isinstance(h5_handle, (str, bytes)):
             self.h5_handle = tables.open_file(h5_handle, "r")
         else:
-            raise TypeError("expected h5_handle to be either h5-file handle or a path to file")
+            raise TypeError(
+                "expected h5_handle to be either h5-file handle or a path to file"
+            )
 
-        genome_row = next(self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome"))
+        genome_row = next(
+            self.h5_handle.root.Genome.where("UniProtSpeciesCode == genome")
+        )
         self.genome_range = (
             int(genome_row["EntryOff"]) + 1,
             int(genome_row["EntryOff"] + genome_row["TotEntries"]),
         )
         genome_df = pandas.DataFrame(
             self.h5_handle.root.Protein.Entries.read_where(
                 "(EntryNr >= {}) & (EntryNr <= {})".format(*self.genome_range)
             )
         )
         self.genome_df = genome_df[
-            (genome_df["AltSpliceVariant"] == 0) | (genome_df["AltSpliceVariant"] == genome_df["EntryNr"])
+            (genome_df["AltSpliceVariant"] == 0)
+            | (genome_df["AltSpliceVariant"] == genome_df["EntryNr"])
         ]
         self.genome_df.reset_index(inplace=True)
         self.relations_df = self._load_pairwise_relations()
 
     def _load_pairwise_relations(self):
         df = pandas.DataFrame(
-            self.h5_handle.get_node("/PairwiseRelation/{}/within".format(self.genome)).read_where("RelType == 5")
+            self.h5_handle.get_node(
+                "/PairwiseRelation/{}/within".format(self.genome)
+            ).read_where("RelType == 5")
         )
         return df[["EntryNr1", "EntryNr2", "SyntenyConservationLocal"]]
 
     def get_neighbor_genes(self, query):
         q = self.genome_df[self.genome_df["EntryNr"] == query]
         if len(q) == 0:
-            logger.error("querying neighbor genes for non-primary variant (EntryNr: {})".format(query))
+            logger.error(
+                "querying neighbor genes for non-primary variant (EntryNr: {})".format(
+                    query
+                )
+            )
             return []
         query_chr = q["Chromosome"]
         neighbor = self.genome_df[
-            max(0, q.index.item() - self.windowsize // 2) : q.index.item() + self.windowsize // 2 + 1
+            max(0, q.index.item() - self.windowsize // 2) : q.index.item()
+            + self.windowsize // 2
+            + 1
         ]
         return neighbor[neighbor["Chromosome"] == query_chr.item()]
 
     def score_of_pair(self, entry1, entry2):
         neigh1 = self.get_neighbor_genes(entry1)
         neigh2 = self.get_neighbor_genes(entry2)
         if len(neigh1) <= 1 or len(neigh2) <= 1:
-            raise TooSmallChromosome("too few genes on chromosome: {}, {}".format(len(neigh1), len(neigh2)))
+            raise TooSmallChromosome(
+                "too few genes on chromosome: {}, {}".format(len(neigh1), len(neigh2))
+            )
 
         rels_among_windows = self.relations_df[
             (self.relations_df["EntryNr1"] >= neigh1.iloc[0]["EntryNr"])
             & (self.relations_df["EntryNr1"] <= neigh1.iloc[-1]["EntryNr"])
             & (self.relations_df["EntryNr2"] >= neigh2.iloc[0]["EntryNr"])
             & (self.relations_df["EntryNr2"] <= neigh2.iloc[-1]["EntryNr"])
         ]
@@ -80,19 +95,25 @@
             "synteny_score_2": score2,
             "mean_synteny_score": (score1 + score2) / 2,
         }
         return res
 
     def compute_scores(self):
         res = []
-        for idx, rel in tqdm(self.relations_df.iterrows(), total=len(self.relations_df)):
+        for idx, rel in tqdm(
+            self.relations_df.iterrows(), total=len(self.relations_df)
+        ):
             try:
                 res.append(self.score_of_pair(rel["EntryNr1"], rel["EntryNr2"]))
             except TooSmallChromosome as e:
-                logging.info("Skipping {}/{}: {}".format(int(rel["EntryNr1"]), int(rel["EntryNr2"]), e))
+                logging.info(
+                    "Skipping {}/{}: {}".format(
+                        int(rel["EntryNr1"]), int(rel["EntryNr2"]), e
+                    )
+                )
                 pass
         return pandas.DataFrame(res)
 
 
 class TooSmallChromosome(Exception):
     pass
```

### Comparing `pyoma-0.13.2/pyoma/browser/tablefmt.py` & `pyoma-0.9.4/pyoma/browser/tablefmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,28 @@
     Fam = tables.Int32Col(pos=1)
     ID = tables.StringCol(255, pos=2)
     Level = tables.StringCol(255, pos=3)
     CompletenessScore = tables.Float32Col(pos=4, dflt=-1)
     ImpliedLosses = tables.Int32Col(pos=5, dflt=-1)
     NrMemberGenes = tables.Int32Col(pos=6, dflt=-1)
     IsRoot = tables.BoolCol(pos=7, dflt=False)
-    IdxPerLevelTable = tables.Int32Col(pos=8, dflt=-1)
 
 
 class OrthoXmlHogTable(tables.IsDescription):
     Fam = tables.UInt32Col(pos=0)
     HogBufferOffset = tables.Int64Col(pos=1)
     HogBufferLength = tables.UInt32Col(pos=2)
     HogAugmentedBufferOffset = tables.Int64Col(pos=3)
     HogAugmentedBufferLength = tables.UInt32Col(pos=4)
 
 
 class AncestralSyntenyRels(tables.IsDescription):
     HogRow1 = tables.UInt32Col(pos=0)
     HogRow2 = tables.UInt32Col(pos=1)
     Weight = tables.Float16Col(pos=2)
-    Evidence = tables.EnumCol(
-        tables.Enum({"linearized": 1, "parsimonious": 2, "any": 4}),
-        pos=3,
-        dflt="any",
-        base="uint8",
-    )
 
 
 class ProteinTable(tables.IsDescription):
     EntryNr = tables.UInt32Col(pos=1)
     SeqBufferOffset = tables.UInt64Col(pos=2)
     SeqBufferLength = tables.UInt32Col(pos=3)
     OmaGroup = tables.UInt32Col(pos=4, dflt=0)
@@ -58,14 +51,16 @@
     CanonicalId = tables.StringCol(20, pos=11, dflt=b"")
     CDNABufferOffset = tables.UInt64Col(pos=12)
     CDNABufferLength = tables.UInt32Col(pos=13)
     MD5ProteinHash = tables.StringCol(32, pos=14)
     DescriptionOffset = tables.UInt32Col(pos=15)
     DescriptionLength = tables.UInt16Col(pos=16)
     SubGenome = tables.StringCol(1, pos=17, dflt=b"")
+    RootHogUpstream = tables.Int32Col(pos=18, dflt=-1)
+    RootHogDownStream = tables.Int32Col(pos=19, dflt=-1)
 
 
 class ProteinCacheInfo(tables.IsDescription):
     EntryNr = tables.UInt32Col(pos=0)
     NrPairwiseOrthologs = tables.UInt32Col(pos=1)
     NrHogInducedPWOrthologs = tables.UInt32Col(pos=2)
     NrHogInducedPWParalogs = tables.UInt32Col(pos=3)
@@ -163,26 +158,14 @@
 class GeneOntologyTable(tables.IsDescription):
     EntryNr = tables.UInt32Col(pos=1)
     TermNr = tables.UInt32Col(pos=2)
     Evidence = tables.StringCol(3, pos=3)
     Reference = tables.StringCol(255, pos=4)
 
 
-class AncestralGeneOntologyTable(tables.IsDescription):
-    HogRow = tables.UInt32Col(pos=1)
-    TermNr = tables.UInt32Col(pos=2)
-    Score = tables.UInt8Col(pos=3)
-    RawScore = tables.Float16Col(pos=4)
-
-
-class GeneOntologyTermCounts(tables.IsDescription):
-    TermNr = tables.UInt32Col(pos=1)
-    Counts = tables.UInt32Col(pos=2)
-
-
 class ECTable(tables.IsDescription):
     EntryNr = tables.UInt32Col(pos=1)
     ECacc = tables.StringCol(16, pos=2)
 
 
 class GenomeTable(tables.IsDescription):
     NCBITaxonId = tables.Int32Col(pos=0)
@@ -194,15 +177,14 @@
     CommonName = tables.StringCol(64, pos=6)
     SynName = tables.StringCol(64, pos=7)
     Release = tables.StringCol(128, pos=8)
     Url = tables.StringCol(255, pos=9)
     Source = tables.StringCol(255, pos=10)
     Date = tables.Time32Col(pos=11)
     IsPolyploid = tables.BoolCol(pos=12)
-    TotGenes = tables.UInt32Col(pos=13, dflt=0)
 
 
 class TaxonomyTable(tables.IsDescription):
     NCBITaxonId = tables.Int32Col(pos=0)
     ParentTaxonId = tables.Int32Col(pos=1)
     Name = tables.StringCol(255, pos=2)
```

### Comparing `pyoma-0.13.2/pyoma/browser/xref_contrib.py` & `pyoma-0.9.4/tests/browser/test_suffixsearch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,307 +1,325 @@
-import collections
-import io
-import multiprocessing
-import itertools
+from __future__ import unicode_literals
+from future.standard_library import install_aliases
+
+install_aliases()
+
+import random
 import re
+import unittest
+
+try:
+    import unittest.mock as mock
+except ImportError:
+    import mock as mock
 import numpy
-import pandas
 import tables
-import logging
-import os
-from pathlib import Path
-from typing import List, Tuple, Set, Union
-from .hogprofile.build import Pipeline, SourceProcess, BaseProfileBuilderProcess, Stage
-
-logger = logging.getLogger(__name__)
-
-
-class GeneEntries:
-    def __init__(self, enrs, main):
-        self.main = main
-        self.enrs = enrs
-
-    def entrynr_slices(self):
-        if self.enrs[-1] - self.enrs[0] == len(self.enrs) - 1:
-            return (slice(self.enrs[0], self.enrs[-1] + 1, 1),)
-        slices, i0 = [], 0
-        for i in range(len(self.enrs)):
-            if self.enrs[i] - self.enrs[i0] == i - i0:
-                continue
-            slices.append(slice(self.enrs[i0], self.enrs[i - 1] + 1, 1))
-            i0 = i
-        slices.append(slice(self.enrs[i0], self.enrs[i] + 1, 1))
-        return tuple(slices)
+import string
+import itertools
+from pyoma.browser import suffixsearch
 
+CHARS = numpy.fromiter(
+    itertools.chain(string.ascii_letters, string.digits, "-_."), dtype="S1"
+)
+
+
+class StringGenerator(object):
+    def __init__(self):
+        self.buffer = None
+        self.pos = 0
+        self.fill_buffer()
+
+    def fill_buffer(self):
+        self.buffer = numpy.random.choice(CHARS, 2 ** 20)
+        self.pos = 0
+
+    def get_string(self, length):
+        if self.pos + length > len(self.buffer):
+            self.fill_buffer()
+        res = self.buffer[self.pos : self.pos + length].tostring()
+        self.pos += length
+        return res
+
+
+def create_h5_with_table(nr_row):
+    f = tables.open_file(
+        "testsuffix.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0
+    )
+    tab_def = numpy.dtype(
+        [("CharCol50", "S50"), ("DblCol", "f8"), ("CharCol200", "S200")]
+    )
+    tab = numpy.zeros(nr_row, tab_def)
+    generator = StringGenerator()
+    tab["CharCol50"] = [
+        generator.get_string(l) for l in numpy.random.randint(0, 51, size=nr_row)
+    ]
+    tab["DblCol"] = numpy.random.rand(nr_row)
+    tab["CharCol200"] = [
+        generator.get_string(l) for l in numpy.random.randint(0, 201, size=nr_row)
+    ]
+    f.create_table("/test", "table", obj=tab, createparents=True)
+    return f
+
+
+def create_h5_with_varlen_string_col(nr_row, off_col_type):
+    f = tables.open_file(
+        "testsuffix.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0
+    )
+    tab_def = numpy.dtype(
+        [("CharCol", "S800"), ("VarCharOff", off_col_type), ("VarCharLen", "i4")]
+    )
+    buf = f.create_earray(
+        "/test", "buffer", tables.StringAtom(1), (0,), createparents=True
+    )
+    tab = numpy.zeros(nr_row, tab_def)
+    generator = StringGenerator()
+    off = 0
+    for i in range(nr_row):
+        l = random.randint(0, 800)
+        val = numpy.ndarray(
+            (l,), buffer=generator.get_string(l), dtype=tables.StringAtom(1)
+        )
+        buf.append(val)
+        tab["VarCharOff"][i] = off
+        tab["VarCharLen"][i] = l
+        tab["CharCol"][i] = val.tostring()
+        off += l
+    f.create_table("/test", "table", obj=tab)
+    return f
 
-class SpliceVariantHelper:
-    def __init__(self, h5, alt_array=None):
-        if alt_array is not None:
-            lookup = numpy.copy(alt_array)
-            lookup[numpy.where(lookup > 0)] -= 1
-        else:
-            pe = h5.get_node("/Protein/Entries")
-            lookup = numpy.zeros(len(pe), dtype="i4")
-            for row in pe.where("AltSpliceVariant > 0"):
-                lookup[row.nrow] = row["AltSpliceVariant"] - 1
-        self.lookup = lookup
-        self.n = len(lookup)
-
-    def iter_genes(self):
-        taken = numpy.zeros(self.n, dtype=bool)
-        for i in range(self.n):
-            if taken[i]:
-                continue
-            if self.lookup[i] == 0:
-                taken[i] = True
-                yield GeneEntries(numpy.array([i + 1], dtype="i4"), i + 1)
-            else:
-                main = self.lookup[i]
-                l = self.lookup[i : i + 1000]
-                res = numpy.where(l == main)[0] + i
-                taken[res] = True
-                yield GeneEntries(res + 1, main + 1)
 
+class SuffixArraySearchTests(unittest.TestCase):
+    def setUp(self):
+        self.h5 = create_h5_with_table(5000)
 
-class KeywordIndexer:
-    def __init__(self, stopwords: Union[os.PathLike, Set[str]]):
-        self.kw = collections.defaultdict(set)
-        if isinstance(stopwords, set):
-            self.stopwords = set(stopwords)
-        else:
-            self.stopwords = set()
-            with open(stopwords, "rt") as fh:
-                for line in fh:
-                    self.stopwords.union(line.split())
-
-    def process(self, desc, enr):
-        pass
-
-
-class XRefIndexHandler(BaseProfileBuilderProcess):
-    def __init__(self, outfile, **kwargs):
-        super().__init__(**kwargs)
-        if outfile is None:
-            outfile = Path(os.getenv("TMPDIR", "/tmp")) / "tmp_index.h5"
-        self.outfile = outfile
-        self.tmp_h5 = outfile + ".tmp"
-        self.kwi = None
-
-    def setup(self):
-        self.xref_h5 = tables.open_file(self.tmp_h5, "w", filters=tables.Filters(6, complib="blosc"))
-        xref_dtype = numpy.dtype([("XRefId", "S50"), ("EntryNr", "i4"), ("XRefRow", "i4")])
-        grp = self.xref_h5.create_group("/", "XRefIndex", title="auxiliary lookup tables with deduplicated xrefs")
-        self.xref_idx = self.xref_h5.create_table(
-            grp,
-            "XRefs",
-            description=xref_dtype,
-            chunkshape=(16384,),
+    def tearDown(self):
+        self.h5.close()
+
+    def test_create_index_for_CharCol50(self):
+        suf = suffixsearch.SuffixIndexBuilderStringCol(
+            self.h5.get_node("/test/table"), "CharCol50", "/test", ignore_case=True
         )
-        self.genenames = collections.defaultdict(list)
-        self.spids = collections.defaultdict(list)
-        self._buffer = []
-        self.kwi = KeywordIndexer()
-
-    def _sort_and_store_xrefs(self):
-        data = self.xref_idx.read()
-        data.sort(order=["XRefId", "EntryNr"])
-        self.xref_h5.close()
-        self.xref_h5 = tables.open_file(self.outfile, "w", filters=tables.Filters(6, complib="blosc"))
-        xref_idx = self.xref_h5.create_table(
-            "/XRefIndex", "XRefs", obj=data, expectedrows=len(data), createparents=True
+        suf()
+        self.assertEqual(
+            self.h5.get_node_attr("/test/table", "CharCol50_suffixindexnode"), "/test"
         )
-        xref_idx.colinstances["XRefId"].create_csindex()
-        self.xref_idx = xref_idx
-
-    def _store_names(self, dic, node, skip_short=0):
-        keys = sorted(dic.keys())
-        max_key_len = max(len(z) for z in keys)
-        dtyp_key = numpy.dtype([("XRefId", "S{}".format(max_key_len)), ("Offset", "i4"), ("Length", "i4")])
-        dtyp_lookup = numpy.dtype([("EntryNr", "i4"), ("XRefRow", "i4")])
-        tab_key = self.xref_h5.create_table("/XRefIndex", node, description=dtyp_key, expectedrows=len(keys))
-        tab_lookup = self.xref_h5.create_table(
-            "/XRefIndex",
-            node + "_lookup",
-            description=dtyp_lookup,
-            expectedrows=sum(len(z) for z in dic.values()),
+        self.assertEqual(
+            self.h5.get_node_attr("/test", "CharCol50_buffer"), "/test/CharCol50_buffer"
         )
-        off, skipped = 0, 0
-        for k in keys:
-            if len(dic[k]) < skip_short:
-                logger.debug("skipping %s from index", k)
-                skipped += 1
-                continue
-            tab_lookup.append(sorted(dic[k]))
-            tab_key.append([(k, off, len(dic[k]))])
-            off += len(dic[k])
-        tab_lookup.flush()
-        tab_key.flush()
-        if len(tab_lookup) != off:
-            raise Exception("Lookup table length does not match key table offsets")
-        tab_key.colinstances["XRefId"].create_csindex()
-        logger.info("stored {} index with {} elements. skipped {} keys".format(node, len(tab_key), skipped))
-
-    def _add_to_buffer(self, e):
-        self._buffer.append(e)
-        if len(self._buffer) >= 2 * self.xref_idx.chunkshape[0]:
-            self._flush()
-
-    def _flush(self):
-        self.xref_idx.append(self._buffer)
-        self._buffer = []
-
-    def add_xref(self, xref, enr, xref_row):
-        xref = xref.lower()
-        self._add_to_buffer((xref, enr, xref_row))
-
-    def add_swissprot(self, id, enr, xref_row):
-        self.spids[id.lower()].append((enr, xref_row))
-        self.add_xref(id, enr, xref_row)
-
-    def add_gene_name(self, id, enr, xref_row):
-        self.genenames[id.lower()].append((enr, xref_row))
-        self.add_xref(id, enr, xref_row)
-
-    def add_keyword(self, enr: int, desc: str):
-        self.kwi.process(desc, enr)
-
-    def handle_input(self, item: Tuple[pandas.DataFrame, List]):
-        df, desc = item
-        for row in df.to_records(index=False):
-            if row["XRefSource"] == 0:
-                self.add_swissprot(row["XRefId"], row["EntryNr"], row["xref_row"])
-            elif row["XRefSource"] in (110, 115):
-                self.add_gene_name(row["XRefId"], row["EntryNr"], row["xref_row"])
-            else:
-                self.add_xref(row["XRefId"], row["EntryNr"], row["xref_row"])
+        self.assertEqual(
+            self.h5.get_node_attr("/test", "CharCol50_offset"), "/test/CharCol50_offset"
+        )
+        self.assertEqual(self.h5.get_node_attr("/test", "CharCol50_ignore_case"), True)
+        try:
+            suf = self.h5.get_node("/test/CharCol50_suffix")
+            buf = self.h5.get_node("/test/CharCol50_buffer")
+            off = self.h5.get_node("/test/CharCol50_offset")
+        except tables.NoSuchNodeError as e:
+            self.assertTrue(False, "Suffix index data not complete: {}".format(e))
+
+    def test_create_index_more_than_one_column(self):
+        cols = ("CharCol50", "CharCol200")
+        for col in cols:
+            suf = suffixsearch.SuffixIndexBuilderStringCol(
+                self.h5.get_node("/test/table"), col, "/test", ignore_case=True
+            )
+            suf()
+        for col in cols:
+            self.assertEqual(
+                "/test/{}_buffer".format(col),
+                self.h5.get_node_attr("/test", col + "_buffer"),
+            )
+            self.assertEqual(
+                "/test/{}_offset".format(col),
+                self.h5.get_node_attr("/test", col + "_offset"),
+            )
 
-    def finalize(self):
-        self._flush()
-        self._sort_and_store_xrefs()
-        self._store_names(self.spids, "SwissProt")
-        self._store_names(self.genenames, "GeneNames", 3)
-        self.xref_h5.close()
-        os.remove(self.tmp_h5)
+    def test_search_case_insensitive(self):
+        tab = self.h5.get_node("/test/table")
+        suffixsearch.SuffixIndexBuilderStringCol(
+            tab, "CharCol50", "/test", ignore_case=True
+        )()
+        search = suffixsearch.SuffixSearcher.from_tablecolumn(tab, "CharCol50")
+        target_row = numpy.random.randint(0, len(tab), size=200)
+        for k, full_query in enumerate(
+            tab.read_coordinates(target_row, field="CharCol50")
+        ):
+            if len(full_query) < 2:
+                continue
+            qlen = random.randint(2, len(full_query) + 1)
+            strt = random.randint(0, len(full_query) + 1 - qlen)
+            query = full_query[strt : strt + qlen]
+            res = search.find(query)
+            self.assertIn(
+                target_row[k],
+                res,
+                "could not find {} (full value {}, row {}) in results ({})".format(
+                    query, full_query, target_row[k], res
+                ),
+            )
+            for target in res:
+                self.assertIsNotNone(
+                    re.search(query, tab[target]["CharCol50"], re.IGNORECASE)
+                )
 
+    def test_search_string_instance(self):
+        tab = self.h5.get_node("/test/table")
+        suffixsearch.SuffixIndexBuilderStringCol(
+            tab, "CharCol50", "/test", ignore_case=True
+        )()
+        search = suffixsearch.SuffixSearcher.from_tablecolumn(tab, "CharCol50")
+        for trial in range(100):
+            row_nr = random.randint(0, len(tab))
+            query = tab[row_nr]["CharCol50"].decode()
+            if len(query) > 3:
+                break
+        else:
+            self.assertTrue(False, "table has no valid row to search")
+        res = search.find(query[2:])
+        self.assertIn(row_nr, res)
+
+    def test_raises_on_non_char_column(self):
+        tab = self.h5.get_node("/test/table")
+        with self.assertRaises(TypeError):
+            suffixsearch.SuffixIndexBuilderStringCol(
+                tab, "DblCol", "/test", ignore_case=True
+            )()
+
+
+class SuffixArrayVarLenSearchTestsCaseInsensitive(unittest.TestCase):
+    ignore_case = True
+
+    def setUp(self):
+        self.h5 = create_h5_with_varlen_string_col(5000, numpy.int32)
+        self.build_index()
+
+    def build_index(self):
+        tab = self.h5.get_node("/test/table")
+        suffixsearch.SuffixIndexBuilderVarStringCol(
+            tab,
+            "VarCharOff",
+            self.h5.get_node("/test/buffer"),
+            "/test",
+            ignore_case=self.ignore_case,
+        )()
 
-RE_VERS = re.compile(rb"(?P<base>[a-z0-9_.-]+)\.\d{1,2}$")
+    def tearDown(self):
+        self.h5.close()
 
+    def test_var_and_fixed_col_have_same_values(self):
+        tab = self.h5.get_node("/test/table")
+        buf = self.h5.get_node("/test/buffer")
+        for row in tab:
+            from_buf = buf[
+                row["VarCharOff"] : (row["VarCharOff"] + row["VarCharLen"])
+            ].tostring()
+            self.assertEqual(row["CharCol"], from_buf)
+
+    def test_existance_of_auxillary_buffers(self):
+        self.assertEqual(
+            self.h5.get_node_attr("/test/table", "VarCharOff_suffixindexnode"), "/test"
+        )
+        if self.ignore_case:
+            self.assertEqual(
+                self.h5.get_node_attr("/test", "VarCharOff_buffer"),
+                "/test/VarCharOff_buffer",
+            )
+        self.assertEqual(
+            self.h5.get_node_attr("/test", "VarCharOff_offset"),
+            "/test/VarCharOff_offset",
+        )
+        self.assertEqual(
+            self.h5.get_node_attr("/test", "VarCharOff_ignore_case"), self.ignore_case
+        )
+        try:
+            suf = self.h5.get_node("/test/VarCharOff_suffix")
+            off = self.h5.get_node("/test/VarCharOff_offset")
+            if self.ignore_case:
+                buf = self.h5.get_node("/test/VarCharOff_buffer")
+            else:
+                with self.assertRaises(tables.NoSuchNodeError):
+                    self.h5.get_node("/test/VarCharOff_buffer")
 
-def rem_vers(x):
-    m = RE_VERS.match(x)
-    if m is not None:
-        return m.group("base")
-    return x
+        except tables.NoSuchNodeError as e:
+            self.assertTrue(False, "Suffix index data not complete: {}".format(e))
 
+    def test_search_pattern(self):
+        tab = self.h5.get_node("/test/table")
+        search = suffixsearch.SuffixSearcher.from_tablecolumn(tab, "VarCharOff")
+        target_row = numpy.random.randint(0, len(tab), size=200)
+        for k, full_query in enumerate(
+            tab.read_coordinates(target_row, field="CharCol")
+        ):
+            if len(full_query) < 2:
+                continue
+            qlen = random.randint(2, len(full_query) + 1)
+            strt = random.randint(0, len(full_query) + 1 - qlen)
+            query = full_query[strt : strt + qlen]
+            res = search.find(query)
+            self.assertIn(
+                target_row[k],
+                res,
+                "could not find {} (full value {}, row {}) in results ({})".format(
+                    query, full_query, target_row[k], res
+                ),
+            )
+            for target in res:
+                if self.ignore_case:
+                    self.assertIsNotNone(
+                        re.search(query, tab[target]["CharCol"], flags=re.IGNORECASE)
+                    )
+                else:
+                    if not query in tab[target]["CharCol"]:
+                        # we didn't add a sentinel, could be a combination with the next value
+                        combined = b"".join(tab[target : target + 2]["CharCol"])
+                        self.assertIn(query, combined)
 
-class GeneGenerator(SourceProcess):
-    def __init__(self, h5_path, **kwargs):
-        super().__init__(**kwargs)
-        self.h5_path = h5_path
-        self.h5 = None
-        self.splice_helper = None
+    def test_non_existing_pattern(self):
+        tab = self.h5.get_node("/test/table")
+        search = suffixsearch.SuffixSearcher.from_tablecolumn(tab, "VarCharOff")
+        res = search.find("ZZZZzz")
+        self.assertEqual(0, len(res))
 
-    def setup(self):
-        self.h5 = tables.open_file(self.h5_path)
-        self.splice_helper = SpliceVariantHelper(self.h5)
 
-    def generate_data(self):
-        for gene in self.splice_helper.iter_genes():
-            yield gene
+class SuffixArrayVarLenSearchTestsCaseSensitive(
+    SuffixArrayVarLenSearchTestsCaseInsensitive
+):
+    ignore_case = False
 
-    def finalize(self):
-        self.h5.close()
 
+class SuffixBuilderFactoryTester(unittest.TestCase):
+    offset_col_type = numpy.int16
 
-class XRefReducer(BaseProfileBuilderProcess):
-    def __init__(self, h5_path, **kwargs):
-        super().__init__(**kwargs)
-        self.h5_path = h5_path
-        self.h5 = None
-        self.xref_tab = None
-        self.xref_eof = None
-
-    def setup(self):
-        self.h5 = tables.open_file(self.h5_path)
-        self.xref_tab = self.h5.get_node("/XRef")
-        try:
-            self.xref_eof = self.h5.get_node("/XRef_EntryNr_offset").read()
-        except tables.NoSuchNodeError:
-            pass
+    def setUp(self):
+        self.h5 = create_h5_with_varlen_string_col(100, self.offset_col_type)
 
-    def finalize(self):
+    def tearDown(self):
         self.h5.close()
 
-    def _load_xrefs_with_entry_offset(self, gene):
-        xrefs = pandas.DataFrame(
-            numpy.hstack(
-                list(
-                    map(
-                        lambda s: self.xref_tab[self.xref_eof[s.start] : self.xref_eof[s.stop]],
-                        gene.entrynr_slices(),
-                    )
-                )
-            )
+    @mock.patch("pyoma.browser.suffixsearch.SuffixIndexBuilderVarStringCol")
+    @mock.patch("pyoma.browser.suffixsearch.SuffixIndexBuilderStringCol")
+    def test_fix_string_column(self, FixStrSuffixMock, VarStrSuffixMock):
+        tab = self.h5.get_node("/test/table")
+        suffixsearch.create_suffix_index(tab, "CharCol", ignore_case=True)
+        FixStrSuffixMock.assert_called_once_with(
+            tab, "CharCol", self.h5.get_node("/test/_si_table"), ignore_case=True
         )
-        xrefs["xref_row"] = pandas.Series(
-            itertools.chain.from_iterable(
-                map(
-                    lambda s: range(self.xref_eof[s.start], self.xref_eof[s.stop]),
-                    gene.entrynr_slices(),
-                )
-            )
-        )
-        return xrefs
+        VarStrSuffixMock.assert_not_called()
 
-    def _load_xrefs_with_where_cond(self, gene):
-        query = " | ".join(
-            ["((EntryNr >= {}) & (EntryNr < {}))".format(s.start, s.stop) for s in gene.entrynr_slices()]
+    @mock.patch("pyoma.browser.suffixsearch.SuffixIndexBuilderVarStringCol")
+    @mock.patch("pyoma.browser.suffixsearch.SuffixIndexBuilderStringCol")
+    def test_var_string_column(self, FixStrSuffixMock, VarStrSuffixMock):
+        tab = self.h5.get_node("/test/table")
+        buf = "/test/buffer"
+        suffixsearch.create_suffix_index(tab, "VarCharOff", buf, ignore_case=True)
+        FixStrSuffixMock.assert_not_called()
+        VarStrSuffixMock.called_once_with(
+            tab,
+            "VarCharOff",
+            self.h5.get_node(buf),
+            self.h5.get_node("/test/_si_table"),
+            ignore_case=True,
         )
-        dtype = [("xref_row", "i8")] + self.xref_tab.dtype.descr
-        buf = io.BytesIO()
-        for row in self.xref_tab.where(query):
-            buf.write(row.nrow.tobytes())
-            buf.write(row.fetch_all_fields().tobytes())
-        data = numpy.frombuffer(buf.getbuffer(), dtype=dtype)
-        return pandas.DataFrame(data)
-
-    def _load_descriptions(self, gene):
-        query = " | ".join([f"((EntryNr >= {s.start}) & (EntryNr < {s.stop}))" for s in gene.entrynr_slices()])
-        descriptions = []
-        desc_buf = self.h5.get_node("/Protein/DescriptionBuffer")
-        for row in self.h5.get_node("/Protein/Entries").where(query):
-            desc = (
-                desc_buf[row["DescriptionOffset"] : row["DescriptionOffset"] + row["DescriptionLength"]]
-                .tobytes()
-                .decode()
-            )
-            descriptions.append((row["EntryNr"], desc))
-        return descriptions
-
-    def handle_input(self, gene):
-        if self.xref_eof is None:
-            xrefs = self._load_xrefs_with_where_cond(gene)
-        else:
-            xrefs = self._load_xrefs_with_entry_offset(gene)
-        xrefs["is_main"] = xrefs["EntryNr"] == gene.main
 
-        # transformations
-        xrefs["XRefId"] = xrefs["XRefId"].apply(bytes.lower).apply(rem_vers)
 
-        # sort such that first element per xrefid is the one we want to keep in the index
-        sorted_xrefs = xrefs.sort_values(["Verification", "is_main", "XRefSource"], ascending=[True, False, True])
-        res = sorted_xrefs.groupby("XRefId").first().reset_index()
-        desc = self._load_descriptions(gene)
-        return res, desc
-
-
-def reduce_xrefs(h5_path, outpath=None, nr_procs=None):
-    pipeline = Pipeline()
-    if nr_procs is None:
-        nr_procs = multiprocessing.cpu_count()
-
-    pipeline.add_stage(Stage(GeneGenerator, nr_procs=1, h5_path=h5_path))
-    pipeline.add_stage(Stage(XRefReducer, nr_procs=nr_procs, h5_path=h5_path))
-    pipeline.add_stage(Stage(XRefIndexHandler, nr_procs=1, outfile=outpath))
-    print("setup pipeline, about to start it")
-    pipeline.run()
-    print("finished computing a reduced set of xrefs")
+class SuffixBuilderFactoryTesterUnsignedColOffset(SuffixBuilderFactoryTester):
+    offset_col_type = numpy.uint64
```

### Comparing `pyoma-0.13.2/pyoma/hpc.py` & `pyoma-0.9.4/pyoma/hpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import hashlib
-import math
 import os
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class JobArray(object):
     def __init__(self, nr_procs, this_proc_nr):
         self.nr_procs = int(nr_procs)
         self.this_proc_nr = int(this_proc_nr)
-        if self.nr_procs < 1 or self.this_proc_nr < 1 or self.this_proc_nr > self.nr_procs:
+        if (
+            self.nr_procs < 1
+            or self.this_proc_nr < 1
+            or self.this_proc_nr > self.nr_procs
+        ):
             raise ValueError(
-                "cannot determine HPC parallel job ids: nr_procs={}, this_proc_nr={}".format(nr_procs, this_proc_nr)
+                "cannot determine HPC parallel job ids: nr_procs={}, this_proc_nr={}".format(
+                    nr_procs, this_proc_nr
+                )
             )
 
     def is_my_job(self, chunk):
         chunk = str(chunk).encode("utf-8") if not isinstance(chunk, bytes) else chunk
         h = hashlib.md5(chunk)
         as_int = int(h.hexdigest(), 16)
         res = (as_int % self.nr_procs) == (self.this_proc_nr - 1)
-        logger.debug("chunk %s to be processed: %s", chunk, res)
+        logger.debug("chunk {} to be processed: {}".format(chunk, res))
         return res
 
     def __repr__(self):
-        return "{}({},{})".format(self.__class__.__name__, self.nr_procs, self.this_proc_nr)
+        return "{}({},{})".format(
+            self.__class__.__name__, self.nr_procs, self.this_proc_nr
+        )
 
     def __str__(self):
         return "Jobarray process {} of {}".format(self.this_proc_nr, self.nr_procs)
 
     def modify_filename(self, basename):
         if self.nr_procs > 1:
             base, ext = os.path.splitext(basename)
-            nr_digits = math.floor(math.log10(self.nr_procs)) + 1
-            this_proc = f"{self.this_proc_nr}".zfill(nr_digits)
-            return f"{base}_{this_proc}-{self.nr_procs}{ext}"
+            return "{}_{}-{}{}".format(base, self.this_proc_nr, self.nr_procs, ext)
         return basename
 
 
 def detect_hpc_jobarray(nr_procs, this_proc_nr=None):
     if this_proc_nr is not None:
         return JobArray(nr_procs, int(this_proc_nr))
     if os.getenv("LSB_JOBID"):
```

### Comparing `pyoma-0.13.2/pyoma/inference/db.py` & `pyoma-0.9.4/pyoma/inference/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import tables
 import numpy as np
 
-from functools import lru_cache
+try:
+    from functools import lru_cache
+except ImportError:
+    from functools32 import lru_cache
 from builtins import filter
 
 
 class RelationsOfEntry(object):
     """
     This container class contains the relations from one given query
     gene in one other genome. E.g. all the BestMatches from HUMAN2 in
@@ -43,34 +46,38 @@
 
     def set_relations(self, value):
         if isinstance(value, (list, set, int)):
             value = np.array(value)
         elif not isinstance(value, np.ndarray):
             raise ValueError("Parameter not expected")
 
-        if value.dtype == int:
+        if value.dtype == np.int:
             value_idx = self.data["EntryNr2"].searchsorted(value)
             if not (self.data["EntryNr2"][value_idx] == value).all():
                 missing_matches = value[self.data["EntryNr2"][value_idx] != value]
-                raise ValueError("Not all entries found in Matches: {0!r:s}".format(missing_matches))
+                raise ValueError(
+                    u"Not all entries found in Matches: {0!r:s}".format(missing_matches)
+                )
         elif value.dtype == self.data.dtype:
-            raise NotImplementedError("setitem with replacement view not implemented")
+            raise NotImplementedError(u"setitem with replacement view not implemented")
         else:
-            raise ValueError("Unexpected dtype in parameter: {0!:s}".format(value.dtype))
+            raise ValueError(
+                u"Unexpected dtype in parameter: {0!:s}".format(value.dtype)
+            )
         self._set_relationflags_on_rows(value_idx)
 
     def _set_relationflags_on_rows(self, row_indexes):
         """method which sets the column flags to the appropriate
         relation type for the indexes of the data buffer. The base
-        class does not change any flags."""
+        class does not change any flags. """
         pass
 
 
 class CanonicalBestMatchesOfEntry(RelationsOfEntry):
-    """ "variant that only looks at the main splicing variant"""
+    """"variant that only looks at the main splicing variant"""
 
     @staticmethod
     def filter(row):
         return row["isCanonicalSplicing"]
 
     def _set_relationflags_on_rows(self, row_indexes):
         mask = np.zeros(len(self.data), dtype="bool")
@@ -119,15 +126,15 @@
         elif key == "VP":
             res = VPairsOfEntry(self.data)
         elif key == "BM":
             res = CanonicalBestMatchesOfEntry(self.data)
         elif key == "ALL":
             res = RelationsOfEntry(self.data)
         else:
-            raise KeyError("Unexpected key: {0!r:s}".format(key))
+            raise KeyError(u"Unexpected key: {0!r:s}".format(key))
         return res
 
     def __setitem__(self, key, value):
         rels_obj = self.__getitem__(key)
         rels_obj.set_relations(value)
         self._data_changed = True
 
@@ -139,25 +146,25 @@
     def __init__(self, mtab, itab):
         self.matches = mtab
         self.entry_offset = itab
         self.rels = [None] * len(itab)
 
     def __getitem__(self, item):
         if not isinstance(item, int):
-            raise IndexError("Invalid index or slice: {0!r:s}".format(item))
+            raise IndexError(u"Invalid index or slice: {0!r:s}".format(item))
         if item < 0:
-            raise IndexError("Invalid index or slice: {0!r:s}".format(item))
+            raise IndexError(u"Invalid index or slice: {0!r:s}".format(item))
         if item < 0:
-            raise IndexError("Invalid index or slice: {0!r:s}".format(item))
+            raise IndexError(u"Invalid index or slice: {0!r:s}".format(item))
         if item < 0:
             item += len(self.entry_offset)
         else:
             item -= 1
         if item >= len(self.entry_offset):
-            raise IndexError("Index is out of bound: {}".format(item))
+            raise IndexError(u"Index is out of bound: {}".format(item))
         if not self.rels[item] is None:
             return self.rels[item]
 
         range_of_entry = self.entry_offset[item]
         data = self.matches[range_of_entry[0] : range_of_entry[1]]
         self.rels[item] = RelationManager(data)
         return self.rels[item]
@@ -186,21 +193,29 @@
             filters = None
         self.db_handle = tables.open_file(file, mode=mode, filters=filters)
         self.genome_data = self.db_handle.get_node("/GenomeSummary")
 
     @lru_cache(maxsize=256)
     def matches(self, genome1, genome2):
         try:
-            mtab = self.db_handle.get_node("/Matches/{}/{}/Relations".format(genome1, genome2))
-            itab = self.db_handle.get_node("/Matches/{}/{}/ProteinIndex".format(genome1, genome2))
+            mtab = self.db_handle.get_node(
+                "/Matches/{}/{}/Relations".format(genome1, genome2)
+            )
+            itab = self.db_handle.get_node(
+                "/Matches/{}/{}/ProteinIndex".format(genome1, genome2)
+            )
         except tables.NoSuchNodeError:
-            raise KeyError("genome pair does not exist in database")
+            raise KeyError(u"genome pair does not exist in database")
         gs = self.genome_data.read_where("UniProtSpeciesCode==b'{}'".format(genome1))
         if len(itab) != gs["TotEntries"]:
-            raise OmaDBError("Nr of Protein does not match: {} vs {}".format(len(itab), gs["TotEntries"]))
+            raise OmaDBError(
+                u"Nr of Protein does not match: {} vs {}".format(
+                    len(itab), gs["TotEntries"]
+                )
+            )
         return GenomePair(mtab, itab)
 
     def close(self):
         self.db_handle.close()
 
 
 class OmaDBError(Exception):
```

### Comparing `pyoma-0.13.2/pyoma/inference/tabledef.py` & `pyoma-0.9.4/pyoma/inference/tabledef.py`

 * *Files identical despite different names*

### Comparing `pyoma-0.13.2/pyoma/orthoxml/compare.py` & `pyoma-0.9.4/pyoma/orthoxml/compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from xml.etree.ElementTree import XMLParser
 from datasketch import MinHash, MinHashLSH
-from ..common import auto_open
+import gzip
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Comparer(object):
     def __init__(self):
@@ -51,15 +51,18 @@
             gene = self.genes[gene_id]
             if gene is not None:
                 self.cur_hog_memb.append(gene)
         elif tag == "{http://orthoXML.org/2011/}orthologGroup":
             if self.cur_hog_depth == 0:
                 self.cur_hog_id = int(attrib["id"])
             self.cur_hog_depth += 1
-        elif tag == "{http://orthoXML.org/2011/}property" and attrib["name"] == "TaxRange":
+        elif (
+            tag == "{http://orthoXML.org/2011/}property"
+            and attrib["name"] == "TaxRange"
+        ):
             if self.cur_hog_depth == 1:
                 self.levels[self.cur_hog_id] = attrib["value"]
 
     def end(self, tag):
         if tag == "{http://orthoXML.org/2011/}orthologGroup":
             self.cur_hog_depth -= 1
             if self.cur_hog_depth == 0:
@@ -76,15 +79,16 @@
 class Analysis(object):
     def __init__(self, hogs, rootlevels):
         self.hogs = hogs
         self.rootlevels = rootlevels
 
 
 def load_toplevel_hogs(fpath, species_to_skip=None):
-    with auto_open(fpath) as fh:
+    open_ = gzip.open if fpath.endswith(".gz") else open
+    with open_(fpath) as fh:
         if species_to_skip is None:
             gene_mapper = GeneMapper()
         else:
             gene_mapper = FilteredSpeciesGeneMapper(species_to_skip)
         toplevelparser = ToplevelOrthoXMLParser(gene_mapper)
         parser = XMLParser(target=toplevelparser)
         for line in fh:
```

### Comparing `pyoma-0.13.2/pyoma.egg-info/SOURCES.txt` & `pyoma-0.9.4/pyoma.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,60 @@
-LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 bin/importdata.py
 bin/map_to_closest_seq
 bin/oma2hdf
 pyoma/__init__.py
 pyoma/common.py
 pyoma/hpc.py
 pyoma.egg-info/PKG-INFO
 pyoma.egg-info/SOURCES.txt
 pyoma.egg-info/dependency_links.txt
 pyoma.egg-info/requires.txt
 pyoma.egg-info/top_level.txt
-pyoma/application/__init__.py
-pyoma/application/enrichment.py
 pyoma/browser/KmerEncoder.py
 pyoma/browser/OrthoXMLSplitter.py
 pyoma/browser/__init__.py
-pyoma/browser/ancestral_genome.py
 pyoma/browser/ancestral_synteny.py
 pyoma/browser/check_db_consistency.py
 pyoma/browser/compute_cache.py
 pyoma/browser/convert.drw
 pyoma/browser/convert.py
 pyoma/browser/convert_omastandalone.drw
 pyoma/browser/convert_omastandalone.py
 pyoma/browser/db.py
-pyoma/browser/db_contrib.py
 pyoma/browser/decorators.py
-pyoma/browser/exceptions.py
 pyoma/browser/geneontology.py
 pyoma/browser/hoghelper.py
 pyoma/browser/hogidmap.py
 pyoma/browser/homoeologs.py
-pyoma/browser/idmapper.py
 pyoma/browser/linkout.py
 pyoma/browser/locus_parser.py
 pyoma/browser/models.py
 pyoma/browser/sanitychecks.py
-pyoma/browser/search.py
 pyoma/browser/suffixsearch.py
 pyoma/browser/synteny.py
 pyoma/browser/tablefmt.py
-pyoma/browser/xref_contrib.py
 pyoma/browser/hogprofile/__init__.py
 pyoma/browser/hogprofile/build.py
 pyoma/browser/hogprofile/hashutils.py
 pyoma/browser/hogprofile/pyhamutils.py
 pyoma/browser/hogprofile/query.py
 pyoma/browser/hogprofile/tree_helper.py
 pyoma/inference/__init__.py
 pyoma/inference/algo.py
 pyoma/inference/db.py
 pyoma/inference/tabledef.py
 pyoma/orthoxml/__init__.py
 pyoma/orthoxml/compare.py
-tests/test_common.py
-tests/application/__init__.py
-tests/application/test_enrichment.py
 tests/browser/__init__.py
 tests/browser/test_compare_hog_levels.py
 tests/browser/test_db.py
-tests/browser/test_hoghelper.py
-tests/browser/test_hogidmap.py
 tests/browser/test_import.py
 tests/browser/test_locusparser.py
 tests/browser/test_models.py
 tests/browser/test_orthoxmlsplitter.py
-tests/browser/test_performance_bigdb.py
-tests/browser/test_search.py
 tests/browser/test_suffixsearch.py
-tests/browser/test_xref_helper.py
 tests/browser/test_xrefs.py
 tests/inference/__init__.py
 tests/inference/test_db.py
```

### Comparing `pyoma-0.13.2/setup.py` & `pyoma-0.9.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
 import os
 import shutil
 
 name = "pyoma"
 
 req_packages = [
-    "numpy >= 1.20",
-    "tables >= 3.8.0",
+    "numpy >= 1.16",
+    "tables >= 3.5.1",
     "future",
-    "fuzzyset2 >= 0.1.1",
+    "fuzzyset >= 0.0.17",
     "tqdm",
     "pyopa >= 0.8",
     "pandas >= 0.22",
-    'biopython >= 1.76 ; python_version >= "3.6"',
+    'biopython >= 1.76, <= 1.77 ; python_version >= "3.6"',
     'biopython == 1.76 ; python_version < "3.6"',
     "datasketch",
     "ete3",
     "networkx",
-    "property_manager",
 ]
 
 cur_dir = os.path.abspath(os.path.dirname(__file__))
 
 # Create oma2hdf to install
 shutil.copyfile("bin/importdata.py", "bin/oma2hdf")
 
@@ -46,45 +45,33 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     scripts=["bin/importdata.py", "bin/oma2hdf", "bin/map_to_closest_seq"],
     package_data={"pyoma": ["browser/*.drw"]},
     install_requires=req_packages,
     extras_require={
         "create_db": [
             "PySAIS",
             "familyanalyzer>=0.7.3",
             "matplotlib",
             "scikit-learn",
             "scikit-fuzzy",
-            "pebble",
             "lark-parser",
             "pyham",
         ],
-        "enrichment": [
-            "plotly",
-            "scikit-learn",
-            "statsmodels",
-            "scipy",
-        ],
-        "notebooks": [
-            "jupyter",
-            "matplotlib",
-            "seaborn",
-        ],
         "docs": ["sphinx"],
     },
     test_require=["nose"],
-    python_requires=">=3.6",
+    python_requires=">=3.5",
 )
 
 # Remove local copy of oma2hdf (installed)
 os.remove("bin/oma2hdf")
```

### Comparing `pyoma-0.13.2/tests/browser/test_compare_hog_levels.py` & `pyoma-0.9.4/tests/browser/test_compare_hog_levels.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,15 @@
                 (1, b"HOG:0000001.1a", b"Parent"),
                 (1, b"HOG:0000001.1b", b"Parent"),
                 (1, b"HOG:0000001.1c", b"Parent"),
             ],
             dtype=[("Fam", "i4"), ("ID", "S255"), ("Level", "S255")],
         )
         child = numpy.array(
-            [
-                (1, b"HOG:0000001.1a", b"Child"),
-                (1, b"HOG:0000001.1c.4b", b"Child"),
-            ],
+            [(1, b"HOG:0000001.1a", b"Child"), (1, b"HOG:0000001.1c.4b", b"Child"),],
             dtype=[("Fam", "i4"), ("ID", "S255"), ("Level", "S255")],
         )
         exp_res = [
             (child[0], "retained"),
             (parent[1], "lost"),
             (child[1], "duplicated"),
         ]
```

### Comparing `pyoma-0.13.2/tests/browser/test_db.py` & `pyoma-0.9.4/tests/browser/test_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import division, print_function, unicode_literals
 
 import random
 import types
 import unittest
 
-import numpy.testing
-
 try:
     import unittest.mock as mock
 except ImportError:
     import mock
 from pyoma.browser.db import *
 from pyoma.browser import tablefmt
 from Bio.SeqRecord import SeqRecord
@@ -43,96 +41,45 @@
     path2 = os.path.abspath(os.path.join(os.getenv("PYOMA_DB_PATH", "./"), dbfn))
     if os.path.isfile(path2) and is_hdf5_file(path2):
         return path2
     else:
         raise IOError("cannot access {}. (Tried {} and {})".format(dbfn, path1, path2))
 
 
-class TestWithDbInstance(unittest.TestCase):
+class DatabaseTests(unittest.TestCase):
     db = None
-    db_file_name = "TestDb.h5"
 
     @classmethod
     def setUpClass(cls):
-        path = find_path_to_test_db(cls.db_file_name)
-        logger.info("Loading %s for DatabaseTests", path)
+        path = find_path_to_test_db("TestDb.h5")
+        logger.info("Loading {} for DatabaseTests".format(path))
         cls.db = Database(path)
 
     @classmethod
     def tearDownClass(cls):
-        cls.db.close()
-
+        cls.db.get_hdf5_handle().close()
 
-class DatabaseTests(TestWithDbInstance):
     def test_get_vpairs_of_entry_with_orthologs(self):
         for entry_nr, exp_vps_cnt in [(12, 3), (1, 0), (4, 1)]:
             vps = self.db.get_vpairs(entry_nr)
             self.assertTrue(isinstance(vps, numpy.ndarray))
             self.assertEqual(exp_vps_cnt, len(vps))
             self.assertEqual(
                 sorted(["EntryNr1", "EntryNr2", "RelType", "Distance", "Score"]),
                 sorted(vps.dtype.fields.keys()),
             )
 
-    def test_get_vpairs_between_species_is_same_as_loading_all_vpairs(self):
-        g1, g2 = "YEAST", "SCHPO"
-        t0 = time.time()
-        rng1 = self.db.id_mapper["OMA"].genome_range(g1)
-        rng2 = self.db.id_mapper["OMA"].genome_range(g2)
-        expected = []
-        for en in range(rng1[0], rng1[1] + 1):
-            for vp in self.db.get_vpairs(en):
-                if rng2[0] <= vp["EntryNr2"] <= rng2[1]:
-                    expected.append(vp)
-        expected = numpy.fromiter(expected, dtype=expected[0].dtype)
-        t1 = time.time()
-        actual = self.db.get_vpairs_between_species_pair(g1, g2)
-        t2 = time.time()
-        numpy.testing.assert_equal(expected, actual)
-        self.assertLess(10 * (t2 - t1), t1 - t0, "expect at least 10x speedup")
-
-    def test_get_hoginducedpairs_between_species_is_same_as_loading_all_hoginduced(
-        self,
-    ):
-        g1, g2 = "YEAST", "SCHPO"
-        t0 = time.time()
-        rng1 = self.db.id_mapper["OMA"].genome_range(g1)
-        rng2 = self.db.id_mapper["OMA"].genome_range(g2)
-        expected = []
-        for en in range(rng1[0], rng1[1] + 1):
-            for vp in self.db.get_hog_induced_pairwise_orthologs(en):
-                if rng2[0] <= vp["EntryNr"] <= rng2[1]:
-                    expected.append((en, int(vp["EntryNr"])))
-        expected = numpy.fromiter(expected, dtype=[("EntryNr1", "u4"), ("EntryNr2", "u4")])
-        t1 = time.time()
-        actual = self.db.get_hog_induced_orthologs_between_genome_pair(g1, g2)
-        actual = actual[["EntryNr1", "EntryNr2"]].copy()
-        actual.sort()
-        t2 = time.time()
-        numpy.testing.assert_equal(expected, actual)
-        self.assertLess(5 * (t2 - t1), t1 - t0, "expect at least 5x speedup")
-
     def test_neighborhood_close_to_boundary(self):
         query, window = 3, 7
         neighbors, idx = self.db.neighbour_genes(query, window)
         self.assertEqual(query - 1, idx)
         self.assertEqual(neighbors["EntryNr"][idx], query)
         expected_entry_nrs = numpy.arange(1, query + window + 1, dtype="i4")
         self.assertTrue(numpy.array_equal(expected_entry_nrs, neighbors["EntryNr"]))
 
-    def test_count_rows_of_index_column_with_value(self):
-        entrynr = 12
-        vps = self.db.get_vpairs(entrynr)
-        vp_tab = self.db._get_vptab(entrynr)
-        self.assertEqual(len(vps), count_rows_of_index_column_with_value(vp_tab, "EntryNr1", entrynr))
-
-        # check that it raises KeyError if operated on a column that is not indexed
-        with self.assertRaises(KeyError, msg="Operating on non-indexed column should raise KeyError"):
-            count_rows_of_index_column_with_value(vp_tab, "EntryNr2", entrynr)
-
     def test_hog_family(self):
         entry = numpy.zeros(1, dtype=tables.dtype_from_descr(tablefmt.ProteinTable))
         entry["OmaHOG"] = b""
         with self.assertRaises(Singleton):
             self.db.hog_family(entry[0])
         entry["OmaHOG"] = b"HOG:0000523"
         self.assertEqual(523, self.db.hog_family(entry[0]))
@@ -217,15 +164,17 @@
 
     def test_get_subhogs_with_subids(self):
         for hog_id, level, exp_subhogid in (
             ("HOG:0000474", "Eukaryota", "HOG:0000474.1d.2c"),
             ("HOG:0000165", "Fungi", "HOG:0000165.1a"),
         ):
             with self.subTest(hog_id=hog_id, level=level):
-                hogs = list(self.db.get_subhogs(hog_id, level=level, include_subids=True))
+                hogs = list(
+                    self.db.get_subhogs(hog_id, level=level, include_subids=True)
+                )
                 self.assertIn(exp_subhogid, [h.hog_id for h in hogs])
                 self.assertNotIn(level, [h.level for h in hogs])
 
     def test_get_hog_with_level(self):
         for hog_id, level in (
             ("HOG:0000002.2b", "Saccharomyces cerevisiae (strain ATCC 204508 / S288c)"),
             ("HOG:0000005.1b", "Saccharomycetaceae"),
@@ -302,28 +251,34 @@
         s = self.db.get_sequence(enr)[ii:jj]
         return s, enr, ii, jj
 
     def test_approx_search(self):
         # Test for random subsequence of 10 random sequences.
         for _ in range(10):
             s, enr, start_idx, end_idx = self.get_random_subsequence()
-            approx_search_results = self.db.seq_search.approx_search(s, is_sanitised=True)
+            approx_search_results = self.db.seq_search.approx_search(
+                s, is_sanitised=True
+            )
             self.assertIn(
                 enr,
                 {z[0] for z in approx_search_results},
-                "approx search for entry {}[{}:{}] failed.".format(enr - 1, start_idx, end_idx),
+                "approx search for entry {}[{}:{}] failed.".format(
+                    enr - 1, start_idx, end_idx
+                ),
             )
 
     def test_specific_approx_search_that_failed_on_jenkins(self):
         # TODO fix this problem!
         enrs = [15885, 16452]
         ranges = [(39, 376), (55, 140)]
         for enr, (start_idx, end_idx) in zip(enrs, ranges):
             seq = self.db.get_sequence(enr)[start_idx:end_idx]
-            approx_search_results = self.db.seq_search.approx_search(seq, is_sanitised=True)
+            approx_search_results = self.db.seq_search.approx_search(
+                seq, is_sanitised=True
+            )
             enrs_with_approx_match = {z[0] for z in approx_search_results}
             self.assertIn(enr, enrs_with_approx_match)
 
     def test_map_to_hog(self):
         hog_mapper = ClosestSeqMapper(self.db)
         seqs = []
         entry_nrs = []
@@ -365,38 +320,20 @@
         query = 14677  # Q8I237
         exons = self.db.get_exons(query)
         self.assertEqual(3, len(exons))
 
     def test_go_term_search(self):
         query = "GO:0004575"
         nrs = self.db.entrynrs_with_go_annotation(query, evidence="IDA")
-        self.assertGreaterEqual(len(nrs), 1, "query GO term is known to occure at least in MAL32_YEAST")
+        self.assertGreaterEqual(
+            len(nrs), 1, "query GO term is known to occure at least in MAL32_YEAST"
+        )
         for enr in nrs:
             self.assertIn(4575, self.db.get_gene_ontology_annotations(enr)["TermNr"])
 
-    def test_go_ic_values(self):
-        terms = ["GO:003674", "GO:008150"]
-        for term in terms:
-            with self.subTest(case=term):
-                gof = self.db.freq_aware_gene_ontology
-                ic = gof.ic(term)
-                self.assertAlmostEqual(0, ic)
-
-    def test_go_lin_same_term_is_1(self):
-        self.assertEqual(1, self.db.freq_aware_gene_ontology.lin_similarity(55, 55))
-
-    def test_go_semantic_sim_of_same_term(self):
-        self.assertGreater(1, self.db.freq_aware_gene_ontology.semantic_similarity(55, 55))
-
-    def test_mindepth_of_go(self):
-        examples = [(8150, 0), (168, 7), (5689, 5)]
-        for term, exp_depth in examples:
-            with self.subTest(case=term):
-                self.assertEqual(exp_depth, self.db.gene_ontology.ensure_term(term).min_depth)
-
     def test_induced_pairwise_orthologs(self):
         query = "YEAST3523"
         query_entry = self.db.ensure_entry(self.db.id_resolver.resolve(query))
         orthologs = self.db.get_hog_induced_pairwise_orthologs(query_entry)
         self.assertEqual(3, len(orthologs))
         self.assertCountEqual([b"1:1", b"1:1", b"m:1"], orthologs["RelType"])
 
@@ -406,31 +343,14 @@
         orthologs = self.db.get_hog_induced_pairwise_paralogs(query_entry)
         self.assertEqual(1, len(orthologs))
         self.assertEqual(
             b"Saccharomyces cerevisiae (strain ATCC 204508 / S288c)",
             orthologs["DivergenceLevel"],
         )
 
-    def test_ancestral_synteny_graph(self):
-        query_hog = "HOG:0000005"
-        query_level = "Fungi"
-        graph = self.db.get_syntentic_hogs(query_level, query_hog, steps=2)
-        self.assertIn(query_hog, graph)
-
-    def test_ancestral_syteny_of_genome(self):
-        query_level = "Fungi"
-        graph = self.db.get_syntenic_hogs(level=query_level)
-        self.assertIn("HOG:0000005", graph)
-        self.assertEqual(len(graph.nodes), self.db.count_hogs_at_level(query_level))
-
-    def test_extant_syntey_of_genome(self):
-        query_level = "YEAST"
-        graph = self.db.get_extant_synteny_graph(query_level)
-        self.assertIn("YEAST00012", graph)
-
 
 class XRefDatabaseMock(Database):
     def __init__(self, name=None):
         if name is None:
             name = "xref.h5"
         f = tables.open_file(name, "w", driver="H5FD_CORE", driver_core_backing_store=0)
         entries = numpy.zeros(5, tables.dtype_from_descr(tablefmt.ProteinTable))
@@ -438,49 +358,42 @@
         t = f.create_table("/Protein", "Entries", obj=entries, createparents=True)
         t.colinstances["EntryNr"].create_csindex()
         xref = numpy.zeros(10, tables.dtype_from_descr(tablefmt.XRefTable))
         xref["EntryNr"] = numpy.arange(1, 6, 0.5).astype(numpy.int32)
         xref["XRefSource"] = numpy.tile([0, 20], 5)
         xref["XRefId"] = ["XA{:03}g1.4".format(i) for i in range(10)]
         xref["Verification"] = tuple(itertools.islice(itertools.cycle([0, 2, 4]), 10))
-        x = f.create_table("/", "XRef", tablefmt.XRefTable, obj=xref)
-        x.colinstances["EntryNr"].create_csindex()
-        x.colinstances["XRefId"].create_csindex()
+        f.create_table("/", "XRef", tablefmt.XRefTable, obj=xref)
         f.create_group("/", "XRef_Index")
         for n in ("suffix", "buffer", "offset"):
             f.create_carray("/XRef_Index", n, obj=numpy.ones((5,), "i4"))
         self.db = f
-        self._on_close_notify = []
-        self._close_fh = True
 
 
 class XRefIdMapperTest(unittest.TestCase):
     @classmethod
     def setUp(self):
         patch_db = XRefDatabaseMock()
         self.xrefmapper = XrefIdMapper(patch_db)
 
     def tearDown(self):
-        self.xrefmapper._db.close()
+        self.xrefmapper._db.db.close()
 
     def test_multiple_xrefs_per_entry(self):
         xref_e1 = self.xrefmapper.map_entry_nr(1)
         self.assertEqual(len(xref_e1), 2)
 
     def test_map_many_entries(self):
         all_mapped = self.xrefmapper.map_many_entry_nrs(numpy.arange(1, 4))
-        expected_len = 4 if isinstance(self.xrefmapper, XRefNoApproximateIdMapper) else 6
+        expected_len = (
+            4 if isinstance(self.xrefmapper, XRefNoApproximateIdMapper) else 6
+        )
         self.assertEqual((expected_len,), all_mapped.shape)
         self.assertEqual(self.xrefmapper.xref_tab.dtype, all_mapped.dtype)
 
-    def test_entry_nr_range(self):
-        all_mapped = self.xrefmapper.map_many_entry_nrs(numpy.arange(1, 4))
-        range_mapped = self.xrefmapper.map_entry_nr_range(1, 4)
-        numpy.testing.assert_equal(all_mapped, range_mapped)
-
     def test_map_entry_iterator(self):
         it = self.xrefmapper.iter_xrefs_for_entry_nr(1)
         self.assertTrue(isinstance(it, types.GeneratorType), "not a generator")
         exp_xrefs = ["XA000g1.4", "XA001g1.4"]
         for dic in it:
             self.assertIn(dic["xref"], exp_xrefs)
 
@@ -515,27 +428,29 @@
     def setUp(self):
         patch_db = XRefDatabaseMock("test_idresolver.h5")
         self.xrefmapper = XrefIdMapper(patch_db)
         self.id_resolver = IDResolver(patch_db)
         patch_db.id_mapper = {"XRef": self.xrefmapper}
 
     def tearDown(self):
-        self.xrefmapper._db.close()
+        self.xrefmapper._db.db.close()
 
     def test_search_of_modified_xref(self):
         xref = "XA002g1.4"
         res = self.id_resolver.search_xrefs(xref, return_seq_modified=True)
         self.assertEqual(2, res[0])
         self.assertTrue(res[1], "expected that {} is a modified sequence".format(xref))
 
     def test_search_of_unchecked_xref(self):
         xref = "XA001g1.4"
         res = self.id_resolver.search_xrefs(xref, return_seq_modified=True)
         self.assertEqual(1, res[0])
-        self.assertFalse(res[1], "expected that {} is a unchecked sequence".format(xref))
+        self.assertFalse(
+            res[1], "expected that {} is a unchecked sequence".format(xref)
+        )
 
 
 class TaxonomyTest(unittest.TestCase):
     tax_input = None
     maxDiff = None  # show complete strings if test fails
 
     @classmethod
@@ -565,22 +480,32 @@
                 "Fungi",
                 "Opisthokonta",
                 "Eukaryota",
             ],
         )
 
     def test_newick(self):
-        member = frozenset([self.tax._taxon_from_numeric(x)["Name"] for x in self.tax.tax_table["NCBITaxonId"]])
+        member = frozenset(
+            [
+                self.tax._taxon_from_numeric(x)["Name"]
+                for x in self.tax.tax_table["NCBITaxonId"]
+            ]
+        )
         phylo = self.tax.get_induced_taxonomy(member, collapse=True)
         expected = "(((Ashbya gossypii [strain ATCC 10895 / CBS 109.51 / FGSC 9923 / NRRL Y-1056],Saccharomyces cerevisiae [strain ATCC 204508 / S288c])Saccharomycetaceae,Schizosaccharomyces pombe [strain 972 / ATCC 24843])Ascomycota,Plasmodium falciparum [isolate 3D7])Eukaryota;"
         expected = expected.replace(" ", "_")
         self.assertEqual(expected, phylo.newick())
 
     def test_phylogeny(self):
-        member = frozenset([self.tax._taxon_from_numeric(x)["Name"] for x in self.tax.tax_table["NCBITaxonId"]])
+        member = frozenset(
+            [
+                self.tax._taxon_from_numeric(x)["Name"]
+                for x in self.tax.tax_table["NCBITaxonId"]
+            ]
+        )
         phylo = self.tax.get_induced_taxonomy(member, collapse=True)
         expected = {
             "id": 2759,
             "name": "Eukaryota",
             "children": [
                 {
                     "id": 4890,
@@ -727,154 +652,14 @@
         )
 
     def test_induced_subtree_retains_internal_species(self):
         phylo = self.tax.get_induced_taxonomy([20, 40], augment_parents=True)
         self.assertIn(30, phylo.tax_table["NCBITaxonId"])
 
 
-def _get_taxtab():
-    # a random sample of 30 species from a production OMA release
-    taxtab = numpy.array(
-        [
-            (2, 0, b"Bacteria"),
-            (633, 1649845, b"Yersinia pseudotuberculosis"),
-            (1224, 2, b"Proteobacteria"),
-            (1236, 1224, b"Gammaproteobacteria"),
-            (2759, 0, b"Eukaryota"),
-            (5204, 451864, b"Basidiomycota"),
-            (5334, 5204, b"Schizophyllum commune"),
-            (5660, 2759, b"Leishmania braziliensis"),
-            (5786, 2759, b"Dictyostelium purpureum"),
-            (5794, 2698737, b"Apicomplexa"),
-            (5807, 5794, b"Cryptosporidium parvum"),
-            (5864, 5794, b"Babesia"),
-            (5866, 5864, b"Babesia bigemina"),
-            (6412, 33317, b"Helobdella robusta"),
-            (6960, 33317, b"Hexapoda"),
-            (7263, 6960, b"Drosophila arizonae"),
-            (9813, 32524, b"Procavia capensis"),
-            (13735, 32524, b"Pelodiscus sinensis"),
-            (28211, 1224, b"Alphaproteobacteria"),
-            (29760, 2759, b"Vitis vinifera"),
-            (32524, 33213, b"Amniota"),
-            (33154, 2759, b"Opisthokonta"),
-            (33213, 33154, b"Bilateria"),
-            (33317, 33213, b"Protostomia"),
-            (37360, 2698737, b"Plasmodiophora brassicae"),
-            (55529, 2759, b"Guillardia theta"),
-            (91347, 1236, b"Enterobacterales"),
-            (119060, 1224, b"Burkholderiaceae"),
-            (158441, 6960, b"Folsomia candida"),
-            (164328, 2698737, b"Phytophthora ramorum"),
-            (214092, 1649845, b"Yersinia pestis CO92"),
-            (
-                264198,
-                119060,
-                b"Cupriavidus pinatubonensis (strain JMP 134 / LMG 1197)",
-            ),
-            (
-                273123,
-                633,
-                b"Yersinia pseudotuberculosis serotype I (strain IP32953)",
-            ),
-            (
-                284812,
-                451864,
-                b"Schizosaccharomyces pombe (strain 972 / ATCC 24843)",
-            ),
-            (
-                323261,
-                1236,
-                b"Nitrosococcus oceani (strain ATCC 19707 / BCRC 17464 / NCIMB 11848 / C-107)",
-            ),
-            (338187, 1236, b"Vibrio campbellii (strain ATCC BAA-1116 / BB120)"),
-            (347255, 28211, b"Rickettsia africae (strain ESF-5)"),
-            (353152, 5807, b"Cryptosporidium parvum (strain Iowa II)"),
-            (
-                355278,
-                2,
-                b"Leptospira biflexa serovar Patoc (strain Patoc 1 / Ames)",
-            ),
-            (391774, 1224, b"Desulfovibrio vulgaris subsp. vulgaris (strain DP4)"),
-            (451864, 33154, b"Dikarya"),
-            (
-                502801,
-                633,
-                b"Yersinia pseudotuberculosis serotype IB (strain PB1/+)",
-            ),
-            (578458, 5334, b"Schizophyllum commune (strain H4-8 / FGSC 9210)"),
-            (626418, 119060, b"Burkholderia glumae (strain BGR1)"),
-            (640131, 91347, b"Klebsiella variicola (strain At-22)"),
-            (
-                713600,
-                91347,
-                b"Buchnera aphidicola subsp. Acyrthosiphon pisum (strain JF98)",
-            ),
-            (
-                754035,
-                28211,
-                b"Mesorhizobium australicum (strain HAMBI 3006 / LMG 24608 / WSM2073)",
-            ),
-            (905079, 55529, b"Guillardia theta (strain CCMP2712)"),
-            (1133968, 5864, b"Babesia microti (strain RI)"),
-            (1230383, 5204, b"Malassezia sympodialis (strain ATCC 42132)"),
-            (1649845, 91347, b"Yersinia pseudotuberculosis complex"),
-            (2698737, 2759, b"Sar"),
-        ],
-        dtype=tables.dtype_from_descr(tablefmt.TaxonomyTable),
-    )
-    return taxtab
-
-
-class LucaBasedTaxonomyTests(unittest.TestCase):
-    def setUp(self):
-        taxtab = _get_taxtab()
-        self.tax = Taxonomy(taxtab)
-        self.nr_species = 30
-
-    def test_root_is_luca(self):
-        self.assertEqual(self.tax._get_root_taxon()["Name"], b"LUCA")
-
-    def test_search_luca(self):
-        node = self.tax.get_taxnode_from_name_or_taxid("LUCA")
-        self.assertEqual(len(node), 1)
-        self.assertEqual(node["Name"], b"LUCA")
-
-    def test_extend_genomes(self):
-        self.assertEqual(len(self.tax.get_taxid_of_extent_genomes()), self.nr_species)
-
-    def test_search_approx_luca(self):
-        self.assertIn("LUCA", [x[1] for x in self.tax.approx_search("luca")])
-
-    def test_numeric_luca_is_found(self):
-        self.assertEqual(self.tax.get_taxnode_from_name_or_taxid(0)["Name"], b"LUCA")
-
-    def test_subtaxonomy_does_not_contain_luca_anymore(self):
-        # subset of only eukaryotes
-        subtax = self.tax.get_induced_taxonomy([451864, 55529, 158441], collapse=True, augment_parents=True)
-        self.assertNotIn(b"LUCA", subtax._get_root_taxon()["Name"])
-
-    def test_as_newick_works(self):
-        self.assertTrue(self.tax.newick().endswith("LUCA;"), self.tax.newick()[-30:])
-
-
-class LucaWithNegTaxIDGenomeTaxonomyTests(LucaBasedTaxonomyTests):
-    def setUp(self):
-        taxtab = _get_taxtab()
-        taxtab = numpy.append(
-            taxtab,
-            numpy.array([(-2, 451864, b"Some Random Genome")], dtype=taxtab.dtype),
-        )
-        self.tax = Taxonomy(taxtab)
-        self.nr_species = 31
-
-    def test_neg_taxid_species_in_newick(self):
-        self.assertIn("Some_Random_Genome", self.tax.newick())
-
-
 class DBMock(object):
     def __init__(self, h5):
         self.h5 = h5
 
     def get_hdf5_handle(self):
         return self.h5
 
@@ -944,26 +729,9 @@
         test_seq = io.StringIO(">test\nAS")
         seq_iter = SeqIO.parse(test_seq, format="fasta")
         with self.assertLogs("pyoma", level=logging.INFO) as cm:
             anno = list(self.fast_mapper.iter_projected_goannotations(seq_iter))
         self.assertIn("Skipping", "\n".join(cm.output))
         self.assertEqual(0, len(anno))
 
-    def check_mapped_seqs(self, seqs, way="Exact"):
-        with self.assertLogs("pyoma", level=logging.INFO) as cm:
-            anno = list(self.fast_mapper.iter_projected_goannotations(seqs))
-        for a in anno:
-            with_ = self.fast_mapper.db.id_mapper["OMA"].map_entry_nr(int(a["DB_Object_ID"]))
-            self.assertEqual(f"{way}:{with_}".split(":"), a["With"].split(":")[:2])
-        self.assertGreaterEqual(len(a), 1)
-
-    def test_search_existing_sequences(self):
-        seqs = [SeqRecord(id=f"{enr}", seq=Seq(self.fast_mapper.db.get_sequence(enr).decode())) for enr in range(1, 5)]
-        self.check_mapped_seqs(seqs, way="Exact")
-
-    def test_search_inexact_search_seq(self):
-        seqs = []
-        for en in range(1, 5):
-            s = self.fast_mapper.db.get_sequence(en).decode()
-            modif_seq = s.replace("A", "R")
-            seqs.append(SeqRecord(id=f"{en}", seq=Seq(modif_seq)))
-        self.check_mapped_seqs(seqs, way="Approx")
+    def test_search_existing_sequance(self):
+        pass
```

### Comparing `pyoma-0.13.2/tests/browser/test_locusparser.py` & `pyoma-0.9.4/tests/browser/test_locusparser.py`

 * *Files identical despite different names*

### Comparing `pyoma-0.13.2/tests/browser/test_orthoxmlsplitter.py` & `pyoma-0.9.4/tests/browser/test_orthoxmlsplitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,17 @@
         self.assertEqual(3, self.splitter.create_new_orthoxml.call_count)
 
     def test_extract_subset(self):
         self.splitter(hogs_to_extract=[1, 2])
         self.assertEqual(2, self.splitter.create_new_orthoxml.call_count)
 
     def test_extract_subset_into_single_file(self):
-        self.splitter(hogs_to_extract=[1, 2], single_hog_files=True, basename="single.orthoxml")
+        self.splitter(
+            hogs_to_extract=[1, 2], single_hog_files=True, basename="single.orthoxml"
+        )
         self.assertEqual(1, self.splitter.create_new_orthoxml.call_count)
         args, kwargs = self.splitter.create_new_orthoxml.call_args
         self.assertEqual(args[0], os.path.join(self.outdir, "single.orthoxml"))
 
     def test_raises_exception_on_single_hog_files_without_filename(self):
         with self.assertRaises(ValueError):
             self.splitter(hogs_to_extract=[1, 2], single_hog_files=True)
@@ -103,15 +105,20 @@
 
     def setUp(self):
         self.outdir = os.path.join(self.tmpdir, "splits")
         self.splitter = OrthoXMLSplitter(self.infile, self.outdir)()
 
     def load_data_of_file(self, fn):
         xml = lxml.etree.parse(fn)
-        genes = [g.get("id") for g in xml.getroot().findall(".//{http://orthoXML.org/2011/}gene")]
+        genes = [
+            g.get("id")
+            for g in xml.getroot().findall(".//{http://orthoXML.org/2011/}gene")
+        ]
         return genes
 
     def test_properly_split_in_hogs(self):
         for nr in range(1, 4):
-            fn = os.path.join(self.outdir, "HOG{:07d}.orthoxml".format(nr))
+            fn = os.path.join(self.outdir, "HOG{:06d}.orthoxml".format(nr))
             exp = [str(nr), str(nr + 10)]
-            self.assertEqual(sorted(self.load_data_of_file(fn)), sorted(exp), "{} failed.".format(fn))
+            self.assertEqual(
+                sorted(self.load_data_of_file(fn)), sorted(exp), "{} failed.".format(fn)
+            )
```

### Comparing `pyoma-0.13.2/tests/browser/test_xrefs.py` & `pyoma-0.9.4/tests/browser/test_xrefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,20 @@
             self.importer.xrefs,
         )
 
     def test_multi_handler(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         enum = pyoma.tablefmt.XRefTable.columns.get("XRefSource").enum
         verif = pyoma.tablefmt.XRefTable.columns.get("Verification").enum
-        self.assertIn((2, enum["Swiss Model"], b"P21122", verif.unchecked), self.importer.xrefs)
-        self.assertIn((2, enum["Swiss Model"], b"Q24S32", verif.unchecked), self.importer.xrefs)
+        self.assertIn(
+            (2, enum["Swiss Model"], b"P21122", verif.unchecked), self.importer.xrefs
+        )
+        self.assertIn(
+            (2, enum["Swiss Model"], b"Q24S32", verif.unchecked), self.importer.xrefs
+        )
 
     def test_regex_of_ensembl_ids(self, mock_up):
         for case in ("ENSG00000162687", "ENSMUSP00000162687"):
             match = self.importer.ENS_RE.match(case)
             self.assertIsNotNone(match)
 
     def test_potential_flush_gets_called(self, mock_up):
@@ -89,22 +93,28 @@
         self.db_parser.parse_entrytags(self.data)
         self.assertEqual(callback.call_count, 5)
 
     def test_ensembgenomes_ids(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         enum = pyoma.tablefmt.XRefTable.columns.get("XRefSource").enum
         verif = pyoma.tablefmt.XRefTable.columns.get("Verification").enum
-        self.assertIn((4, enum.EnsemblGenomes, b"CBG23988", verif.exact), self.importer.xrefs)
+        self.assertIn(
+            (4, enum.EnsemblGenomes, b"CBG23988", verif.exact), self.importer.xrefs
+        )
 
     def test_uniprot_ids(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         enum = pyoma.tablefmt.XRefTable.columns.get("XRefSource").enum
         verif = pyoma.tablefmt.XRefTable.columns.get("Verification").enum
-        self.assertIn((3, enum["UniProtKB/TrEMBL"], b"L8ECQ9", verif.exact), self.importer.xrefs)
-        self.assertIn((3, enum["UniProtKB/TrEMBL"], b"Q6CI62", verif.exact), self.importer.xrefs)
+        self.assertIn(
+            (3, enum["UniProtKB/TrEMBL"], b"L8ECQ9", verif.exact), self.importer.xrefs
+        )
+        self.assertIn(
+            (3, enum["UniProtKB/TrEMBL"], b"Q6CI62", verif.exact), self.importer.xrefs
+        )
         mock_up.assert_called_with(self.up_extra_adder, "K7JG62", 5)
 
     def test_go(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         self.assertEqual(len(self.go_manager.add_annotations.call_args_list), 2)
 
     def test_ec(self, mock_up):
@@ -116,36 +126,43 @@
         self.db_parser.parse_entrytags(self.data)
         self.importer.flush_buffers()
         enum = pyoma.tablefmt.XRefTable.columns.get("XRefSource").enum
         verif = pyoma.tablefmt.XRefTable.columns.get("Verification").enum
         args, kwargs = self.importer.xref_tab.append.call_args_list[0]
         buffer = args[0]
         self.assertIn(
-            (5, enum.SourceAC, b"NV21158-PA", verif.exact),
-            buffer,
+            (5, enum.SourceAC, b"NV21158-PA", verif.exact), buffer,
         )
         self.assertIn(
-            (5, enum.SourceAC, b"NV21158-RA", verif.exact),
-            buffer,
+            (5, enum.SourceAC, b"NV21158-RA", verif.exact), buffer,
         )
         self.assertIn(
-            (5, enum.EnsemblGenomes, b"NV21158-RA", verif.exact),
-            buffer,
+            (5, enum.EnsemblGenomes, b"NV21158-RA", verif.exact), buffer,
         )
 
     def test_disambiguate(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         enum = pyoma.tablefmt.XRefTable.columns.get("XRefSource").enum
         verif = pyoma.tablefmt.XRefTable.columns.get("Verification").enum
-        self.assertIn((3, enum["FlyBase"], b"FBgn0218776", verif.unchecked), self.importer.xrefs)
-        self.assertIn((3, enum["FlyBase"], b"FBtr0247427", verif.unchecked), self.importer.xrefs)
-        self.assertIn((3, enum["SourceAC"], b"FBtr0247427", verif.exact), self.importer.xrefs)
-        self.assertIn((2, enum["SourceID"], b"BLABLA22", verif.exact), self.importer.xrefs)
+        self.assertIn(
+            (3, enum["FlyBase"], b"FBgn0218776", verif.unchecked), self.importer.xrefs
+        )
+        self.assertIn(
+            (3, enum["FlyBase"], b"FBtr0247427", verif.unchecked), self.importer.xrefs
+        )
+        self.assertIn(
+            (3, enum["SourceAC"], b"FBtr0247427", verif.exact), self.importer.xrefs
+        )
+        self.assertIn(
+            (2, enum["SourceID"], b"BLABLA22", verif.exact), self.importer.xrefs
+        )
         self.assertIn((2, enum["SourceID"], b"BLA22", verif.exact), self.importer.xrefs)
-        self.assertIn((1, enum["SourceID"], b"ENSG00000204640", verif.exact), self.importer.xrefs)
+        self.assertIn(
+            (1, enum["SourceID"], b"ENSG00000204640", verif.exact), self.importer.xrefs
+        )
         self.assertIn(
             (1, enum["Ensembl Gene"], b"ENSG00000204640", verif.exact),
             self.importer.xrefs,
         )
         self.assertIn(
             (1, enum["Ensembl Protein"], b"ENSP00000366061", verif.exact),
             self.importer.xrefs,
@@ -154,15 +171,17 @@
             (1, enum["Ensembl Transcript"], b"ENST00000376865", verif.exact),
             self.importer.xrefs,
         )
 
     def test_descriptions_passed_to_description_manager(self, mock_up):
         self.db_parser.parse_entrytags(self.data)
         self.assertEqual(len(self.desc_manager.add_description.call_args_list), 2)
-        self.assertEqual((3, "β-hemoglobin"), self.desc_manager.add_description.call_args[0])
+        self.assertEqual(
+            (3, "β-hemoglobin"), self.desc_manager.add_description.call_args[0]
+        )
 
     def test_remove_duplicated_xrefs(self, mock_up):
         ref = (1, 10, "test_id", "unchecked")
         res = (1, 10, b"test_id", 2)
         self.importer.FLUSH_SIZE = 20
         for i in range(self.importer.FLUSH_SIZE + 1):
             self.importer._add_to_xrefs(*ref)
@@ -180,17 +199,21 @@
         self.xref_tab.append.assert_not_called()
         self.importer.potential_flush()
         self.xref_tab.append.assert_called_once_with([res])
 
 
 class DescriptionManagerTest(unittest.TestCase):
     def setUp(self):
-        h5file = tables.open_file("test.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0)
+        h5file = tables.open_file(
+            "test.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0
+        )
         nr_rows = 3
-        data = numpy.zeros(nr_rows, dtype=tables.dtype_from_descr(pyoma.tablefmt.ProteinTable))
+        data = numpy.zeros(
+            nr_rows, dtype=tables.dtype_from_descr(pyoma.tablefmt.ProteinTable)
+        )
         data["EntryNr"] = numpy.arange(1, nr_rows + 1)
         h5file.create_table("/", "Entries", pyoma.tablefmt.ProteinTable, obj=data)
         self.h5 = h5file
 
     def tearDown(self):
         self.h5.close()
 
@@ -199,15 +222,15 @@
             for i, desc in enumerate(descs):
                 dm.add_description(i + 1, desc)
         exp_lens = numpy.array(list(len(z.encode("utf-8")) for z in descs), dtype="i4")
         exp_offs = numpy.cumsum(exp_lens) - exp_lens[0]
         entry_tab = self.h5.get_node("/Entries")
         numpy.array_equal(exp_lens, entry_tab.col("DescriptionLength"))
         numpy.array_equal(exp_offs, entry_tab.col("DescriptionOffset"))
-        txt = self.h5.get_node("/Descr").read().tobytes()
+        txt = self.h5.get_node("/Descr").read().tostring()
         self.assertEqual("".join(descs).encode("utf-8"), txt)
 
     def test_add_one_desc_per_entry(self):
         descs = ["hello", "some more lengthy test", "a"]
         self.check_descriptions_one_per_entry(descs)
 
     def test_add_with_unicode(self):
@@ -217,25 +240,27 @@
     def test_severl_descr_per_entry(self):
         descs = [["blabla", "βgamma", "bar"], [""], ["xxx", "yyy"]]
         with pyoma.DescriptionManager(self.h5, "/Entries", "/Descr") as dm:
             for i, per_entry_set in enumerate(descs):
                 for desc in per_entry_set:
                     dm.add_description(i + 1, desc)
         exp_txt = "".join(["; ".join(z) for z in descs])
-        txt_in_db = self.h5.get_node("/Descr").read().tobytes()
+        txt_in_db = self.h5.get_node("/Descr").read().tostring()
         self.assertEqual(exp_txt.encode("utf-8"), txt_in_db)
 
 
 class TestGeneOntologyManager(pyoma.GeneOntologyManager):
     ontology_url = "file://" + os.path.dirname(__file__) + "/go-basic-tiny.obo"
 
 
 class GeneOntologyManagerTest(unittest.TestCase):
     def setUp(self):
-        self.h5file = tables.open_file("test.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0)
+        self.h5file = tables.open_file(
+            "test.h5", "w", driver="H5FD_CORE", driver_core_backing_store=0
+        )
 
     def tearDown(self):
         self.h5file.close()
 
     def store_and_retrieve_data(self, enr, gos):
         with TestGeneOntologyManager(self.h5file, "/Annotation/GO", "/obo") as man:
             man.add_annotations(enr, gos)
@@ -263,16 +288,20 @@
         self.assertEqual("dummy-test/2017-04-18", vers)
 
     def test_add_obsolete_term_is_skipped(self):
         import sys
 
         if sys.version_info >= (3, 4):
             with self.assertLogs("pyoma", level="WARNING") as log:
-                res = self.store_and_retrieve_data(1, "GO:0003822@[[IEA,{OMA_Fun:001}]]")
-                self.assertIn("invalid GO term for entry 1: GO:0003822", ";".join(log.output))
+                res = self.store_and_retrieve_data(
+                    1, "GO:0003822@[[IEA,{OMA_Fun:001}]]"
+                )
+                self.assertIn(
+                    "invalid GO term for entry 1: GO:0003822", ";".join(log.output)
+                )
         else:
             res = self.store_and_retrieve_data(1, "GO:0003822@[[IEA,{OMA_Fun:001}]]")
         self.assertEqual(0, len(res))
 
     def test_go_obo_version(self):
         self.store_and_retrieve_data(1, "")
         obo = self.h5file.get_node("/obo")
```

### Comparing `pyoma-0.13.2/tests/inference/test_db.py` & `pyoma-0.9.4/tests/inference/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,35 +44,43 @@
         vpairs = pyoma.inference.db.VPairsOfEntry(self.indata)
         for en2 in (2, 1, 6):
             self.assertFalse(en2 in vpairs)
         self.assertTrue(5 in vpairs)
 
     def test_iterator(self):
         spairs = pyoma.inference.db.StablePairsOfEntry(self.indata)
-        self.assertEqual([x["EntryNr2"] for x in spairs], [1, 5], "Unexpected members in SPairs")
+        self.assertEqual(
+            [x["EntryNr2"] for x in spairs], [1, 5], "Unexpected members in SPairs"
+        )
 
     def test_matches(self):
         vpairs = pyoma.inference.db.VPairsOfEntry(self.indata)
-        self.assertEqual(1, len(vpairs.relations()), "Unexpected number of VPs returned")
+        self.assertEqual(
+            1, len(vpairs.relations()), "Unexpected number of VPs returned"
+        )
 
 
 class GenomePairTest(unittest.TestCase):
     def setUp(self):
         matches, itab = get_test_data()
         itab = np.array([0, 3, 3, 5, 5, 5, 5, 5, 5, 6]).reshape(5, 2)
         self.genome_pair = pyoma.inference.db.GenomePair(matches, itab)
 
     def test_get_entry(self):
-        prot1_matches = [(m["EntryNr1"], m["EntryNr2"]) for m in self.genome_pair[1]["ALL"]]
+        prot1_matches = [
+            (m["EntryNr1"], m["EntryNr2"]) for m in self.genome_pair[1]["ALL"]
+        ]
         self.assertEqual(
             [(1, 1), (1, 5), (1, 6)],
             prot1_matches,
             "unexpected matches with ALL selector",
         )
-        prot2_matches = [(m["EntryNr1"], m["EntryNr2"]) for m in self.genome_pair[2]["SP"]]
+        prot2_matches = [
+            (m["EntryNr1"], m["EntryNr2"]) for m in self.genome_pair[2]["SP"]
+        ]
         self.assertEqual([(2, 4)], prot2_matches, "unexpected matches with SP selector")
         self.assertEqual(
             0,
             len(self.genome_pair[3]["ALL"].relations()),
             "Unexpected matches, should be empty",
         )
 
@@ -80,15 +88,17 @@
         prot1_before = [z["EntryNr2"] for z in self.genome_pair[1]["BM"]]
         self.assertEqual([1, 5], prot1_before, "test-setup failed")
         self.genome_pair[1]["VP"] = [1, 6]
         prot2_after = [z["EntryNr2"] for z in self.genome_pair[1]["BM"]]
         self.assertEqual([1, 5, 6], prot2_after, "change of VP should set BM flag")
 
     def test_fail_if_not_member(self):
-        self.assertRaises(ValueError, self.genome_pair[2]["BM"].set_relations, [4, 6, 8])
+        self.assertRaises(
+            ValueError, self.genome_pair[2]["BM"].set_relations, [4, 6, 8]
+        )
 
     def test_iterators_in_sync(self):
         # create iterator before any changes on data
         bm_it = iter(self.genome_pair[1]["BM"])
         # set new bm pairs
         new_matches = [5, 6]
         self.genome_pair[1]["BM"] = new_matches
```

