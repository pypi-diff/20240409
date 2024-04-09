# Comparing `tmp/ogc_na-0.3.44.tar.gz` & `tmp/ogc_na-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.3.44.tar", last modified: Tue Apr  9 08:14:30 2024, max compression
+gzip compressed data, was "ogc_na-0.3.5.tar", last modified: Tue Jul 25 09:00:54 2023, max compression
```

## Comparing `ogc_na-0.3.44.tar` & `ogc_na-0.3.5.tar`

### file list

```diff
@@ -1,65 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.605177 ogc_na-0.3.44/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.593177 ogc_na-0.3.44/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.593177 ogc_na-0.3.44/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-09 08:14:23.000000 ogc_na-0.3.44/.github/workflows/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-09 08:14:23.000000 ogc_na-0.3.44/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-09 08:14:23.000000 ogc_na-0.3.44/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 08:14:23.000000 ogc_na-0.3.44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-09 08:14:30.605177 ogc_na-0.3.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-09 08:14:23.000000 ogc_na-0.3.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.593177 ogc_na-0.3.44/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-09 08:14:23.000000 ogc_na-0.3.44/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 08:14:23.000000 ogc_na-0.3.44/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-09 08:14:23.000000 ogc_na-0.3.44/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 08:14:23.000000 ogc_na-0.3.44/docs/jsonld-uplift.md
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-04-09 08:14:23.000000 ogc_na-0.3.44/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-09 08:14:23.000000 ogc_na-0.3.44/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.593177 ogc_na-0.3.44/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.597177 ogc_na-0.3.44/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc/na/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39808 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/gsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    35503 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.597177 ogc_na-0.3.44/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/input_filters/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16511 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 08:14:23.000000 ogc_na-0.3.44/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.601177 ogc_na-0.3.44/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 08:14:30.000000 ogc_na-0.3.44/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 08:14:23.000000 ogc_na-0.3.44/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.601177 ogc_na-0.3.44/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 08:14:23.000000 ogc_na-0.3.44/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 08:14:23.000000 ogc_na-0.3.44/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 08:14:23.000000 ogc_na-0.3.44/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:14:30.605177 ogc_na-0.3.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 08:14:23.000000 ogc_na-0.3.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.601177 ogc_na-0.3.44/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:30.601177 ogc_na-0.3.44/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/schema-vocab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-09 08:14:23.000000 ogc_na-0.3.44/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.430309 ogc_na-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 09:00:41.000000 ogc_na-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-25 09:00:41.000000 ogc_na-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 09:00:41.000000 ogc_na-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 09:00:54.438309 ogc_na-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 09:00:41.000000 ogc_na-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-25 09:00:41.000000 ogc_na-0.3.5/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-25 09:00:41.000000 ogc_na-0.3.5/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.430309 ogc_na-0.3.5/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc/na/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34070 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-25 09:00:41.000000 ogc_na-0.3.5/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.434309 ogc_na-0.3.5/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 09:00:54.000000 ogc_na-0.3.5/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-25 09:00:41.000000 ogc_na-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-25 09:00:41.000000 ogc_na-0.3.5/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-25 09:00:41.000000 ogc_na-0.3.5/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 09:00:41.000000 ogc_na-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:00:54.438309 ogc_na-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 09:00:41.000000 ogc_na-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:54.438309 ogc_na-0.3.5/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/schema-vocab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-25 09:00:41.000000 ogc_na-0.3.5/test/test_profile.py
```

### Comparing `ogc_na-0.3.44/.github/workflows/python-publish.yml` & `ogc_na-0.3.5/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - 'v*'
   workflow_dispatch: 
 
 permissions:
   contents: read
 
 jobs:
-  pypi-publish:
+  deploy:
 
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     #- name: Create release
     #  uses: actions/create-release@latest
```

### Comparing `ogc_na-0.3.44/.gitignore` & `ogc_na-0.3.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -280,9 +280,7 @@
 # Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
 poetry.toml
 
 
 # End of https://www.toptal.com/developers/gitignore/api/python,pycharm
 
 ogc/na/_version.py
-.idea/modules.xml
-.idea/
```

### Comparing `ogc_na-0.3.44/README.md` & `ogc_na-0.3.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 # ogc-na-tools
 
-## TL;DR
-
-You can install the tools with `pip`:
-
-```shell
-pip install ogc-na
-```
-
 ## Purpose
 This repository contains tools used to maintain controlled vocabularies and knowledge assets managed by the OGC Naming Authority. Such tools may have wider general applicability and be refactored into tool specific repositories.
 
 ## Scope
 The tools here manage ETL processes for ingesting source data into a dynamic knowledge graph. Whilst this is quite a generic scope, this provides examples of how to use a range of resources that others may reuse to achieve similar results.
 
 ## Highlights
