# Comparing `tmp/kitconcept.solr-1.0.0a5.tar.gz` & `tmp/kitconcept.solr-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitconcept.solr-1.0.0a5.tar", last modified: Fri Mar  1 11:58:58 2024, max compression
+gzip compressed data, was "kitconcept.solr-1.0.0a6.tar", last modified: Tue Apr  9 11:42:45 2024, max compression
```

## Comparing `kitconcept.solr-1.0.0a5.tar` & `kitconcept.solr-1.0.0a6.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.561617 kitconcept.solr-1.0.0a5/
--rw-r--r--   0 ree        (501) staff       (20)     1342 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/.editorconfig
--rw-r--r--   0 ree        (501) staff       (20)     2024 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/.pre-commit-config.yaml
--rw-r--r--   0 ree        (501) staff       (20)     1588 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/CHANGES.md
--rw-r--r--   0 ree        (501) staff       (20)       55 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/CONTRIBUTORS.md
--rw-r--r--   0 ree        (501) staff       (20)    18092 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/LICENSE.GPL
--rw-r--r--   0 ree        (501) staff       (20)      231 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/MANIFEST.in
--rw-r--r--   0 ree        (501) staff       (20)     5489 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/Makefile
--rw-r--r--   0 ree        (501) staff       (20)    13546 2024-03-01 11:58:58.561313 kitconcept.solr-1.0.0a5/PKG-INFO
--rw-r--r--   0 ree        (501) staff       (20)    10791 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/README.md
--rw-r--r--   0 ree        (501) staff       (20)       56 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/constraints-5.2.txt
--rw-r--r--   0 ree        (501) staff       (20)       78 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/constraints-6.0.txt
--rw-r--r--   0 ree        (501) staff       (20)       78 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/constraints.txt
--rw-r--r--   0 ree        (501) staff       (20)      164 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/docker-compose.yml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.547719 kitconcept.solr-1.0.0a5/docs/
--rw-r--r--   0 ree        (501) staff       (20)    28415 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/docs/dlr.svg
--rw-r--r--   0 ree        (501) staff       (20)     9029 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/docs/fz-juelich.svg
--rw-r--r--   0 ree        (501) staff       (20)      168 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/instance.yaml
--rw-r--r--   0 ree        (501) staff       (20)     4734 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/pyproject.toml
--rw-r--r--   0 ree        (501) staff       (20)       83 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/requirements-5.2.txt
--rw-r--r--   0 ree        (501) staff       (20)       32 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/requirements-6.0.txt
--rw-r--r--   0 ree        (501) staff       (20)       32 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/requirements.txt
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.547982 kitconcept.solr-1.0.0a5/scripts/
--rw-r--r--   0 ree        (501) staff       (20)      465 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/scripts/solr_activate_and_reindex.py
--rw-r--r--   0 ree        (501) staff       (20)       38 2024-03-01 11:58:58.561665 kitconcept.solr-1.0.0a5/setup.cfg
--rw-r--r--   0 ree        (501) staff       (20)     2357 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/setup.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.548112 kitconcept.solr-1.0.0a5/solr/
--rw-r--r--   0 ree        (501) staff       (20)      361 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/Dockerfile
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.548387 kitconcept.solr-1.0.0a5/solr/bin/
--rwxr-xr-x   0 ree        (501) staff       (20)      179 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/bin/solr-start
--rwxr-xr-x   0 ree        (501) staff       (20)      177 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/bin/solr-stop
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.548531 kitconcept.solr-1.0.0a5/solr/etc/
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.549417 kitconcept.solr-1.0.0a5/solr/etc/conf/
--rw-r--r--   0 ree        (501) staff       (20)    78514 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/conf/mapping-FoldToASCII.txt
--rw-r--r--   0 ree        (501) staff       (20)    18902 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/conf/schema.xml
--rw-r--r--   0 ree        (501) staff       (20)    10235 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/conf/solrconfig.xml
--rw-r--r--   0 ree        (501) staff       (20)        0 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/conf/stopwords.txt
--rw-r--r--   0 ree        (501) staff       (20)      149 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/conf/synonyms.txt
--rw-r--r--   0 ree        (501) staff       (20)       11 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/solr/etc/core.properties
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.540805 kitconcept.solr-1.0.0a5/src/
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.549557 kitconcept.solr-1.0.0a5/src/kitconcept/
--rw-r--r--   0 ree        (501) staff       (20)       56 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/__init__.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.552021 kitconcept.solr-1.0.0a5/src/kitconcept/solr/
--rw-r--r--   0 ree        (501) staff       (20)      208 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/__init__.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.552338 kitconcept.solr-1.0.0a5/src/kitconcept/solr/behaviors/
--rw-r--r--   0 ree        (501) staff       (20)        0 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/behaviors/__init__.py
--rw-r--r--   0 ree        (501) staff       (20)      127 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/behaviors/configure.zcml
--rw-r--r--   0 ree        (501) staff       (20)      468 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/configure.zcml
--rw-r--r--   0 ree        (501) staff       (20)      349 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/dependencies.zcml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.552638 kitconcept.solr-1.0.0a5/src/kitconcept/solr/indexers/
--rw-r--r--   0 ree        (501) staff       (20)      149 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/indexers/configure.zcml
--rw-r--r--   0 ree        (501) staff       (20)     5129 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/indexers/text.py
--rw-r--r--   0 ree        (501) staff       (20)     1915 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/interfaces.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.553005 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.541263 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.553286 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/LC_MESSAGES/
--rw-r--r--   0 ree        (501) staff       (20)      696 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/LC_MESSAGES/kitconcept.solr.po
--rw-r--r--   0 ree        (501) staff       (20)      646 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/LC_MESSAGES/plone.po
--rw-r--r--   0 ree        (501) staff       (20)      814 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/kitconcept.solr.pot
--rw-r--r--   0 ree        (501) staff       (20)     2488 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/update.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.541869 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.553563 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/
--rw-r--r--   0 ree        (501) staff       (20)      164 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/browserlayer.xml
--rw-r--r--   0 ree        (501) staff       (20)      184 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/metadata.xml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.553706 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/registry/
--rw-r--r--   0 ree        (501) staff       (20)     1037 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/registry/kitconcept.solr.interfaces.IKitconceptSolrSettings.xml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.553972 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/
--rw-r--r--   0 ree        (501) staff       (20)      312 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/metadata.xml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.554117 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/registry/
--rw-r--r--   0 ree        (501) staff       (20)      343 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/registry/plone.i18n.interfaces.ILanguageSchema.xml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.554255 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/types/
--rw-r--r--   0 ree        (501) staff       (20)        0 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/types/.gitkeep
--rw-r--r--   0 ree        (501) staff       (20)      107 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/testing/types.xml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.554366 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/uninstall/
--rw-r--r--   0 ree        (501) staff       (20)      118 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 ree        (501) staff       (20)     1220 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles.zcml
--rw-r--r--   0 ree        (501) staff       (20)     2033 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/reindex_helpers.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.555048 kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/
--rw-r--r--   0 ree        (501) staff       (20)        0 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/__init__.py
--rw-r--r--   0 ree        (501) staff       (20)      323 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/configure.zcml
--rw-r--r--   0 ree        (501) staff       (20)    11418 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/solr.py
--rw-r--r--   0 ree        (501) staff       (20)     7346 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/solr_utils.py
--rw-r--r--   0 ree        (501) staff       (20)      985 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/setuphandlers.py
--rw-r--r--   0 ree        (501) staff       (20)      930 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/testing.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.555355 kitconcept.solr-1.0.0a5/src/kitconcept/solr/upgrades/
--rw-r--r--   0 ree        (501) staff       (20)        0 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/upgrades/__init__.py
--rw-r--r--   0 ree        (501) staff       (20)      174 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/src/kitconcept/solr/upgrades/configure.zcml
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.550625 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/
--rw-r--r--   0 ree        (501) staff       (20)    13546 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/PKG-INFO
--rw-r--r--   0 ree        (501) staff       (20)     3791 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/SOURCES.txt
--rw-r--r--   0 ree        (501) staff       (20)        1 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/dependency_links.txt
--rw-r--r--   0 ree        (501) staff       (20)      120 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/entry_points.txt
--rw-r--r--   0 ree        (501) staff       (20)       11 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/namespace_packages.txt
--rw-r--r--   0 ree        (501) staff       (20)        1 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/not-zip-safe
--rw-r--r--   0 ree        (501) staff       (20)      219 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/requires.txt
--rw-r--r--   0 ree        (501) staff       (20)       11 2024-03-01 11:58:58.000000 kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/top_level.txt
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.555485 kitconcept.solr-1.0.0a5/tests/
--rw-r--r--   0 ree        (501) staff       (20)      357 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/conftest.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.555619 kitconcept.solr-1.0.0a5/tests/services/
--rw-r--r--   0 ree        (501) staff       (20)     6808 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/conftest.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.556071 kitconcept.solr-1.0.0a5/tests/services/content_filters/
--rw-r--r--   0 ree        (501) staff       (20)     1090 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/content_filters/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     2044 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/content_filters/test_endpoint_contentfields.py
--rw-r--r--   0 ree        (501) staff       (20)     2542 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/content_filters/test_endpoint_portaltype.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.556209 kitconcept.solr-1.0.0a5/tests/services/custom_config/
--rw-r--r--   0 ree        (501) staff       (20)     2595 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/custom_config/test_endpoint_custom.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.556394 kitconcept.solr-1.0.0a5/tests/services/default_config/
--rw-r--r--   0 ree        (501) staff       (20)     5115 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/default_config/test_endpoint_default.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.557016 kitconcept.solr-1.0.0a5/tests/services/encoding/
--rw-r--r--   0 ree        (501) staff       (20)     1714 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/encoding/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     2612 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/encoding/test_endpoint_encoding.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.557328 kitconcept.solr-1.0.0a5/tests/services/facet_conditions/
--rw-r--r--   0 ree        (501) staff       (20)     2259 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/facet_conditions/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)    11917 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/facet_conditions/test_facet_conditions.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.557914 kitconcept.solr-1.0.0a5/tests/services/language/
--rw-r--r--   0 ree        (501) staff       (20)     1853 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/language/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     1969 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/language/test_endpoint_language.py
--rw-r--r--   0 ree        (501) staff       (20)     2379 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/language/test_endpoint_local_multilingual.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.558068 kitconcept.solr-1.0.0a5/tests/services/local_search/
--rw-r--r--   0 ree        (501) staff       (20)     5365 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/local_search/test_endpoint_local.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.558453 kitconcept.solr-1.0.0a5/tests/services/permission/
--rw-r--r--   0 ree        (501) staff       (20)     3029 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/permission/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     5605 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/permission/test_endpoint_permissions.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.558861 kitconcept.solr-1.0.0a5/tests/services/prevent_injection/
--rw-r--r--   0 ree        (501) staff       (20)     1229 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/prevent_injection/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     5123 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/prevent_injection/test_prevent_injection.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.559080 kitconcept.solr-1.0.0a5/tests/services/response/
--rw-r--r--   0 ree        (501) staff       (20)     1855 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/response/test_response.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.559419 kitconcept.solr-1.0.0a5/tests/services/roles_and_users/
--rw-r--r--   0 ree        (501) staff       (20)     1607 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/roles_and_users/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     1737 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/services/roles_and_users/test_roles_and_users.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.559726 kitconcept.solr-1.0.0a5/tests/setup/
--rw-r--r--   0 ree        (501) staff       (20)     2207 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/setup/test_setup_install.py
--rw-r--r--   0 ree        (501) staff       (20)      631 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-03-01 11:58:58.561100 kitconcept.solr-1.0.0a5/tests/utils/
--rw-r--r--   0 ree        (501) staff       (20)     2462 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/conftest.py
--rw-r--r--   0 ree        (501) staff       (20)     3051 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils.py
--rw-r--r--   0 ree        (501) staff       (20)     1371 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_emptylabels.py
--rw-r--r--   0 ree        (501) staff       (20)      958 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_emptysearchtabs.py
--rw-r--r--   0 ree        (501) staff       (20)     1798 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_escape.py
--rw-r--r--   0 ree        (501) staff       (20)    13863 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_facet_conditions.py
--rw-r--r--   0 ree        (501) staff       (20)     1405 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_fieldlwithcomma.py
--rw-r--r--   0 ree        (501) staff       (20)     1352 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_missinglabels.py
--rw-r--r--   0 ree        (501) staff       (20)      723 2024-03-01 11:58:57.000000 kitconcept.solr-1.0.0a5/tests/utils/test_utils_replace_reserved.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.487729 kitconcept.solr-1.0.0a6/
+-rw-r--r--   0 ree        (501) staff       (20)     1342 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/.editorconfig
+-rw-r--r--   0 ree        (501) staff       (20)     2024 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/.pre-commit-config.yaml
+-rw-r--r--   0 ree        (501) staff       (20)     1732 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/CHANGES.md
+-rw-r--r--   0 ree        (501) staff       (20)       55 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/CONTRIBUTORS.md
+-rw-r--r--   0 ree        (501) staff       (20)    18092 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/LICENSE.GPL
+-rw-r--r--   0 ree        (501) staff       (20)      231 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/MANIFEST.in
+-rw-r--r--   0 ree        (501) staff       (20)     5489 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/Makefile
+-rw-r--r--   0 ree        (501) staff       (20)    13690 2024-04-09 11:42:45.487537 kitconcept.solr-1.0.0a6/PKG-INFO
+-rw-r--r--   0 ree        (501) staff       (20)    10791 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/README.md
+-rw-r--r--   0 ree        (501) staff       (20)       56 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/constraints-5.2.txt
+-rw-r--r--   0 ree        (501) staff       (20)       78 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/constraints-6.0.txt
+-rw-r--r--   0 ree        (501) staff       (20)       78 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/constraints.txt
+-rw-r--r--   0 ree        (501) staff       (20)      164 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/docker-compose.yml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.475648 kitconcept.solr-1.0.0a6/docs/
+-rw-r--r--   0 ree        (501) staff       (20)    28415 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/docs/dlr.svg
+-rw-r--r--   0 ree        (501) staff       (20)     9029 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/docs/fz-juelich.svg
+-rw-r--r--   0 ree        (501) staff       (20)      168 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/instance.yaml
+-rw-r--r--   0 ree        (501) staff       (20)     4734 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/pyproject.toml
+-rw-r--r--   0 ree        (501) staff       (20)       83 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/requirements-5.2.txt
+-rw-r--r--   0 ree        (501) staff       (20)       32 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/requirements-6.0.txt
+-rw-r--r--   0 ree        (501) staff       (20)       32 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/requirements.txt
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.475805 kitconcept.solr-1.0.0a6/scripts/
+-rw-r--r--   0 ree        (501) staff       (20)      465 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/scripts/solr_activate_and_reindex.py
+-rw-r--r--   0 ree        (501) staff       (20)       38 2024-04-09 11:42:45.487783 kitconcept.solr-1.0.0a6/setup.cfg
+-rw-r--r--   0 ree        (501) staff       (20)     2357 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/setup.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.475932 kitconcept.solr-1.0.0a6/solr/
+-rw-r--r--   0 ree        (501) staff       (20)      361 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/Dockerfile
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.476196 kitconcept.solr-1.0.0a6/solr/bin/
+-rwxr-xr-x   0 ree        (501) staff       (20)      179 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/bin/solr-start
+-rwxr-xr-x   0 ree        (501) staff       (20)      177 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/bin/solr-stop
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.476322 kitconcept.solr-1.0.0a6/solr/etc/
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.477065 kitconcept.solr-1.0.0a6/solr/etc/conf/
+-rw-r--r--   0 ree        (501) staff       (20)    78514 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/conf/mapping-FoldToASCII.txt
+-rw-r--r--   0 ree        (501) staff       (20)    18902 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/conf/schema.xml
+-rw-r--r--   0 ree        (501) staff       (20)    10235 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/conf/solrconfig.xml
+-rw-r--r--   0 ree        (501) staff       (20)        0 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/conf/stopwords.txt
+-rw-r--r--   0 ree        (501) staff       (20)      149 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/conf/synonyms.txt
+-rw-r--r--   0 ree        (501) staff       (20)       11 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/solr/etc/core.properties
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.470135 kitconcept.solr-1.0.0a6/src/
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.477203 kitconcept.solr-1.0.0a6/src/kitconcept/
+-rw-r--r--   0 ree        (501) staff       (20)       56 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/__init__.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.479315 kitconcept.solr-1.0.0a6/src/kitconcept/solr/
+-rw-r--r--   0 ree        (501) staff       (20)      208 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/__init__.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.479573 kitconcept.solr-1.0.0a6/src/kitconcept/solr/behaviors/
+-rw-r--r--   0 ree        (501) staff       (20)        0 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/behaviors/__init__.py
+-rw-r--r--   0 ree        (501) staff       (20)      127 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/behaviors/configure.zcml
+-rw-r--r--   0 ree        (501) staff       (20)      468 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/configure.zcml
+-rw-r--r--   0 ree        (501) staff       (20)      349 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/dependencies.zcml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.479839 kitconcept.solr-1.0.0a6/src/kitconcept/solr/indexers/
+-rw-r--r--   0 ree        (501) staff       (20)      149 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/indexers/configure.zcml
+-rw-r--r--   0 ree        (501) staff       (20)     5129 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/indexers/text.py
+-rw-r--r--   0 ree        (501) staff       (20)     1915 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/interfaces.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.480146 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.470652 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.480424 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/LC_MESSAGES/
+-rw-r--r--   0 ree        (501) staff       (20)      696 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/LC_MESSAGES/kitconcept.solr.po
+-rw-r--r--   0 ree        (501) staff       (20)      646 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--   0 ree        (501) staff       (20)      814 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/kitconcept.solr.pot
+-rw-r--r--   0 ree        (501) staff       (20)     2488 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/update.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.471244 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.480712 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/
+-rw-r--r--   0 ree        (501) staff       (20)      164 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/browserlayer.xml
+-rw-r--r--   0 ree        (501) staff       (20)      184 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/metadata.xml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.480846 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/registry/
+-rw-r--r--   0 ree        (501) staff       (20)     1037 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/registry/kitconcept.solr.interfaces.IKitconceptSolrSettings.xml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.481116 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/
+-rw-r--r--   0 ree        (501) staff       (20)      312 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/metadata.xml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.481248 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/registry/
+-rw-r--r--   0 ree        (501) staff       (20)      343 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/registry/plone.i18n.interfaces.ILanguageSchema.xml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.481385 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/types/
+-rw-r--r--   0 ree        (501) staff       (20)        0 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/types/.gitkeep
+-rw-r--r--   0 ree        (501) staff       (20)      107 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/testing/types.xml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.481488 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/uninstall/
+-rw-r--r--   0 ree        (501) staff       (20)      118 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 ree        (501) staff       (20)     1220 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles.zcml
+-rw-r--r--   0 ree        (501) staff       (20)     2033 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/reindex_helpers.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.482003 kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/
+-rw-r--r--   0 ree        (501) staff       (20)        0 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/__init__.py
+-rw-r--r--   0 ree        (501) staff       (20)      323 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/configure.zcml
+-rw-r--r--   0 ree        (501) staff       (20)    11568 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/solr.py
+-rw-r--r--   0 ree        (501) staff       (20)     7346 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/solr_utils.py
+-rw-r--r--   0 ree        (501) staff       (20)      985 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/setuphandlers.py
+-rw-r--r--   0 ree        (501) staff       (20)      930 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/testing.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.482263 kitconcept.solr-1.0.0a6/src/kitconcept/solr/upgrades/
+-rw-r--r--   0 ree        (501) staff       (20)        0 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/upgrades/__init__.py
+-rw-r--r--   0 ree        (501) staff       (20)      174 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/src/kitconcept/solr/upgrades/configure.zcml
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.478245 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/
+-rw-r--r--   0 ree        (501) staff       (20)    13690 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/PKG-INFO
+-rw-r--r--   0 ree        (501) staff       (20)     3847 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/SOURCES.txt
+-rw-r--r--   0 ree        (501) staff       (20)        1 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/dependency_links.txt
+-rw-r--r--   0 ree        (501) staff       (20)      120 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/entry_points.txt
+-rw-r--r--   0 ree        (501) staff       (20)       11 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/namespace_packages.txt
+-rw-r--r--   0 ree        (501) staff       (20)        1 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/not-zip-safe
+-rw-r--r--   0 ree        (501) staff       (20)      219 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/requires.txt
+-rw-r--r--   0 ree        (501) staff       (20)       11 2024-04-09 11:42:45.000000 kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/top_level.txt
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.482397 kitconcept.solr-1.0.0a6/tests/
+-rw-r--r--   0 ree        (501) staff       (20)      357 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/conftest.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.482534 kitconcept.solr-1.0.0a6/tests/services/
+-rw-r--r--   0 ree        (501) staff       (20)     6808 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/conftest.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.482999 kitconcept.solr-1.0.0a6/tests/services/content_filters/
+-rw-r--r--   0 ree        (501) staff       (20)     1090 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/content_filters/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     2044 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/content_filters/test_endpoint_contentfields.py
+-rw-r--r--   0 ree        (501) staff       (20)     2542 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/content_filters/test_endpoint_portaltype.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.483297 kitconcept.solr-1.0.0a6/tests/services/custom_config/
+-rw-r--r--   0 ree        (501) staff       (20)     2595 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/custom_config/test_endpoint_custom.py
+-rw-r--r--   0 ree        (501) staff       (20)     2112 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/custom_config/test_endpoint_first_tab.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.483442 kitconcept.solr-1.0.0a6/tests/services/default_config/
+-rw-r--r--   0 ree        (501) staff       (20)     5115 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/default_config/test_endpoint_default.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.483728 kitconcept.solr-1.0.0a6/tests/services/encoding/
+-rw-r--r--   0 ree        (501) staff       (20)     1714 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/encoding/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     2612 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/encoding/test_endpoint_encoding.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.483999 kitconcept.solr-1.0.0a6/tests/services/facet_conditions/
+-rw-r--r--   0 ree        (501) staff       (20)     2259 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/facet_conditions/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)    11917 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/facet_conditions/test_facet_conditions.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.484430 kitconcept.solr-1.0.0a6/tests/services/language/
+-rw-r--r--   0 ree        (501) staff       (20)     1853 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/language/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     1969 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/language/test_endpoint_language.py
+-rw-r--r--   0 ree        (501) staff       (20)     2379 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/language/test_endpoint_local_multilingual.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.484664 kitconcept.solr-1.0.0a6/tests/services/local_search/
+-rw-r--r--   0 ree        (501) staff       (20)     5365 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/local_search/test_endpoint_local.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.485045 kitconcept.solr-1.0.0a6/tests/services/permission/
+-rw-r--r--   0 ree        (501) staff       (20)     3029 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/permission/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     5605 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/permission/test_endpoint_permissions.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.485351 kitconcept.solr-1.0.0a6/tests/services/prevent_injection/
+-rw-r--r--   0 ree        (501) staff       (20)     1229 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/prevent_injection/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     5123 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/prevent_injection/test_prevent_injection.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.485513 kitconcept.solr-1.0.0a6/tests/services/response/
+-rw-r--r--   0 ree        (501) staff       (20)     1855 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/response/test_response.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.485790 kitconcept.solr-1.0.0a6/tests/services/roles_and_users/
+-rw-r--r--   0 ree        (501) staff       (20)     1607 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/roles_and_users/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     1737 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/services/roles_and_users/test_roles_and_users.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.486085 kitconcept.solr-1.0.0a6/tests/setup/
+-rw-r--r--   0 ree        (501) staff       (20)     2207 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/setup/test_setup_install.py
+-rw-r--r--   0 ree        (501) staff       (20)      631 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 ree        (501) staff       (20)        0 2024-04-09 11:42:45.487332 kitconcept.solr-1.0.0a6/tests/utils/
+-rw-r--r--   0 ree        (501) staff       (20)     2462 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/conftest.py
+-rw-r--r--   0 ree        (501) staff       (20)     3051 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils.py
+-rw-r--r--   0 ree        (501) staff       (20)     1371 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_emptylabels.py
+-rw-r--r--   0 ree        (501) staff       (20)      958 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_emptysearchtabs.py
+-rw-r--r--   0 ree        (501) staff       (20)     1798 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_escape.py
+-rw-r--r--   0 ree        (501) staff       (20)    13863 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_facet_conditions.py
+-rw-r--r--   0 ree        (501) staff       (20)     1405 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_fieldlwithcomma.py
+-rw-r--r--   0 ree        (501) staff       (20)     1352 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_missinglabels.py
+-rw-r--r--   0 ree        (501) staff       (20)      723 2024-04-09 11:42:44.000000 kitconcept.solr-1.0.0a6/tests/utils/test_utils_replace_reserved.py
```

### Comparing `kitconcept.solr-1.0.0a5/.editorconfig` & `kitconcept.solr-1.0.0a6/.editorconfig`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/.pre-commit-config.yaml` & `kitconcept.solr-1.0.0a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/CHANGES.md` & `kitconcept.solr-1.0.0a6/CHANGES.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2024-04-09)
+
+
+### Bug fixes:
+
+- Fix first tab condition @reebalazs [#26](https://github.com/kitconcept/kitconcept.solr/issues/26)
+
+
 ## 1.0.0a5 (2024-03-01)
 
 
 ### New features:
 
 - Add support for sidebar facet conditions @reebalazs [#24](https://github.com/kitconcept/kitconcept.solr/issues/24)
```