@@ -29,17 +21,14 @@
 
 * `ingest_json`: Performs JSON-to-JSON-LD semantic uplifts [(read more)](https://opengeospatial.github.io/ogc-na-tools/reference/ogc/na/ingest_json/) 
 * `update_vocabs`: Allows defining RDF entailment + validation + upload pipelines [(read more)](https://opengeospatial.github.io/ogc-na-tools/reference/ogc/na/update_vocabs/)
 * `annotate_schema`: Annotates JSON schemas by leveraging `@modelReference` links to JSON-LD contexts [(read more)](https://opengeospatial.github.io/ogc-na-tools/reference/ogc/na/annotate_schema/)
 
 ## Development
 
-Note: This is only necessary if you are going to work *on* the tools themselves, not *with* them (see [TL;DR](#tldr)
-above). 
-
 To install runtime and development dependencies, run:
 
 ```shell
 pip install -e .[dev]
 ```
 
 ### Building the documentation
```

### Comparing `ogc_na-0.3.44/docs/examples.md` & `ogc_na-0.3.5/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/docs/gen_ref_pages.py` & `ogc_na-0.3.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/docs/index.md` & `ogc_na-0.3.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/docs/tutorials.md` & `ogc_na-0.3.5/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/mkdocs.yml` & `ogc_na-0.3.5/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,15 @@
       handlers:
         python:
           import:
             - https://rdflib.readthedocs.io/en/stable/objects.inv
           options:
             docstring_style: sphinx
 
-markdown_extensions:
-  - admonition
-  - pymdownx.details
-  - pymdownx.superfences
-
 watch:
   - ogc
 
 nav:
   - Overview: index.md
   - Tutorials: tutorials.md
   - Examples: examples.md
-  - JSON-LD Uplift: jsonld-uplift.md
   - Reference: reference/
```

### Comparing `ogc_na-0.3.44/ogc/na/annotate_schema.py` & `ogc_na-0.3.5/ogc/na/annotate_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,41 +112,36 @@
 The resulting context will be printed to the standard output.
 
 """
 
 from __future__ import annotations
 
 import argparse
-import csv
 import dataclasses
 import json
 import logging
 import re
 import sys
-from collections import deque
 from operator import attrgetter
 from pathlib import Path
 from typing import Any, AnyStr, Callable, Sequence, Iterable
 from urllib.parse import urlparse, urljoin
 
 import jsonschema
 import requests_cache
 
-from ogc.na.util import is_url, load_yaml, LRUCache, dump_yaml, \
-    merge_contexts, merge_dicts, dict_contains, JSON_LD_KEYWORDS
+from ogc.na.util import is_url, load_yaml, LRUCache, dump_yaml, merge_contexts, merge_dicts
 
 logger = logging.getLogger(__name__)
 
 ANNOTATION_PREFIX = 'x-jsonld-'
-ANNOTATION_CONTEXT = f'{ANNOTATION_PREFIX}context'
-ANNOTATION_ID = f'{ANNOTATION_PREFIX}id'
-ANNOTATION_PREFIXES = f'{ANNOTATION_PREFIX}prefixes'
-ANNOTATION_EXTRA_TERMS = f'{ANNOTATION_PREFIX}extra-terms'
-ANNOTATION_BASE = f'{ANNOTATION_PREFIX}base'
-
+ANNOTATION_CONTEXT = 'x-jsonld-context'
+ANNOTATION_ID = 'x-jsonld-id'
+ANNOTATION_PREFIXES = 'x-jsonld-prefixes'
+ANNOTATION_EXTRA_TERMS = 'x-jsonld-extra-terms'
 ANNOTATION_IGNORE_EXPAND = [ANNOTATION_CONTEXT, ANNOTATION_EXTRA_TERMS, ANNOTATION_PREFIXES]
 
 CURIE_TERMS = '@id', '@type', '@index'
 
 context_term_cache = LRUCache(maxsize=20)
 requests_session = requests_cache.CachedSession('ogc.na.annotate_schema', backend='memory', expire_after=180)
 
@@ -182,22 +177,19 @@
         self._schema_cache: dict[str | Path, tuple[Any, bool]] = {}
 
     @staticmethod
     def _get_branch(schema: dict, ref: str):
         path = re.sub(r'^#?/?', '', ref).split('/')
         pointer = schema
         for item in path:
-            if item:
+            if path:
                 pointer = pointer[item]
         return pointer
 
-    def load_contents(self, s: str | Path) -> tuple[dict, bool]:
-        """
-        Load the contents of a schema. Can be overriden by subclasses to alter the loading process.
-        """
+    def _load_contents(self, s: str | Path) -> tuple[dict, bool]:
         contents, is_json = self._schema_cache.get(s, (None, False))
         if contents is None:
             contents, is_json = load_json_yaml(read_contents(s)[0])
             self._schema_cache[s] = contents, is_json
         return contents, is_json
 
     def resolve_ref(self, ref: str | Path, from_schema: ReferencedSchema | None = None) -> tuple[Path | str, str]:
@@ -213,16 +205,14 @@
                 location = Path(location)
 
         if isinstance(location, Path):
             if location.is_absolute():
                 location = location.resolve()
             elif not from_schema:
                 location = self.working_directory.joinpath(location).resolve()
-            elif from_schema.full_contents.get('$id'):
-                location = urljoin(from_schema.full_contents['$id'], str(location))
             elif not isinstance(from_schema.location, Path):
                 location = urljoin(from_schema.location, str(location))
             else:
                 location = from_schema.location.resolve().parent.joinpath(location).resolve()
 
         if location is None:
             raise ValueError(f'Unexpected ref type {type(ref).__name__}')
@@ -245,15 +235,15 @@
                                         fragment=ref[1:],
                                         subschema=SchemaResolver._get_branch(from_schema.full_contents, ref),
                                         full_contents=from_schema.full_contents,
                                         chain=chain,
                                         ref=ref,
                                         is_json=from_schema.is_json)
 
-            contents, is_json = self.load_contents(schema_source)
+            contents, is_json = self._load_contents(schema_source)
             if fragment:
                 return ReferencedSchema(location=schema_source, fragment=fragment,
                                         subschema=SchemaResolver._get_branch(contents, fragment),
                                         full_contents=contents,
                                         chain=chain,
                                         ref=ref,
                                         is_json=is_json)
@@ -335,17 +325,16 @@
 
 
 def resolve_context(ctx: Path | str | dict | list, expand_uris=True) -> ResolvedContext:
     if not ctx:
         return ResolvedContext()
 
     prefixes = {}
-
     def expand_uri(curie, ctx_stack):
-        if not expand_uris or not ctx_stack or not curie or curie in JSON_LD_KEYWORDS:
+        if not expand_uris or not ctx_stack or not curie or curie[0] == '@':
             return curie
         if ':' in curie:
             prefix, localpart = curie.split(':', 1)
         else:
             prefix, localpart = None, None
         for c in reversed(ctx_stack):
             if localpart:
@@ -385,14 +374,16 @@
             fetched = r.json().get('@context')
             if fetched:
                 resolved = resolve_context(fetched)
         elif isinstance(inner_ctx, Sequence):
             resolved_ctx = {}
             inner_prefixes = {}
             for ctx_entry in inner_ctx:
+                if isinstance(ctx_entry, dict):
+                    ctx_entry = ctx_entry.get('@context')
                 resolved_entry = resolve_context(ctx_entry)
                 inner_prefixes.update(resolved_entry.prefixes)
                 resolved = ResolvedContext(merge_dicts(resolved_entry.context, resolved_ctx), inner_prefixes)
         else:
             if '@context' in inner_ctx:
                 inner_ctx = inner_ctx['@context']
             resolved = ResolvedContext(inner_ctx, {})
@@ -430,37 +421,31 @@
     Builds a set of annotated JSON schemas from a collection of input schemas
     that have `x-jsonld-context`s to JSON-LD context documents.
 
     The results will be stored in the `schemas` property (a dictionary of
     schema-path-or-url -> AnnotatedSchema mappings).
     """
 
-    def __init__(self, schema_resolver: SchemaResolver | None = None,
-                 ref_mapper: Callable[[str, Any], str] | None = None,
-                 ignore_existing: bool = False):
+    def __init__(self, ref_mapper: Callable[[str, Any], str] | None = None):
         """
-        :schema_resolver: an optional SchemaResolver to resolve references
         :ref_mapper: an optional function to map JSON `$ref`'s before resolving them
         """
-        self.schema_resolver = schema_resolver or SchemaResolver()
+        self._schema_resolver = SchemaResolver()
         self._ref_mapper = ref_mapper
-        self.ignore_existing = ignore_existing
 
     def process_schema(self, location: Path | str | None,
-                       default_context: str | Path | dict | None = None,
-                       contents: dict | None = None) -> AnnotatedSchema | None:
-        resolved_schema = self.schema_resolver.resolve_schema(location)
-        if contents:
-            # overriden
-            schema = contents
-        else:
-            schema = resolved_schema.subschema
+                       default_context: str | Path | dict | None = None) -> AnnotatedSchema | None:
+        resolved_schema = self._schema_resolver.resolve_schema(location)
+        schema = resolved_schema.subschema
 
-        if all(x not in schema for x in ('schema', 'openapi')):
-            validate_schema(schema)
+        try:
+            if '$schema' in schema and all(x not in schema for x in ('schema', 'openapi')):
+                validate_schema(schema)
+        except jsonschema.exceptions.SchemaError:
+            return None
 
         context_fn = schema.get(ANNOTATION_CONTEXT)
         schema.pop(ANNOTATION_CONTEXT, None)
 
         context = {}
         prefixes = {}
 
@@ -469,40 +454,38 @@
                                         and isinstance(default_context, Path)
                                         and default_context.resolve() == context_fn.resolve())):
             # Only load the provided context if it's different from the schema-referenced one
             resolved_default_context = resolve_context(default_context)
             context, prefixes = attrgetter('context', 'prefixes')(resolved_default_context)
 
         if context_fn:
-            context_fn, fragment = self.schema_resolver.resolve_ref(context_fn, resolved_schema)
+            context_fn, fragment = self._schema_resolver.resolve_ref(context_fn, resolved_schema)
             schema_context = resolve_context(context_fn)
 
             context = merge_contexts(context, schema_context.context)
             prefixes = prefixes | schema_context.prefixes
 
-        updated_refs: set[int] = set()
-
         def find_prop_context(prop, context_stack) -> dict | None:
             for ctx in reversed(context_stack):
                 vocab = ctx.get('@vocab')
                 if prop in ctx:
                     prop_ctx = ctx[prop]
                     if isinstance(prop_ctx, str):
-                        if vocab and ':' not in prop_ctx and prop_ctx not in JSON_LD_KEYWORDS:
+                        if vocab and ':' not in prop_ctx and prop_ctx[0] != '@':
                             prop_ctx = f"{vocab}{prop_ctx}"
                         return {'@id': prop_ctx}
                     elif '@id' not in prop_ctx and not vocab:
                         raise ValueError(f'Missing @id for property {prop} in context {json.dumps(ctx, indent=2)}')
                     else:
-                        result = {k: v for k, v in prop_ctx.items() if k in JSON_LD_KEYWORDS}
+                        result = {k: v for k, v in prop_ctx.items() if k.startswith('@')}
                         if vocab:
                             prop_id = result.get('@id')
                             if not prop_id:
                                 result['@id'] = f"{vocab}{prop}"
-                            elif ':' not in prop_id and prop_id not in JSON_LD_KEYWORDS:
+                            elif ':' not in prop_id and prop_id[0] != '@':
                                 result['@id'] = f"{vocab}{prop_id}"
                         return result
                 elif '@vocab' in ctx:
                     return {'@id': f"{ctx['@vocab']}{prop}"}
 
         def process_properties(obj: dict, context_stack: list[dict[str, Any]],
                                from_schema: ReferencedSchema, level) -> Iterable[str]:
@@ -511,35 +494,24 @@
             if not properties:
                 return ()
             if not isinstance(properties, dict):
                 raise ValueError('"properties" must be a dictionary')
 
             used_terms = set()
             for prop in list(properties.keys()):
-                if prop in JSON_LD_KEYWORDS:
+                if prop[0] == '@':
                     # skip JSON-LD keywords
                     continue
                 prop_value = properties[prop]
-
-                if not isinstance(prop_value, dict):
-                    continue
-
-                for key in list(prop_value.keys()):
-                    if self.ignore_existing and key.startswith(ANNOTATION_PREFIX):
-                        prop_value.pop(key, None)
-
                 prop_ctx = find_prop_context(prop, context_stack)
                 if prop_ctx:
                     used_terms.add(prop)
                     prop_schema_ctx = {f"{ANNOTATION_PREFIX}{k[1:]}": v
                                        for k, v in prop_ctx.items()
-                                       if k in JSON_LD_KEYWORDS and k != '@context'}
-                    prop_ctx_base = prop_ctx.get('@context', {}).get('@base')
-                    if prop_ctx_base:
-                        prop_schema_ctx[ANNOTATION_BASE] = prop_ctx_base
+                                       if k[0] == '@' and k != '@context'}
 
                     if not prop_value or prop_value is True:
                         properties[prop] = prop_schema_ctx
                     else:
                         for k, v in prop_schema_ctx.items():
                             prop_value.setdefault(k, v)
 
@@ -553,47 +525,29 @@
 
         def process_subschema(subschema, context_stack, from_schema: ReferencedSchema, level=1) -> Iterable[str]:
             if not subschema or not isinstance(subschema, dict):
                 return ()
 
             used_terms = set()
 
-            if '$ref' in subschema and id(subschema) not in updated_refs:
+            if '$ref' in subschema:
                 if self._ref_mapper:
                     subschema['$ref'] = self._ref_mapper(subschema['$ref'], subschema)
                 if subschema['$ref'].startswith('#/') or subschema['$ref'].startswith(f"{from_schema.location}#/"):
-                    target_schema = self.schema_resolver.resolve_schema(subschema['$ref'], from_schema)
+                    target_schema = self._schema_resolver.resolve_schema(subschema['$ref'], from_schema)
                     if target_schema:
-                        used_terms.update(process_subschema(target_schema.subschema, context_stack,
-                                                            target_schema, level + 1))
-                updated_refs.add(id(subschema))
+                        used_terms.update(process_subschema(target_schema.subschema, context_stack, target_schema, level + 1))
 
             # Annotate oneOf, allOf, anyOf
             for p in ('oneOf', 'allOf', 'anyOf'):
                 collection = subschema.get(p)
                 if collection and isinstance(collection, list):
                     for entry in collection:
                         used_terms.update(process_subschema(entry, context_stack, from_schema, level + 1))
 
-            # Annotate definitions and $defs
-            for p in ('definitions', '$defs'):
-                defs = subschema.get(p)
-                if defs and isinstance(defs, dict):
-                    for entry in defs.values():
-                        used_terms.update(process_subschema(entry, context_stack, from_schema, level + 1))
-
-            for p in ('then', 'else', 'additionalProperties'):
-                branch = subschema.get(p)
-                if branch and isinstance(branch, dict):
-                    used_terms.update(process_subschema(branch, context_stack, from_schema, level))
-
-            for pp in subschema.get('patternProperties', {}).values():
-                if pp and isinstance(pp, dict):
-                    used_terms.update(process_subschema(pp, context_stack, from_schema, level + 1))
-
             # Annotate main schema
             schema_type = subschema.get('type')
             if not schema_type and 'properties' in subschema:
                 schema_type = 'object'
 
             if schema_type == 'object':
                 used_terms.update(process_properties(subschema, context_stack, from_schema, level + 1))
@@ -605,26 +559,21 @@
             for p, bu in subschema.get(ANNOTATION_PREFIXES, {}).items():
                 if p not in prefixes:
                     prefixes[p] = bu
 
             if len(context_stack) == level and context_stack[-1]:
                 extra_terms = {}
                 for k, v in context_stack[-1].items():
-                    if k not in JSON_LD_KEYWORDS and k not in prefixes and k not in used_terms:
+                    if k[0] != '@' and k not in prefixes and k not in used_terms:
                         if isinstance(v, dict):
                             if len(v) == 1 and '@id' in v:
                                 v = v['@id']
                             else:
-                                v = {f"{ANNOTATION_PREFIX}{vk[1:]}": vv
-                                     for vk, vv in v.items()
-                                     if vk in JSON_LD_KEYWORDS}
-                        if isinstance(v, str) and v[-1] in ('#', '/', ':'):
-                            prefixes[k] = v
-                        else:
-                            extra_terms[k] = v
+                                v = {f"{ANNOTATION_PREFIX}{vk[1:]}": vv for vk, vv in v.items() if vk[0] == '@'}
+                        extra_terms[k] = v
                 if extra_terms:
                     subschema.setdefault(ANNOTATION_EXTRA_TERMS, {}).update(extra_terms)
 
             return used_terms
 
         process_subschema(schema, [context], resolved_schema)
 
@@ -640,227 +589,182 @@
 
 class ContextBuilder:
     """
     Builds a JSON-LD context from a set of annotated JSON schemas.
     """
 
     def __init__(self, location: Path | str = None,
-                 compact: bool = True,
-                 schema_resolver: SchemaResolver = None,
-                 version=1.1):
+                 compact: bool = True, ref_mapper: Callable[[str], str] | None = None):
         """
         :param location: file or URL load the annotated schema from
         :param compact: whether to compact the resulting context (remove redundancies, compact CURIEs)
         :ref_mapper: an optional function to map JSON `$ref`'s before resolving them
         """
         self.context = {'@context': {}}
         self._parsed_schemas: dict[str | Path, dict] = {}
+        self._ref_mapper = ref_mapper
 
-        self.schema_resolver = schema_resolver or SchemaResolver()
+        self._resolver = SchemaResolver()
 
         self.location = location
 
-        self.visited_properties: dict[str, str | None] = {}
-        self._missed_properties: dict[str, Any] = {}  # Dict instead of set to keep order of insertion
         context = self._build_context(self.location, compact)
-        if context:
-            context['@version'] = version
         self.context = {'@context': context}
 
     def _build_context(self, schema_location: str | Path,
                        compact: bool = True) -> dict:
 
         parsed = self._parsed_schemas.get(schema_location)
         if parsed:
             return parsed
 
-        root_schema = self.schema_resolver.resolve_schema(schema_location)
+        root_schema = self._resolver.resolve_schema(schema_location)
 
         prefixes = {}
 
         own_context = {}
 
         if prefixes:
             own_context.update(prefixes)
 
         def read_properties(subschema: dict, from_schema: ReferencedSchema,
-                            onto_context: dict, schema_path: list[str]) -> dict | None:
-            if schema_path:
-                schema_path_str = '/' + '/'.join(schema_path)
-            else:
-                schema_path_str = ''
+                            property_chain: list) -> dict | None:
             if not isinstance(subschema, dict):
                 return None
             if subschema.get('type', 'object') != 'object':
                 return None
+            subschema_context = {}
             for prop, prop_val in subschema.get('properties', {}).items():
-                full_property_path = schema_path + [prop]
-                full_property_path_str = f"{schema_path_str}/{prop}"
-                self.visited_properties.setdefault(full_property_path_str, None)
-                if from_schema == root_schema:
-                    self._missed_properties.setdefault(full_property_path_str, True)
                 if not isinstance(prop_val, dict):
                     continue
-                prop_context = {'@context': {}}
+                prop_context = {}
                 for term, term_val in prop_val.items():
-                    if term == ANNOTATION_BASE:
-                        prop_context.setdefault('@context', {})['@base'] = term_val
-                    elif term.startswith(ANNOTATION_PREFIX) and term not in ANNOTATION_IGNORE_EXPAND:
-                        if term == ANNOTATION_ID:
-                            self.visited_properties[full_property_path_str] = term_val
-                            self._missed_properties[full_property_path_str] = False
+                    if term.startswith(ANNOTATION_PREFIX) and term not in ANNOTATION_IGNORE_EXPAND:
                         prop_context['@' + term[len(ANNOTATION_PREFIX):]] = term_val
-
+                inner_context = process_subschema(prop_val, from_schema, property_chain + ['properties', prop])
+                if inner_context:
+                    prop_context['@context'] = inner_context
                 if isinstance(prop_context.get('@id'), str):
-                    self.visited_properties[full_property_path_str] = prop_context['@id']
-                    self._missed_properties[full_property_path_str] = False
-                    if prop_context['@id'] == '@nest':
-                        process_subschema(prop_val, from_schema, onto_context, full_property_path)
-                    else:
-                        process_subschema(prop_val, from_schema, prop_context['@context'], full_property_path)
-                    if prop not in onto_context or isinstance(onto_context[prop], str):
-                        onto_context[prop] = prop_context
-                    else:
-                        merge_contexts(onto_context[prop], prop_context)
-                else:
-                    process_subschema(prop_val, from_schema, onto_context, full_property_path)
+                    subschema_context[prop] = prop_context
+                elif inner_context:
+                    subschema_context = merge_contexts(subschema_context, inner_context, from_schema, property_chain)
 
-        imported_prefixes: dict[str | Path, dict[str, str]] = {}
-        imported_extra_terms: dict[str | Path, dict[str, str]] = {}
+            return subschema_context
 
-        def process_subschema(subschema: dict, from_schema: ReferencedSchema, onto_context: dict,
-                              schema_path: list[str]) -> dict | None:
+        def process_subschema(subschema, from_schema, property_chain=None) -> dict | None:
+
+            if property_chain is None:
+                property_chain = []
 
             if not isinstance(subschema, dict):
                 return None
 
-            if subschema.get(ANNOTATION_BASE):
-                onto_context['@base'] = subschema[ANNOTATION_BASE]
-
-            read_properties(subschema, from_schema, onto_context, schema_path)
+            sub_context = read_properties(subschema, from_schema, property_chain) or {}
 
             if '$ref' in subschema:
                 ref = subschema['$ref']
-                referenced_schema = self.schema_resolver.resolve_schema(ref, from_schema)
+                if self._ref_mapper:
+                    ref = self._ref_mapper(ref)
+                referenced_schema = self._resolver.resolve_schema(ref, from_schema)
                 if referenced_schema:
-                    process_subschema(referenced_schema.subschema, referenced_schema, onto_context,
-                                      schema_path)
+                    merge_contexts(sub_context,
+                                   process_subschema(referenced_schema.subschema, referenced_schema))
 
             for i in ('allOf', 'anyOf', 'oneOf'):
                 l = subschema.get(i)
                 if isinstance(l, list):
                     for idx, sub_subschema in enumerate(l):
-                        process_subschema(sub_subschema, from_schema, onto_context,
-                                          schema_path)
+                        sub_context = merge_contexts(sub_context,
+                                                     process_subschema(sub_subschema,
+                                                                       from_schema,
+                                                                       property_chain + [f"{i}[{idx}]"]),
+                                                     from_schema, property_chain)
 
-            for i in ('prefixItems', 'items', 'contains', 'then', 'else', 'additionalProperties'):
+            for i in ('prefixItems', 'items', 'contains'):
                 l = subschema.get(i)
                 if isinstance(l, dict):
-                    process_subschema(l, from_schema, onto_context, schema_path)
-
-            for pp_k, pp in subschema.get('patternProperties', {}).items():
-                if isinstance(pp, dict):
-                    process_subschema(pp, from_schema, onto_context, schema_path + [pp_k])
+                    items_ctx = process_subschema(l, from_schema, property_chain + [i])
+                    sub_context = merge_contexts(sub_context, items_ctx, from_schema, property_chain)
 
             if ANNOTATION_EXTRA_TERMS in subschema:
                 for extra_term, extra_term_context in subschema[ANNOTATION_EXTRA_TERMS].items():
-                    if extra_term not in onto_context:
-                        if isinstance(extra_term_context, dict):
-                            extra_term_context = {f"@{k[len(ANNOTATION_PREFIX):]}": v
-                                                  for k, v in extra_term_context.items()}
-                        onto_context[extra_term] = extra_term_context
+                    if extra_term not in sub_context:
+                        if isinstance(extra_term_context, str):
+                            extra_term_context = {'@id': extra_term_context}
+                        elif isinstance(extra_term_context, dict):
+                            extra_term_context = {f"@{k[len(ANNOTATION_PREFIX):]}": v for k, v in extra_term_context.items()}
+                        sub_context[extra_term] = extra_term_context
+
+            if sub_context:
+                fixed_sub_context = {}
+                for prop, prop_ctx in sub_context.items():
+                    if prop.startswith('@'):
+                        continue
+                    if '@id' in prop_ctx:
+                        fixed_sub_context[prop] = prop_ctx
+                    elif prop_ctx.get('@context'):
+                        merge_contexts(fixed_sub_context, prop_ctx['@context'], from_schema, property_chain)
+                sub_context = fixed_sub_context
+
+            sub_prefixes = subschema.get(ANNOTATION_PREFIXES)
+            if isinstance(sub_prefixes, dict):
+                prefixes.update(sub_prefixes)
 
-            if from_schema:
-                current_ref = f"{from_schema.location}{from_schema.ref}"
-                if current_ref not in imported_prefixes:
-                    sub_prefixes = subschema.get(ANNOTATION_PREFIXES, {})
-                    sub_prefixes |= from_schema.full_contents.get(ANNOTATION_PREFIXES, {})
-                    if sub_prefixes:
-                        imported_prefixes[current_ref] = sub_prefixes
-
-                if current_ref not in imported_extra_terms:
-                    sub_extra_terms = from_schema.full_contents.get(ANNOTATION_EXTRA_TERMS)
-                    if sub_extra_terms:
-                        imported_extra_terms[current_ref] = sub_extra_terms
-            else:
-                sub_prefixes = subschema.get(ANNOTATION_PREFIXES)
-                if isinstance(sub_prefixes, dict):
-                    prefixes.update({k: v for k, v in sub_prefixes.items() if k not in prefixes})
-
-        process_subschema(root_schema.subschema, root_schema, own_context, [])
-
-        for imported_et in imported_extra_terms.values():
-            for term, v in imported_et.items():
-                if term not in own_context:
-                    if isinstance(v, dict):
-                        v = {f"@{k[len(ANNOTATION_PREFIX):]}": val for k, val in v.items()}
-                    own_context[term] = v
+            return sub_context
 
-        for imported_prefix in imported_prefixes.values():
-            for p, v in imported_prefix.items():
-                if p not in prefixes:
-                    prefixes[p] = v
+        own_context = merge_contexts(own_context, process_subschema(root_schema.subschema, root_schema),
+                                     root_schema)
 
         for prefix in list(prefixes.keys()):
             if prefix not in own_context:
                 own_context[prefix] = {'@id': prefixes[prefix]}
             else:
                 del prefixes[prefix]
 
         if compact:
 
             def compact_uri(uri: str) -> str:
-                if uri in JSON_LD_KEYWORDS:
+                if uri.startswith('@'):
                     # JSON-LD keyword
                     return uri
 
                 for pref, pref_uri in prefixes.items():
                     if uri.startswith(pref_uri) and len(pref_uri) < len(uri):
                         local_part = uri[len(pref_uri):]
                         if local_part.startswith('//'):
                             return uri
                         return f"{pref}:{local_part}"
 
                 return uri
 
             def compact_branch(branch, context_stack=None) -> bool:
                 child_context_stack = context_stack + [branch] if context_stack else [branch]
-                terms = list(k for k in branch.keys() if k not in JSON_LD_KEYWORDS)
+                terms = list(k for k in branch.keys() if k[0] != '@')
 
                 changed = False
                 for term in terms:
                     term_value = branch[term]
-
-                    if isinstance(term_value, dict) and '@context' in term_value:
-                        if not term_value['@context']:
-                            del term_value['@context']
-                        else:
-                            while True:
-                                if not compact_branch(term_value['@context'], child_context_stack):
-                                    break
-
+                    deleted = False
                     if context_stack:
                         for ctx in context_stack:
-                            if term not in ctx:
-                                continue
-                            other = ctx[term]
-                            if isinstance(term_value, str):
-                                term_value = {'@id': term_value}
-                            if isinstance(other, str):
-                                other = {'@id': other}
-                            if dict_contains(other, term_value):
+                            if term in ctx and ctx[term] == term_value:
                                 del branch[term]
+                                deleted = True
                                 changed = True
                                 break
+                    if not deleted and isinstance(term_value, dict) and '@context' in term_value:
+                        while True:
+                            if not compact_branch(term_value['@context'], child_context_stack):
+                                break
 
                 return changed
 
             def compact_uris(branch, context_stack=None):
                 child_context_stack = context_stack + [branch] if context_stack else [branch]
-                terms = list(k for k in branch.keys() if k not in JSON_LD_KEYWORDS)
+                terms = list(k for k in branch.keys() if k[0] != '@')
                 for term in terms:
                     term_value = branch.get(term)
                     if isinstance(term_value, str):
                         branch[term] = compact_uri(term_value)
                     elif isinstance(term_value, dict):
                         if '@id' in term_value:
                             term_value['@id'] = compact_uri(term_value['@id'])
@@ -871,22 +775,18 @@
 
             compact_branch(own_context)
             compact_uris(own_context)
 
         self._parsed_schemas[schema_location] = own_context
         return own_context
 
-    @property
-    def missed_properties(self):
-        return [k for (k, v) in self._missed_properties.items() if v]
-
 
 def dump_annotated_schema(schema: AnnotatedSchema, subdir: Path | str = 'annotated',
-                          root_dir: Path | str | None = None,
-                          output_fn_transform: Callable[[Path], Path] | None = None) -> None:
+                           root_dir: Path | str | None = None,
+                           output_fn_transform: Callable[[Path], Path] | None = None) -> None:
     """
     Creates a "mirror" directory (named `annotated` by default) with the resulting
     schemas annotated by a `SchemaAnnotator`.
 
     :param schema: the `AnnotatedSchema` to dump
     :param subdir: a name for the mirror directory
     :param root_dir: root directory for computing relative paths to schemas
@@ -912,14 +812,15 @@
             json.dump(schema.schema, f, indent=2)
     else:
         dump_yaml(schema.schema, output_fn)
 
 
 def _main():
     parser = argparse.ArgumentParser(
+        prog='JSON Schema @id injector'
     )
 
     parser.add_argument(
         'schema',
         help='Entrypoint JSON Schema (filename or URL)',
     )
 
@@ -953,25 +854,14 @@
     parser.add_argument(
         '-b',
         '--context-batch',
         help="Write JSON-LD context to a file with the same name and .jsonld extension (implies --build-context)",
         action='store_true',
     )
 
-    parser.add_argument(
-        '--dump-visited',
-        help='Dump visited properties and their ids to a file',
-    )
-
-    parser.add_argument(
-        '--ignore-existing',
-        help="Ignore existing x-jsonld- properties when annotating",
-        action='store_true',
-    )
-
     args = parser.parse_args()
 
     if not args.schema:
         print('Error: no file and no URL provided', file=sys.stderr)
         parser.print_usage(file=sys.stderr)
         sys.exit(2)
 
@@ -979,27 +869,16 @@
         ctx_builder = ContextBuilder(args.schema)
         if args.context_batch:
             fn = Path(args.file).with_suffix('.jsonld')
             with open(fn, 'w') as f:
                 json.dump(ctx_builder.context, f, indent=2)
         else:
             print(json.dumps(ctx_builder.context, indent=2))
-        if args.dump_visited:
-            def write_visited(stream):
-                writer = csv.writer(stream, delimiter='\t')
-                writer.writerow(['path', '@id'])
-                writer.writerows(ctx_builder.visited_properties.items())
-
-            if args.dump_visited == '-':
-                write_visited(sys.stdout)
-            else:
-                with open(args.dump_visited, 'w', newline='') as f:
-                    write_visited(f)
     else:
-        annotator = SchemaAnnotator(ignore_existing=args.ignore_existing)
+        annotator = SchemaAnnotator()
         annotated = annotator.process_schema(args.schema, args.context)
         print(dump_yaml(annotated.schema))
 
 
 if __name__ == '__main__':
     logging.basicConfig(
         stream=sys.stderr,
```

### Comparing `ogc_na-0.3.44/ogc/na/domain_config.py` & `ogc_na-0.3.5/ogc/na/domain_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     `dcfg:hasUpliftDefinition` can also be used to declare (ordered) semantic uplift definitions, either
     from profile artifacts or from files.
     """
 
     def __init__(self, source: Union[Graph, str, Path, IO], working_directory: str | Path = None,
                  profile_sources: str | Path | Iterable[str | Path] | None = None,
-                 ignore_artifact_errors=False, local_artifacts_mappings: dict | None = None):
+                 ignore_artifact_errors=False):
         """
         Creates a new DomainConfiguration, optionally specifying the working directory.
 
         :param source: Graph or Turtle file to load
         :param working_directory: the working directory to use for local paths.
         """
         if working_directory:
@@ -120,17 +120,15 @@
         elif isinstance(source, str) or isinstance(source, Path):
             self.working_directory = Path(source).parent.resolve()
         else:
             self.working_directory = Path().resolve()
         logger.info("Working directory: %s", self.working_directory)
         self.entries = ConfigurationEntryList()
         self.uplift_entries = UpliftConfigurationEntryList()
-        self.local_artifacts_mappings = {}
-        if local_artifacts_mappings:
-            self.local_artifacts_mappings.update(local_artifacts_mappings)
+        self.local_artifacts_mapping = {}
         self.profile_registry: ProfileRegistry | None = None
         self._profile_sources = profile_sources
         self._ignore_artifact_errors = ignore_artifact_errors
 
         self._load(source)
 
     def _load(self, source: Union[Graph, str, IO]):
@@ -159,59 +157,54 @@
 
             if bool(cfg_graph.value(catalog_ref, DCFG.ignoreProfileArtifactErrors)):
                 ignore_profile_artifact_errors = True
 
             # Local artifacts mapping
             for mapping_ref in cfg_graph.objects(catalog_ref, DCFG.localArtifactMapping):
                 base_uri = str(cfg_graph.value(mapping_ref, DCFG.baseURI))
-                if base_uri in self.local_artifacts_mappings:
-                    logger.debug("Local artifact mapping for %s overriden", base_uri)
-                    # Overriden
-                    continue
                 local_path = Path(str(cfg_graph.value(mapping_ref, DCFG.localPath)))
                 logger.debug("Found local artifact mapping: %s -> %s", base_uri, local_path)
-                self.local_artifacts_mappings[base_uri] = local_path
+                self.local_artifacts_mapping[base_uri] = local_path
 
             # Profile sources
             for p in cfg_graph.objects(catalog_ref, DCFG.hasProfileSource):
                 if not isinstance(p, Literal):
                     continue
                 if p.value.startswith('sparql:'):
                     prof_sources.add(p.value)
                 else:
                     prof_sources.update(self.working_directory.glob(p.value))
 
             if self._profile_sources:
                 prof_sources.update(self._profile_sources)
 
         self.profile_registry = ProfileRegistry(prof_sources,
-                                                ignore_artifact_errors=ignore_profile_artifact_errors,
-                                                local_artifact_mappings=self.local_artifacts_mappings)
+                                                ignore_artifact_errors=ignore_profile_artifact_errors)
 
         for cfg_ref in cfg_graph.objects(predicate=DCAT.dataset):
 
             globs = [str(g) for g in cfg_graph.objects(cfg_ref, DCFG.glob)]
 
             # DomainConfigurationEntry specific properties
             uri_root_filter = cfg_graph.value(cfg_ref, DCFG.uriRootFilter)
             profile_refs = cast(list[URIRef], list(cfg_graph.objects(cfg_ref, DCTERMS.conformsTo)))
 
             # UpliftConfigurationEntry specific properties
             found_uplift_defs = []
             max_order = None
             for uplift_def_ref in cfg_graph.objects(cfg_ref, DCFG.hasUpliftDefinition):
                 order = cfg_graph.value(uplift_def_ref, DCFG.order)
-                if order is not None and (max_order is None or int(order) > max_order):
-                    max_order = int(order)
+                if order is not None and (max_order is None or order > max_order):
+                    max_order = order
                 target_prof = cfg_graph.value(uplift_def_ref, DCFG.profile)
                 target_file = cfg_graph.value(uplift_def_ref, DCFG.file)
                 if target_prof:
                     found_uplift_defs.append([order, target_prof])
                 elif target_file:
-                    found_uplift_defs.append([order, self.working_directory.joinpath(str(target_file)).resolve()])
+                    found_uplift_defs.append([order, self.working_directory.joinpath(target_file).resolve()])
             uplift_defs = [p[1] for p in
                            sorted(found_uplift_defs,
                                   key=lambda u: u[0] if u[0] is not None else max_order + 1)]
 
             identifier = cfg_graph.value(cfg_ref, DCTERMS.identifier) or str(cfg_ref)
 
             if profile_refs:
```

### Comparing `ogc_na-0.3.44/ogc/na/download.py` & `ogc_na-0.3.5/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/ogc/na/gsp.py` & `ogc_na-0.3.5/ogc/na/gsp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 SPARQL Graph Store Protocol operations
 """
 from __future__ import annotations
 
 import argparse
-import getpass
 import sys
 from io import IOBase
 from pathlib import Path
 from typing import Generator, IO
 
 import requests
 from rdflib import Graph
@@ -153,40 +152,20 @@
 
     parser.add_argument(
         '--data-file',
         help='Data file for add/post and replace/put operations. If "-", read from stdin',
     )
 
     parser.add_argument(
-        '-u',
-        '--username',
-        help='Username for HTTP authentication',
-    )
-
-    parser.add_argument(
-        '-p',
-        '--password',
-        help='Password for HTTP authentication',
-    )
-
-    parser.add_argument(
-        '-P',
-        '--request-password',
-        action='store_true',
-        help='Request password from the user interactively',
+        '--auth',
+        help='HTTP Authentication in the form username:password',
     )
 
     args = parser.parse_args()
-
-    if args.request_password:
-        password = getpass.getpass("Password: ")
-    else:
-        password = args.password
-
-    auth = (args.username, password) if args.username else None
+    auth = tuple(args.auth.split(':', 1)) if args.auth else None
     gs = GraphStore(args.graph_store, auth_details=auth)
     if args.operation in ('add', 'replace', 'post', 'put'):
         if not (args.data or args.data_file):
             parser.error('Operation requires either --data or --data-file')
         if args.data and args.data_file:
             parser.error('Only one of --data, --data-file must be provided')
         if args.data == '-':
```

### Comparing `ogc_na-0.3.44/ogc/na/ingest_json.py` & `ogc_na-0.3.5/ogc/na/ingest_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 3. Otherwise, a `_json-context.yml` file in the same directory will be used, if it exists.
 
 If no context definition file is found after performing the previous 3 steps, then the file will
 be skipped.
 """
 from __future__ import annotations
 import argparse
-import functools
 import json
 import logging
 import os
 import os.path
 import re
 import sys
 import uuid
@@ -39,16 +38,18 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from os import scandir
 from pathlib import Path
 from typing import Union, Optional, Sequence, cast, Iterable, Any
 
 import jq
+import pyld.jsonld
 from jsonpath_ng.ext import parse as json_path_parse
 from jsonschema import validate as json_validate
+from pyld import jsonld
 from rdflib import Graph, DC, DCTERMS, SKOS, OWL, RDF, RDFS, XSD, DCAT
 from rdflib.namespace import Namespace, DefinedNamespace
 
 from ogc.na import util, profile
 from ogc.na.domain_config import UpliftConfigurationEntry, DomainConfiguration
 from ogc.na.provenance import ProvenanceMetadata, FileProvenanceMetadata, generate_provenance
 from ogc.na.input_filters import apply_input_filter
@@ -73,19 +74,14 @@
 }
 
 VOCAB_DELIMITERS = {"#", "/", ":"}
 
 UPLIFT_CONTEXT_SCHEMA = {
     "type": "object",
     "properties": {
-        "input-filter": {
-            "type": "object",
-            "maxProperties": 1,
-            "minProperties": 1,
-        },
         "path-scope": {
             "type": "string",
             "enum": ["graph", "document"],
         },
         "transform": {
             "anyOf": [
                 {
@@ -144,14 +140,31 @@
 class UpliftResult:
     input_file: Path = None
     uplifted_json: dict | list = None
     graph: Graph = None
     output_files: list[Path] = field(default_factory=list)
 
 
+def _document_loader(secure: bool = False,
+                     url_whitelist: Optional[Union[Sequence, bool]] = None,
+                     **kwargs):
+    if url_whitelist is False:
+        raise ValueError("Remote document fetching is disabled (url_whitelist is False)")
+    if isinstance(url_whitelist, str):
+        url_whitelist = (re.compile(url_whitelist),)
+    wrapped = jsonld.requests_document_loader(secure=secure, **kwargs)
+
+    def loader(url, options=None):
+        if url_whitelist is not None and not any(re.match(r, url) for r in url_whitelist if r):
+            raise ValueError('Remote document fetching not allowed for URL {}'.format(url))
+        return wrapped(url, options=options or {})
+
+    return loader
+
+
 def validate_context(context: Union[dict, str] = None,
                      filename: Union[str, Path] = None,
                      transform_args: dict | None = None) -> dict:
     if not context and not filename:
         return {}
     if bool(context) == bool(filename):
         raise ValueError("Only one of context or filename required")
@@ -199,33 +212,37 @@
     if not isinstance(json_doc, list):
         json_doc = [json_doc]
     json_doc.extend(prov)
     return json_doc
 
 
 def uplift_json(data: dict | list, context: dict,
+                fetch_timeout: int = 5,
                 fetch_url_whitelist: Optional[Union[Sequence, bool]] = None,
                 transform_args: dict | None = None) -> dict:
     """
     Transform a JSON document loaded in a dict, and embed JSON-LD context into it.
 
     WARNING: This function modifies the input dict. If that is not desired, make a copy
     before invoking.
 
     :param data: the JSON document in dict format
     :param context: YAML context definition
+    :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception.
     :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: the transformed and JSON-LD-enriched data
     """
 
     context_position = context.get('position', 'before')
 
+    jsonld.set_document_loader(_document_loader(timeout=fetch_timeout, url_whitelist=fetch_url_whitelist))
+
     validate_context(context, transform_args=transform_args)
 
     # Check whether @graph scoping is necessary for transformations and paths
     scoped_graph = context.get('scope', 'graph') == 'graph' and '@graph' in data
     data_graph = data['@graph'] if scoped_graph else data
 
     # Check if pre-transform necessary
@@ -265,23 +282,22 @@
         if not loc or loc in ['.', '$']:
             global_context = val
         else:
             items = json_path_parse(loc).find(data_graph)
             for item in items:
                 item.value['@context'] = _get_injected_context(item.value, val, context_position)
 
-    if isinstance(data_graph, dict):
-        data_context = data_graph.pop('@context', None)
-        if data_context:
-            if not global_context:
-                global_context = data_context
-            elif isinstance(global_context, list):
-                global_context.extend(data_context)
-            else:
-                global_context = [data_context, global_context]
+    data_context = data_graph.pop('@context', None)
+    if data_context:
+        if not global_context:
+            global_context = data_context
+        elif isinstance(global_context, list):
+            global_context.extend(data_context)
+        else:
+            global_context = [data_context, global_context]
 
     if (global_context and not isinstance(data_graph, dict)) or scoped_graph:
         return {
             '@context': _get_injected_context(data, global_context, context_position),
             '@graph': data_graph,
         }
     else:
@@ -322,22 +338,24 @@
 
     return result
 
 
 def generate_graph(input_data: dict | list,
                    context: dict[str, Any] | Sequence[dict] = None,
                    base: str | None = None,
+                   fetch_timeout: int = 5,
                    fetch_url_whitelist: Sequence[str] | bool | None = None,
                    transform_args: dict | None = None) -> UpliftResult:
     """
     Create a graph from an input JSON document and a YAML context definition file.
 
     :param input_data: input JSON data in dict or list format
     :param context: context definition in dict format, or list thereof
     :param base: base URI for JSON-LD context
+    :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception.
     :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: a tuple with the resulting RDFLib Graph and the JSON-LD enriched file name
     """
 
@@ -351,76 +369,70 @@
         for prefix, ns in DEFAULT_NAMESPACES.items():
             g.bind(prefix, Namespace(ns))
 
         context_list = context if isinstance(context, Sequence) else (context,)
         for context_entry in context_list:
             base_uri = context_entry.get('base-uri', base_uri)
             jdoc_ld = uplift_json(input_data, context_entry,
+                                  fetch_timeout=fetch_timeout,
+                                  fetch_url_whitelist=fetch_url_whitelist,
                                   transform_args=transform_args)
             if 'context' in context_entry:
                 if '$' in context_entry['context']:
                     root_ctx = context_entry['context']['$']
                 elif '.' in context_entry['context']:
                     root_ctx = context_entry['context']['.']
                 else:
                     continue
 
-                if isinstance(root_ctx, dict):
-                    for term, term_val in root_ctx.items():
-                        if not term.startswith('@') \
-                                and isinstance(term_val, str) \
-                                and re.match(r'.+[#/:]$', term_val) \
-                                and is_iri(term_val):
-                            g.bind(term, term_val)
+                for term, term_val in root_ctx.items():
+                    if not term.startswith('@') \
+                            and isinstance(term_val, str) \
+                            and re.match(r'.+[#/:]$', term_val) \
+                            and is_iri(term_val):
+                        g.bind(term, term_val)
 
+        options = {}
         if not base:
             if base_uri:
-                base = context['base-uri']
+                options['base'] = context['base-uri']
             elif '@context' in jdoc_ld:
                 # Try to extract from @context
                 # If it is a list, iterate until @base is found
                 base = None
                 if isinstance(jdoc_ld['@context'], list):
                     for entry in jdoc_ld['@context']:
                         if not isinstance(entry, dict):
                             continue
                         base = entry.get('@base')
                         if base:
                             break
                 else:
                     # If not a list, just look @base up
                     base = jdoc_ld['@context'].get('@base')
+        if base:
+            options['base'] = base
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug('Uplifted JSON:\n%s', json.dumps(jdoc_ld, indent=2))
 
-    def remote_context_url_filter(url_whitelist: str | list[str], url: str):
-        if url_whitelist is False:
-            return False
-        if url_whitelist is True or url_whitelist is None:
-            return True
-        if isinstance(url_whitelist, str):
-            url_whitelist = re.compile(url_whitelist)
-        else:
-            url_whitelist = [re.compile(x) for x in url_whitelist if x]
-        return any(re.match(r, url) for r in url_whitelist)
-
-    g.parse(data=json.dumps(jdoc_ld), format='json-ld', base=base,
-            remote_context_url_filter=functools.partial(remote_context_url_filter, fetch_url_whitelist))
+    expanded = pyld.jsonld.expand(jdoc_ld, options)
+    g.parse(data=json.dumps(expanded), format='json-ld')
 
     return UpliftResult(graph=g, uplifted_json=jdoc_ld)
 
 
 def process_file(input_fn: str | Path,
                  jsonld_fn: str | Path | bool | None = False,
                  ttl_fn: str | Path | bool | None = False,
                  context_fn: str | Path | Sequence[str | Path] | None = None,
                  domain_cfg: DomainConfiguration | None = None,
                  base: str | None = None,
                  provenance_base_uri: str | bool | None = None,
                  provenance_process_id: str | None = None,
+                 fetch_timeout: int = 5,
                  fetch_url_whitelist: bool | Sequence[str] | None = None,
                  transform_args: dict | None = None) -> UpliftResult | None:
     """
     Process input file and generate output RDF files.
 
     :param input_fn: input filename
     :param jsonld_fn: output JSON-lD filename (None for automatic).
@@ -431,14 +443,15 @@
         1. From a file with the same name but yml/yaml extension (test.json -> test.yml)
         2. From the domain_cfg
         3. From a _json-context.yml/_json-context.yaml file in the same directory
     :param domain_cfg: domain configuration with uplift definition locations
     :param base: base URI for JSON-LD
     :param provenance_base_uri: base URI for provenance resources
     :param provenance_process_id: process identifier for provenance tracking
+    :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception
     :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: List of output files created
     """
 
@@ -477,16 +490,16 @@
     # Apply input filter of first context only (if any)
     input_filters = contexts[0].get('input-filter')
     if input_filters:
         if not isinstance(input_filters, dict):
             raise ValueError('input-filter must be an object')
         input_data = apply_input_filter(input_fn, input_filters)
     else:
-        # Accept both JSON and YAML
-        input_data = util.load_yaml(input_fn)
+        with open(input_fn, 'r') as j:
+            input_data = json.load(j)
 
     if logger.isEnabledFor(logging.DEBUG):
         logger.debug('Input data:\n%s', json.dumps(input_data, indent=2))
 
     provenance_metadata: ProvenanceMetadata | None = None
     if provenance_base_uri is not False:
         used = [FileProvenanceMetadata(filename=input_fn, mime_type='application/json')]
@@ -509,14 +522,15 @@
 
     if not base:
         base = str(input_fn)
 
     uplift_result = generate_graph(input_data,
                                    context=contexts,
                                    base=base,
+                                   fetch_timeout=fetch_timeout,
                                    fetch_url_whitelist=fetch_url_whitelist,
                                    transform_args=transform_args)
 
     uplift_result.input_file = input_fn
 
     # False = do not generate
     # None = auto filename
@@ -560,15 +574,15 @@
 
 
 def find_contexts(filename: Path | str,
                   domain_config: DomainConfiguration | None = None) -> list[Path | str] | None:
     """
     Find the YAML context file for a given filename, with the following precedence:
         1. Search in registry (if provided)
-        2. Search file with same base name but with yaml/yml or "-uplift.yml" extension.
+        2. Search file with same base name but with yaml/yml extension.
         3. Find _json-context.yml/yaml file in same directory
     :param filename: the filename for which to find the context
     :param domain_config: an optional filename:yamlContextFile mapping
     :return: the YAML context definition paths (Path) and/or profile URIs (str)
     """
 
     if not isinstance(filename, Path):
@@ -578,26 +592,22 @@
     if domain_config:
         entry: UpliftConfigurationEntry = domain_config.uplift_entries.find_entry_for_file(filename)
         if entry:
             return entry.uplift_definitions
 
     # 2. Same filename with yml/yaml extension or autodetect in dir
     for context_path in (
-        filename.with_name(filename.stem + '-uplift.yml'),
-        filename.with_name(filename.stem + '-uplift.yaml'),
         filename.with_suffix('.yml'),
         filename.with_suffix('.yaml'),
         filename.with_suffix('').with_suffix('.yml'),
         filename.with_suffix('').with_suffix('.yaml'),
         filename.parent / '_json-context.yml',
         filename.parent / '_json-context.yaml',
     ):
-        if filename == context_path:
-            continue
-        if context_path.is_file() and not (filename.suffix == '.jsonld' and filename.with_suffix('.json').is_file()):
+        if context_path.is_file():
             logger.info(f'Autodetected context {context_path} for file {filename}')
             return [context_path]
 
 
 def filenames_from_context(context_fn: Path | str,
                            domain_config: DomainConfiguration | None) -> list[Path]:
     """
@@ -650,17 +660,17 @@
             context_fn: str | Path | None = None,
             jsonld_fn: bool | str | Path | None = False,
             ttl_fn: bool | str | Path | None = False,
             batch: bool = False,
             base: str = None,
             skip_on_missing_context: bool = False,
             provenance_base_uri: Optional[Union[str, bool]] = None,
+            fetch_timeout: int = 5,
             fetch_url_whitelist: Optional[Union[Sequence, bool]] = None,
-            transform_args: dict | None = None,
-            file_filter: str | re.Pattern = None) -> list[UpliftResult]:
+            transform_args: dict | None = None) -> list[UpliftResult]:
     """
     Performs the JSON-LD uplift process.
 
     :param input_files: list of input, plain JSON files
     :param domain_cfg: domain configuration including uplift definition locations
     :param context_fn: used to force the YAML context file name for the uplift. If `None`,
            it will be autodetected
@@ -669,19 +679,19 @@
     :param ttl_fn: output file name for the Turtle RDF content. If it is `False`, no Turtle
            output will be generated. If it is `None`, output will be written to stdout.
     :param batch: in batch mode, all JSON input files are obtained from the context registry
            and processed
     :param base: base URI to employ
     :param skip_on_missing_context: whether to silently fail if no context file is found
     :param provenance_base_uri: base URI for provenance resources
+    :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception
     :param transform_args: Additional arguments to pass as variables to the jq transform
-    :param file_filter: Filename filter for input files
     :return: a list of JSON-LD and/or Turtle output files
     """
     result: list[UpliftResult] = []
     process_id = str(uuid.uuid4())
     workdir = Path()
     if isinstance(input_files, str) or not isinstance(input_files, Sequence):
         input_files = (input_files,)
@@ -699,57 +709,52 @@
                 remaining_fn.append(input_file)
         while remaining_fn:
             fn = str(remaining_fn.popleft())
 
             if not fn or not os.path.isfile(fn):
                 continue
 
-            if file_filter and not re.search(file_filter, fn):
-                continue
-
             if re.match(r'.*\.ya?ml$', fn):
-                # Check whether this is a context definition or a doc to uplift
-                has_context = bool(find_contexts(fn, domain_cfg))
-
-                if not has_context:
-                    # Potential context file found, try to find corresponding JSON/JSON-LD file(s)
-                    logger.info('Potential YAML context file found: %s', fn)
-                    remaining_fn.extend(filenames_from_context(fn, domain_config=domain_cfg) or [])
-                    continue
+                # Context file found, try to find corresponding JSON/JSON-LD file(s)
+                logger.info('Potential YAML context file found: %s', fn)
+                remaining_fn.extend(filenames_from_context(fn, domain_config=domain_cfg) or [])
+                continue
 
             logger.info('File %s matches, processing', fn)
             try:
                 result.append(process_file(
                     fn,
                     jsonld_fn=False if jsonld_fn is False else None,
                     ttl_fn=False if ttl_fn is False else None,
                     context_fn=None,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
+                    fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
                     domain_cfg=domain_cfg,
                     transform_args=transform_args,
                 ))
             except MissingContextException as e:
-                if skip_on_missing_context or batch:
+                if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
                 else:
                     raise
     else:
         for input_file in input_files:
             try:
                 result.append(process_file(
                     input_file,
                     jsonld_fn=jsonld_fn if jsonld_fn is not None else '-',
                     ttl_fn=ttl_fn if ttl_fn is not None else '-',
                     context_fn=context_fn,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
+                    fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
                     domain_cfg=domain_cfg,
                     transform_args=transform_args,
                 ))
             except Exception as e:
                 if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
@@ -832,68 +837,53 @@
     parser.add_argument(
         '--provenance-base-uri',
         help='Base URI to employ for provenance metadata generation (from working directory)'
     )
 
     parser.add_argument(
         '--url-whitelist',
+        '-w',
         nargs='*',
         help='Regular expression for URL whitelisting'
     )
 
     parser.add_argument(
         '--use-git-status',
         action='store_true',
         help='Use git status for obtaining batch filenames'
     )
 
     parser.add_argument(
-        '-a',
-        '--all',
-        action='store_true',
-        help='Run uplift for all catalog files in batch mode'
-    )
-
-    parser.add_argument(
         '--debug',
         action='store_true',
         help='Enable debug mode'
     )
 
     parser.add_argument(
-        '-w',
         '--work-dir',
         help='Set root directory for globs in domain configurations'
     )
 
     parser.add_argument(
         '--transform-arg',
         nargs='*',
         help='Additional argument to pass to the jq transforms in the form variable=value'
     )
 
-    parser.add_argument(
-        '--file-filter',
-        help='Regular expression to filter input filenames',
-    )
-
     args = parser.parse_args()
 
     if args.domain_config:
         domain_cfg = DomainConfiguration(args.domain_config, args.work_dir)
     else:
         domain_cfg = None
 
     input_files = args.input
-    if args.batch:
-        if args.use_git_status:
-            git_status = util.git_status()
-            input_files = git_status['added'] + git_status['modified'] + [r[1] for r in git_status['renamed']]
-        elif args.all:
-            input_files = list(set(fn for fn in domain_cfg.uplift_entries.find_all()))
+    if args.batch and args.use_git_status:
+        git_status = util.git_status()
+        input_files = git_status['added'] + git_status['modified'] + [r[1] for r in git_status['renamed']]
     elif not input_files:
         print("Error: no input files provided")
         sys.exit(1)
 
     if args.debug:
         logger.setLevel(logging.DEBUG)
 
@@ -907,15 +897,14 @@
                      jsonld_fn=args.json_ld_file if args.json_ld else False,
                      ttl_fn=args.ttl_file if args.ttl else False,
                      batch=args.batch,
                      skip_on_missing_context=args.skip_on_missing_context,
                      provenance_base_uri=False if args.no_provenance else args.provenance_base_uri,
                      fetch_url_whitelist=args.url_whitelist,
                      transform_args=transform_args,
-                     file_filter=args.file_filter,
              )
 
     if args.fs:
         print(args.fs.join(str(output_file) for r in result for output_file in r.output_files))
 
 
 if __name__ == '__main__':
```

### Comparing `ogc_na-0.3.44/ogc/na/input_filters/__init__.py` & `ogc_na-0.3.5/ogc/na/input_filters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Any, IO, TextIO
 
 from ogc.na.util import deep_update
 
 
 def apply_input_filter(stream: IO | bytes | str | Path, filters: dict[str, dict]) -> dict[str, Any] | list:
-    filter_name, filter_conf = next(iter(filters.items()))
+    filter_name, filter_conf = filters.popitem()
 
     metadata = {
         'filter': {
             'name': filter_name,
             'conf': filter_conf,
         },
     }
```

### Comparing `ogc_na-0.3.44/ogc/na/input_filters/csv.py` & `ogc_na-0.3.5/ogc/na/input_filters/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,46 +12,44 @@
     header row will be skipped.
 * `skip-rows` (default: `0`): number of rows to skip at the beginning of the file (apart from the header and pre-header
     ones if `rows` is `dict`).
 * `delimiter` (default: `,`): field separator character
 * `quotechar` (default: `"`): char used to quote (enclose) field values
 * `skip-empty-rows` (default: `True`): whether to omit empty rows (i.e., those with no values) from the result
 * `trim-values` (default: `False`): whether to apply `.strip()` to the resulting values
-* `charset` (default: `utf-8`): specific charset to use when opening the file
 """
 from __future__ import annotations
 
 import csv
-from io import StringIO
+from io import BytesIO, TextIOWrapper, StringIO
 from typing import IO, Any
 
 from ogc.na import util
 
 DEFAULT_CONF = {
     'rows': 'dict',
     'header-row': 0,
     'skip-rows': 0,
     'delimiter': ',',
     'quotechar': '"',
     'skip-empty-rows': True,
     'trim-values': False,
-    'charset': 'utf-8',
 }
 
 
 def apply_filter(content: bytes, conf: dict[str, Any] | None) -> tuple[dict[str, Any] | list, dict[str, Any] | None]:
     conf = util.deep_update(DEFAULT_CONF, conf) if conf else DEFAULT_CONF
 
     metadata = {
         'filter': {
             'conf': conf,
         },
     }
 
-    textio = StringIO(content.decode(conf['charset']))
+    textio = StringIO(content.decode('utf-8'))
     reader = csv.reader(textio, delimiter=conf['delimiter'], quotechar=conf['quotechar'])
 
     headers = None
     if conf['rows'] == 'dict':
         header_row = max(conf['header-row'], 0)
         # Skip to header row
         for i in range(header_row):
```

### Comparing `ogc_na-0.3.44/ogc/na/profile.py` & `ogc_na-0.3.5/ogc/na/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 from collections import deque
 from typing import Union, Sequence, Optional, Generator, Any, cast, Iterable
 from rdflib import Graph, RDF, PROF, OWL, URIRef, DCTERMS, Namespace, RDFS
 
 from ogc.na import util
 from pathlib import Path
 
-from ogc.na.validation import ProfileValidationReport, ProfilesValidationReport
-from ogc.na.models import ValidationReport
+from ogc.na.validation import ProfileValidationReport, ProfilesValidationReport, ValidationReport
 
 PROFROLE = Namespace('http://www.w3.org/ns/dx/prof/role/')
 
 ROLE_ENTAILMENT = PROFROLE.entailment
 ROLE_ENTAILMENT_CLOSURE = PROFROLE['entailment-closure']
 ROLE_VALIDATION = PROFROLE.validation
 ROLE_VALIDATION_CLOSURE = PROFROLE['validation-closure']
@@ -243,15 +242,15 @@
             self.profiles[profile_ref] = profile
             for same_as_ref in g.objects(profile_ref, OWL.sameAs):
                 self.profiles[cast(URIRef, same_as_ref)] = profile
 
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"Profiles loaded: %s", [str(p) for p in self.profiles])
         else:
-            logger.info(f"Loaded {len(self.profiles)} profiles")
+            logger.info(f"Loaded {len(self.profiles)}")
 
     def _apply_mappings(self, uri: str) -> Path | str:
         """
         Returns the longest match in self._local_artifact_mappings (prefixes)
         for a given URI, or the URI itself if not found
         """
```

### Comparing `ogc_na-0.3.44/ogc/na/provenance.py` & `ogc_na-0.3.5/ogc/na/provenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from rdflib.term import Node
 
 try:
     import git
 except ImportError:
     git = None
 from rdflib import Graph, URIRef, Literal, DCTERMS, RDF, RDFS, PROV, BNode
-from requests.utils import requote_uri
 
 from ogc.na import __version__, __url__
 
 
 @dataclass
 class FileProvenanceMetadata:
     filename: Union[str, Path] = None
@@ -58,20 +57,19 @@
                           base_uri: Optional[str] = None) -> URIRef:
     entity = None
     mime = None
     if metadata:
         mime = metadata.mime_type
 
         if metadata.uri:
-            metadata_uri = requote_uri(metadata.uri)
             if metadata.use_bnode:
                 entity = BNode()
-                g.add((entity, RDFS.seeAlso, URIRef(metadata_uri)))
+                g.add((entity, RDFS.seeAlso, URIRef(metadata.uri)))
             else:
-                entity = URIRef(metadata_uri)
+                entity = URIRef(metadata.uri)
         elif metadata.filename:
             filename = Path(metadata.filename).resolve()
             uri = None
 
             if not mime:
                 try:
                     mime = mimetypes.guess_type(filename)[0]
@@ -80,15 +78,15 @@
 
             if root_directory and base_uri:
                 root_directory = Path(root_directory).resolve()
                 if filename.is_relative_to(root_directory):
                     rel = filename.relative_to(root_directory)
                     uri = f"{base_uri}{'/' if '#' not in base_uri and not base_uri.endswith('/') else ''}{rel}"
 
-            uri = requote_uri(uri) if uri else filename.as_uri()
+            uri = uri if uri else filename.as_uri()
             if metadata.use_bnode:
                 entity = BNode()
                 g.add((entity, RDFS.seeAlso, URIRef(uri)))
             else:
                 entity = URIRef(uri)
 
             if git:
```

### Comparing `ogc_na-0.3.44/ogc/na/update_vocabs.py` & `ogc_na-0.3.5/ogc/na/update_vocabs.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     :param g: the [Graph][rdflib.Graph] for which to find the target URI
     :return: a [Node][rdflib.term.Node] generator
     """
     for s in g.subjects(predicate=RDF.type, object=SKOS.ConceptScheme):
         yield str(s)
 
 
-def get_entailed_base_path(f: Path, g: Graph, rootpattern: Union[str, None] = None,
+def get_entailed_base_path(f: Path, g: Graph, rootpattern: str = '/def/',
                            entailed_dir: str = DEFAULT_ENTAILED_DIR) -> tuple:
     """
     Tries to find the base output file path for an entailed version of a source Graph.
 
     :param f: the original path of the source file
     :param g: the [Graph][rdflib.Graph] loaded from the source file
     :param rootpattern: a root pattern to filter candidate URIs
@@ -160,15 +160,15 @@
     elif canonical_filename.startswith('/'):
         canonical_filename = canonical_filename[1:]
 
     return (f.parent / entailed_dir / Path(canonical_filename),
             canonical_filename, conceptscheme)
 
 
-def make_rdf(filename: Union[str, Path], g: Graph, rootpath: Union[str, None] = None,
+def make_rdf(filename: Union[str, Path], g: Graph, rootpath='/def/',
              entailment_directory: Union[str, Path] = DEFAULT_ENTAILED_DIR,
              provenance_metadata: ProvenanceMetadata = None,) -> Path:
     """
     Serializes entailed RDF graphs in several output formats for a given input
     graph.
 
     :param filename: the original source filename
@@ -178,17 +178,14 @@
     :param entailment_directory: name for the output subdirectory for entailed files
     :return: the output path for the Turtle version of the entailed files
     """
     if not isinstance(filename, Path):
         filename = Path(filename)
     filename = filename.resolve()
 
-    if isinstance(entailment_directory, Path):
-        entailment_directory = entailment_directory.resolve()
-
     loadable_ttl = None
     newbasepath, canonical_filename, conceptschemeuri = \
         get_entailed_base_path(filename, g, rootpath, entailment_directory)
     if newbasepath:
         newbasepath.parent.mkdir(parents=True, exist_ok=True)
     for entailed_format in ENTAILED_FORMATS:
         if newbasepath:
@@ -376,35 +373,34 @@
             add_list = args.added.split(",")
             logger.info("Added: %s", add_list)
 
         if args.removed:
             dellist = args.removed.split(',')
             logger.info("Removed: %s", dellist)
 
-    local_artifacts_mappings = {}
-    if args.local_artifact_mappings:
-        for mappingstr in args.local_artifact_mappings:
-            mapping = mappingstr.split('=', 1)
-            if len(mapping) < 2:
-                raise Exception(f"Invalid local artifact mapping: {mappingstr}")
-            local_artifacts_mappings[mapping[0]] = mapping[1]
-
     domain_cfg = DomainConfiguration(args.domain_cfg, working_directory=args.working_directory,
                                      profile_sources=args.profile_source,
-                                     ignore_artifact_errors=args.ignore_artifact_errors,
-                                     local_artifacts_mappings=local_artifacts_mappings)
+                                     ignore_artifact_errors=args.ignore_artifact_errors)
     cfg_entries = domain_cfg.entries
     if not len(cfg_entries):
         if args.domain:
             logger.warning('No configuration found in %s for domain %s, exiting',
                            args.domain_cfg, args.domain)
         else:
             logger.warning('No configuration found in %s exiting', args.domain_cfg)
         sys.exit(1)
 
+    artifact_mappings = dict(domain_cfg.local_artifacts_mapping)
+    if args.local_artifact_mappings:
+        for mappingstr in args.local_artifact_mappings:
+            mapping = mappingstr.split('=', 1)
+            if len(mapping < 2):
+                raise Exception(f"Invalid local artifact mapping: {mappingstr}")
+            artifact_mappings[mapping[0]] = mapping[1]
+
     profile_registry = domain_cfg.profile_registry
 
     modified: dict[Path, DomainConfigurationEntry]
     added: dict[Path, DomainConfigurationEntry]
     if args.batch:
         modified = cfg_entries.find_all()
         added = {}
@@ -452,21 +448,27 @@
                 for res in validation_result.used_resources or ():
                     add_artifact(res)
 
             docrelpath = Path(os.path.relpath(doc, args.working_directory))
             if output_path:
                 output_doc = output_path.resolve() / docrelpath
                 entailment_dir = output_doc.parent / args.entailment_directory
+                output_doc = entailment_dir / output_doc.name
             else:
-                entailment_dir = DEFAULT_ENTAILED_DIR
+                entailment_dir = Path(args.entailment_directory).resolve()
+                output_doc = entailment_dir / doc.name
+
+            os.makedirs(output_doc.parent, exist_ok=True)
+            os.makedirs(entailment_dir, exist_ok=True)
+
+            with open(output_doc.with_suffix('.txt'), 'w') as validation_file:
+                validation_file.write(validation_result.text)
 
             loadable_path = make_rdf(doc, newg, cfg.uri_root_filter,
                                      entailment_dir, provenance_metadata)
-            with open(loadable_path.with_suffix('.txt'), 'w') as validation_file:
-                validation_file.write(validation_result.text)
 
             if args.update:
                 loadables = {
                     loadable_path: loadable_path
                 }
                 for p, g in profile_registry.get_annotations(newg).items():
                     if p != loadable_path:
```

### Comparing `ogc_na-0.3.44/ogc/na/util.py` & `ogc_na-0.3.5/ogc/na/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,35 @@
 #!/usr/bin/env python3
 """
 General utilities module.
 """
 from __future__ import annotations
-
-import argparse
 import os.path
 import shlex
 from glob import glob, iglob
 from pathlib import Path
 from time import time
 from typing import Optional, Union, Any, Mapping, Hashable
 
 import requests
 import rfc3987
 
 from rdflib import Graph
 from pyshacl import validate as shacl_validate
 from urllib.parse import urlparse
 
-from ogc.na.models import ValidationReport
+from ogc.na.validation import ValidationReport
 
 import yaml
 
 try:
     from yaml import CLoader as YamlLoader, CSafeLoader as SafeYamlLoader, CDumper as YamlDumper
 except ImportError:
     from yaml import Loader as YamlLoader, SafeLoader as SafeYamlLoader, Dumper as YamlDumper
 
-JSON_LD_KEYWORDS = {
-    '@base',
-    '@container',
-    '@context',
-    '@direction',
-    '@graph',
-    '@id',
-    '@import',
-    '@included',
-    '@index',
-    '@json',
-    '@language',
-    '@list',
-    '@nest',
-    '@none',
-    '@prefix',
-    '@propagate',
-    '@protected',
-    '@reverse',
-    '@set',
-    '@type',
-    '@value',
-    '@version',
-    '@vocab'
-}
-
 
 class ContextMergeError(Exception):
     pass
 
 
 def copy_triples(src: Graph, dst: Optional[Graph] = None) -> Graph:
     """
@@ -120,30 +92,28 @@
     if entailed_extra:
         for triple in entailed_extra:
             g.remove(triple)
 
     return g
 
 
-def validate(g: Graph, shacl_graph: Graph, extra: Optional[Graph] = None,
-             **kwargs) -> ValidationReport:
+def validate(g: Graph, shacl_graph: Graph, extra: Optional[Graph] = None) -> ValidationReport:
     """
     Perform SHACL validation on a data [Graph][rdflib.Graph].
 
     :param g: input data Graph
     :param shacl_graph: SHACL graph for validation
     :param extra: Graph with additional ontological information for validation
     :return: the resulting [][ogc.na.validation.ValidationReport]
     """
     return ValidationReport(shacl_validate(data_graph=g,
                                            shacl_graph=shacl_graph,
                                            ont_graph=extra,
                                            inference='rdfs',
-                                           advanced=True,
-                                           **kwargs))
+                                           advanced=True))
 
 
 def is_url(url: str, http_only: bool = False) -> bool:
     """
     Checks whether a string is a valid URL.
 
     :param url: the input string
@@ -305,104 +275,43 @@
         'added': added,
         'modified': modified,
         'deleted': deleted,
         'renamed': renamed,
     }
 
 
-def merge_contexts(a: dict, b: dict, fix_nest=True) -> dict[str, Any]:
+def merge_contexts(a: dict, b: dict, from_schema=None, property_chain=None) -> dict[str, Any]:
     if not b:
         return a
     if not a:
         if isinstance(a, dict):
             a.update(b)
             return a
         return b
     for term in list(a.keys()):
         va = a[term]
+        if isinstance(va, str):
+            va = {'@id': va}
+            a[term] = va
         vb = b.get(term)
-        if term not in JSON_LD_KEYWORDS:
-            if isinstance(va, str):
-                va = {'@id': va}
-                a[term] = va
-            if isinstance(vb, str):
-                vb = {'@id': vb}
-            if vb:
-                for vb_term, vb_term_val in vb.items():
-                    if vb_term != '@context':
-                        va[vb_term] = vb_term_val
-                if '@context' in vb:
-                    if '@context' not in va:
-                        va['@context'] = vb['@context']
-                    elif isinstance(va['@context'], list):
-                        if isinstance(vb['@context'], list):
-                            va['@context'].extend(vb['@context'])
-                        else:
-                            va['@context'].append(vb['@context'])
-                    elif isinstance(vb['@context'], list):
-                        va['@context'] = [va['@context'], *vb['@context']]
+        if isinstance(vb, str):
+            vb = {'@id': vb}
+        if vb:
+            for vb_term, vb_term_val in vb.items():
+                if vb_term != '@context':
+                    va[vb_term] = vb_term_val
+            if '@context' in vb:
+                if '@context' not in va:
+                    va['@context'] = vb['@context']
+                elif isinstance(va['@context'], list):
+                    if isinstance(vb['@context'], list):
+                        va['@context'].extend(vb['@context'])
                     else:
-                        va['@context'] = merge_contexts(va['@context'], vb['@context'])
-        elif vb:
-            a[term] = vb
+                        va['@context'].append(vb['@context'])
+                elif isinstance(vb['@context'], list):
+                    va['@context'] = [va['@context'], *vb['@context']]
+                else:
+                    va['@context'] = merge_contexts(va['@context'], vb['@context'], from_schema, property_chain)
     for t, tb in b.items():
         if t not in a:
             a[t] = tb
-
-    if fix_nest:
-        # fix nested @context inside @nest terms
-        # spec is unclear, but our tooling of interest (json-ld playground, rdflib) do not support it
-        # see: https://github.com/json-ld/json-ld.org/issues/737
-        pending_merges = []
-        for term in list(a.keys()):
-            if isinstance(a[term], dict) and a[term].get('@id') == '@nest':
-                nested_ctx = a[term].pop('@context', None)
-                if nested_ctx:
-                    pending_merges.append(nested_ctx)
-                a[term] = '@nest'
-        for pm in pending_merges:
-            a = merge_contexts(a, pm)
-
     return a
-
-
-def dict_contains(greater: dict, smaller: dict):
-    for k, v in smaller.items():
-        if k not in greater:
-            return False
-        gv = greater[k]
-        if isinstance(v, dict):
-            if not isinstance(gv, dict) or not dict_contains(gv, v):
-                return False
-        elif gv != v:
-            return False
-    return True
-
-
-def cmd_join(args):
-    g = Graph()
-    for src in args.input:
-        g.parse(src)
-
-    if args.output:
-        g.serialize(args.output, format=args.format or 'ttl')
-    else:
-        print(g.serialize(format=args.format or 'ttl'))
-
-
-def _main():
-    parser = argparse.ArgumentParser()
-    subparsers = parser.add_subparsers(dest="command", required=True)
-
-    join_parser = subparsers.add_parser('join', help='Join RDF files')
-    join_parser.add_argument('input', nargs='+')
-    join_parser.add_argument('-o', '--output', help='Output file')
-    join_parser.add_argument('-f', '--format', help='Output format')
-
-    args = parser.parse_args()
-
-    if args.command == 'join':
-        cmd_join(args)
-
-
-if __name__ == '__main__':
-    _main()
```

### Comparing `ogc_na-0.3.44/ogc/na/validation.py` & `ogc_na-0.3.5/ogc/na/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 #!/usr/bin/env python3
 """
 This module defines auxiliary classes to represent [pySHACL](https://github.com/RDFLib/pySHACL)
 validation reports.
 """
 from __future__ import annotations
 from pathlib import Path
-from typing import Union
+from typing import Union, Iterable
 from urllib.parse import urlsplit
 from urllib.request import urlopen
 
 import jsonschema
 import requests
 from rdflib import URIRef, Graph
 
 from ogc.na import util
-from ogc.na.models import ValidationReport
+
+
+class ValidationReport:
+    """
+    Validation report from a single validation result.
+
+    Structures a pySHACL tuple report into `result`, `graph` and `text`
+    fields.
+    """
+
+    def __init__(self, pyshacl_result: tuple,
+                 used_resources: Iterable[Union[str, Path]] = None):
+        """
+        :param pyshacl_result: result from executing [pyshacl.validate]
+        """
+        self.result, self.graph, self.text = pyshacl_result
+        self.used_resources: set[Union[str, Path]] = set(used_resources) if used_resources else set()
 
 
 class ProfileValidationReport:
     """
     Validation report for a given [profile](https://www.w3.org/TR/dx-prof/).
     """
```

### Comparing `ogc_na-0.3.44/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.3.5/ogc_na.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 .gitignore
 MANIFEST.in
 README.md
 mkdocs.yml
 pyproject.toml
 requirements.txt
 setup.py
-.github/workflows/mkdocs.yml
 .github/workflows/python-publish.yml
 docs/examples.md
 docs/gen_ref_pages.py
 docs/index.md
-docs/jsonld-uplift.md
 docs/tutorials.md
 ogc/na/__init__.py
 ogc/na/_version.py
 ogc/na/annotate_schema.py
 ogc/na/domain_config.py
 ogc/na/download.py
 ogc/na/gsp.py
 ogc/na/ingest_json.py
-ogc/na/models.py
 ogc/na/profile.py
 ogc/na/provenance.py
 ogc/na/update_vocabs.py
 ogc/na/util.py
 ogc/na/validation.py
 ogc/na/input_filters/__init__.py
 ogc/na/input_filters/csv.py
-ogc/na/input_filters/xml.py
 ogc_na.egg-info/PKG-INFO
 ogc_na.egg-info/SOURCES.txt
 ogc_na.egg-info/dependency_links.txt
 ogc_na.egg-info/requires.txt
 ogc_na.egg-info/top_level.txt
 rdf/catalog-v001.xml
 rdf/domaincfg.vocab.ttl
```

### Comparing `ogc_na-0.3.44/pyproject.toml` & `ogc_na-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/rdf/domaincfg.vocab.ttl` & `ogc_na-0.3.5/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/test/data/headers.csv` & `ogc_na-0.3.5/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/test/data/uplift_context_valid.yml` & `ogc_na-0.3.5/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/test/test_annotate_schema.py` & `ogc_na-0.3.5/test/test_annotate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import unittest
 from pathlib import Path
 
+from rich import json
+
 from ogc.na import annotate_schema
 from ogc.na.annotate_schema import SchemaAnnotator
 
 THIS_DIR = Path(__file__).parent
 DATA_DIR = THIS_DIR / 'data'
```

### Comparing `ogc_na-0.3.44/test/test_ingest_json.py` & `ogc_na-0.3.5/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/test/test_input_filters_csv.py` & `ogc_na-0.3.5/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.44/test/test_profile.py` & `ogc_na-0.3.5/test/test_profile.py`

 * *Files identical despite different names*