### Comparing `kitconcept.solr-1.0.0a5/LICENSE.GPL` & `kitconcept.solr-1.0.0a6/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/Makefile` & `kitconcept.solr-1.0.0a6/Makefile`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/PKG-INFO` & `kitconcept.solr-1.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitconcept.solr
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: An opinionated Solr integration for Plone
 Home-page: https://github.com/kitconcept/kitconcept.solr
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/kitconcept.solr
 Project-URL: Source, https://github.com/kitconcept/kitconcept.solr
@@ -349,14 +349,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2024-04-09)
+
+
+### Bug fixes:
+
+- Fix first tab condition @reebalazs [#26](https://github.com/kitconcept/kitconcept.solr/issues/26)
+
+
 ## 1.0.0a5 (2024-03-01)
 
 
 ### New features:
 
 - Add support for sidebar facet conditions @reebalazs [#24](https://github.com/kitconcept/kitconcept.solr/issues/24)
```

### Comparing `kitconcept.solr-1.0.0a5/README.md` & `kitconcept.solr-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/docs/dlr.svg` & `kitconcept.solr-1.0.0a6/docs/dlr.svg`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/docs/fz-juelich.svg` & `kitconcept.solr-1.0.0a6/docs/fz-juelich.svg`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/pyproject.toml` & `kitconcept.solr-1.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/setup.py` & `kitconcept.solr-1.0.0a6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="kitconcept.solr",
-    version="1.0.0a5",
+    version="1.0.0a6",
     description="An opinionated Solr integration for Plone",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `kitconcept.solr-1.0.0a5/solr/etc/conf/mapping-FoldToASCII.txt` & `kitconcept.solr-1.0.0a6/solr/etc/conf/mapping-FoldToASCII.txt`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/solr/etc/conf/schema.xml` & `kitconcept.solr-1.0.0a6/solr/etc/conf/schema.xml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/solr/etc/conf/solrconfig.xml` & `kitconcept.solr-1.0.0a6/solr/etc/conf/solrconfig.xml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/indexers/text.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/indexers/text.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/interfaces.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/interfaces.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/LC_MESSAGES/kitconcept.solr.po` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/LC_MESSAGES/kitconcept.solr.po`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/de/LC_MESSAGES/plone.po` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/kitconcept.solr.pot` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/kitconcept.solr.pot`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/locales/update.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/locales/update.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles/default/registry/kitconcept.solr.interfaces.IKitconceptSolrSettings.xml` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles/default/registry/kitconcept.solr.interfaces.IKitconceptSolrSettings.xml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/profiles.zcml` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/profiles.zcml`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/reindex_helpers.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/reindex_helpers.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/solr.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/solr.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,17 @@
         if group_select is not None:
             try:
                 group_select = int(group_select)
             except ValueError:
                 raise BadRequest(
                     "Property 'group_select` must be an integer, if specified"
                 )
+        elif len(solr_config.filters) > 0:
+            # By default select group 0 (unless there are no filters defined)
+            group_select = 0
 
         facet_fields = (
             solr_config.select_facet_fields(group_select)
             if group_select is not None
             else []
         )
```

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/services/solr_utils.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/services/solr_utils.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/setuphandlers.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept/solr/testing.py` & `kitconcept.solr-1.0.0a6/src/kitconcept/solr/testing.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/PKG-INFO` & `kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitconcept.solr
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: An opinionated Solr integration for Plone
 Home-page: https://github.com/kitconcept/kitconcept.solr
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/kitconcept.solr
 Project-URL: Source, https://github.com/kitconcept/kitconcept.solr
@@ -349,14 +349,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2024-04-09)
+
+
+### Bug fixes:
+
+- Fix first tab condition @reebalazs [#26](https://github.com/kitconcept/kitconcept.solr/issues/26)
+
+
 ## 1.0.0a5 (2024-03-01)
 
 
 ### New features:
 
 - Add support for sidebar facet conditions @reebalazs [#24](https://github.com/kitconcept/kitconcept.solr/issues/24)
```

### Comparing `kitconcept.solr-1.0.0a5/src/kitconcept.solr.egg-info/SOURCES.txt` & `kitconcept.solr-1.0.0a6/src/kitconcept.solr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 src/kitconcept/solr/upgrades/configure.zcml
 tests/conftest.py
 tests/services/conftest.py
 tests/services/content_filters/conftest.py
 tests/services/content_filters/test_endpoint_contentfields.py
 tests/services/content_filters/test_endpoint_portaltype.py
 tests/services/custom_config/test_endpoint_custom.py
+tests/services/custom_config/test_endpoint_first_tab.py
 tests/services/default_config/test_endpoint_default.py
 tests/services/encoding/conftest.py
 tests/services/encoding/test_endpoint_encoding.py
 tests/services/facet_conditions/conftest.py
 tests/services/facet_conditions/test_facet_conditions.py
 tests/services/language/conftest.py
 tests/services/language/test_endpoint_language.py
```

### Comparing `kitconcept.solr-1.0.0a5/tests/services/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/content_filters/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/content_filters/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/content_filters/test_endpoint_contentfields.py` & `kitconcept.solr-1.0.0a6/tests/services/content_filters/test_endpoint_contentfields.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/content_filters/test_endpoint_portaltype.py` & `kitconcept.solr-1.0.0a6/tests/services/content_filters/test_endpoint_portaltype.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/custom_config/test_endpoint_custom.py` & `kitconcept.solr-1.0.0a6/tests/services/custom_config/test_endpoint_custom.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/default_config/test_endpoint_default.py` & `kitconcept.solr-1.0.0a6/tests/services/default_config/test_endpoint_default.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/encoding/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/encoding/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/encoding/test_endpoint_encoding.py` & `kitconcept.solr-1.0.0a6/tests/services/encoding/test_endpoint_encoding.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/facet_conditions/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/facet_conditions/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/facet_conditions/test_facet_conditions.py` & `kitconcept.solr-1.0.0a6/tests/services/facet_conditions/test_facet_conditions.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/language/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/language/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/language/test_endpoint_language.py` & `kitconcept.solr-1.0.0a6/tests/services/language/test_endpoint_language.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/language/test_endpoint_local_multilingual.py` & `kitconcept.solr-1.0.0a6/tests/services/language/test_endpoint_local_multilingual.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/local_search/test_endpoint_local.py` & `kitconcept.solr-1.0.0a6/tests/services/local_search/test_endpoint_local.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/permission/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/permission/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/permission/test_endpoint_permissions.py` & `kitconcept.solr-1.0.0a6/tests/services/permission/test_endpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/prevent_injection/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/prevent_injection/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/prevent_injection/test_prevent_injection.py` & `kitconcept.solr-1.0.0a6/tests/services/prevent_injection/test_prevent_injection.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/response/test_response.py` & `kitconcept.solr-1.0.0a6/tests/services/response/test_response.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/roles_and_users/conftest.py` & `kitconcept.solr-1.0.0a6/tests/services/roles_and_users/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/services/roles_and_users/test_roles_and_users.py` & `kitconcept.solr-1.0.0a6/tests/services/roles_and_users/test_roles_and_users.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/setup/test_setup_install.py` & `kitconcept.solr-1.0.0a6/tests/setup/test_setup_install.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/setup/test_setup_uninstall.py` & `kitconcept.solr-1.0.0a6/tests/setup/test_setup_uninstall.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/conftest.py` & `kitconcept.solr-1.0.0a6/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_emptylabels.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_emptylabels.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_emptysearchtabs.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_emptysearchtabs.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_escape.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_escape.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_facet_conditions.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_facet_conditions.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_fieldlwithcomma.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_fieldlwithcomma.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_missinglabels.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_missinglabels.py`

 * *Files identical despite different names*

### Comparing `kitconcept.solr-1.0.0a5/tests/utils/test_utils_replace_reserved.py` & `kitconcept.solr-1.0.0a6/tests/utils/test_utils_replace_reserved.py`

 * *Files identical despite different names*

