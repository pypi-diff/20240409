# Comparing `tmp/ibridges-0.1.2.tar.gz` & `tmp/ibridges-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibridges-0.1.2.tar", last modified: Tue Mar  5 10:08:11 2024, max compression
+gzip compressed data, was "ibridges-0.1.3.tar", last modified: Tue Apr  9 11:50:44 2024, max compression
```

## Comparing `ibridges-0.1.2.tar` & `ibridges-0.1.3.tar`

### file list

```diff
@@ -1,115 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.232985 ibridges-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 10:08:02.000000 ibridges-0.1.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.208985 ibridges-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.212985 ibridges-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/workflows/integration-tests-irods.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/workflows/integration-tests-yoda.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-05 10:08:02.000000 ibridges-0.1.2/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-05 10:08:02.000000 ibridges-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-05 10:08:02.000000 ibridges-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-05 10:08:02.000000 ibridges-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-03-05 10:08:11.232985 ibridges-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-05 10:08:02.000000 ibridges-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_catalog/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_catalog/init-user-db.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_catalog_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_catalog_provider/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_catalog_provider/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_catalog_provider/setup-4.3.1.input
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.212985 ibridges-0.1.2/docker/irods_client/environments/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_client/environments/plain-irods/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/environments/plain-irods/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/environments/plain-irods/irods_environment.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_client/environments/yoda/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/environments/yoda/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/environments/yoda/irods_environment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_client/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/beach.rtf
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/bunny.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/example.r
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.216986 ibridges-0.1.2/docker/irods_client/testdata/more_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/more_data/polarbear.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/plant.rtf
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/testdata/sun.rtf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.220986 ibridges-0.1.2/docker/irods_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_data_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker/irods_client/tests/test_ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-05 10:08:02.000000 ibridges-0.1.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.220986 ibridges-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.220986 ibridges-0.1.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-05 10:08:02.000000 ibridges-0.1.2/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/ibridges/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/data_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-05 10:08:02.000000 ibridges-0.1.2/ibridges/tickets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.228985 ibridges-0.1.2/ibridges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 10:08:11.000000 ibridges-0.1.2/ibridges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-05 10:08:02.000000 ibridges-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 10:08:11.232985 ibridges-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-03-05 10:08:02.000000 ibridges-0.1.2/tests/test_irodspath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-03-05 10:08:02.000000 ibridges-0.1.2/tests/testdata/bunny.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/tests/testdata/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-05 10:08:02.000000 ibridges-0.1.2/tests/testdata/subfolder/sun.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/01-Setup-and-connect.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/02-Working-with-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/03-iRODS-Paths.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/04-Metadata.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/05-Data-Sharing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/Data_sync.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/QuickStart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.224985 ibridges-0.1.2/tutorials/example_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/example_rules/example.r
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/iRODS_paths.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:08:11.228985 ibridges-0.1.2/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject1.png
--rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject2.png
--rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject3.png
--rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject4.png
--rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject5.png
--rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/DataObject6.png
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/Save_json.png
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-03-05 10:08:02.000000 ibridges-0.1.2/tutorials/img/Yoda_environment.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.077844 ibridges-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:50:39.000000 ibridges-0.1.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.053844 ibridges-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/integration-tests-irods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/integration-tests-yoda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 11:50:39.000000 ibridges-0.1.3/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 11:50:39.000000 ibridges-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 11:50:39.000000 ibridges-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 11:50:39.000000 ibridges-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-09 11:50:44.077844 ibridges-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-09 11:50:39.000000 ibridges-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.057844 ibridges-0.1.3/docker/irods_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog/init-user-db.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_catalog_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_catalog_provider/setup-4.3.1.input
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.053844 ibridges-0.1.3/docker/irods_client/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/environments/plain-irods/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/irods_environment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/plain-irods/irods_environment_testuser.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/environments/yoda/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/yoda/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/environments/yoda/irods_environment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/beach.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/bunny.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/example.r
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.061844 ibridges-0.1.3/docker/irods_client/testdata/more_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/more_data/polarbear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/plant.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/testdata/sun.rtf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docker/irods_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_data_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker/irods_client/tests/test_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 11:50:39.000000 ibridges-0.1.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.065844 ibridges-0.1.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-09 11:50:39.000000 ibridges-0.1.3/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/ibridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 11:50:43.000000 ibridges-0.1.3/ibridges/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/data_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/export_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/icat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13582 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-09 11:50:39.000000 ibridges-0.1.3/ibridges/tickets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.073844 ibridges-0.1.3/ibridges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 11:50:44.000000 ibridges-0.1.3/ibridges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 11:50:39.000000 ibridges-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:50:44.077844 ibridges-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/test_irodspath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/testdata/bunny.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tests/testdata/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 11:50:39.000000 ibridges-0.1.3/tests/testdata/subfolder/sun.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/01-Setup-and-connect.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12711 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/02-Working-with-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/03-iRODS-Paths.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/04-Metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/05-Data-Sharing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/Data_sync.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24498 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/QuickStart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.069844 ibridges-0.1.3/tutorials/example_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/example_rules/example.r
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/iRODS_paths.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:50:44.073844 ibridges-0.1.3/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   227136 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   246217 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   277830 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   297047 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   291147 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject5.png
+-rw-r--r--   0 runner    (1001) docker     (127)   303681 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/DataObject6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/Save_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-09 11:50:39.000000 ibridges-0.1.3/tutorials/img/Yoda_environment.png
```

### Comparing `ibridges-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `ibridges-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `ibridges-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/.github/workflows/integration-tests-yoda.yml` & `ibridges-0.1.3/.github/workflows/integration-tests-yoda.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/.github/workflows/main.yml` & `ibridges-0.1.3/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         include:
           - os: windows-latest
             python-version: "3.11"
           - os: macos-latest
             python-version: "3.11"
     runs-on: ${{ matrix.os }}
 
@@ -35,18 +35,14 @@
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[test]
 
-    - name: Lint with PyLint
-      run: |
-        pylint ibridges
-
     - name: Check types with MyPy
       run: |
         mypy ibridges
 
     - name: Check if documentation builds.
       run: |
         cd docs; make html SPHINXOPTS="--keep-going"
```

### Comparing `ibridges-0.1.2/.github/workflows/pypi_release.yml` & `ibridges-0.1.3/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/.gitignore` & `ibridges-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/.readthedocs.yaml` & `ibridges-0.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/LICENSE` & `ibridges-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/PKG-INFO` & `ibridges-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6962 7269  : 2.1.Name: ibri
 00000020: 6467 6573 0a56 6572 7369 6f6e 3a20 302e  dges.Version: 0.
-00000030: 312e 320a 5375 6d6d 6172 793a 2050 6163  1.2.Summary: Pac
+00000030: 312e 330a 5375 6d6d 6172 793a 2050 6163  1.3.Summary: Pac
 00000040: 6b61 6765 2066 6f72 2061 6363 6573 7369  kage for accessi
 00000050: 6e67 2064 6174 6120 616e 6420 6d65 7461  ng data and meta
 00000060: 6461 7461 206f 6e20 6952 6f64 7320 7365  data on iRods se
 00000070: 7276 6572 732e 0a41 7574 686f 722d 656d  rvers..Author-em
 00000080: 6169 6c3a 2043 6872 6973 7469 6e65 2053  ail: Christine S
 00000090: 7461 6967 6572 203c 632e 7374 6169 6765  taiger <c.staige
 000000a0: 7240 7575 2e6e 6c3e 0a4c 6963 656e 7365  r@uu.nl>.License
@@ -160,234 +160,287 @@
 000009f0: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
 00000a00: 7068 696e 785f 696e 6c69 6e65 5f74 6162  phinx_inline_tab
 00000a10: 733b 2065 7874 7261 203d 3d20 2274 6573  s; extra == "tes
 00000a20: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
 00000a30: 3a20 7370 6869 6e78 5f63 6f70 7962 7574  : sphinx_copybut
 00000a40: 746f 6e3b 2065 7874 7261 203d 3d20 2274  ton; extra == "t
 00000a50: 6573 7422 0a0a 2320 6942 7269 6467 6573  est"..# iBridges
-00000a60: 0a5b 215b 5d28 6874 7470 733a 2f2f 6769  .[![](https://gi
-00000a70: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
-00000a80: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
-00000a90: 6765 732f 6163 7469 6f6e 732f 776f 726b  ges/actions/work
-00000aa0: 666c 6f77 732f 696e 7465 6772 6174 696f  flows/integratio
-00000ab0: 6e2d 7465 7374 732d 6972 6f64 732e 796d  n-tests-irods.ym
-00000ac0: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-00000ad0: 6368 3d64 6576 656c 6f70 295d 2868 7474  ch=develop)](htt
-00000ae0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000af0: 5574 7265 6368 7455 6e69 7665 7273 6974  UtrechtUniversit
-00000b00: 792f 6942 7269 6467 6573 2f61 6374 696f  y/iBridges/actio
-00000b10: 6e73 2f77 6f72 6b66 6c6f 7773 2f69 6e74  ns/workflows/int
-00000b20: 6567 7261 7469 6f6e 2d74 6573 7473 2d69  egration-tests-i
-00000b30: 726f 6473 2e79 6d6c 2920 5b21 5b5d 2868  rods.yml) [![](h
-00000b40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b50: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
-00000b60: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
-00000b70: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6d  ions/workflows/m
-00000b80: 6169 6e2e 796d 6c2f 6261 6467 652e 7376  ain.yml/badge.sv
-00000b90: 673f 6272 616e 6368 3d64 6576 656c 6f70  g?branch=develop
-00000ba0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000bb0: 622e 636f 6d2f 5574 7265 6368 7455 6e69  b.com/UtrechtUni
-00000bc0: 7665 7273 6974 792f 6942 7269 6467 6573  versity/iBridges
-00000bd0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000be0: 7773 2f6d 6169 6e2e 796d 6c29 200a 5b21  ws/main.yml) .[!
-00000bf0: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
-00000c00: 622e 636f 6d2f 5574 7265 6368 7455 6e69  b.com/UtrechtUni
-00000c10: 7665 7273 6974 792f 6942 7269 6467 6573  versity/iBridges
-00000c20: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000c30: 7773 2f69 6e74 6567 7261 7469 6f6e 2d74  ws/integration-t
-00000c40: 6573 7473 2d79 6f64 612e 796d 6c2f 6261  ests-yoda.yml/ba
-00000c50: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00000c60: 2f2f 6769 7468 7562 2e63 6f6d 2f55 7472  //github.com/Utr
-00000c70: 6563 6874 556e 6976 6572 7369 7479 2f69  echtUniversity/i
-00000c80: 4272 6964 6765 732f 6163 7469 6f6e 732f  Bridges/actions/
-00000c90: 776f 726b 666c 6f77 732f 696e 7465 6772  workflows/integr
-00000ca0: 6174 696f 6e2d 7465 7374 732d 796f 6461  ation-tests-yoda
-00000cb0: 2e79 6d6c 2920 215b 5d28 6874 7470 733a  .yml) ![](https:
-00000cc0: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
-00000cd0: 672f 7072 6f6a 6563 7473 2f69 6272 6964  g/projects/ibrid
-00000ce0: 6765 732f 6261 6467 652f 3f76 6572 7369  ges/badge/?versi
-00000cf0: 6f6e 3d6c 6174 6573 7426 7374 796c 653d  on=latest&style=
-00000d00: 666c 6174 2d64 6566 6175 6c74 290a 0a23  flat-default)..#
-00000d10: 2320 4162 6f75 740a 0a69 4272 6964 6765  # About..iBridge
-00000d20: 7320 6973 206c 6962 7261 7279 2066 6f72  s is library for
-00000d30: 2073 6369 656e 7469 6669 6320 7072 6f67   scientific prog
-00000d40: 7261 6d6d 6572 7320 7768 6f20 6172 6520  rammers who are 
-00000d50: 776f 726b 696e 6720 7769 7468 2064 6174  working with dat
-00000d60: 6120 696e 2069 524f 4453 2e20 5765 2070  a in iRODS. We p
-00000d70: 726f 7669 6465 2061 2077 7261 7070 6572  rovide a wrapper
-00000d80: 2061 726f 756e 6420 7468 6520 5b70 7974   around the [pyt
-00000d90: 686f 6e2d 6972 6f64 7363 6c69 656e 745d  hon-irodsclient]
-00000da0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000db0: 672f 7072 6f6a 6563 742f 7079 7468 6f6e  g/project/python
-00000dc0: 2d69 726f 6473 636c 6965 6e74 2f29 2074  -irodsclient/) t
-00000dd0: 6f20 6661 6369 6c69 7461 7465 2065 6173  o facilitate eas
-00000de0: 7920 696e 7465 7261 6374 696f 6e20 7769  y interaction wi
-00000df0: 7468 2074 6865 2069 524f 4453 2073 6572  th the iRODS ser
-00000e00: 7665 722e 0a0a 5369 6e63 6520 6942 7269  ver...Since iBri
-00000e10: 6467 6573 2069 7320 736f 6c65 6c79 2062  dges is solely b
-00000e20: 6173 6564 206f 6e20 7079 7468 6f6e 2069  ased on python i
-00000e30: 7420 776f 726b 7320 6f6e 2061 6c6c 206f  t works on all o
-00000e40: 7065 7261 7469 6e67 2073 7973 7465 6d73  perating systems
-00000e50: 2e0a 0a2d 2052 756e 7320 6f6e 2050 7974  ...- Runs on Pyt
-00000e60: 686f 6e20 332e 3820 6f72 2068 6967 6865  hon 3.8 or highe
-00000e70: 722e 0a2d 2053 7570 706f 7274 6564 2069  r..- Supported i
-00000e80: 524f 4453 2073 6572 7665 7220 7665 7273  RODS server vers
-00000e90: 696f 6e73 3a20 342e 322e 3131 206f 7220  ions: 4.2.11 or 
-00000ea0: 6869 6768 6572 2061 6e64 2034 2e33 2e30  higher and 4.3.0
-00000eb0: 206f 7220 6869 6768 6572 2e0a 0a20 3c70   or higher... <p
-00000ec0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000ed0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000ee0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ef0: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
-00000f00: 7479 2f69 4272 6964 6765 732f 6973 7375  ty/iBridges/issu
-00000f10: 6573 2f6e 6577 3f61 7373 6967 6e65 6573  es/new?assignees
-00000f20: 3d26 6c61 6265 6c73 3d26 7072 6f6a 6563  =&labels=&projec
-00000f30: 7473 3d26 7465 6d70 6c61 7465 3d62 7567  ts=&template=bug
-00000f40: 5f72 6570 6f72 742e 6d64 2674 6974 6c65  _report.md&title
-00000f50: 3d25 3542 4255 4725 3544 223e 5265 706f  =%5BBUG%5D">Repo
-00000f60: 7274 2042 7567 3c2f 613e 0a20 2020 202e  rt Bug</a>.    .
-00000f70: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000f90: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
-00000fa0: 7479 2f69 4272 6964 6765 732f 6973 7375  ty/iBridges/issu
-00000fb0: 6573 2f6e 6577 3f61 7373 6967 6e65 6573  es/new?assignees
-00000fc0: 3d26 6c61 6265 6c73 3d26 7072 6f6a 6563  =&labels=&projec
-00000fd0: 7473 3d26 7465 6d70 6c61 7465 3d66 6561  ts=&template=fea
-00000fe0: 7475 7265 5f72 6571 7565 7374 2e6d 6426  ture_request.md&
-00000ff0: 7469 746c 653d 2535 4246 4541 5455 5245  title=%5BFEATURE
-00001000: 2535 4422 3e52 6571 7565 7374 2046 6561  %5D">Request Fea
-00001010: 7475 7265 3c2f 613e 0a20 2020 202e 0a20  ture</a>.    .. 
-00001020: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00001030: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
-00001040: 7472 6563 6874 556e 6976 6572 7369 7479  trechtUniversity
-00001050: 2f69 4272 6964 6765 732f 6469 7363 7573  /iBridges/discus
-00001060: 7369 6f6e 732f 6361 7465 676f 7269 6573  sions/categories
-00001070: 2f69 6465 6173 223e 5368 6172 6520 616e  /ideas">Share an
-00001080: 2069 6465 613c 2f61 3e0a 2020 2020 2e0a   idea</a>.    ..
-00001090: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-000010a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000010b0: 5574 7265 6368 7455 6e69 7665 7273 6974  UtrechtUniversit
-000010c0: 792f 6942 7269 6467 6573 2f64 6973 6375  y/iBridges/discu
-000010d0: 7373 696f 6e73 2f63 6174 6567 6f72 6965  ssions/categorie
-000010e0: 732f 6765 6e65 7261 6c22 3e4c 6561 7665  s/general">Leave
-000010f0: 2073 6f6d 6520 6665 6564 6261 636b 3c2f   some feedback</
-00001100: 613e 0a20 2020 202e 0a20 2020 203c 6120  a>.    ..    <a 
-00001110: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001120: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
-00001130: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
-00001140: 6765 732f 6469 7363 7573 7369 6f6e 732f  ges/discussions/
-00001150: 6361 7465 676f 7269 6573 2f71 2d61 223e  categories/q-a">
-00001160: 4173 6b20 6120 7175 6573 7469 6f6e 3c2f  Ask a question</
-00001170: 613e 0a20 203c 2f70 3e0a 3c2f 703e 0a0a  a>.  </p>.</p>..
-00001180: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00001190: 2323 2320 4672 6f6d 2047 6974 6875 6220  ### From Github 
-000011a0: 7265 706f 7369 746f 7279 0a60 6060 0a67  repository.```.g
-000011b0: 6974 2063 6c6f 6e65 2067 6974 4067 6974  it clone git@git
-000011c0: 6875 622e 636f 6d3a 5574 7265 6368 7455  hub.com:UtrechtU
-000011d0: 6e69 7665 7273 6974 792f 6942 7269 6467  niversity/iBridg
-000011e0: 6573 2e67 6974 0a63 6420 6942 7269 6467  es.git.cd iBridg
-000011f0: 6573 0a70 6970 2069 6e73 7461 6c6c 202e  es.pip install .
-00001200: 0a60 6060 0a0a 2323 2320 5079 7069 2069  .```..### Pypi i
-00001210: 6e73 7461 6c6c 0a60 6060 0a70 6970 2069  nstall.```.pip i
-00001220: 6e73 7461 6c6c 2069 6272 6964 6765 730a  nstall ibridges.
-00001230: 6060 600a 0a23 2320 5573 6167 650a 6060  ```..## Usage.``
-00001240: 6070 790a 2320 4372 6561 7465 2061 6e20  `py.# Create an 
-00001250: 6952 4f44 5320 7365 7373 696f 6e0a 6672  iRODS session.fr
-00001260: 6f6d 2069 6272 6964 6765 7320 696d 706f  om ibridges impo
-00001270: 7274 2053 6573 7369 6f6e 0a0a 7365 7373  rt Session..sess
-00001280: 696f 6e20 3d20 5365 7373 696f 6e28 6972  ion = Session(ir
-00001290: 6f64 735f 656e 765f 7061 7468 3d22 7e2f  ods_env_path="~/
-000012a0: 2e69 726f 6473 2f69 726f 6473 5f65 6e76  .irods/irods_env
-000012b0: 6972 6f6e 6d65 6e74 2e6a 736f 6e22 2c20  ironment.json", 
-000012c0: 7061 7373 776f 7264 3d22 6d79 7061 7373  password="mypass
-000012d0: 776f 7264 2229 0a0a 2320 5570 6c6f 6164  word")..# Upload
-000012e0: 2064 6174 610a 6672 6f6d 2069 6272 6964   data.from ibrid
-000012f0: 6765 7320 696d 706f 7274 2075 706c 6f61  ges import uploa
-00001300: 640a 0a75 706c 6f61 6428 7365 7373 696f  d..upload(sessio
-00001310: 6e2c 2022 2f79 6f75 722f 6c6f 6361 6c2f  n, "/your/local/
-00001320: 7061 7468 222c 2022 2f69 726f 6473 2f70  path", "/irods/p
-00001330: 6174 6822 290a 0a23 2044 6f77 6e6c 6f61  ath")..# Downloa
-00001340: 6420 6461 7461 0a66 726f 6d20 6962 7269  d data.from ibri
-00001350: 6467 6573 2069 6d70 6f72 7420 646f 776e  dges import down
-00001360: 6c6f 6164 0a0a 646f 776e 6c6f 6164 2873  load..download(s
-00001370: 6573 7369 6f6e 2c20 222f 6972 6f64 732f  ession, "/irods/
-00001380: 7061 7468 222c 2022 2f6f 7468 6572 2f6c  path", "/other/l
-00001390: 6f63 616c 2f70 6174 6822 290a 0a60 6060  ocal/path")..```
-000013a0: 0a0a 2323 2054 7574 6f72 6961 6c73 0a23  ..## Tutorials.#
-000013b0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000013c0: 0a2d 202a 2a5b 5265 6164 5468 6544 6f63  .- **[ReadTheDoc
-000013d0: 735d 2868 7474 7073 3a2f 2f69 6272 6964  s](https://ibrid
-000013e0: 6765 732e 7265 6164 7468 6564 6f63 732e  ges.readthedocs.
-000013f0: 696f 2f65 6e2f 6c61 7465 7374 2f29 2a2a  io/en/latest/)**
-00001400: 0a0a 2323 2320 4775 6964 6573 0a2d 205b  ..### Guides.- [
-00001410: 5175 6963 6b53 7461 7274 5d28 5475 746f  QuickStart](Tuto
-00001420: 7269 616c 732f 5175 6963 6b53 7461 7274  rials/QuickStart
-00001430: 2e69 7079 6e62 290a 2d20 5b69 524f 4453  .ipynb).- [iRODS
-00001440: 2050 6174 6873 5d28 5475 746f 7269 616c   Paths](Tutorial
-00001450: 732f 6952 4f44 535f 7061 7468 732e 6970  s/iRODS_paths.ip
-00001460: 796e 6229 0a2d 205b 4461 7461 2073 796e  ynb).- [Data syn
-00001470: 6368 726f 6e69 7361 7469 6f6e 5d28 5475  chronisation](Tu
-00001480: 746f 7269 616c 732f 4461 7461 5f73 796e  torials/Data_syn
-00001490: 632e 6970 796e 6229 0a0a 2323 2320 4265  c.ipynb)..### Be
-000014a0: 6769 6e6e 6572 7320 7475 746f 7269 616c  ginners tutorial
-000014b0: 730a 2d20 5b53 6574 7570 2063 6c69 656e  s.- [Setup clien
-000014c0: 7420 636f 6e66 6967 7572 6174 696f 6e5d  t configuration]
-000014d0: 2854 7574 6f72 6961 6c73 2f30 312d 5365  (Tutorials/01-Se
-000014e0: 7475 702d 616e 642d 636f 6e6e 6563 742e  tup-and-connect.
-000014f0: 6970 796e 6229 0a2d 205b 576f 726b 696e  ipynb).- [Workin
-00001500: 6720 7769 7468 2064 6174 615d 2854 7574  g with data](Tut
-00001510: 6f72 6961 6c73 2f30 322d 576f 726b 696e  orials/02-Workin
-00001520: 672d 7769 7468 2d64 6174 612e 6970 796e  g-with-data.ipyn
-00001530: 6229 0a2d 205b 6952 4f44 5320 616e 6420  b).- [iRODS and 
-00001540: 6c6f 6361 6c20 5061 7468 735d 2854 7574  local Paths](Tut
-00001550: 6f72 6961 6c73 2f30 332d 6952 4f44 532d  orials/03-iRODS-
-00001560: 5061 7468 732e 6970 796e 6229 0a2d 205b  Paths.ipynb).- [
-00001570: 4d65 7461 6461 7461 5d28 5475 746f 7269  Metadata](Tutori
-00001580: 616c 732f 3034 2d4d 6574 6164 6174 612e  als/04-Metadata.
-00001590: 6970 796e 6229 0a2d 205b 5368 6172 696e  ipynb).- [Sharin
-000015a0: 6720 6461 7461 5d28 5475 746f 7269 616c  g data](Tutorial
-000015b0: 732f 3035 2d44 6174 612d 5368 6172 696e  s/05-Data-Sharin
-000015c0: 672e 6970 796e 6229 0a0a 2323 2041 7574  g.ipynb)..## Aut
-000015d0: 686f 7273 0a0a 2a2a 4368 7269 7374 696e  hors..**Christin
-000015e0: 6520 5374 6169 6765 7220 284d 6169 6e74  e Staiger (Maint
-000015f0: 6169 6e65 7229 205b 4f52 4349 445d 2868  ainer) [ORCID](h
-00001600: 7474 7073 3a2f 2f6f 7263 6964 2e6f 7267  ttps://orcid.org
-00001610: 2f30 3030 302d 3030 3032 2d36 3735 342d  /0000-0002-6754-
-00001620: 3736 3437 292a 2a0a 0a2d 202a 5761 6765  7647)**..- *Wage
-00001630: 6e69 6e67 656e 2055 6e69 7665 7273 6974  ningen Universit
-00001640: 7920 2620 5265 7365 6172 6368 2a20 3230  y & Research* 20
-00001650: 3231 202d 2032 3032 320a 2d20 2a55 7472  21 - 2022.- *Utr
-00001660: 6563 6874 2055 6e69 7665 7273 6974 792a  echt University*
-00001670: 2032 3032 320a 0a2a 2a54 696d 2076 616e   2022..**Tim van
-00001680: 2044 6161 6c65 6e2a 2a2c 202a 5761 6765   Daalen**, *Wage
-00001690: 6e69 6e67 656e 2055 6e69 7665 7273 6974  ningen Universit
-000016a0: 7920 2620 5265 7365 6172 6368 2a20 3230  y & Research* 20
-000016b0: 3231 0a0a 2a2a 4d61 6172 7465 6e20 5363  21..**Maarten Sc
-000016c0: 6865 726d 6572 2028 4d61 696e 7461 696e  hermer (Maintain
-000016d0: 6572 2920 5b4f 5243 4944 5d28 6874 7470  er) [ORCID](http
-000016e0: 733a 2f2f 6f72 6369 642e 6f72 672f 6d79  s://orcid.org/my
-000016f0: 2d6f 7263 6964 3f6f 7263 6964 3d30 3030  -orcid?orcid=000
-00001700: 302d 3030 3031 2d36 3737 302d 3331 3535  0-0001-6770-3155
-00001710: 292a 2a2c 202a 5574 7265 6368 7420 556e  )**, *Utrecht Un
-00001720: 6976 6572 7369 7479 2a20 3230 3233 0a0a  iversity* 2023..
-00001730: 2a2a 5261 6f75 6c20 5363 6872 616d 2028  **Raoul Schram (
-00001740: 4d61 696e 7461 696e 6572 2920 5b4f 5243  Maintainer) [ORC
-00001750: 4944 5d28 6874 7470 733a 2f2f 6f72 6369  ID](https://orci
-00001760: 642e 6f72 672f 6d79 2d6f 7263 6964 3f6f  d.org/my-orcid?o
-00001770: 7263 6964 3d30 3030 302d 3030 3031 2d36  rcid=0000-0001-6
-00001780: 3631 362d 3233 3058 292a 2a2e 200a 2a55  616-230X)**. .*U
-00001790: 7472 6563 6874 2055 6e69 7665 7273 6974  trecht Universit
-000017a0: 792a 2032 3032 330a 0a23 2320 436f 6e74  y* 2023..## Cont
-000017b0: 7269 6275 746f 7273 0a0a 2a2a 4a2e 502e  ributors..**J.P.
-000017c0: 204d 6320 4661 726c 616e 642a 2a2c 0a2a   Mc Farland**,.*
-000017d0: 556e 6976 6572 7369 7479 206f 6620 4772  University of Gr
-000017e0: 6f6e 696e 6765 6e2c 2043 656e 7465 7220  oningen, Center 
-000017f0: 666f 7220 496e 666f 726d 6174 696f 6e20  for Information 
-00001800: 5465 6368 6e6f 6c6f 6779 2a2c 2032 3032  Technology*, 202
-00001810: 320a 0a23 2320 4c69 6365 6e73 650a 5468  2..## License.Th
-00001820: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
-00001830: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
-00001840: 2047 504c 2d76 3320 6c69 6365 6e73 652e   GPL-v3 license.
-00001850: 0a54 6865 2066 756c 6c20 6c69 6365 6e73  .The full licens
-00001860: 6520 6361 6e20 6265 2066 6f75 6e64 2069  e can be found i
-00001870: 6e20 5b4c 4943 454e 5345 5d28 4c49 4345  n [LICENSE](LICE
-00001880: 4e53 4529 2e0a                           NSE)..
+00000a60: 0a5b 215b 5079 5049 2076 6572 7369 6f6e  .[![PyPI version
+00000a70: 5d28 6874 7470 733a 2f2f 6261 6467 652e  ](https://badge.
+00000a80: 6675 7279 2e69 6f2f 7079 2f69 6272 6964  fury.io/py/ibrid
+00000a90: 6765 732e 7376 6729 5d28 6874 7470 733a  ges.svg)](https:
+00000aa0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000ab0: 7079 2f69 6272 6964 6765 7329 0a5b 215b  py/ibridges).[![
+00000ac0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ad0: 2e63 6f6d 2f55 7472 6563 6874 556e 6976  .com/UtrechtUniv
+00000ae0: 6572 7369 7479 2f69 4272 6964 6765 732f  ersity/iBridges/
+00000af0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000b00: 732f 696e 7465 6772 6174 696f 6e2d 7465  s/integration-te
+00000b10: 7374 732d 6972 6f64 732e 796d 6c2f 6261  sts-irods.yml/ba
+00000b20: 6467 652e 7376 673f 6272 616e 6368 3d64  dge.svg?branch=d
+00000b30: 6576 656c 6f70 295d 2868 7474 7073 3a2f  evelop)](https:/
+00000b40: 2f67 6974 6875 622e 636f 6d2f 5574 7265  /github.com/Utre
+00000b50: 6368 7455 6e69 7665 7273 6974 792f 6942  chtUniversity/iB
+00000b60: 7269 6467 6573 2f61 6374 696f 6e73 2f77  ridges/actions/w
+00000b70: 6f72 6b66 6c6f 7773 2f69 6e74 6567 7261  orkflows/integra
+00000b80: 7469 6f6e 2d74 6573 7473 2d69 726f 6473  tion-tests-irods
+00000b90: 2e79 6d6c 2920 5b21 5b5d 2868 7474 7073  .yml) [![](https
+00000ba0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5574  ://github.com/Ut
+00000bb0: 7265 6368 7455 6e69 7665 7273 6974 792f  rechtUniversity/
+00000bc0: 6942 7269 6467 6573 2f61 6374 696f 6e73  iBridges/actions
+00000bd0: 2f77 6f72 6b66 6c6f 7773 2f6d 6169 6e2e  /workflows/main.
+00000be0: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
+00000bf0: 616e 6368 3d64 6576 656c 6f70 295d 2868  anch=develop)](h
+00000c00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c10: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
+00000c20: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
+00000c30: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6d  ions/workflows/m
+00000c40: 6169 6e2e 796d 6c29 200a 5b21 5b5d 2868  ain.yml) .[![](h
+00000c50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c60: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
+00000c70: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
+00000c80: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f69  ions/workflows/i
+00000c90: 6e74 6567 7261 7469 6f6e 2d74 6573 7473  ntegration-tests
+00000ca0: 2d79 6f64 612e 796d 6c2f 6261 6467 652e  -yoda.yml/badge.
+00000cb0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000cc0: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+00000cd0: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00000ce0: 6765 732f 6163 7469 6f6e 732f 776f 726b  ges/actions/work
+00000cf0: 666c 6f77 732f 696e 7465 6772 6174 696f  flows/integratio
+00000d00: 6e2d 7465 7374 732d 796f 6461 2e79 6d6c  n-tests-yoda.yml
+00000d10: 2920 215b 5d28 6874 7470 733a 2f2f 7265  ) ![](https://re
+00000d20: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000d30: 6f6a 6563 7473 2f69 6272 6964 6765 732f  ojects/ibridges/
+00000d40: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000d50: 6174 6573 7426 7374 796c 653d 666c 6174  atest&style=flat
+00000d60: 2d64 6566 6175 6c74 290a 0a69 4272 6964  -default)..iBrid
+00000d70: 6765 7320 6973 206c 6962 7261 7279 2066  ges is library f
+00000d80: 6f72 2073 6369 656e 7469 6669 6320 7072  or scientific pr
+00000d90: 6f67 7261 6d6d 6572 7320 7768 6f20 6172  ogrammers who ar
+00000da0: 6520 776f 726b 696e 6720 7769 7468 2064  e working with d
+00000db0: 6174 6120 696e 2069 524f 4453 2e20 5765  ata in iRODS. We
+00000dc0: 2070 726f 7669 6465 2061 2077 7261 7070   provide a wrapp
+00000dd0: 6572 2061 726f 756e 6420 7468 6520 5b70  er around the [p
+00000de0: 7974 686f 6e2d 6972 6f64 7363 6c69 656e  ython-irodsclien
+00000df0: 745d 2868 7474 7073 3a2f 2f70 7970 692e  t](https://pypi.
+00000e00: 6f72 672f 7072 6f6a 6563 742f 7079 7468  org/project/pyth
+00000e10: 6f6e 2d69 726f 6473 636c 6965 6e74 2f29  on-irodsclient/)
+00000e20: 2074 6f20 6661 6369 6c69 7461 7465 2065   to facilitate e
+00000e30: 6173 7920 696e 7465 7261 6374 696f 6e20  asy interaction 
+00000e40: 7769 7468 2074 6865 2069 524f 4453 2073  with the iRODS s
+00000e50: 6572 7665 722e 2069 4272 6964 6765 7320  erver. iBridges 
+00000e60: 6973 2063 7572 7265 6e74 6c79 2073 7469  is currently sti
+00000e70: 6c6c 2069 6e20 7665 7279 2061 6374 6976  ll in very activ
+00000e80: 6520 6465 7665 6c6f 706d 656e 742e 0a0a  e development...
+00000e90: 2323 2048 6967 686c 6967 6874 730a 0a2d  ## Highlights..-
+00000ea0: 2057 6f72 6b73 206f 6e20 5769 6e64 6f77   Works on Window
+00000eb0: 732c 204d 6163 204f 5320 616e 6420 4c69  s, Mac OS and Li
+00000ec0: 6e75 780a 2d20 5275 6e73 206f 6e20 5079  nux.- Runs on Py
+00000ed0: 7468 6f6e 2033 2e38 206f 7220 6869 6768  thon 3.8 or high
+00000ee0: 6572 2e0a 2d20 5375 7070 6f72 7465 6420  er..- Supported 
+00000ef0: 6952 4f44 5320 7365 7276 6572 2076 6572  iRODS server ver
+00000f00: 7369 6f6e 733a 2034 2e32 2e31 3120 6f72  sions: 4.2.11 or
+00000f10: 2068 6967 6865 7220 616e 6420 342e 332e   higher and 4.3.
+00000f20: 3020 6f72 2068 6967 6865 722e 0a2d 202a  0 or higher..- *
+00000f30: 2a49 6e74 6572 6163 7469 7665 2063 6f6e  *Interactive con
+00000f40: 6e65 6374 696f 6e2a 2a20 746f 2079 6f75  nection** to you
+00000f50: 7220 6952 6f64 7320 7365 7276 6572 2e0a  r iRods server..
+00000f60: 2d20 2a2a 5570 6c6f 6164 2a2a 2061 6e64  - **Upload** and
+00000f70: 202a 2a44 6f77 6e6c 6f61 642a 2a20 796f   **Download** yo
+00000f80: 7572 2064 6174 612e 0a2d 204d 616e 6970  ur data..- Manip
+00000f90: 756c 6174 6520 7468 6520 2a2a 6d65 7461  ulate the **meta
+00000fa0: 6461 7461 2a2a 206f 6e20 7468 6520 6952  data** on the iR
+00000fb0: 4f44 5320 7365 7276 6572 2e0a 2d20 2a2a  ODS server..- **
+00000fc0: 5379 6e63 6872 6f6e 697a 652a 2a20 796f  Synchronize** yo
+00000fd0: 7572 2064 6174 6120 6265 7477 6565 6e20  ur data between 
+00000fe0: 796f 7572 206c 6f63 616c 2063 6f6d 7075  your local compu
+00000ff0: 7465 7220 616e 6420 7468 6520 6952 4f44  ter and the iROD
+00001000: 5320 7365 7276 6572 2e0a 2d20 4372 6561  S server..- Crea
+00001010: 7465 2061 6e64 206d 616e 6970 756c 6174  te and manipulat
+00001020: 6520 2a2a 5469 636b 6574 732a 2a20 746f  e **Tickets** to
+00001030: 2074 656d 706f 7261 7269 6c79 2067 7261   temporarily gra
+00001040: 6e74 2061 6363 6573 7320 746f 206f 7574  nt access to out
+00001050: 7369 6465 2075 7365 7273 2e0a 2d20 2a2a  side users..- **
+00001060: 5365 6172 6368 2a2a 2074 6872 6f75 6768  Search** through
+00001070: 2061 6c6c 206d 6574 6164 6174 6120 666f   all metadata fo
+00001080: 7220 796f 7572 2064 6174 6173 6574 206f  r your dataset o
+00001090: 7220 636f 6c6c 6563 7469 6f6e 2e0a 2d20  r collection..- 
+000010a0: 536d 616c 6c20 6e75 6d62 6572 206f 6620  Small number of 
+000010b0: 6465 7065 6e64 656e 6369 6573 2028 6070  dependencies (`p
+000010c0: 7974 686f 6e2d 6972 6f64 7363 6c69 656e  ython-irodsclien
+000010d0: 7460 2061 6e64 2060 7471 646d 6029 0a2d  t` and `tqdm`).-
+000010e0: 2053 6166 6520 6465 6661 756c 7420 6f70   Safe default op
+000010f0: 7469 6f6e 7320 7768 656e 2077 6f72 6b69  tions when worki
+00001100: 6e67 2077 6974 6820 796f 7572 2064 6174  ng with your dat
+00001110: 612e 0a0a 0a20 3c70 2061 6c69 676e 3d22  a.... <p align="
+00001120: 6365 6e74 6572 223e 0a20 2020 203c 6120  center">.    <a 
+00001130: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001140: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+00001150: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00001160: 6765 732f 6973 7375 6573 2f6e 6577 3f61  ges/issues/new?a
+00001170: 7373 6967 6e65 6573 3d26 6c61 6265 6c73  ssignees=&labels
+00001180: 3d26 7072 6f6a 6563 7473 3d26 7465 6d70  =&projects=&temp
+00001190: 6c61 7465 3d62 7567 5f72 6570 6f72 742e  late=bug_report.
+000011a0: 6d64 2674 6974 6c65 3d25 3542 4255 4725  md&title=%5BBUG%
+000011b0: 3544 223e 5265 706f 7274 2042 7567 3c2f  5D">Report Bug</
+000011c0: 613e 0a20 2020 202e 0a20 2020 203c 6120  a>.    ..    <a 
+000011d0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000011e0: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+000011f0: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00001200: 6765 732f 6973 7375 6573 2f6e 6577 3f61  ges/issues/new?a
+00001210: 7373 6967 6e65 6573 3d26 6c61 6265 6c73  ssignees=&labels
+00001220: 3d26 7072 6f6a 6563 7473 3d26 7465 6d70  =&projects=&temp
+00001230: 6c61 7465 3d66 6561 7475 7265 5f72 6571  late=feature_req
+00001240: 7565 7374 2e6d 6426 7469 746c 653d 2535  uest.md&title=%5
+00001250: 4246 4541 5455 5245 2535 4422 3e52 6571  BFEATURE%5D">Req
+00001260: 7565 7374 2046 6561 7475 7265 3c2f 613e  uest Feature</a>
+00001270: 0a20 2020 202e 0a20 2020 203c 6120 6872  .    ..    <a hr
+00001280: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001290: 7562 2e63 6f6d 2f55 7472 6563 6874 556e  ub.com/UtrechtUn
+000012a0: 6976 6572 7369 7479 2f69 4272 6964 6765  iversity/iBridge
+000012b0: 732f 6469 7363 7573 7369 6f6e 732f 6361  s/discussions/ca
+000012c0: 7465 676f 7269 6573 2f69 6465 6173 223e  tegories/ideas">
+000012d0: 5368 6172 6520 616e 2069 6465 613c 2f61  Share an idea</a
+000012e0: 3e0a 2020 2020 2e0a 2020 2020 3c61 2068  >.    ..    <a h
+000012f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001300: 6875 622e 636f 6d2f 5574 7265 6368 7455  hub.com/UtrechtU
+00001310: 6e69 7665 7273 6974 792f 6942 7269 6467  niversity/iBridg
+00001320: 6573 2f64 6973 6375 7373 696f 6e73 2f63  es/discussions/c
+00001330: 6174 6567 6f72 6965 732f 6765 6e65 7261  ategories/genera
+00001340: 6c22 3e4c 6561 7665 2073 6f6d 6520 6665  l">Leave some fe
+00001350: 6564 6261 636b 3c2f 613e 0a20 2020 202e  edback</a>.    .
+00001360: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00001370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001380: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
+00001390: 7479 2f69 4272 6964 6765 732f 6469 7363  ty/iBridges/disc
+000013a0: 7573 7369 6f6e 732f 6361 7465 676f 7269  ussions/categori
+000013b0: 6573 2f71 2d61 223e 4173 6b20 6120 7175  es/q-a">Ask a qu
+000013c0: 6573 7469 6f6e 3c2f 613e 0a20 203c 2f70  estion</a>.  </p
+000013d0: 3e0a 3c2f 703e 0a0a 2323 2049 6e73 7461  >.</p>..## Insta
+000013e0: 6c6c 6174 696f 6e0a 0a54 6865 7265 2061  llation..There a
+000013f0: 7265 2074 776f 206d 6169 6e20 7761 7973  re two main ways
+00001400: 2074 6f20 696e 7374 616c 6c20 6942 7269   to install iBri
+00001410: 6467 6573 2e20 5468 6520 7265 636f 6d6d  dges. The recomm
+00001420: 656e 6465 6420 7761 7920 6973 2074 6f20  ended way is to 
+00001430: 7573 6520 7468 6520 7374 6162 6c65 2076  use the stable v
+00001440: 6572 7369 6f6e 2074 6861 7420 6973 2061  ersion that is a
+00001450: 7661 696c 6162 6c65 206f 6e20 5079 5069  vailable on PyPi
+00001460: 3a0a 0a60 6060 6261 7368 0a70 6970 2069  :..```bash.pip i
+00001470: 6e73 7461 6c6c 2069 6272 6964 6765 730a  nstall ibridges.
+00001480: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00001490: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+000014a0: 756e 7374 6162 6c65 2076 6572 7369 6f6e  unstable version
+000014b0: 2074 6f20 7465 7374 206f 7574 206e 6577   to test out new
+000014c0: 2066 6561 7475 7265 732c 2079 6f75 2063   features, you c
+000014d0: 616e 2069 6e73 7461 6c6c 2074 6865 2064  an install the d
+000014e0: 6576 656c 6f70 6d65 6e74 2062 7261 6e63  evelopment branc
+000014f0: 683a 0a0a 6060 6062 6173 680a 7069 7020  h:..```bash.pip 
+00001500: 696e 7374 616c 6c20 6769 742b 6874 7470  install git+http
+00001510: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
+00001520: 7472 6563 6874 556e 6976 6572 7369 7479  trechtUniversity
+00001530: 2f69 4272 6964 6765 732e 6769 7440 6465  /iBridges.git@de
+00001540: 7665 6c6f 700a 6060 600a 0a23 2320 5573  velop.```..## Us
+00001550: 6167 650a 0a42 656c 6f77 2061 7265 2073  age..Below are s
+00001560: 6f6d 6520 6261 7369 6320 6578 616d 706c  ome basic exampl
+00001570: 6573 206f 6620 7468 6520 6665 6174 7572  es of the featur
+00001580: 6573 2069 6e20 6942 7269 6467 6573 2e0a  es in iBridges..
+00001590: 0a60 6060 7079 0a23 2043 7265 6174 6520  .```py.# Create 
+000015a0: 616e 2069 524f 4453 2073 6573 7369 6f6e  an iRODS session
+000015b0: 0a66 726f 6d20 6962 7269 6467 6573 2069  .from ibridges i
+000015c0: 6d70 6f72 7420 5365 7373 696f 6e0a 0a73  mport Session..s
+000015d0: 6573 7369 6f6e 203d 2053 6573 7369 6f6e  ession = Session
+000015e0: 2869 726f 6473 5f65 6e76 5f70 6174 683d  (irods_env_path=
+000015f0: 227e 2f2e 6972 6f64 732f 6972 6f64 735f  "~/.irods/irods_
+00001600: 656e 7669 726f 6e6d 656e 742e 6a73 6f6e  environment.json
+00001610: 222c 2070 6173 7377 6f72 643d 226d 7970  ", password="myp
+00001620: 6173 7377 6f72 6422 290a 0a23 2055 706c  assword")..# Upl
+00001630: 6f61 6420 6461 7461 0a66 726f 6d20 6962  oad data.from ib
+00001640: 7269 6467 6573 2069 6d70 6f72 7420 7570  ridges import up
+00001650: 6c6f 6164 0a0a 7570 6c6f 6164 2873 6573  load..upload(ses
+00001660: 7369 6f6e 2c20 222f 796f 7572 2f6c 6f63  sion, "/your/loc
+00001670: 616c 2f70 6174 6822 2c20 222f 6972 6f64  al/path", "/irod
+00001680: 732f 7061 7468 2229 0a0a 2320 446f 776e  s/path")..# Down
+00001690: 6c6f 6164 2064 6174 610a 6672 6f6d 2069  load data.from i
+000016a0: 6272 6964 6765 7320 696d 706f 7274 2064  bridges import d
+000016b0: 6f77 6e6c 6f61 640a 0a64 6f77 6e6c 6f61  ownload..downloa
+000016c0: 6428 7365 7373 696f 6e2c 2022 2f69 726f  d(session, "/iro
+000016d0: 6473 2f70 6174 6822 2c20 222f 6f74 6865  ds/path", "/othe
+000016e0: 722f 6c6f 6361 6c2f 7061 7468 2229 0a0a  r/local/path")..
+000016f0: 6060 600a 0a23 2320 5475 746f 7269 616c  ```..## Tutorial
+00001700: 730a 2323 2320 446f 6375 6d65 6e74 6174  s.### Documentat
+00001710: 696f 6e0a 2d20 2a2a 5b52 6561 6454 6865  ion.- **[ReadThe
+00001720: 446f 6373 5d28 6874 7470 733a 2f2f 6962  Docs](https://ib
+00001730: 7269 6467 6573 2e72 6561 6474 6865 646f  ridges.readthedo
+00001740: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001750: 292a 2a0a 0a23 2323 2047 7569 6465 730a  )**..### Guides.
+00001760: 2d20 5b51 7569 636b 5374 6172 745d 2874  - [QuickStart](t
+00001770: 7574 6f72 6961 6c73 2f51 7569 636b 5374  utorials/QuickSt
+00001780: 6172 742e 6970 796e 6229 0a2d 205b 6952  art.ipynb).- [iR
+00001790: 4f44 5320 5061 7468 735d 2874 7574 6f72  ODS Paths](tutor
+000017a0: 6961 6c73 2f69 524f 4453 5f70 6174 6873  ials/iRODS_paths
+000017b0: 2e69 7079 6e62 290a 2d20 5b44 6174 6120  .ipynb).- [Data 
+000017c0: 7379 6e63 6872 6f6e 6973 6174 696f 6e5d  synchronisation]
+000017d0: 2874 7574 6f72 6961 6c73 2f44 6174 615f  (tutorials/Data_
+000017e0: 7379 6e63 2e69 7079 6e62 290a 0a23 2323  sync.ipynb)..###
+000017f0: 2042 6567 696e 6e65 7273 2074 7574 6f72   Beginners tutor
+00001800: 6961 6c73 0a2d 205b 5365 7475 7020 636c  ials.- [Setup cl
+00001810: 6965 6e74 2063 6f6e 6669 6775 7261 7469  ient configurati
+00001820: 6f6e 5d28 7475 746f 7269 616c 732f 3031  on](tutorials/01
+00001830: 2d53 6574 7570 2d61 6e64 2d63 6f6e 6e65  -Setup-and-conne
+00001840: 6374 2e69 7079 6e62 290a 2d20 5b57 6f72  ct.ipynb).- [Wor
+00001850: 6b69 6e67 2077 6974 6820 6461 7461 5d28  king with data](
+00001860: 7475 746f 7269 616c 732f 3032 2d57 6f72  tutorials/02-Wor
+00001870: 6b69 6e67 2d77 6974 682d 6461 7461 2e69  king-with-data.i
+00001880: 7079 6e62 290a 2d20 5b69 524f 4453 2061  pynb).- [iRODS a
+00001890: 6e64 206c 6f63 616c 2050 6174 6873 5d28  nd local Paths](
+000018a0: 7475 746f 7269 616c 732f 3033 2d69 524f  tutorials/03-iRO
+000018b0: 4453 2d50 6174 6873 2e69 7079 6e62 290a  DS-Paths.ipynb).
+000018c0: 2d20 5b4d 6574 6164 6174 615d 2874 7574  - [Metadata](tut
+000018d0: 6f72 6961 6c73 2f30 342d 4d65 7461 6461  orials/04-Metada
+000018e0: 7461 2e69 7079 6e62 290a 2d20 5b53 6861  ta.ipynb).- [Sha
+000018f0: 7269 6e67 2064 6174 615d 2874 7574 6f72  ring data](tutor
+00001900: 6961 6c73 2f30 352d 4461 7461 2d53 6861  ials/05-Data-Sha
+00001910: 7269 6e67 2e69 7079 6e62 290a 0a23 2320  ring.ipynb)..## 
+00001920: 4175 7468 6f72 730a 0a2a 2a43 6872 6973  Authors..**Chris
+00001930: 7469 6e65 2053 7461 6967 6572 2028 4d61  tine Staiger (Ma
+00001940: 696e 7461 696e 6572 2920 5b4f 5243 4944  intainer) [ORCID
+00001950: 5d28 6874 7470 733a 2f2f 6f72 6369 642e  ](https://orcid.
+00001960: 6f72 672f 3030 3030 2d30 3030 322d 3637  org/0000-0002-67
+00001970: 3534 2d37 3634 3729 2a2a 0a0a 2d20 2a57  54-7647)**..- *W
+00001980: 6167 656e 696e 6765 6e20 556e 6976 6572  ageningen Univer
+00001990: 7369 7479 2026 2052 6573 6561 7263 682a  sity & Research*
+000019a0: 2032 3032 3120 2d20 3230 3232 0a2d 202a   2021 - 2022.- *
+000019b0: 5574 7265 6368 7420 556e 6976 6572 7369  Utrecht Universi
+000019c0: 7479 2a20 3230 3232 0a0a 2a2a 5469 6d20  ty* 2022..**Tim 
+000019d0: 7661 6e20 4461 616c 656e 2a2a 2c20 2a57  van Daalen**, *W
+000019e0: 6167 656e 696e 6765 6e20 556e 6976 6572  ageningen Univer
+000019f0: 7369 7479 2026 2052 6573 6561 7263 682a  sity & Research*
+00001a00: 2032 3032 310a 0a2a 2a4d 6161 7274 656e   2021..**Maarten
+00001a10: 2053 6368 6572 6d65 7220 284d 6169 6e74   Schermer (Maint
+00001a20: 6169 6e65 7229 205b 4f52 4349 445d 2868  ainer) [ORCID](h
+00001a30: 7474 7073 3a2f 2f6f 7263 6964 2e6f 7267  ttps://orcid.org
+00001a40: 2f6d 792d 6f72 6369 643f 6f72 6369 643d  /my-orcid?orcid=
+00001a50: 3030 3030 2d30 3030 312d 3637 3730 2d33  0000-0001-6770-3
+00001a60: 3135 3529 2a2a 2c20 2a55 7472 6563 6874  155)**, *Utrecht
+00001a70: 2055 6e69 7665 7273 6974 792a 2032 3032   University* 202
+00001a80: 330a 0a2a 2a52 616f 756c 2053 6368 7261  3..**Raoul Schra
+00001a90: 6d20 284d 6169 6e74 6169 6e65 7229 205b  m (Maintainer) [
+00001aa0: 4f52 4349 445d 2868 7474 7073 3a2f 2f6f  ORCID](https://o
+00001ab0: 7263 6964 2e6f 7267 2f6d 792d 6f72 6369  rcid.org/my-orci
+00001ac0: 643f 6f72 6369 643d 3030 3030 2d30 3030  d?orcid=0000-000
+00001ad0: 312d 3636 3136 2d32 3330 5829 2a2a 2e20  1-6616-230X)**. 
+00001ae0: 0a2a 5574 7265 6368 7420 556e 6976 6572  .*Utrecht Univer
+00001af0: 7369 7479 2a20 3230 3233 0a0a 2323 2043  sity* 2023..## C
+00001b00: 6f6e 7472 6962 7574 6f72 730a 0a2a 2a4a  ontributors..**J
+00001b10: 2e50 2e20 4d63 2046 6172 6c61 6e64 2a2a  .P. Mc Farland**
+00001b20: 2c0a 2a55 6e69 7665 7273 6974 7920 6f66  ,.*University of
+00001b30: 2047 726f 6e69 6e67 656e 2c20 4365 6e74   Groningen, Cent
+00001b40: 6572 2066 6f72 2049 6e66 6f72 6d61 7469  er for Informati
+00001b50: 6f6e 2054 6563 686e 6f6c 6f67 792a 2c20  on Technology*, 
+00001b60: 3230 3232 0a0a 2323 204c 6963 656e 7365  2022..## License
+00001b70: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001b80: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001b90: 7468 6520 4d49 5420 6c69 6365 6e73 652e  the MIT license.
+00001ba0: 0a54 6865 2066 756c 6c20 6c69 6365 6e73  .The full licens
+00001bb0: 6520 6361 6e20 6265 2066 6f75 6e64 2069  e can be found i
+00001bc0: 6e20 5b4c 4943 454e 5345 5d28 4c49 4345  n [LICENSE](LICE
+00001bd0: 4e53 4529 2e0a                           NSE)..
```

### Comparing `ibridges-0.1.2/docker/.gitattributes` & `ibridges-0.1.3/docker/.gitattributes`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/README.md` & `ibridges-0.1.3/docker/README.md`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_catalog_provider/Dockerfile` & `ibridges-0.1.3/docker/irods_catalog_provider/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_catalog_provider/entrypoint.sh` & `ibridges-0.1.3/docker/irods_catalog_provider/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/Dockerfile` & `ibridges-0.1.3/docker/irods_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/entrypoint.sh` & `ibridges-0.1.3/docker/irods_client/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/environments/yoda/config.toml` & `ibridges-0.1.3/docker/irods_client/environments/yoda/config.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/environments/yoda/irods_environment.json` & `ibridges-0.1.3/docker/irods_client/environments/yoda/irods_environment.json`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/testdata/beach.rtf` & `ibridges-0.1.3/docker/irods_client/testdata/beach.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/testdata/bunny.rtf` & `ibridges-0.1.3/docker/irods_client/testdata/bunny.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/testdata/more_data/polarbear.txt` & `ibridges-0.1.3/docker/irods_client/testdata/more_data/polarbear.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/testdata/plant.rtf` & `ibridges-0.1.3/docker/irods_client/testdata/plant.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/testdata/sun.rtf` & `ibridges-0.1.3/docker/irods_client/testdata/sun.rtf`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/tests/conftest.py` & `ibridges-0.1.3/docker/irods_client/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/tests/test_data_ops.py` & `ibridges-0.1.3/docker/irods_client/tests/test_data_ops.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/tests/test_permissions.py` & `ibridges-0.1.3/docker/irods_client/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker/irods_client/tests/test_session.py` & `ibridges-0.1.3/docker/irods_client/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ibridges import Session
 from ibridges.interactive import interactive_auth
 
 def test_session_from_cached_pw(config, irods_env):
     # test only for plain irods
     if config.get("create_session_from_cached_pw", True):
-        session = Session(irods_env_path=config["env_path"])
+        session = Session(config["env_path"])
         assert session.has_valid_irods_session()
         assert ".".join(str(x) for x in session.server_version) == config["server_version"]
         assert session.home == irods_env["irods_home"]
         assert session.default_resc == irods_env["irods_default_resource"]
         assert session.host == irods_env["irods_host"]
         assert session.port == irods_env["irods_port"]
         assert session.username == irods_env["irods_user_name"]
```

### Comparing `ibridges-0.1.2/docker/irods_client/tests/test_sync.py` & `ibridges-0.1.3/docker/irods_client/tests/test_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 
     # upload
     sync_data(session=session,
          source=testdata,
          target=ipath,
          max_level=None,
          dry_run=False,
-         ignore_checksum=False,
-         copy_empty_folders=True,
-         verify_checksum=True)
+         copy_empty_folders=True)
 
     for cur_file in list(testdata.glob("*")):
         s_ipath = IrodsPath(session, "~", "empty", cur_file.name)
         if cur_file.is_file():
             assert s_ipath.dataobject_exists(), "File not uploaded"
             cur_obj=get_dataobject(session=session, path=s_ipath)
             assert _calc_checksum(cur_file)==(cur_obj.checksum
@@ -67,17 +65,15 @@
 
     # download
     sync_data(session=session,
         source=ipath,
         target=tmpdir,
         max_level=None,
         dry_run=False,
-        ignore_checksum=False,
-        copy_empty_folders=True,
-        verify_checksum=True)
+        copy_empty_folders=True)
 
     for cur_file in list(testdata.glob("*")):
         if cur_file.is_file():
             assert (tmpdir / cur_file.name).exists(), "File not downloaded"
             assert _calc_checksum(tmpdir / cur_file.name)== \
                 _calc_checksum(testdata / cur_file.name), "Checksums not identical after download"
         elif cur_file.is_dir():
```

### Comparing `ibridges-0.1.2/docker/irods_client/tests/test_ticket.py` & `ibridges-0.1.3/docker/irods_client/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docker-compose.yml` & `ibridges-0.1.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/Makefile` & `ibridges-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/make.bat` & `ibridges-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/source/api.rst` & `ibridges-0.1.3/docs/source/api.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,36 @@
 
 .. automodule:: ibridges.data_operations
    :members:
    :undoc-members:
    :show-inheritance:
 
 
-ibridges.interactive module
----------------------------
+ibridges.export\_metadata module
+--------------------------------
 
-.. automodule:: ibridges.interactive
+.. automodule:: ibridges.export_metadata
    :members:
    :undoc-members:
    :show-inheritance:
 
 
-ibridges.keywords module
-------------------------
+ibridges.icat\_columns module
+--------------------------------
 
-.. automodule:: ibridges.keywords
+.. automodule:: ibridges.icat_columns
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+
+ibridges.interactive module
+---------------------------
+
+.. automodule:: ibridges.interactive
    :members:
    :undoc-members:
    :show-inheritance:
 
 
 ibridges.meta module
 --------------------
@@ -111,14 +120,14 @@
 
 .. automodule:: ibridges.tickets
    :members:
    :undoc-members:
    :show-inheritance:
 
 
-Module contents
----------------
+.. Module contents
+.. ---------------
 
-.. automodule:: ibridges
-   :members:
-   :undoc-members:
-   :show-inheritance:
+.. .. automodule:: ibridges
+..    :members:
+..    :undoc-members:
+..    :show-inheritance:
```

### Comparing `ibridges-0.1.2/docs/source/conf.py` & `ibridges-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/source/faq.rst` & `ibridges-0.1.3/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/source/index.rst` & `ibridges-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/docs/source/quickstart.rst` & `ibridges-0.1.3/docs/source/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -100,9 +100,9 @@
 
 Closing the session
 -------------------
 When you are done with your session, you should generally close it:
 
 .. code:: python
 
-    del session
+    session.close()
```

### Comparing `ibridges-0.1.2/ibridges/__init__.py` & `ibridges-0.1.3/ibridges/__init__.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/ibridges/data_operations.py` & `ibridges-0.1.3/ibridges/data_operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """Collections and data objects."""
+from __future__ import annotations
+
 import os
 import warnings
 from pathlib import Path
 from typing import Optional, Union
 
 import irods.collection
 import irods.data_object
 import irods.exception
+import irods.keywords as kw
 from irods.models import DataObject
 
-from ibridges import keywords as kw
+import ibridges.icat_columns as icat
 from ibridges.path import IrodsPath
 from ibridges.session import Session
 
+NUM_THREADS = 4
 
 def get_dataobject(session: Session,
                    path: Union[str, IrodsPath]) -> irods.data_object.iRODSDataObject:
     """Instantiate an iRODS data object.
 
     Parameters
     ----------
     session :
         Session with connection to the server to get the data object from.
     path : str
         Name of an iRODS data object.
 
+    Raises
+    ------
+    ValueError:
+        If the path is pointing to a collection and not a data object.
+
     Returns
     -------
     iRODSDataObject
         Instance of the data object with `path`.
 
     """
     path = IrodsPath(session, path)
@@ -36,14 +45,44 @@
         return session.irods_session.data_objects.get(str(path))
     if path.collection_exists():
         raise ValueError("Error retrieving data object, path is linked to a collection."
                          " Use get_collection instead to retrieve the collection.")
 
     raise irods.exception.DataObjectDoesNotExist(path)
 
+def get_collection(session: Session,
+                   path: Union[str, IrodsPath]) -> irods.collection.iRODSCollection:
+    """Instantiate an iRODS collection.
+
+    Parameters
+    ----------
+    session :
+        Session to get the collection from.
+    path : str
+        Name of an iRODS collection.
+
+    Raises
+    ------
+    ValueError:
+        If the path points to a dataobject and not a collection.
+
+    Returns
+    -------
+    iRODSCollection
+        Instance of the collection with `path`.
+
+    """
+    path = IrodsPath(session, path)
+    if path.collection_exists():
+        return session.irods_session.collections.get(str(path))
+    if path.dataobject_exists():
+        raise ValueError("Error retrieving collection, path is linked to a data object."
+                         " Use get_dataobject instead to retrieve the data object.")
+    raise irods.exception.CollectionDoesNotExist(path)
+
 def obj_replicas(obj: irods.data_object.iRODSDataObject) -> list[tuple[int, str, str, int, str]]:
     """Retrieve information about replicas (copies of the file on different resources).
 
     It does so for a data object in the iRODS system.
 
     Parameters
     ----------
@@ -67,39 +106,14 @@
     }
 
     replicas = [(r.number, r.resource_name, r.checksum,
                  r.size, repl_states.get(r.status, r.status)) for r in obj.replicas]
 
     return replicas
 
-def get_collection(session: Session,
-                   path: Union[str, IrodsPath]) -> irods.collection.iRODSCollection:
-    """Instantiate an iRODS collection.
-
-    Parameters
-    ----------
-    session :
-        Session to get the collection from.
-    path : str
-        Name of an iRODS collection.
-
-    Returns
-    -------
-    iRODSCollection
-        Instance of the collection with `path`.
-
-    """
-    path = IrodsPath(session, path)
-    if path.collection_exists():
-        return session.irods_session.collections.get(str(path))
-    if path.dataobject_exists():
-        raise ValueError("Error retrieving collection, path is linked to a data object."
-                         " Use get_dataobject instead to retrieve the data object.")
-    raise irods.exception.CollectionDoesNotExist(path)
-
 def is_dataobject(item) -> bool:
     """Determine if item is an iRODS data object."""
     return isinstance(item, irods.data_object.iRODSDataObject)
 
 def is_collection(item) -> bool:
     """Determine if item is an iRODS collection."""
     return isinstance(item, irods.collection.iRODSCollection)
@@ -135,15 +149,15 @@
                            irods_path / local_path.name).dataobject_exists() \
                  or irods_path.dataobject_exists()
 
     if options is None:
         options = {}
     options.update({
         kw.ALL_KW: '',
-        kw.NUM_THREADS_KW: kw.NUM_THREADS,
+        kw.NUM_THREADS_KW: NUM_THREADS,
         kw.REG_CHKSUM_KW: '',
         kw.VERIFY_CHKSUM_KW: ''
     })
 
     if resc_name not in ['', None]:
         options[kw.RESC_NAME_KW] = resc_name
     if overwrite or not obj_exists:
@@ -171,50 +185,55 @@
     """
     irods_path = IrodsPath(session, irods_path)
     if not irods_path.dataobject_exists():
         raise ValueError("irods_path must be a data object.")
     if options is None:
         options = {}
     options.update({
-        kw.NUM_THREADS_KW: kw.NUM_THREADS,
+        kw.NUM_THREADS_KW: NUM_THREADS,
         kw.VERIFY_CHKSUM_KW: '',
         })
     if overwrite:
         options[kw.FORCE_FLAG_KW] = ''
 
     session.irods_session.data_objects.get(str(irods_path), local_path, **options)
 
-def _create_irods_dest(local_path: Path, irods_path: IrodsPath):
+def _create_irods_dest(local_path: Path, irods_path: IrodsPath
+                       ) -> list[tuple[Path, IrodsPath]]:
     """Assembles the irods destination paths for upload of a folder."""
     upload_path = irods_path.joinpath(local_path.name)
-    paths = [(root.removeprefix(str(local_path)), f)
+    paths = [(str(Path(root).relative_to(local_path)), f)
              for root, _, files in os.walk(local_path) for f in files]
 
     source_to_dest = [(local_path.joinpath(folder.lstrip(os.sep), file_name),
                        upload_path.joinpath(folder.lstrip(os.sep), file_name))
                        for folder, file_name in paths]
 
     return source_to_dest
 
 def _upload_collection(session: Session, local_path: Union[str, Path],
                        irods_path: Union[str, IrodsPath],
-                       overwrite: bool = False, resc_name: str = '',
+                       overwrite: bool = False, ignore_err: bool = False, resc_name: str = '',
                        options: Optional[dict] = None):
     """Upload a local directory to iRODS.
 
     Parameters
     ----------
     session :
         Session to upload the collection to.
     local_path : Path
         Absolute path to the directory to upload
     irods_path : IrodsPath
         Absolute irods destination path
     overwrite : bool
         If data already exists on iRODS, overwrite
+    ignore_err : bool
+        If an error occurs during upload, and ignore_err is set to True, any errors encountered
+        will be transformed into warnings and iBridges will continue to upload the remaining files.
+        By default all errors will stop the process of uploading.
     resc_name : str
         Name of the resource to which data is uploaded, by default the server will decide
     options : dict
         More options for the upload
 
     """
     local_path = Path(local_path)
@@ -225,46 +244,58 @@
 
     source_to_dest = _create_irods_dest(local_path, irods_path)
     for source, dest in source_to_dest:
         _ = create_collection(session, dest.parent)
         try:
             _obj_put(session, source, dest, overwrite, resc_name, options)
         except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
-            warnings.warn(f'Upload: Object already exists\n\tSkipping {source}')
+            warnings.warn(f'Object already exists\tSkipping {source}')
+        except KeyError as e:
+            if ignore_err is True:
+                warnings.warn(f'Upload failed: {source}\n'+repr(e))
+            else:
+                raise ValueError(f'Upload failed: {source}: '+repr(e)) from e
 
-def _create_local_dest(session: Session, irods_path: IrodsPath, local_path: Path):
+def _create_local_dest(session: Session, irods_path: IrodsPath, local_path: Path
+                       ) -> list[tuple[IrodsPath, Path]]:
     """Assembles the local destination paths for download of a collection."""
     # get all data objects
     coll = get_collection(session, irods_path)
     all_objs = _get_data_objects(session, coll)
 
     download_path = local_path.joinpath(irods_path.name.lstrip('/'))
-    source_to_dest = [(IrodsPath(session, subcoll_path, obj_name),
-                      Path(download_path,
-                           subcoll_path.removeprefix(str(irods_path)).lstrip('/'),
-                           obj_name))
-                      for subcoll_path, obj_name, _, _ in all_objs]
-
+    source_to_dest: list[tuple[IrodsPath, Path]] = []
+    for subcoll_path, obj_name, _, _ in all_objs:
+        cur_ipath = IrodsPath(session, subcoll_path, obj_name)
+        cur_lpath = (download_path / IrodsPath(session, subcoll_path).relative_to(irods_path)
+                                   / obj_name)
+        source_to_dest.append((cur_ipath, cur_lpath))
     return source_to_dest
 
 
 def _download_collection(session: Session, irods_path: Union[str, IrodsPath], local_path: Path,
-                         overwrite: bool = False, options: Optional[dict] = None):
+                         overwrite: bool = False, ignore_err: bool = False,
+                         options: Optional[dict] = None):
     """Download a collection to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
     irods_path : IrodsPath
         Absolute irods source path pointing to a collection
     local_path : Path
         Absolute path to the destination directory
     overwrite : bool
         Overwrite existing local data
+    ignore_err : bool
+        If an error occurs during download, and ignore_err is set to True, any errors encountered
+        will be transformed into warnings and iBridges will continue to download the remaining
+        files.
+        By default all errors will stop the process of uploading.
     options : dict
         More options for the download
 
     """
     irods_path = IrodsPath(session, irods_path)
     if not irods_path.collection_exists():
         raise ValueError("irods_path must be a collection.")
@@ -274,73 +305,104 @@
     for source, dest in source_to_dest:
         # ensure local folder exists
         if not dest.parent.is_dir():
             os.makedirs(dest.parent)
         try:
             _obj_get(session, source, dest, overwrite, options)
         except irods.exception.OVERWRITE_WITHOUT_FORCE_FLAG:
-            warnings.warn(f'Download: File already exists\n\tSkipping {source}')
+            warnings.warn(f'File already exists\tSkipping {source}')
+        except KeyError as e:
+            if ignore_err is True:
+                warnings.warn(f'Download failed: {source}i\n'+repr(e))
+            else:
+                raise ValueError(f'Download failed: {source}: '+repr(e)) from e
 
 def upload(session: Session, local_path: Union[str, Path], irods_path: Union[str, IrodsPath],
-           overwrite: bool = False, resc_name: str = '', options: Optional[dict] = None):
+           overwrite: bool = False, ignore_err: bool = False,
+           resc_name: str = '', options: Optional[dict] = None):
     """Upload a local directory or file to iRODS.
 
     Parameters
     ----------
     session :
         Session to upload the data to.
     local_path : Path
         Absolute path to the directory to upload
     irods_path : IrodsPath
         Absolute irods destination path
     overwrite : bool
         If data object or collection already exists on iRODS, overwrite
+    ignore_err : bool
+        If an error occurs during upload, and ignore_err is set to True, any errors encountered
+        will be transformed into warnings and iBridges will continue to upload the remaining files.
+        By default all errors will stop the process of uploading.
     resc_name : str
         Name of the resource to which data is uploaded, by default the server will decide
     options : dict
         More options for the upload
 
+    Raises
+    ------
+    ValueError:
+        If the local_path is not a valid filename of directory.
+    PermissionError:
+        If the iRods server does not allow the collection or data object to be created.
+
     """
     local_path = Path(local_path)
     try:
         if local_path.is_dir():
-            _upload_collection(session, local_path, irods_path, overwrite, resc_name, options)
+            _upload_collection(session, local_path, irods_path, overwrite, ignore_err,
+                               resc_name, options)
         else:
             _obj_put(session, local_path, irods_path, overwrite, resc_name, options)
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise irods.exception.CUT_ACTION_PROCESSED_ERR(
+        raise PermissionError(
             f"During upload operation to '{irods_path}': iRODS server forbids action.") from exc
 
 def download(session: Session, irods_path: Union[str, IrodsPath], local_path: Union[str, Path],
-             overwrite: bool = False, _resc_name: str = '', options: Optional[dict] = None):
+             overwrite: bool = False, ignore_err: bool = False, options: Optional[dict] = None):
     """Download a collection or data object to the local filesystem.
 
     Parameters
     ----------
     session :
         Session to download the collection from.
     irods_path : IrodsPath
         Absolute irods source path pointing to a collection
     local_path : Path
         Absolute path to the destination directory
     overwrite : bool
-        Overwrite existing local data
+        If an error occurs during download, and ignore_err is set to True, any errors encountered
+        will be transformed into warnings and iBridges will continue to download the remaining
+        files.
+        By default all errors will stop the process of downloading.
+    ignore_err : bool
+        Collections: If download of an item fails print error and continue with next item.
     options : dict
         More options for the download
 
+    Raises
+    ------
+    PermissionError:
+        If the iRods server (for whatever reason) forbids downloading the file or
+        (part of the) collection.
+    ValueError:
+        If the irods_path is not pointing to either a collection or a data object.
+
     """
     irods_path = IrodsPath(session, irods_path)
     local_path = Path(local_path)
     try:
         if irods_path.collection_exists():
-            _download_collection(session, irods_path, local_path, overwrite, options)
+            _download_collection(session, irods_path, local_path, overwrite, ignore_err, options)
         else:
             _obj_get(session, irods_path, local_path, overwrite, options)
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise irods.exception.CUT_ACTION_PROCESSED_ERR(
+        raise PermissionError(
             f"During download operation from '{irods_path}': iRODS server forbids action."
             ) from exc
 
 def get_size(session: Session, item: Union[irods.data_object.iRODSDataObject,
                                irods.collection.iRODSCollection]) -> int:
     """Collect the sizes of a data object or a collection.
 
@@ -380,17 +442,17 @@
 
     """
     # all objects in the collection
     objs = [(obj.collection.path, obj.name, obj.size, obj.checksum)
             for obj in coll.data_objects]
 
     # all objects in subcollections
-    data_query = session.irods_session.query(kw.COLL_NAME, kw.DATA_NAME,
+    data_query = session.irods_session.query(icat.COLL_NAME, icat.DATA_NAME,
                                                   DataObject.size, DataObject.checksum)
-    data_query = data_query.filter(kw.LIKE(kw.COLL_NAME, coll.path+"/%"))
+    data_query = data_query.filter(icat.LIKE(icat.COLL_NAME, coll.path+"/%"))
     for res in data_query.get_results():
         path, name, size, checksum = res.values()
         objs.append((path, name, size, checksum))
 
     return objs
 
 def create_collection(session: Session,
@@ -400,14 +462,19 @@
     Parameters
     ----------
     session:
         Session to create the collection for.
     coll_path: IrodsPath
         Collection path
 
+    Raises
+    ------
+    PermissionError:
+        If creating a collection is not allowed by the server.
+
     """
     try:
         return session.irods_session.collections.create(str(coll_path))
     except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-        raise irods.exception.CUT_ACTION_PROCESSED_ERR(
+        raise PermissionError(
                 f"While creating collection at '{coll_path}': iRODS server forbids action."
               ) from exc
```

### Comparing `ibridges-0.1.2/ibridges/interactive.py` & `ibridges-0.1.3/ibridges/interactive.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,33 +11,52 @@
 DEFAULT_IENV_PATH = Path(os.path.expanduser("~")).joinpath(".irods", "irods_environment.json")
 
 def interactive_auth(password: Optional[str] = None,
                      irods_env_path: Union[str, Path] = DEFAULT_IENV_PATH) -> Session:
     """Interactive authentication with iRODS server.
 
     Stores the password in ~/.irods/.irodsA upon success.
+
+    Parameters
+    ----------
+    password:
+        Password to make the connection with. If not supplied, you will be asked interactively.
+    irods_env_path:
+        Path to the irods environment.
+
+    Raises
+    ------
+    FileNotFoundError:
+        If the irods_env_path does not exist.
+    ValueError:
+        If the connection to the iRods server cannot be established.
+
+    Returns
+    -------
+        A connected session to the server.
+
     """
     if not os.path.exists(irods_env_path):
         print(f'File not found: {irods_env_path}')
         raise FileNotFoundError
 
     if os.path.exists(Path(os.path.expanduser("~")).joinpath(".irods", ".irodsA")):
         try:
-            session = Session(irods_env_path=irods_env_path)
+            session = Session(irods_env_path)
             return session
         except IndexError:
             print('INFO: The cached password in ~/.irods/.irodsA has been corrupted')
         except ValueError:
             print('INFO: The cached password in ~/.irods/.irodsA is wrong.')
 
     with open(irods_env_path, "r", encoding="utf-8") as f:
         ienv = json.load(f)
     if password is not None:
         try:
-            session = Session(irods_env=ienv, password=password)
+            session = Session(ienv, password=password)
             session.write_pam_password()
             return session
         except ValueError:
             print('INFO: The provided password is wrong.')
     else:
         n_tries = 0
         success = False
```

### Comparing `ibridges-0.1.2/ibridges/meta.py` & `ibridges-0.1.3/ibridges/meta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """metadata operations."""
-from typing import Iterator, Optional, Sequence, Union
+from __future__ import annotations
+
+from typing import Any, Iterator, Optional, Sequence, Union
 
 import irods.exception
 import irods.meta
 
+from ibridges.data_operations import is_dataobject
+
 
 class MetaData():
     """Irods metadata operations."""
 
     def __init__(self, item):
         """Initialize the metadata object.
 
@@ -48,16 +52,16 @@
         """Return a string showing all metadata entries."""
         # Sort the list of items name -> value -> units, where None is the lowest
         meta_list = list(self)
         meta_list = sorted(meta_list, key=lambda m: (m.units is None, m.units))
         meta_list = sorted(meta_list, key=lambda m: (m.value is None, m.value))
         meta_list = sorted(meta_list, key=lambda m: (m.name is None, m.name))
         meta_str = ""
-        for m in meta_list:
-            meta_str += f" - {{name: {m.name}, value: {m.value}, units: {m.units}}}\n"
+        for meta in meta_list:
+            meta_str += f" - {{name: {meta.name}, value: {meta.value}, units: {meta.units}}}\n"
         return meta_str
 
     def add(self, key: str, value: str, units: Optional[str] = None):
         """Add metadata to an item.
 
         This will never overwrite an existing entry.
 
@@ -66,26 +70,30 @@
         key:
             Key of the new entry to add to the item.
         value:
             Value of the new entry to add to the item.
         units:
             The units of the new entry.
 
-        Throws:
-            CATALOG_ALREADY_HAS_ITEM_BY_THAT_NAME
+        Raises
+        ------
+        ValueError:
+            If the metadata already exists.
+        PermissionError:
+            If the metadata cannot be updated because the user does not have sufficient permissions.
 
         """
         try:
             if (key, value, units) in self:
                 raise irods.exception.CATALOG_ALREADY_HAS_ITEM_BY_THAT_NAME()
             self.item.metadata.add(key, value, units)
         except irods.exception.CATALOG_ALREADY_HAS_ITEM_BY_THAT_NAME as error:
             raise ValueError("ADD META: Metadata already present") from error
         except irods.exception.CAT_NO_ACCESS_PERMISSION as error:
-            raise ValueError("UPDATE META: no permissions") from error
+            raise PermissionError("UPDATE META: no permissions") from error
 
     def set(self, key: str, value: str, units: Optional[str] = None):
         """Set the metadata entry.
 
         If the metadata entry already exists, then all metadata entries with
         the same key will be deleted before adding the new entry. An alternative
         is using the add method to only add to the metadata entries and not
@@ -96,15 +104,18 @@
         key:
             Key of the new entry to add to the item.
         value:
             Value of the new entry to add to the item.
         units:
             The units of the new entry.
 
-        Throws: CAT_NO_ACCESS_PERMISSION
+        Raises
+        ------
+        PermissionError:
+            If the user does not have sufficient permissions to set the metadata.
 
         """
         self.delete(key, None)
         self.add(key, value, units)
 
     def delete(self, key: str, value: Optional[str], units: Optional[str] = None):
         """Delete a metadata entry of an item.
@@ -114,16 +125,20 @@
         key:
             Key of the new entry to add to the item.
         value:
             Value of the new entry to add to the item.
         units:
             The units of the new entry.
 
-        Throws:
-            CAT_SUCCESS_BUT_WITH_NO_INFO: metadata did not exist
+        Raises
+        ------
+        KeyError:
+            If the to be deleted key cannot be found.
+        PermissionError:
+            If the user has insufficient permissions to delete the metadata.
 
         """
         try:
             if value is None:
                 metas = self.item.metadata.get_all(key)
                 value_units = [(m.value, m.units) for m in metas]
                 if (value, units) not in value_units:
@@ -135,10 +150,49 @@
             raise KeyError(f"Cannot delete metadata with key '{key}', value '{value}'"
                              f" and units '{units}' since it does not exist.") from error
         except irods.exception.CAT_NO_ACCESS_PERMISSION as error:
             raise ValueError("Cannot delete metadata due to insufficient permission for "
                              "path '{item.path}'.") from error
 
     def clear(self):
-        """Delete all metadata belonging to the item."""
+        """Delete all metadata belonging to the item.
+
+        Raises
+        ------
+        PermissionError:
+            If the user has insufficient permissions to delete the metadata.
+
+        """
         for meta in self:
             self.item.metadata.remove(meta)
+
+    def to_dict(self, keys: Optional[list] = None) -> dict:
+        """Convert iRODS metadata (AVUs) and system information to a python dictionary.
+
+        {
+            "name": item.name,
+            "irods_id": item.id, #iCAT database ID
+             "checksum": item.checksum if the item is a data object
+             "metadata": [(m.name, m.value, m.units)]
+        }
+
+        Parameters
+        ----------
+        keys:
+            List of Attribute names which should be exported to "metadata".
+            By default all will be exported.
+
+        Returns
+        -------
+            Dictionary containing the metadata.
+
+        """
+        meta_dict: dict[str, Any] = {}
+        meta_dict["name"] = self.item.name
+        meta_dict["irods_id"] = self.item.id
+        if is_dataobject(self.item):
+            meta_dict["checksum"] = self.item.checksum
+        if keys is None:
+            meta_dict["metadata"] = [(m.name, m.value, m.units) for m in self]
+        else:
+            meta_dict["metadata"] = [(m.name, m.value, m.units) for m in self if m.name in keys]
+        return meta_dict
```

### Comparing `ibridges-0.1.2/ibridges/path.py` & `ibridges-0.1.3/ibridges/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,48 +84,60 @@
         -------
             The parent just above the current directory
 
         """
         return IrodsPath(self.session, self._path.parent)
 
     def remove(self):
-        """Remove the data behind an iRODS path."""
+        """Remove the data behind an iRODS path.
+
+        Raises
+        ------
+        PermissionError:
+            If the user has insufficient permission to remove the data.
+
+        """
         try:
             if self.collection_exists():
                 coll = self.session.irods_session.collections.get(str(self))
                 coll.remove()
             elif self.dataobject_exists():
                 obj = self.session.irods_session.data_objects.get(str(self))
                 obj.unlink()
         except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-            raise irods.exception.CUT_ACTION_PROCESSED_ERR(
+            raise PermissionError(
                 f"While removing {self}: iRODS server forbids action.") from exc
 
     @staticmethod
     def create_collection(session,
                           coll_path: Union[IrodsPath, str]) -> irods.collection.iRODSCollection:
         """Create a collection and all collections in its path.
 
         Parameters
         ----------
         session:
             Session for which the collection is created.
         coll_path:
             Irods path to the collection to be created.
 
+        Raises
+        ------
+        PermissionError:
+            If the collection cannot be created due to insufficient permissions.
+
         Returns
         -------
         collection:
             The newly created collection.
 
         """
         try:
             return session.irods_session.collections.create(str(coll_path))
         except irods.exception.CUT_ACTION_PROCESSED_ERR as exc:
-            raise irods.exception.CUT_ACTION_PROCESSED_ERR(
+            raise PermissionError(
                 "While creating collection '{coll_path}': iRODS server forbids action.") from exc
 
     def rename(self):
         """Rename the collection or data object."""
         raise NotImplementedError("Rename not implemented yet.")
 
     def collection_exists(self) -> bool:
@@ -146,7 +158,11 @@
         Parameters
         ----------
         depth : int
             Stops after depth many iterations, even if the tree is deeper.
 
         """
         raise NotImplementedError("Walk method not implemented yet.")
+
+    def relative_to(self, other: IrodsPath) -> PurePosixPath:
+        """Calculate the relative path compared to our path."""
+        return PurePosixPath(self.absolute_path()).relative_to(PurePosixPath(other.absolute_path()))
```

### Comparing `ibridges-0.1.2/ibridges/permissions.py` & `ibridges-0.1.3/ibridges/permissions.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/ibridges/resources.py` & `ibridges-0.1.3/ibridges/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """resource operations."""
+from __future__ import annotations
+
 from typing import Optional
 
 import irods.exception
 import irods.resource
 
-from ibridges import keywords as kw
+from ibridges import icat_columns as icat
 from ibridges.session import Session
 
 
 class Resources():
     """Irods Resource operations."""
 
     def __init__(self, session: Session):
@@ -34,15 +36,16 @@
         Returns
         -------
         iRODSResource
             Instance of the resource with `resc_name`.
 
         Raises
         ------
-            irods.exception.ResourceDoesNotExist
+        irods.exception.ResourceDoesNotExist:
+            If the resource does not exist.
 
         """
         try:
             return self.session.irods_session.resources.get(resc_name)
         except irods.exception.ResourceDoesNotExist as error:
             return {'successful': False, 'reason': repr(error)}
 
@@ -119,15 +122,15 @@
         NOTE: free_space of a resource is the free_space annotated, if
               so annotated, otherwise it is the sum of the free_space of
               all its children.
 
         """
         if self._resources is None or update:
             query = self.session.irods_session.query(
-                kw.RESC_NAME, kw.RESC_PARENT, kw.RESC_STATUS, kw.RESC_CONTEXT)
+                icat.RESC_NAME, icat.RESC_PARENT, icat.RESC_STATUS, icat.RESC_CONTEXT)
             resc_list = []
             for item in query.get_results():
                 name, parent, status, context = item.values()
                 free_space = 0
                 if parent is None:
                     free_space = self.get_free_space(name)
                 metadata = {
```

### Comparing `ibridges-0.1.2/ibridges/rules.py` & `ibridges-0.1.3/ibridges/rules.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/ibridges/search.py` & `ibridges-0.1.3/ibridges/search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Data query."""
+from __future__ import annotations
+
 from typing import Optional, Union
 
-from ibridges import keywords as kw
+from ibridges import icat_columns as icat
 from ibridges.path import IrodsPath
 from ibridges.session import Session
 
 
 def search_data(session: Session, path: Optional[Union[str, IrodsPath]] = None,
            checksum: Optional[str] = None, key_vals: Optional[dict] = None) -> list[dict]:
     """Retrieve all collections and data objects.
@@ -22,14 +24,19 @@
     path: str
         (Partial) path or IrodsPath
     checksum: str
         (Partial) checksum
     key_vals : dict
         Attribute name mapping to values.
 
+    Raises
+    ------
+    ValueError:
+        If no search criterium is supplied.
+
     Returns
     -------
     list: [dict]
         List of dictionaries with keys:
         COLL_NAME (absolute path of the collection),
         DATA_NAME (name of the data object),
         D_DATA_CHECKSUM (checksum of the data object)
@@ -38,30 +45,30 @@
     """
     if path is None and checksum is None and key_vals is None:
         raise ValueError(
                 "QUERY: Error while searching in the metadata: No query criteria set." \
                         + " Please supply either a path, checksum or key_vals.")
 
     # create the query for collections; we only want to return the collection name
-    coll_query = session.irods_session.query(kw.COLL_NAME)
+    coll_query = session.irods_session.query(icat.COLL_NAME)
     # create the query for data objects; we need the collection name, the data name and its checksum
-    data_query = session.irods_session.query(kw.COLL_NAME, kw.DATA_NAME,
-                                             kw.DATA_CHECKSUM)
+    data_query = session.irods_session.query(icat.COLL_NAME, icat.DATA_NAME,
+                                             icat.DATA_CHECKSUM)
     if path:
-        coll_query = coll_query.filter(kw.LIKE(kw.COLL_NAME, str(path)))
-        data_query = data_query.filter(kw.LIKE(kw.COLL_NAME, str(path)))
+        coll_query = coll_query.filter(icat.LIKE(icat.COLL_NAME, str(path)))
+        data_query = data_query.filter(icat.LIKE(icat.COLL_NAME, str(path)))
     if key_vals:
         for key in key_vals:
-            data_query.filter(kw.LIKE(kw.META_DATA_ATTR_NAME, key))
-            coll_query.filter(kw.LIKE(kw.META_COLL_ATTR_NAME, key))
+            data_query.filter(icat.LIKE(icat.META_DATA_ATTR_NAME, key))
+            coll_query.filter(icat.LIKE(icat.META_COLL_ATTR_NAME, key))
             if key_vals[key]:
-                data_query.filter(kw.LIKE(kw.META_DATA_ATTR_VALUE, key_vals[key]))
-                coll_query.filter(kw.LIKE(kw.META_COLL_ATTR_VALUE, key_vals[key]))
+                data_query.filter(icat.LIKE(icat.META_DATA_ATTR_VALUE, key_vals[key]))
+                coll_query.filter(icat.LIKE(icat.META_COLL_ATTR_VALUE, key_vals[key]))
     if checksum:
-        data_query = data_query.filter(kw.LIKE(kw.DATA_CHECKSUM, checksum))
+        data_query = data_query.filter(icat.LIKE(icat.DATA_CHECKSUM, checksum))
     # gather results
     results = list(data_query.get_results())
     if checksum is None:
         coll_res = list(coll_query.get_results())
         if len(coll_res) > 0:
             results.extend(coll_res)
```

### Comparing `ibridges-0.1.2/ibridges/session.py` & `ibridges-0.1.3/ibridges/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,85 @@
 """session operations."""
 import json
-import os
 import warnings
 from pathlib import Path
 from typing import Optional, Union
 
 import irods.session
-from irods.exception import NetworkException
-
-from ibridges.keywords import exceptions
+from irods.exception import (
+    CAT_INVALID_AUTHENTICATION,
+    CAT_INVALID_USER,
+    CAT_PASSWORD_EXPIRED,
+    PAM_AUTH_PASSWORD_FAILED,
+    NetworkException,
+)
+from irods.session import NonAnonymousLoginWithoutPassword, iRODSSession
 
 
 class Session:
     """Irods session authentication."""
 
-    def __init__(self, irods_env: Optional[dict] = None,
-                 irods_env_path: Optional[Union[str, Path]] = None,
-                 password: Optional[str] = None, irods_home: Optional[str] = None):
+    def __init__(self,
+                 irods_env: Union[dict, str, Path],
+                 password: Optional[str] = None,
+                 irods_home: Optional[str] = None):
         """IRODS authentication with Python client.
 
         Parameters
         ----------
         irods_env: dict
-            Dictionary from irods_environment.json
-        irods_env_path:
-            File to read the dictionary from if irods_env is not supplied.
+            Dictionary from irods_environment.json or file to read the
+            dictionary from if irods_env is not supplied.
         password : str
             Plain text password.
         irods_home:
             Override the home directory of irods. Otherwise attempt to retrive the value
             from the irods environment dictionary. If it is not there either, then use
             /{zone}/home/{username}.
 
-        """
-        if irods_env is None and irods_env_path is None:
-            raise ValueError("CONNECTION ERROR: no irods environment given.")
-        if irods_env is not None and irods_env_path is not None:
-            warnings.warn("Environment dictionary will be overwritten with irods environment file")
-        if irods_env_path is not None:
-            if os.path.isfile(irods_env_path):
-                with open(irods_env_path, "r", encoding="utf-8") as f:
-                    irods_env = json.load(f)
-                if not isinstance(irods_env, dict):
-                    raise TypeError(f"Error reading environment file '{irods_env_path}': "
-                                    f"expected dictionary, got {type(irods_env)}.")
-            else:
-                raise ValueError(f"CONNECTION ERROR: {irods_env_path} path does not exist.")
+        Raises
+        ------
+        FileNotFoundError:
+            If the irods_env parameter is interpreted as a file name and not found.
+        TypeError:
+            If the irods_env parameter is not a dict, str or Path.
+        LoginError:
+            If the connection to the iRods server fails to establish.
+
+        """
+        irods_env_path = None
+        if isinstance(irods_env, (str, Path)):
+            irods_env_path = Path(irods_env)
+            if not irods_env_path.is_file():
+                raise FileNotFoundError(f"Cannot find irods environment file '{irods_env}'")
+            with irods_env_path.open("r", encoding="utf-8") as envfd:
+                irods_env = json.load(envfd)
+        if not isinstance(irods_env, dict):
+            raise TypeError(f"Error reading environment file '{irods_env_path}': "
+                            f"expected dictionary, got {type(irods_env)}.")
 
         self._password = password
-        self._irods_env: dict = irods_env  # type: ignore
+        self._irods_env: dict = irods_env
         self._irods_env_path = irods_env_path
-        self._irods_session = self.connect()
+        self.irods_session = self.connect()
         if irods_home is not None:
             self.home = irods_home
         if "irods_home" not in self._irods_env:
             self.home = '/'+self.zone+'/home/'+self.username
 
+    def __enter__(self):
+        """Connect to the iRods server if not already connected."""
+        if not self.has_valid_irods_session():
+            self.connect()
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_trace_back):
+        """Disconnect from the iRods server."""
+        self.close()
+
     @property
     def home(self) -> str:
         """Current working directory for irods.
 
         In the iRods community this is known as 'irods_home', in file system terms
         it would be the current working directory.
 
@@ -70,62 +90,32 @@
         """
         return self._irods_env["irods_home"]
 
     @home.setter
     def home(self, value):
         self._irods_env["irods_home"] = value
 
-    def __del__(self):
-        """Clean up the irods session as well."""
-        del self.irods_session
-
-    @property
-    def irods_session(self) -> irods.session.iRODSSession:
-        """IRODS session creation.
-
-        Returns
-        -------
-        iRODSSession
-            iRODS connection based on the current environment and password.
-
-        """
-        return self._irods_session
-
-    @irods_session.deleter
-    def irods_session(self):
-        """Properly delete iRODS session."""
-        if self._irods_session is not None:
-            # In case the iRODS session is not fully there.
-            try:
-                self._irods_session.cleanup()
-            except NameError:
-                pass
-            except AttributeError:
-                pass
-            del self._irods_session
-            self._irods_session = None
-
     # Authentication workflow methods
     def has_valid_irods_session(self) -> bool:
         """Check if the iRODS session is valid.
 
         Returns
         -------
         bool
             Is the session valid?
 
         """
-        return self.server_version != ()
+        return self.irods_session is not None and self.server_version != ()
 
-    def connect(self):
+    def connect(self) -> iRODSSession:
         """Establish an iRODS session."""
         user = self._irods_env.get('irods_user_name', '')
         if user == 'anonymous':
             # TODOx: implement and test for SSL enabled iRODS
-            # self._irods_session = iRODSSession(user='anonymous',
+            # self.irods_session = iRODSSession(user='anonymous',
             #                        password='',
             #                        zone=zone,
             #                        port=1247,
             #                        host=host)
             raise NotImplementedError
         # authentication with irods environment and password
         if self._password is None or self._password == '':
@@ -133,56 +123,58 @@
             print("Auth without password")
             return self.authenticate_using_auth_file()
 
         # irods environment and given password
         print("Auth with password")
         return self.authenticate_using_password()
 
-    def authenticate_using_password(self):
+    def close(self) -> None:
+        """Disconnect the irods session.
+
+        This closes the connection, and makes the session available for
+        reconnection with `connect`.
+        """
+        if self.irods_session is not None:
+            self.irods_session.do_configure = {}
+            self.irods_session.cleanup()
+            self.irods_session = None
+
+    def authenticate_using_password(self) -> iRODSSession:
         """Authenticate with the iRods server using a password."""
         try:
-            self._irods_session = irods.session.iRODSSession(password=self._password,
+            irods_session = irods.session.iRODSSession(password=self._password,
                                                              **self._irods_env)
-            assert self._irods_session.server_version != ()
-            return self._irods_session
-        except ValueError as e:
-            raise ValueError("Unexpected value in irods_environment.json; ") from e
-        except NetworkException as e:
-            raise ValueError(
-                "Host, port, irods_client_server_policy or irods_client_server_negotiation not set"
-                " correctly in irods_environment.json; ") from e
+            _ = irods_session.server_version
         except Exception as e:
-            if repr(e) in exceptions:
-                raise ValueError(exceptions[repr(e)]+"; ") from e
-            raise e
+            raise _translate_irods_error(e) from e
+        if irods_session.server_version == ():
+            raise LoginError("iRodsServer does not return a server version.")
+        return irods_session
 
-    def authenticate_using_auth_file(self):
+    def authenticate_using_auth_file(self) -> iRODSSession:
         """Authenticate with an authentication file."""
         try:
-            self._irods_session = irods.session.iRODSSession(
-                    irods_env_file=self._irods_env_path)
-            assert self._irods_session.server_version != ()
-            return self._irods_session
-        except ValueError as e:
-            raise ValueError("Unexpected value in irods_environment.json; ") from e
-        except NetworkException as e:
-            raise ValueError(
-                "Host, port or irods_client_server_negotiation not set correctly in "
-                "irods_environment.json; ") from e
+            irods_session = irods.session.iRODSSession(
+                irods_env_file=self._irods_env_path)
+            _ = irods_session.server_version
+        except NonAnonymousLoginWithoutPassword as e:
+            raise ValueError("No cached password found.") from e
         except Exception as e:
-            if repr(e) in exceptions:
-                raise ValueError(exceptions[repr(e)]+"; "+repr(e)) from e
-            raise e
+            raise _translate_irods_error(e) from e
+        if irods_session.server_version == ():
+            raise LoginError("iRodsServer does not return a server version.")
+        return irods_session
+
 
     def write_pam_password(self):
         """Store the password in the iRODS authentication file in obfuscated form."""
-        connection = self._irods_session.pool.get_connection()
-        pam_passwords = self._irods_session.pam_pw_negotiated
+        connection = self.irods_session.pool.get_connection()
+        pam_passwords = self.irods_session.pam_pw_negotiated
         if len(pam_passwords):
-            irods_auth_file = self._irods_session.get_irods_password_file()
+            irods_auth_file = self.irods_session.get_irods_password_file()
             with open(irods_auth_file, 'w', encoding='utf-8') as authfd:
                 authfd.write(
                     irods.password_obfuscation.encode(pam_passwords[0]))
         else:
             warnings.warn('WARNING -- unable to cache obfuscated password locally')
         connection.release()
 
@@ -192,86 +184,60 @@
 
         Returns
         -------
         str
             Resource name.
 
         """
-        if self._irods_session:
+        if self.irods_session:
             try:
-                return self._irods_session.default_resource
+                return self.irods_session.default_resource
             except AttributeError:
                 pass
         raise ValueError("'irods_default_resource' not set in iRODS configuration.")
 
-    @property
-    def host(self) -> str:
-        """Retrieve hostname of the iRODS server.
-
-        Returns
-        -------
-        str
-            Hostname.
-
-        """
-        if self._irods_session:
-            return self._irods_session.host
-        return ''
-
-    @property
-    def port(self) -> str:
-        """Retrieve port of the iRODS server.
-
-        Returns
-        -------
-        str
-            Port.
-
-        """
-        if self._irods_session:
-            return self._irods_session.port
-        return ''
+    def __getattr__(self, item):
+        """Pass through a few attributes from irods_session."""
+        if item in ["host", "port", "username", "zone"]:
+            if self.irods_session is None:
+                raise AttributeError("Need a valid iRods session to get '{item}'.")
+            return getattr(self.irods_session, item)
+        return super().__getattribute__(item)
 
     @property
     def server_version(self) -> tuple:
         """Retrieve version of the iRODS server.
 
         Returns
         -------
         tuple
             Server version: (major, minor, patch).
 
         """
         try:
-            return self._irods_session.server_version
+            return self.irods_session.server_version
         except Exception as e:
-            if repr(e) in exceptions:
-                raise ValueError(exceptions[repr(e)]) from e
-            raise e
+            raise _translate_irods_error(e) from e
 
-    @property
-    def username(self) -> str:
-        """Retrieve username.
 
-        Returns
-        -------
-        str
-            Username.
+class LoginError(ValueError):
+    """Error indicating a failure to log into the iRods server."""
 
-        """
-        if self._irods_session:
-            return self._irods_session.username
-        return ''
 
-    @property
-    def zone(self) -> str:
-        """Retrieve the zone name.
 
-        Returns
-        -------
-        str
-            Zone.
-
-        """
-        if self._irods_session:
-            return self._irods_session.zone
-        return ''
+def _translate_irods_error(exc) -> Exception:  # pylint: disable=too-many-return-statements
+    if isinstance(exc, NetworkException) and exc.msg.startswith(
+            'Client-Server negotiation failure'):
+        return LoginError("Host, port, irods_client_server_policy or "
+                          "irods_client_server_negotiation not set correctly in "
+                          "irods_environment.json")
+    if isinstance(exc, CAT_INVALID_USER):
+        return LoginError("User credentials are not accepted")
+    if isinstance(exc, PAM_AUTH_PASSWORD_FAILED):
+        return LoginError("Wrong password")
+    if isinstance(exc, CAT_PASSWORD_EXPIRED):
+        return LoginError("Cached password is expired")
+    if isinstance(exc, CAT_INVALID_AUTHENTICATION):
+        return LoginError("Cached password is wrong")
+    if isinstance(exc, ValueError):
+        return LoginError("Unexpected value in irods_environment; ")
+    return LoginError("Unknown problem creating irods session.")
```

### Comparing `ibridges-0.1.2/ibridges/sync.py` & `ibridges-0.1.3/ibridges/sync.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 class FileObject(NamedTuple):
     """Object to hold attributes from local and remote files."""
 
     name: str
     path: str
     size: int
-    checksum: Optional[str]
+    checksum: str
 
 class FolderObject:
     """Object to hold attributes from local and remote folders/collections."""
 
     def __init__(self,
                  path: str = '',
                  n_files: int = 0,
@@ -80,30 +80,31 @@
 
         return self.path==other.path
 
     def __hash__(self):
         """Hash the path as a hash for the folder."""
         return hash(self.path)
 
-def sync_data(session: Session,   #pylint: disable=too-many-arguments
+def sync_data(session: Session,
          source: Union[str, Path, IrodsPath],
          target: Union[str, Path, IrodsPath],
          max_level: Optional[int] = None,
          dry_run: bool = False,
-         ignore_checksum: bool = False,
-         copy_empty_folders: bool = False,
-         verify_checksum: bool = True,
-         on_checksum_fail: str = 'error') -> None:
+         ignore_err: bool = False,
+         copy_empty_folders: bool = False) -> dict:
     """Synchronize the data between a local copy (local file system) and the copy stored in iRODS.
 
     The command can be in one of the two modes: synchronization of data from the client's local file
     system to iRODS, or from iRODS to the local file system. The mode is determined by the type of
     the values for `source` and `target` (IrodsPath or str/Path).
 
+    The command considers the file size and the checksum to determine whether a file should be
+    synchronized.
 
+    
     Parameters
     ----------
     session : ibridges.Session
         An authorized iBridges session.
     source : str or Path or IrodsPath
         Existing local folder or iRODS collection. An exception will be raised if it doesn't exist.
     target : str or Path or IrodsPath
@@ -112,61 +113,55 @@
         Controls the depth up to which the file tree will be synchronized. A max level of 1
         synchronizes only the source's root, max level 2 also includes the first set of
         subfolders/subcollections and their contents, etc. Set to None, there is no limit
         (full recursive synchronization).
     dry_run : bool, default False
         List all source files and folders that need to be synchronized without actually
         performing synchronization.
-    ignore_checksum : bool, default False
-        If set to True, only the file size is used for determining whether synchronization is
-        needed, rather than size and checksum value. This mode gives a potentially faster
-        operation but the result is less accurate.
+    ignore_err : If an error occurs during the transfer, and ignore_err is set to True, 
+        any errors encountered will be transformed into warnings and iBridges will continue
+        to transfer the remaining files.
     copy_empty_folders : bool, default False
         Controls whether folders/collections that contain no files or  subfolders/subcollections
         will be synchronized.
-    verify_checksum : bool, default True
-        Calculate and verify the checksum on files after up- or downloading. A checksum mismatch
-        will generate an error, but will not abort the  synchronization process.
-    on_checksum_fail : {'warn', 'error'}
-        Behaviour when a checksum verification fails. 'warn' prints an error and procedes; 'error'
-        terminates the program with an exception (default). To ignore checksum verification errors,
-        set `verify_checksum` to False.
 
+
+    Returns
+    -------
+        A dict object containing two keys: 'changed_folders' and 'changed_files'.
+        These contain lists of changed folders and files, respectively
+        (or of to-be-changed folders and files, when in dry-run mode).
     """
-    _param_checks(source, target, on_checksum_fail)
+    _param_checks(source, target)
 
     if isinstance(source, IrodsPath):
         if not source.collection_exists():
             raise ValueError(f"Source collection '{source.absolute_path()}' does not exist")
         src_files, src_folders=_get_irods_tree(
             coll=get_collection(session=session, path=source),
-            max_level=max_level,
-            ignore_checksum=ignore_checksum)
+            max_level=max_level)
     else:
         if not Path(source).is_dir():
             raise ValueError(f"Source folder '{source}' does not exist")
         src_files, src_folders=_get_local_tree(
             path=Path(source),
-            max_level=max_level,
-            ignore_checksum=ignore_checksum)
+            max_level=max_level)
 
     if isinstance(target, IrodsPath):
         if not target.collection_exists():
             raise ValueError(f"Target collection '{target.absolute_path()}' does not exist")
         tgt_files, tgt_folders=_get_irods_tree(
             coll=get_collection(session=session, path=target),
-            max_level=max_level,
-            ignore_checksum=ignore_checksum)
+            max_level=max_level)
     else:
         if not Path(target).is_dir():
             raise ValueError(f"Target folder '{target}' does not exist")
         tgt_files, tgt_folders=_get_local_tree(
             path=Path(target),
-            max_level=max_level,
-            ignore_checksum=ignore_checksum)
+            max_level=max_level)
 
     folders_diff=sorted(
         set(src_folders).difference(set(tgt_folders)),
         key=lambda x: (x.path.count('/'), x.path))
 
     files_diff=sorted(
         set(src_files).difference(set(tgt_files)),
@@ -181,53 +176,47 @@
             copy_empty_folders=copy_empty_folders)
         _copy_local_to_irods(
             session=session,
             source=Path(source),
             target=target,
             files=files_diff,
             dry_run=dry_run,
-            verify_checksum=verify_checksum,
-            on_checksum_fail=on_checksum_fail)
+            ignore_err=ignore_err)
     else:
         _create_local_folders(
             target=Path(target),
             folders=folders_diff,
             dry_run=dry_run,
             copy_empty_folders=copy_empty_folders)
         _copy_irods_to_local(
             session=session,
             source=source,  # type: ignore
             target=Path(target),
             objects=files_diff,
             dry_run=dry_run,
-            verify_checksum=verify_checksum,
-            on_checksum_fail=on_checksum_fail)
+            ignore_err=ignore_err)
+    return {'changed_folders': folders_diff, 'changed_files': files_diff}
 
-def _param_checks(source, target, on_checksum_fail):
+def _param_checks(source, target):
     if not isinstance(source, IrodsPath) and not isinstance(target, IrodsPath):
         raise TypeError("Either source or target should be an iRODS path.")
 
     if isinstance(source, IrodsPath) and isinstance(target, IrodsPath):
         raise TypeError("iRODS to iRODS copying is not supported.")
 
-    fail_opt=["warn", "error"]
-    if on_checksum_fail not in fail_opt:
-        raise TypeError(f"on_checksum_fail must be on of: {', '.join(fail_opt)}")
-
 def _calc_checksum(filepath):
     f_hash=sha256()
     memv=memoryview(bytearray(128*1024))
     with open(filepath, 'rb', buffering=0) as file:
         for item in iter(lambda : file.readinto(memv), 0):
             f_hash.update(memv[:item])
     return f"sha2:{str(base64.b64encode(f_hash.digest()), encoding='utf-8')}"
 
 def _get_local_tree(path: Path,
-                    max_level: Optional[int] = None,
-                    ignore_checksum: bool = False):
+                    max_level: Optional[int] = None):
 
     # change all sep into /, regardless of platform, for easier comparison
     def fix_local_path(path: str):
         return "/".join(path.split(os.sep))
 
     objects=[]
     collections=[]
@@ -237,55 +226,52 @@
             full_path=Path(root) / file
             rel_path=str(full_path)[len(str(path)):].lstrip(os.sep)
             if max_level is None or rel_path.count(os.sep)<max_level:
                 objects.append(FileObject(
                     name=file,
                     path=fix_local_path(rel_path),
                     size=full_path.stat().st_size,
-                    checksum=None if ignore_checksum else _calc_checksum(full_path)))
+                    checksum=_calc_checksum(full_path)))
 
         collections.extend([FolderObject(
                 fix_local_path(str(Path(root) / dir)[len(str(path)):].lstrip(os.sep)),
                 len([x for x in Path(f"{root}{os.sep}{dir}").iterdir() if x.is_file()]),
                 len([x for x in Path(f"{root}{os.sep}{dir}").iterdir() if x.is_dir()])
             )
             for dir in dirs if max_level is None or dir.count(os.sep)<max_level-1])
 
     return objects, collections
 
 def _get_irods_tree(coll: iRODSCollection,
                     root: str = '',
                     level: int = 0,
-                    max_level: Optional[int] = None,
-                    ignore_checksum: bool = False):
+                    max_level: Optional[int] = None):
 
     root=coll.path if len(root)==0 else root
 
     # chksum() (re)calculates checksum, call only when checksum is empty
     objects=[FileObject(
         x.name,
         x.path[len(root):].lstrip('/'),
         x.size,
-        None if ignore_checksum else (x.checksum if len(x.checksum)>0 else x.chksum()))
+        x.checksum if x.checksum is not None and len(x.checksum)>0 else x.chksum())
         for x in coll.data_objects]
 
     if max_level is None or level<max_level-1:
         collections=[FolderObject(
             x.path[len(root):].lstrip('/'),
             len(x.data_objects),
             len(x.subcollections)) for x in coll.subcollections]
 
         for subcoll in coll.subcollections:
             subobjects, subcollections=_get_irods_tree(
                 coll=subcoll,
                 root=root,
                 level=level+1,
-                max_level=max_level,
-                ignore_checksum=ignore_checksum
-                )
+                max_level=max_level)
             objects.extend(subobjects)
             collections.extend(subcollections)
     else:
         collections=[]
 
     return objects, collections
 
@@ -310,73 +296,71 @@
     if dry_run:
         print("Will create folder(s):")
         print(*[f"  {x}" for x in new_folders], sep='\n')
         return
     for folder in new_folders:
         folder.mkdir(parents=True, exist_ok=True)
 
-def _copy_local_to_irods(session: Session,   #pylint: disable=too-many-arguments
+def _copy_local_to_irods(session: Session,
                          source: Path,
                          target: IrodsPath,
                          files: list[FileObject],
                          dry_run: bool,
-                         verify_checksum: bool,
-                         on_checksum_fail: str) -> None:
+                         ignore_err: bool) -> None:
     if dry_run:
         print(f"Will upload from '{source}' to '{target}':")
         print(*[f"  {x.path}  {x.size}" for x in files], sep='\n')
         return
 
+    if len(files)==0:
+        return
+
     pbar=tqdm(desc='Uploading', total=sum(x.size for x in files))
     for file in files:
         source_path=Path(source) / file.path
         target_path=str(target / file.path)
         try:
             upload(session=session,
                     local_path=source_path,
                     irods_path=target_path,
-                    overwrite=True)
-            if verify_checksum:
-                obj=get_dataobject(session, target_path)
-                if file.checksum != \
-                        (obj.checksum if len(obj.checksum)>0 else obj.chksum()):
-                    msg=f"Checksum mismatch after upload: '{target_path}'"
-                    if on_checksum_fail=='error':
-                        raise ValueError(msg)
-                    if on_checksum_fail=='warn':
-                        print(f"WARNING: {msg}")
+                    overwrite=True,
+                    ignore_err=ignore_err)
+            obj=get_dataobject(session, target_path)
+            if file.checksum != \
+                    (obj.checksum if obj.checksum is not None and len(obj.checksum)>0
+                     else obj.chksum()):
+                raise ValueError(f"Checksum mismatch after upload: '{target_path}'")
 
             pbar.update(file.size)
         except Exception as err:
             raise ValueError(f"Uploading '{source_path}' failed: {repr(err)}") from err
 
-def _copy_irods_to_local(session: Session,     #pylint: disable=too-many-arguments
+def _copy_irods_to_local(session: Session,
                          source: IrodsPath,
                          target: Path,
                          objects: list[FileObject],
                          dry_run: bool,
-                         verify_checksum: bool,
-                         on_checksum_fail: str) -> None:
+                         ignore_err: bool) -> None:
     if dry_run:
         print(f"Will download from '{source}' to '{target}':")
         print(*[f"  {x.path}  {x.size}" for x in objects], sep='\n')
         return
 
+    if len(objects)==0:
+        return
+
     pbar=tqdm(desc='Downloading', total=sum(x.size for x in objects))
     for obj in objects:
         target_path=Path(target) / obj.path
         source_path=str(source / obj.path)
         try:
             download(session=session,
                         irods_path=source_path,
                         local_path=target_path,
-                        overwrite=True)
-            if verify_checksum and obj.checksum != _calc_checksum(target_path):
-                msg=f"Checksum mismatch after download: '{source_path}'"
-                if on_checksum_fail=='error':
-                    raise ValueError(msg)
-                if on_checksum_fail=='warn':
-                    print(f"WARNING: {msg}")
+                        overwrite=True,
+                        ignore_err=ignore_err)
+            if obj.checksum != _calc_checksum(target_path):
+                raise ValueError(f"Checksum mismatch after download: '{source_path}'")
 
             pbar.update(obj.size)
         except Exception as err:
             raise ValueError(f"Downloading '{source_path}' failed: {repr(err)}") from err
```

### Comparing `ibridges-0.1.2/ibridges/tickets.py` & `ibridges-0.1.3/ibridges/tickets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Ticket operations."""
+from __future__ import annotations
+
 from collections import namedtuple
 from datetime import date, datetime
 from typing import Iterable, Optional, Union
 
 import irods.ticket
 from irods.models import TicketQuery
 
-import ibridges.keywords as kw
+import ibridges.icat_columns as icat
 from ibridges.session import Session
 
 TicketData = namedtuple('TicketData', ["name", "type", "path", "expiration_date"])
 
 class Tickets():
     """Irods Ticket operations."""
 
@@ -23,28 +25,35 @@
             instance of the Session class
 
         """
         self.session = session
         self._all_tickets = self.update_tickets()
 
     def create_ticket(self, obj_path: str,
-                      ticket_type: Optional[str] = 'read',
+                      ticket_type: str = 'read',
                       expiry_date: Optional[Union[str, datetime, date]] = None) -> tuple:
         """Create an iRODS ticket.
 
         This allows read access to the object referenced by `obj_path`.
 
         Parameters
         ----------
-        obj_path : str
+        obj_path:
             Collection or data object path to create a ticket for.
-        ticket_type: str
+        ticket_type, optional:
             read or write, default read
-        expiry_date : str
-            Optional expiration date in the form: strftime('%Y-%m-%d.%H:%M:%S')
+        expiry_date, optional:
+            Expiration date as a datetime, date or string in the form strftime('%Y-%m-%d.%H:%M:%S').
+
+        Raises
+        ------
+        TypeError:
+            If the expiry_date has the wrong type.
+        ValueError:
+            If the expiration date cannot be set for whatever reason.
 
         Returns
         -------
         tuple
             Name of ticket and if expiration string successfully set:
             (str, bool)
 
@@ -54,15 +63,15 @@
         expiration_set = False
         if expiry_date is not None:
             if isinstance(expiry_date, date):
                 expiry_date = datetime.combine(expiry_date, datetime.min.time())
             if isinstance(expiry_date, datetime):
                 expiry_date = expiry_date.strftime('%Y-%m-%d.%H:%M:%S')
             if not isinstance(expiry_date, str):
-                raise ValueError("Expecting datetime, date or string type for 'expiry_date' "
+                raise TypeError("Expecting datetime, date or string type for 'expiry_date' "
                                  f"argument, got {type(expiry_date)}")
             try:
                 expiration_set = ticket.modify('expire', expiry_date) == ticket
             except Exception as error:
                 self.delete_ticket(ticket)
                 raise ValueError('Could not set expiration date') from error
         self.update_tickets()
@@ -73,23 +82,56 @@
         yield from self.update_tickets()
 
     @property
     def all_ticket_strings(self) -> list[str]:
         """Get the names of all tickets."""
         return [tick_data.name for tick_data in self._all_tickets]
 
-    def get_ticket(self, ticket_str: str) -> Optional[irods.ticket.Ticket]:
-        """Obtain a ticket using its string identifier."""
+    def get_ticket(self, ticket_str: str) -> irods.ticket.Ticket:
+        """Obtain a ticket using its string identifier.
+
+        Parameters
+        ----------
+        ticket_str:
+            Unique string identifier with which the ticket can be retrieved.
+
+        Raises
+        ------
+        KeyError:
+            If the ticket cannot be found.
+
+        Returns
+        -------
+            Ticket with the correct identifier.
+
+        """
         if ticket_str in self.all_ticket_strings:
             return irods.ticket.Ticket(self.session.irods_session, ticket=ticket_str)
         raise KeyError(f"Cannot obtain ticket: ticket with ticket_str '{ticket_str}' "
                        "does not exist.")
 
-    def delete_ticket(self, ticket: irods.ticket.Ticket, check: bool = False):
-        """Delete irods ticket."""
+    def delete_ticket(self, ticket: Union[str, irods.ticket.Ticket],
+                      check: bool = False):
+        """Delete irods ticket.
+
+        Parameters
+        ----------
+        ticket:
+            Ticket or ticket string identifier to be deleted.
+        check:
+            Whether to check whether the ticket actually exists.
+
+        Raises
+        ------
+        KeyError:
+            If check == True and the ticket does not exist.
+
+        """
+        if isinstance(ticket, str):
+            ticket = self.get_ticket(ticket)
         if ticket.string in self.all_ticket_strings:
             ticket.delete()
             self.update_tickets()
         elif check:
             raise KeyError(f"Cannot delete ticket: ticket '{ticket}' does not exist (anymore).")
 
     def update_tickets(self) -> list[TicketData]:
@@ -117,16 +159,15 @@
                            datetime.fromtimestamp(int(row[TicketQuery.Ticket.expiry_ts]))
                 ))
         return self._all_tickets
 
     def clear(self):
         """Delete all tickets."""
         for tick_data in self.update_tickets():
-            tick = self.get_ticket(tick_data.name)
-            self.delete_ticket(tick)
+            self.delete_ticket(tick_data.name)
         self.update_tickets()
 
     def _id_to_path(self, itemid: str) -> str:
         """Get IRODS path from a given an iRODS item id.
 
         The item (data object or collection) id should come from the
         TicketQuery.Ticket.object_id.
@@ -140,19 +181,19 @@
         Returns
         -------
         str
             collection or data object path
             returns '' if the identifier does not exist any longer
 
         """
-        data_query = self.session.irods_session.query(kw.COLL_NAME, kw.DATA_NAME)
-        data_query = data_query.filter(kw.DATA_ID == itemid)
+        data_query = self.session.irods_session.query(icat.COLL_NAME, icat.DATA_NAME)
+        data_query = data_query.filter(icat.DATA_ID == itemid)
 
         if len(list(data_query)) > 0:
             res = next(data_query.get_results())
             return list(res.values())[0] + "/" + list(res.values())[1]
-        coll_query = self.session.irods_session.query(kw.COLL_NAME)
-        coll_query = coll_query.filter(kw.COLL_ID == itemid)
+        coll_query = self.session.irods_session.query(icat.COLL_NAME)
+        coll_query = coll_query.filter(icat.COLL_ID == itemid)
         if len(list(coll_query)) > 0:
             res = next(coll_query.get_results())
             return list(res.values())[0]
         return ''
```

### Comparing `ibridges-0.1.2/ibridges.egg-info/PKG-INFO` & `ibridges-0.1.3/ibridges.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6962 7269  : 2.1.Name: ibri
 00000020: 6467 6573 0a56 6572 7369 6f6e 3a20 302e  dges.Version: 0.
-00000030: 312e 320a 5375 6d6d 6172 793a 2050 6163  1.2.Summary: Pac
+00000030: 312e 330a 5375 6d6d 6172 793a 2050 6163  1.3.Summary: Pac
 00000040: 6b61 6765 2066 6f72 2061 6363 6573 7369  kage for accessi
 00000050: 6e67 2064 6174 6120 616e 6420 6d65 7461  ng data and meta
 00000060: 6461 7461 206f 6e20 6952 6f64 7320 7365  data on iRods se
 00000070: 7276 6572 732e 0a41 7574 686f 722d 656d  rvers..Author-em
 00000080: 6169 6c3a 2043 6872 6973 7469 6e65 2053  ail: Christine S
 00000090: 7461 6967 6572 203c 632e 7374 6169 6765  taiger <c.staige
 000000a0: 7240 7575 2e6e 6c3e 0a4c 6963 656e 7365  r@uu.nl>.License
@@ -160,234 +160,287 @@
 000009f0: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
 00000a00: 7068 696e 785f 696e 6c69 6e65 5f74 6162  phinx_inline_tab
 00000a10: 733b 2065 7874 7261 203d 3d20 2274 6573  s; extra == "tes
 00000a20: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
 00000a30: 3a20 7370 6869 6e78 5f63 6f70 7962 7574  : sphinx_copybut
 00000a40: 746f 6e3b 2065 7874 7261 203d 3d20 2274  ton; extra == "t
 00000a50: 6573 7422 0a0a 2320 6942 7269 6467 6573  est"..# iBridges
-00000a60: 0a5b 215b 5d28 6874 7470 733a 2f2f 6769  .[![](https://gi
-00000a70: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
-00000a80: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
-00000a90: 6765 732f 6163 7469 6f6e 732f 776f 726b  ges/actions/work
-00000aa0: 666c 6f77 732f 696e 7465 6772 6174 696f  flows/integratio
-00000ab0: 6e2d 7465 7374 732d 6972 6f64 732e 796d  n-tests-irods.ym
-00000ac0: 6c2f 6261 6467 652e 7376 673f 6272 616e  l/badge.svg?bran
-00000ad0: 6368 3d64 6576 656c 6f70 295d 2868 7474  ch=develop)](htt
-00000ae0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000af0: 5574 7265 6368 7455 6e69 7665 7273 6974  UtrechtUniversit
-00000b00: 792f 6942 7269 6467 6573 2f61 6374 696f  y/iBridges/actio
-00000b10: 6e73 2f77 6f72 6b66 6c6f 7773 2f69 6e74  ns/workflows/int
-00000b20: 6567 7261 7469 6f6e 2d74 6573 7473 2d69  egration-tests-i
-00000b30: 726f 6473 2e79 6d6c 2920 5b21 5b5d 2868  rods.yml) [![](h
-00000b40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b50: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
-00000b60: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
-00000b70: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6d  ions/workflows/m
-00000b80: 6169 6e2e 796d 6c2f 6261 6467 652e 7376  ain.yml/badge.sv
-00000b90: 673f 6272 616e 6368 3d64 6576 656c 6f70  g?branch=develop
-00000ba0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000bb0: 622e 636f 6d2f 5574 7265 6368 7455 6e69  b.com/UtrechtUni
-00000bc0: 7665 7273 6974 792f 6942 7269 6467 6573  versity/iBridges
-00000bd0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000be0: 7773 2f6d 6169 6e2e 796d 6c29 200a 5b21  ws/main.yml) .[!
-00000bf0: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
-00000c00: 622e 636f 6d2f 5574 7265 6368 7455 6e69  b.com/UtrechtUni
-00000c10: 7665 7273 6974 792f 6942 7269 6467 6573  versity/iBridges
-00000c20: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000c30: 7773 2f69 6e74 6567 7261 7469 6f6e 2d74  ws/integration-t
-00000c40: 6573 7473 2d79 6f64 612e 796d 6c2f 6261  ests-yoda.yml/ba
-00000c50: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00000c60: 2f2f 6769 7468 7562 2e63 6f6d 2f55 7472  //github.com/Utr
-00000c70: 6563 6874 556e 6976 6572 7369 7479 2f69  echtUniversity/i
-00000c80: 4272 6964 6765 732f 6163 7469 6f6e 732f  Bridges/actions/
-00000c90: 776f 726b 666c 6f77 732f 696e 7465 6772  workflows/integr
-00000ca0: 6174 696f 6e2d 7465 7374 732d 796f 6461  ation-tests-yoda
-00000cb0: 2e79 6d6c 2920 215b 5d28 6874 7470 733a  .yml) ![](https:
-00000cc0: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
-00000cd0: 672f 7072 6f6a 6563 7473 2f69 6272 6964  g/projects/ibrid
-00000ce0: 6765 732f 6261 6467 652f 3f76 6572 7369  ges/badge/?versi
-00000cf0: 6f6e 3d6c 6174 6573 7426 7374 796c 653d  on=latest&style=
-00000d00: 666c 6174 2d64 6566 6175 6c74 290a 0a23  flat-default)..#
-00000d10: 2320 4162 6f75 740a 0a69 4272 6964 6765  # About..iBridge
-00000d20: 7320 6973 206c 6962 7261 7279 2066 6f72  s is library for
-00000d30: 2073 6369 656e 7469 6669 6320 7072 6f67   scientific prog
-00000d40: 7261 6d6d 6572 7320 7768 6f20 6172 6520  rammers who are 
-00000d50: 776f 726b 696e 6720 7769 7468 2064 6174  working with dat
-00000d60: 6120 696e 2069 524f 4453 2e20 5765 2070  a in iRODS. We p
-00000d70: 726f 7669 6465 2061 2077 7261 7070 6572  rovide a wrapper
-00000d80: 2061 726f 756e 6420 7468 6520 5b70 7974   around the [pyt
-00000d90: 686f 6e2d 6972 6f64 7363 6c69 656e 745d  hon-irodsclient]
-00000da0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00000db0: 672f 7072 6f6a 6563 742f 7079 7468 6f6e  g/project/python
-00000dc0: 2d69 726f 6473 636c 6965 6e74 2f29 2074  -irodsclient/) t
-00000dd0: 6f20 6661 6369 6c69 7461 7465 2065 6173  o facilitate eas
-00000de0: 7920 696e 7465 7261 6374 696f 6e20 7769  y interaction wi
-00000df0: 7468 2074 6865 2069 524f 4453 2073 6572  th the iRODS ser
-00000e00: 7665 722e 0a0a 5369 6e63 6520 6942 7269  ver...Since iBri
-00000e10: 6467 6573 2069 7320 736f 6c65 6c79 2062  dges is solely b
-00000e20: 6173 6564 206f 6e20 7079 7468 6f6e 2069  ased on python i
-00000e30: 7420 776f 726b 7320 6f6e 2061 6c6c 206f  t works on all o
-00000e40: 7065 7261 7469 6e67 2073 7973 7465 6d73  perating systems
-00000e50: 2e0a 0a2d 2052 756e 7320 6f6e 2050 7974  ...- Runs on Pyt
-00000e60: 686f 6e20 332e 3820 6f72 2068 6967 6865  hon 3.8 or highe
-00000e70: 722e 0a2d 2053 7570 706f 7274 6564 2069  r..- Supported i
-00000e80: 524f 4453 2073 6572 7665 7220 7665 7273  RODS server vers
-00000e90: 696f 6e73 3a20 342e 322e 3131 206f 7220  ions: 4.2.11 or 
-00000ea0: 6869 6768 6572 2061 6e64 2034 2e33 2e30  higher and 4.3.0
-00000eb0: 206f 7220 6869 6768 6572 2e0a 0a20 3c70   or higher... <p
-00000ec0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000ed0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000ee0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ef0: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
-00000f00: 7479 2f69 4272 6964 6765 732f 6973 7375  ty/iBridges/issu
-00000f10: 6573 2f6e 6577 3f61 7373 6967 6e65 6573  es/new?assignees
-00000f20: 3d26 6c61 6265 6c73 3d26 7072 6f6a 6563  =&labels=&projec
-00000f30: 7473 3d26 7465 6d70 6c61 7465 3d62 7567  ts=&template=bug
-00000f40: 5f72 6570 6f72 742e 6d64 2674 6974 6c65  _report.md&title
-00000f50: 3d25 3542 4255 4725 3544 223e 5265 706f  =%5BBUG%5D">Repo
-00000f60: 7274 2042 7567 3c2f 613e 0a20 2020 202e  rt Bug</a>.    .
-00000f70: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-00000f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000f90: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
-00000fa0: 7479 2f69 4272 6964 6765 732f 6973 7375  ty/iBridges/issu
-00000fb0: 6573 2f6e 6577 3f61 7373 6967 6e65 6573  es/new?assignees
-00000fc0: 3d26 6c61 6265 6c73 3d26 7072 6f6a 6563  =&labels=&projec
-00000fd0: 7473 3d26 7465 6d70 6c61 7465 3d66 6561  ts=&template=fea
-00000fe0: 7475 7265 5f72 6571 7565 7374 2e6d 6426  ture_request.md&
-00000ff0: 7469 746c 653d 2535 4246 4541 5455 5245  title=%5BFEATURE
-00001000: 2535 4422 3e52 6571 7565 7374 2046 6561  %5D">Request Fea
-00001010: 7475 7265 3c2f 613e 0a20 2020 202e 0a20  ture</a>.    .. 
-00001020: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00001030: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
-00001040: 7472 6563 6874 556e 6976 6572 7369 7479  trechtUniversity
-00001050: 2f69 4272 6964 6765 732f 6469 7363 7573  /iBridges/discus
-00001060: 7369 6f6e 732f 6361 7465 676f 7269 6573  sions/categories
-00001070: 2f69 6465 6173 223e 5368 6172 6520 616e  /ideas">Share an
-00001080: 2069 6465 613c 2f61 3e0a 2020 2020 2e0a   idea</a>.    ..
-00001090: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-000010a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000010b0: 5574 7265 6368 7455 6e69 7665 7273 6974  UtrechtUniversit
-000010c0: 792f 6942 7269 6467 6573 2f64 6973 6375  y/iBridges/discu
-000010d0: 7373 696f 6e73 2f63 6174 6567 6f72 6965  ssions/categorie
-000010e0: 732f 6765 6e65 7261 6c22 3e4c 6561 7665  s/general">Leave
-000010f0: 2073 6f6d 6520 6665 6564 6261 636b 3c2f   some feedback</
-00001100: 613e 0a20 2020 202e 0a20 2020 203c 6120  a>.    ..    <a 
-00001110: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001120: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
-00001130: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
-00001140: 6765 732f 6469 7363 7573 7369 6f6e 732f  ges/discussions/
-00001150: 6361 7465 676f 7269 6573 2f71 2d61 223e  categories/q-a">
-00001160: 4173 6b20 6120 7175 6573 7469 6f6e 3c2f  Ask a question</
-00001170: 613e 0a20 203c 2f70 3e0a 3c2f 703e 0a0a  a>.  </p>.</p>..
-00001180: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00001190: 2323 2320 4672 6f6d 2047 6974 6875 6220  ### From Github 
-000011a0: 7265 706f 7369 746f 7279 0a60 6060 0a67  repository.```.g
-000011b0: 6974 2063 6c6f 6e65 2067 6974 4067 6974  it clone git@git
-000011c0: 6875 622e 636f 6d3a 5574 7265 6368 7455  hub.com:UtrechtU
-000011d0: 6e69 7665 7273 6974 792f 6942 7269 6467  niversity/iBridg
-000011e0: 6573 2e67 6974 0a63 6420 6942 7269 6467  es.git.cd iBridg
-000011f0: 6573 0a70 6970 2069 6e73 7461 6c6c 202e  es.pip install .
-00001200: 0a60 6060 0a0a 2323 2320 5079 7069 2069  .```..### Pypi i
-00001210: 6e73 7461 6c6c 0a60 6060 0a70 6970 2069  nstall.```.pip i
-00001220: 6e73 7461 6c6c 2069 6272 6964 6765 730a  nstall ibridges.
-00001230: 6060 600a 0a23 2320 5573 6167 650a 6060  ```..## Usage.``
-00001240: 6070 790a 2320 4372 6561 7465 2061 6e20  `py.# Create an 
-00001250: 6952 4f44 5320 7365 7373 696f 6e0a 6672  iRODS session.fr
-00001260: 6f6d 2069 6272 6964 6765 7320 696d 706f  om ibridges impo
-00001270: 7274 2053 6573 7369 6f6e 0a0a 7365 7373  rt Session..sess
-00001280: 696f 6e20 3d20 5365 7373 696f 6e28 6972  ion = Session(ir
-00001290: 6f64 735f 656e 765f 7061 7468 3d22 7e2f  ods_env_path="~/
-000012a0: 2e69 726f 6473 2f69 726f 6473 5f65 6e76  .irods/irods_env
-000012b0: 6972 6f6e 6d65 6e74 2e6a 736f 6e22 2c20  ironment.json", 
-000012c0: 7061 7373 776f 7264 3d22 6d79 7061 7373  password="mypass
-000012d0: 776f 7264 2229 0a0a 2320 5570 6c6f 6164  word")..# Upload
-000012e0: 2064 6174 610a 6672 6f6d 2069 6272 6964   data.from ibrid
-000012f0: 6765 7320 696d 706f 7274 2075 706c 6f61  ges import uploa
-00001300: 640a 0a75 706c 6f61 6428 7365 7373 696f  d..upload(sessio
-00001310: 6e2c 2022 2f79 6f75 722f 6c6f 6361 6c2f  n, "/your/local/
-00001320: 7061 7468 222c 2022 2f69 726f 6473 2f70  path", "/irods/p
-00001330: 6174 6822 290a 0a23 2044 6f77 6e6c 6f61  ath")..# Downloa
-00001340: 6420 6461 7461 0a66 726f 6d20 6962 7269  d data.from ibri
-00001350: 6467 6573 2069 6d70 6f72 7420 646f 776e  dges import down
-00001360: 6c6f 6164 0a0a 646f 776e 6c6f 6164 2873  load..download(s
-00001370: 6573 7369 6f6e 2c20 222f 6972 6f64 732f  ession, "/irods/
-00001380: 7061 7468 222c 2022 2f6f 7468 6572 2f6c  path", "/other/l
-00001390: 6f63 616c 2f70 6174 6822 290a 0a60 6060  ocal/path")..```
-000013a0: 0a0a 2323 2054 7574 6f72 6961 6c73 0a23  ..## Tutorials.#
-000013b0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000013c0: 0a2d 202a 2a5b 5265 6164 5468 6544 6f63  .- **[ReadTheDoc
-000013d0: 735d 2868 7474 7073 3a2f 2f69 6272 6964  s](https://ibrid
-000013e0: 6765 732e 7265 6164 7468 6564 6f63 732e  ges.readthedocs.
-000013f0: 696f 2f65 6e2f 6c61 7465 7374 2f29 2a2a  io/en/latest/)**
-00001400: 0a0a 2323 2320 4775 6964 6573 0a2d 205b  ..### Guides.- [
-00001410: 5175 6963 6b53 7461 7274 5d28 5475 746f  QuickStart](Tuto
-00001420: 7269 616c 732f 5175 6963 6b53 7461 7274  rials/QuickStart
-00001430: 2e69 7079 6e62 290a 2d20 5b69 524f 4453  .ipynb).- [iRODS
-00001440: 2050 6174 6873 5d28 5475 746f 7269 616c   Paths](Tutorial
-00001450: 732f 6952 4f44 535f 7061 7468 732e 6970  s/iRODS_paths.ip
-00001460: 796e 6229 0a2d 205b 4461 7461 2073 796e  ynb).- [Data syn
-00001470: 6368 726f 6e69 7361 7469 6f6e 5d28 5475  chronisation](Tu
-00001480: 746f 7269 616c 732f 4461 7461 5f73 796e  torials/Data_syn
-00001490: 632e 6970 796e 6229 0a0a 2323 2320 4265  c.ipynb)..### Be
-000014a0: 6769 6e6e 6572 7320 7475 746f 7269 616c  ginners tutorial
-000014b0: 730a 2d20 5b53 6574 7570 2063 6c69 656e  s.- [Setup clien
-000014c0: 7420 636f 6e66 6967 7572 6174 696f 6e5d  t configuration]
-000014d0: 2854 7574 6f72 6961 6c73 2f30 312d 5365  (Tutorials/01-Se
-000014e0: 7475 702d 616e 642d 636f 6e6e 6563 742e  tup-and-connect.
-000014f0: 6970 796e 6229 0a2d 205b 576f 726b 696e  ipynb).- [Workin
-00001500: 6720 7769 7468 2064 6174 615d 2854 7574  g with data](Tut
-00001510: 6f72 6961 6c73 2f30 322d 576f 726b 696e  orials/02-Workin
-00001520: 672d 7769 7468 2d64 6174 612e 6970 796e  g-with-data.ipyn
-00001530: 6229 0a2d 205b 6952 4f44 5320 616e 6420  b).- [iRODS and 
-00001540: 6c6f 6361 6c20 5061 7468 735d 2854 7574  local Paths](Tut
-00001550: 6f72 6961 6c73 2f30 332d 6952 4f44 532d  orials/03-iRODS-
-00001560: 5061 7468 732e 6970 796e 6229 0a2d 205b  Paths.ipynb).- [
-00001570: 4d65 7461 6461 7461 5d28 5475 746f 7269  Metadata](Tutori
-00001580: 616c 732f 3034 2d4d 6574 6164 6174 612e  als/04-Metadata.
-00001590: 6970 796e 6229 0a2d 205b 5368 6172 696e  ipynb).- [Sharin
-000015a0: 6720 6461 7461 5d28 5475 746f 7269 616c  g data](Tutorial
-000015b0: 732f 3035 2d44 6174 612d 5368 6172 696e  s/05-Data-Sharin
-000015c0: 672e 6970 796e 6229 0a0a 2323 2041 7574  g.ipynb)..## Aut
-000015d0: 686f 7273 0a0a 2a2a 4368 7269 7374 696e  hors..**Christin
-000015e0: 6520 5374 6169 6765 7220 284d 6169 6e74  e Staiger (Maint
-000015f0: 6169 6e65 7229 205b 4f52 4349 445d 2868  ainer) [ORCID](h
-00001600: 7474 7073 3a2f 2f6f 7263 6964 2e6f 7267  ttps://orcid.org
-00001610: 2f30 3030 302d 3030 3032 2d36 3735 342d  /0000-0002-6754-
-00001620: 3736 3437 292a 2a0a 0a2d 202a 5761 6765  7647)**..- *Wage
-00001630: 6e69 6e67 656e 2055 6e69 7665 7273 6974  ningen Universit
-00001640: 7920 2620 5265 7365 6172 6368 2a20 3230  y & Research* 20
-00001650: 3231 202d 2032 3032 320a 2d20 2a55 7472  21 - 2022.- *Utr
-00001660: 6563 6874 2055 6e69 7665 7273 6974 792a  echt University*
-00001670: 2032 3032 320a 0a2a 2a54 696d 2076 616e   2022..**Tim van
-00001680: 2044 6161 6c65 6e2a 2a2c 202a 5761 6765   Daalen**, *Wage
-00001690: 6e69 6e67 656e 2055 6e69 7665 7273 6974  ningen Universit
-000016a0: 7920 2620 5265 7365 6172 6368 2a20 3230  y & Research* 20
-000016b0: 3231 0a0a 2a2a 4d61 6172 7465 6e20 5363  21..**Maarten Sc
-000016c0: 6865 726d 6572 2028 4d61 696e 7461 696e  hermer (Maintain
-000016d0: 6572 2920 5b4f 5243 4944 5d28 6874 7470  er) [ORCID](http
-000016e0: 733a 2f2f 6f72 6369 642e 6f72 672f 6d79  s://orcid.org/my
-000016f0: 2d6f 7263 6964 3f6f 7263 6964 3d30 3030  -orcid?orcid=000
-00001700: 302d 3030 3031 2d36 3737 302d 3331 3535  0-0001-6770-3155
-00001710: 292a 2a2c 202a 5574 7265 6368 7420 556e  )**, *Utrecht Un
-00001720: 6976 6572 7369 7479 2a20 3230 3233 0a0a  iversity* 2023..
-00001730: 2a2a 5261 6f75 6c20 5363 6872 616d 2028  **Raoul Schram (
-00001740: 4d61 696e 7461 696e 6572 2920 5b4f 5243  Maintainer) [ORC
-00001750: 4944 5d28 6874 7470 733a 2f2f 6f72 6369  ID](https://orci
-00001760: 642e 6f72 672f 6d79 2d6f 7263 6964 3f6f  d.org/my-orcid?o
-00001770: 7263 6964 3d30 3030 302d 3030 3031 2d36  rcid=0000-0001-6
-00001780: 3631 362d 3233 3058 292a 2a2e 200a 2a55  616-230X)**. .*U
-00001790: 7472 6563 6874 2055 6e69 7665 7273 6974  trecht Universit
-000017a0: 792a 2032 3032 330a 0a23 2320 436f 6e74  y* 2023..## Cont
-000017b0: 7269 6275 746f 7273 0a0a 2a2a 4a2e 502e  ributors..**J.P.
-000017c0: 204d 6320 4661 726c 616e 642a 2a2c 0a2a   Mc Farland**,.*
-000017d0: 556e 6976 6572 7369 7479 206f 6620 4772  University of Gr
-000017e0: 6f6e 696e 6765 6e2c 2043 656e 7465 7220  oningen, Center 
-000017f0: 666f 7220 496e 666f 726d 6174 696f 6e20  for Information 
-00001800: 5465 6368 6e6f 6c6f 6779 2a2c 2032 3032  Technology*, 202
-00001810: 320a 0a23 2320 4c69 6365 6e73 650a 5468  2..## License.Th
-00001820: 6973 2070 726f 6a65 6374 2069 7320 6c69  is project is li
-00001830: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
-00001840: 2047 504c 2d76 3320 6c69 6365 6e73 652e   GPL-v3 license.
-00001850: 0a54 6865 2066 756c 6c20 6c69 6365 6e73  .The full licens
-00001860: 6520 6361 6e20 6265 2066 6f75 6e64 2069  e can be found i
-00001870: 6e20 5b4c 4943 454e 5345 5d28 4c49 4345  n [LICENSE](LICE
-00001880: 4e53 4529 2e0a                           NSE)..
+00000a60: 0a5b 215b 5079 5049 2076 6572 7369 6f6e  .[![PyPI version
+00000a70: 5d28 6874 7470 733a 2f2f 6261 6467 652e  ](https://badge.
+00000a80: 6675 7279 2e69 6f2f 7079 2f69 6272 6964  fury.io/py/ibrid
+00000a90: 6765 732e 7376 6729 5d28 6874 7470 733a  ges.svg)](https:
+00000aa0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000ab0: 7079 2f69 6272 6964 6765 7329 0a5b 215b  py/ibridges).[![
+00000ac0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ad0: 2e63 6f6d 2f55 7472 6563 6874 556e 6976  .com/UtrechtUniv
+00000ae0: 6572 7369 7479 2f69 4272 6964 6765 732f  ersity/iBridges/
+00000af0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000b00: 732f 696e 7465 6772 6174 696f 6e2d 7465  s/integration-te
+00000b10: 7374 732d 6972 6f64 732e 796d 6c2f 6261  sts-irods.yml/ba
+00000b20: 6467 652e 7376 673f 6272 616e 6368 3d64  dge.svg?branch=d
+00000b30: 6576 656c 6f70 295d 2868 7474 7073 3a2f  evelop)](https:/
+00000b40: 2f67 6974 6875 622e 636f 6d2f 5574 7265  /github.com/Utre
+00000b50: 6368 7455 6e69 7665 7273 6974 792f 6942  chtUniversity/iB
+00000b60: 7269 6467 6573 2f61 6374 696f 6e73 2f77  ridges/actions/w
+00000b70: 6f72 6b66 6c6f 7773 2f69 6e74 6567 7261  orkflows/integra
+00000b80: 7469 6f6e 2d74 6573 7473 2d69 726f 6473  tion-tests-irods
+00000b90: 2e79 6d6c 2920 5b21 5b5d 2868 7474 7073  .yml) [![](https
+00000ba0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5574  ://github.com/Ut
+00000bb0: 7265 6368 7455 6e69 7665 7273 6974 792f  rechtUniversity/
+00000bc0: 6942 7269 6467 6573 2f61 6374 696f 6e73  iBridges/actions
+00000bd0: 2f77 6f72 6b66 6c6f 7773 2f6d 6169 6e2e  /workflows/main.
+00000be0: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
+00000bf0: 616e 6368 3d64 6576 656c 6f70 295d 2868  anch=develop)](h
+00000c00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c10: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
+00000c20: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
+00000c30: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f6d  ions/workflows/m
+00000c40: 6169 6e2e 796d 6c29 200a 5b21 5b5d 2868  ain.yml) .[![](h
+00000c50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c60: 6d2f 5574 7265 6368 7455 6e69 7665 7273  m/UtrechtUnivers
+00000c70: 6974 792f 6942 7269 6467 6573 2f61 6374  ity/iBridges/act
+00000c80: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f69  ions/workflows/i
+00000c90: 6e74 6567 7261 7469 6f6e 2d74 6573 7473  ntegration-tests
+00000ca0: 2d79 6f64 612e 796d 6c2f 6261 6467 652e  -yoda.yml/badge.
+00000cb0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000cc0: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+00000cd0: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00000ce0: 6765 732f 6163 7469 6f6e 732f 776f 726b  ges/actions/work
+00000cf0: 666c 6f77 732f 696e 7465 6772 6174 696f  flows/integratio
+00000d00: 6e2d 7465 7374 732d 796f 6461 2e79 6d6c  n-tests-yoda.yml
+00000d10: 2920 215b 5d28 6874 7470 733a 2f2f 7265  ) ![](https://re
+00000d20: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+00000d30: 6f6a 6563 7473 2f69 6272 6964 6765 732f  ojects/ibridges/
+00000d40: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00000d50: 6174 6573 7426 7374 796c 653d 666c 6174  atest&style=flat
+00000d60: 2d64 6566 6175 6c74 290a 0a69 4272 6964  -default)..iBrid
+00000d70: 6765 7320 6973 206c 6962 7261 7279 2066  ges is library f
+00000d80: 6f72 2073 6369 656e 7469 6669 6320 7072  or scientific pr
+00000d90: 6f67 7261 6d6d 6572 7320 7768 6f20 6172  ogrammers who ar
+00000da0: 6520 776f 726b 696e 6720 7769 7468 2064  e working with d
+00000db0: 6174 6120 696e 2069 524f 4453 2e20 5765  ata in iRODS. We
+00000dc0: 2070 726f 7669 6465 2061 2077 7261 7070   provide a wrapp
+00000dd0: 6572 2061 726f 756e 6420 7468 6520 5b70  er around the [p
+00000de0: 7974 686f 6e2d 6972 6f64 7363 6c69 656e  ython-irodsclien
+00000df0: 745d 2868 7474 7073 3a2f 2f70 7970 692e  t](https://pypi.
+00000e00: 6f72 672f 7072 6f6a 6563 742f 7079 7468  org/project/pyth
+00000e10: 6f6e 2d69 726f 6473 636c 6965 6e74 2f29  on-irodsclient/)
+00000e20: 2074 6f20 6661 6369 6c69 7461 7465 2065   to facilitate e
+00000e30: 6173 7920 696e 7465 7261 6374 696f 6e20  asy interaction 
+00000e40: 7769 7468 2074 6865 2069 524f 4453 2073  with the iRODS s
+00000e50: 6572 7665 722e 2069 4272 6964 6765 7320  erver. iBridges 
+00000e60: 6973 2063 7572 7265 6e74 6c79 2073 7469  is currently sti
+00000e70: 6c6c 2069 6e20 7665 7279 2061 6374 6976  ll in very activ
+00000e80: 6520 6465 7665 6c6f 706d 656e 742e 0a0a  e development...
+00000e90: 2323 2048 6967 686c 6967 6874 730a 0a2d  ## Highlights..-
+00000ea0: 2057 6f72 6b73 206f 6e20 5769 6e64 6f77   Works on Window
+00000eb0: 732c 204d 6163 204f 5320 616e 6420 4c69  s, Mac OS and Li
+00000ec0: 6e75 780a 2d20 5275 6e73 206f 6e20 5079  nux.- Runs on Py
+00000ed0: 7468 6f6e 2033 2e38 206f 7220 6869 6768  thon 3.8 or high
+00000ee0: 6572 2e0a 2d20 5375 7070 6f72 7465 6420  er..- Supported 
+00000ef0: 6952 4f44 5320 7365 7276 6572 2076 6572  iRODS server ver
+00000f00: 7369 6f6e 733a 2034 2e32 2e31 3120 6f72  sions: 4.2.11 or
+00000f10: 2068 6967 6865 7220 616e 6420 342e 332e   higher and 4.3.
+00000f20: 3020 6f72 2068 6967 6865 722e 0a2d 202a  0 or higher..- *
+00000f30: 2a49 6e74 6572 6163 7469 7665 2063 6f6e  *Interactive con
+00000f40: 6e65 6374 696f 6e2a 2a20 746f 2079 6f75  nection** to you
+00000f50: 7220 6952 6f64 7320 7365 7276 6572 2e0a  r iRods server..
+00000f60: 2d20 2a2a 5570 6c6f 6164 2a2a 2061 6e64  - **Upload** and
+00000f70: 202a 2a44 6f77 6e6c 6f61 642a 2a20 796f   **Download** yo
+00000f80: 7572 2064 6174 612e 0a2d 204d 616e 6970  ur data..- Manip
+00000f90: 756c 6174 6520 7468 6520 2a2a 6d65 7461  ulate the **meta
+00000fa0: 6461 7461 2a2a 206f 6e20 7468 6520 6952  data** on the iR
+00000fb0: 4f44 5320 7365 7276 6572 2e0a 2d20 2a2a  ODS server..- **
+00000fc0: 5379 6e63 6872 6f6e 697a 652a 2a20 796f  Synchronize** yo
+00000fd0: 7572 2064 6174 6120 6265 7477 6565 6e20  ur data between 
+00000fe0: 796f 7572 206c 6f63 616c 2063 6f6d 7075  your local compu
+00000ff0: 7465 7220 616e 6420 7468 6520 6952 4f44  ter and the iROD
+00001000: 5320 7365 7276 6572 2e0a 2d20 4372 6561  S server..- Crea
+00001010: 7465 2061 6e64 206d 616e 6970 756c 6174  te and manipulat
+00001020: 6520 2a2a 5469 636b 6574 732a 2a20 746f  e **Tickets** to
+00001030: 2074 656d 706f 7261 7269 6c79 2067 7261   temporarily gra
+00001040: 6e74 2061 6363 6573 7320 746f 206f 7574  nt access to out
+00001050: 7369 6465 2075 7365 7273 2e0a 2d20 2a2a  side users..- **
+00001060: 5365 6172 6368 2a2a 2074 6872 6f75 6768  Search** through
+00001070: 2061 6c6c 206d 6574 6164 6174 6120 666f   all metadata fo
+00001080: 7220 796f 7572 2064 6174 6173 6574 206f  r your dataset o
+00001090: 7220 636f 6c6c 6563 7469 6f6e 2e0a 2d20  r collection..- 
+000010a0: 536d 616c 6c20 6e75 6d62 6572 206f 6620  Small number of 
+000010b0: 6465 7065 6e64 656e 6369 6573 2028 6070  dependencies (`p
+000010c0: 7974 686f 6e2d 6972 6f64 7363 6c69 656e  ython-irodsclien
+000010d0: 7460 2061 6e64 2060 7471 646d 6029 0a2d  t` and `tqdm`).-
+000010e0: 2053 6166 6520 6465 6661 756c 7420 6f70   Safe default op
+000010f0: 7469 6f6e 7320 7768 656e 2077 6f72 6b69  tions when worki
+00001100: 6e67 2077 6974 6820 796f 7572 2064 6174  ng with your dat
+00001110: 612e 0a0a 0a20 3c70 2061 6c69 676e 3d22  a.... <p align="
+00001120: 6365 6e74 6572 223e 0a20 2020 203c 6120  center">.    <a 
+00001130: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001140: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+00001150: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00001160: 6765 732f 6973 7375 6573 2f6e 6577 3f61  ges/issues/new?a
+00001170: 7373 6967 6e65 6573 3d26 6c61 6265 6c73  ssignees=&labels
+00001180: 3d26 7072 6f6a 6563 7473 3d26 7465 6d70  =&projects=&temp
+00001190: 6c61 7465 3d62 7567 5f72 6570 6f72 742e  late=bug_report.
+000011a0: 6d64 2674 6974 6c65 3d25 3542 4255 4725  md&title=%5BBUG%
+000011b0: 3544 223e 5265 706f 7274 2042 7567 3c2f  5D">Report Bug</
+000011c0: 613e 0a20 2020 202e 0a20 2020 203c 6120  a>.    ..    <a 
+000011d0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000011e0: 7468 7562 2e63 6f6d 2f55 7472 6563 6874  thub.com/Utrecht
+000011f0: 556e 6976 6572 7369 7479 2f69 4272 6964  University/iBrid
+00001200: 6765 732f 6973 7375 6573 2f6e 6577 3f61  ges/issues/new?a
+00001210: 7373 6967 6e65 6573 3d26 6c61 6265 6c73  ssignees=&labels
+00001220: 3d26 7072 6f6a 6563 7473 3d26 7465 6d70  =&projects=&temp
+00001230: 6c61 7465 3d66 6561 7475 7265 5f72 6571  late=feature_req
+00001240: 7565 7374 2e6d 6426 7469 746c 653d 2535  uest.md&title=%5
+00001250: 4246 4541 5455 5245 2535 4422 3e52 6571  BFEATURE%5D">Req
+00001260: 7565 7374 2046 6561 7475 7265 3c2f 613e  uest Feature</a>
+00001270: 0a20 2020 202e 0a20 2020 203c 6120 6872  .    ..    <a hr
+00001280: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001290: 7562 2e63 6f6d 2f55 7472 6563 6874 556e  ub.com/UtrechtUn
+000012a0: 6976 6572 7369 7479 2f69 4272 6964 6765  iversity/iBridge
+000012b0: 732f 6469 7363 7573 7369 6f6e 732f 6361  s/discussions/ca
+000012c0: 7465 676f 7269 6573 2f69 6465 6173 223e  tegories/ideas">
+000012d0: 5368 6172 6520 616e 2069 6465 613c 2f61  Share an idea</a
+000012e0: 3e0a 2020 2020 2e0a 2020 2020 3c61 2068  >.    ..    <a h
+000012f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001300: 6875 622e 636f 6d2f 5574 7265 6368 7455  hub.com/UtrechtU
+00001310: 6e69 7665 7273 6974 792f 6942 7269 6467  niversity/iBridg
+00001320: 6573 2f64 6973 6375 7373 696f 6e73 2f63  es/discussions/c
+00001330: 6174 6567 6f72 6965 732f 6765 6e65 7261  ategories/genera
+00001340: 6c22 3e4c 6561 7665 2073 6f6d 6520 6665  l">Leave some fe
+00001350: 6564 6261 636b 3c2f 613e 0a20 2020 202e  edback</a>.    .
+00001360: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00001370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001380: 2f55 7472 6563 6874 556e 6976 6572 7369  /UtrechtUniversi
+00001390: 7479 2f69 4272 6964 6765 732f 6469 7363  ty/iBridges/disc
+000013a0: 7573 7369 6f6e 732f 6361 7465 676f 7269  ussions/categori
+000013b0: 6573 2f71 2d61 223e 4173 6b20 6120 7175  es/q-a">Ask a qu
+000013c0: 6573 7469 6f6e 3c2f 613e 0a20 203c 2f70  estion</a>.  </p
+000013d0: 3e0a 3c2f 703e 0a0a 2323 2049 6e73 7461  >.</p>..## Insta
+000013e0: 6c6c 6174 696f 6e0a 0a54 6865 7265 2061  llation..There a
+000013f0: 7265 2074 776f 206d 6169 6e20 7761 7973  re two main ways
+00001400: 2074 6f20 696e 7374 616c 6c20 6942 7269   to install iBri
+00001410: 6467 6573 2e20 5468 6520 7265 636f 6d6d  dges. The recomm
+00001420: 656e 6465 6420 7761 7920 6973 2074 6f20  ended way is to 
+00001430: 7573 6520 7468 6520 7374 6162 6c65 2076  use the stable v
+00001440: 6572 7369 6f6e 2074 6861 7420 6973 2061  ersion that is a
+00001450: 7661 696c 6162 6c65 206f 6e20 5079 5069  vailable on PyPi
+00001460: 3a0a 0a60 6060 6261 7368 0a70 6970 2069  :..```bash.pip i
+00001470: 6e73 7461 6c6c 2069 6272 6964 6765 730a  nstall ibridges.
+00001480: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
+00001490: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+000014a0: 756e 7374 6162 6c65 2076 6572 7369 6f6e  unstable version
+000014b0: 2074 6f20 7465 7374 206f 7574 206e 6577   to test out new
+000014c0: 2066 6561 7475 7265 732c 2079 6f75 2063   features, you c
+000014d0: 616e 2069 6e73 7461 6c6c 2074 6865 2064  an install the d
+000014e0: 6576 656c 6f70 6d65 6e74 2062 7261 6e63  evelopment branc
+000014f0: 683a 0a0a 6060 6062 6173 680a 7069 7020  h:..```bash.pip 
+00001500: 696e 7374 616c 6c20 6769 742b 6874 7470  install git+http
+00001510: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
+00001520: 7472 6563 6874 556e 6976 6572 7369 7479  trechtUniversity
+00001530: 2f69 4272 6964 6765 732e 6769 7440 6465  /iBridges.git@de
+00001540: 7665 6c6f 700a 6060 600a 0a23 2320 5573  velop.```..## Us
+00001550: 6167 650a 0a42 656c 6f77 2061 7265 2073  age..Below are s
+00001560: 6f6d 6520 6261 7369 6320 6578 616d 706c  ome basic exampl
+00001570: 6573 206f 6620 7468 6520 6665 6174 7572  es of the featur
+00001580: 6573 2069 6e20 6942 7269 6467 6573 2e0a  es in iBridges..
+00001590: 0a60 6060 7079 0a23 2043 7265 6174 6520  .```py.# Create 
+000015a0: 616e 2069 524f 4453 2073 6573 7369 6f6e  an iRODS session
+000015b0: 0a66 726f 6d20 6962 7269 6467 6573 2069  .from ibridges i
+000015c0: 6d70 6f72 7420 5365 7373 696f 6e0a 0a73  mport Session..s
+000015d0: 6573 7369 6f6e 203d 2053 6573 7369 6f6e  ession = Session
+000015e0: 2869 726f 6473 5f65 6e76 5f70 6174 683d  (irods_env_path=
+000015f0: 227e 2f2e 6972 6f64 732f 6972 6f64 735f  "~/.irods/irods_
+00001600: 656e 7669 726f 6e6d 656e 742e 6a73 6f6e  environment.json
+00001610: 222c 2070 6173 7377 6f72 643d 226d 7970  ", password="myp
+00001620: 6173 7377 6f72 6422 290a 0a23 2055 706c  assword")..# Upl
+00001630: 6f61 6420 6461 7461 0a66 726f 6d20 6962  oad data.from ib
+00001640: 7269 6467 6573 2069 6d70 6f72 7420 7570  ridges import up
+00001650: 6c6f 6164 0a0a 7570 6c6f 6164 2873 6573  load..upload(ses
+00001660: 7369 6f6e 2c20 222f 796f 7572 2f6c 6f63  sion, "/your/loc
+00001670: 616c 2f70 6174 6822 2c20 222f 6972 6f64  al/path", "/irod
+00001680: 732f 7061 7468 2229 0a0a 2320 446f 776e  s/path")..# Down
+00001690: 6c6f 6164 2064 6174 610a 6672 6f6d 2069  load data.from i
+000016a0: 6272 6964 6765 7320 696d 706f 7274 2064  bridges import d
+000016b0: 6f77 6e6c 6f61 640a 0a64 6f77 6e6c 6f61  ownload..downloa
+000016c0: 6428 7365 7373 696f 6e2c 2022 2f69 726f  d(session, "/iro
+000016d0: 6473 2f70 6174 6822 2c20 222f 6f74 6865  ds/path", "/othe
+000016e0: 722f 6c6f 6361 6c2f 7061 7468 2229 0a0a  r/local/path")..
+000016f0: 6060 600a 0a23 2320 5475 746f 7269 616c  ```..## Tutorial
+00001700: 730a 2323 2320 446f 6375 6d65 6e74 6174  s.### Documentat
+00001710: 696f 6e0a 2d20 2a2a 5b52 6561 6454 6865  ion.- **[ReadThe
+00001720: 446f 6373 5d28 6874 7470 733a 2f2f 6962  Docs](https://ib
+00001730: 7269 6467 6573 2e72 6561 6474 6865 646f  ridges.readthedo
+00001740: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001750: 292a 2a0a 0a23 2323 2047 7569 6465 730a  )**..### Guides.
+00001760: 2d20 5b51 7569 636b 5374 6172 745d 2874  - [QuickStart](t
+00001770: 7574 6f72 6961 6c73 2f51 7569 636b 5374  utorials/QuickSt
+00001780: 6172 742e 6970 796e 6229 0a2d 205b 6952  art.ipynb).- [iR
+00001790: 4f44 5320 5061 7468 735d 2874 7574 6f72  ODS Paths](tutor
+000017a0: 6961 6c73 2f69 524f 4453 5f70 6174 6873  ials/iRODS_paths
+000017b0: 2e69 7079 6e62 290a 2d20 5b44 6174 6120  .ipynb).- [Data 
+000017c0: 7379 6e63 6872 6f6e 6973 6174 696f 6e5d  synchronisation]
+000017d0: 2874 7574 6f72 6961 6c73 2f44 6174 615f  (tutorials/Data_
+000017e0: 7379 6e63 2e69 7079 6e62 290a 0a23 2323  sync.ipynb)..###
+000017f0: 2042 6567 696e 6e65 7273 2074 7574 6f72   Beginners tutor
+00001800: 6961 6c73 0a2d 205b 5365 7475 7020 636c  ials.- [Setup cl
+00001810: 6965 6e74 2063 6f6e 6669 6775 7261 7469  ient configurati
+00001820: 6f6e 5d28 7475 746f 7269 616c 732f 3031  on](tutorials/01
+00001830: 2d53 6574 7570 2d61 6e64 2d63 6f6e 6e65  -Setup-and-conne
+00001840: 6374 2e69 7079 6e62 290a 2d20 5b57 6f72  ct.ipynb).- [Wor
+00001850: 6b69 6e67 2077 6974 6820 6461 7461 5d28  king with data](
+00001860: 7475 746f 7269 616c 732f 3032 2d57 6f72  tutorials/02-Wor
+00001870: 6b69 6e67 2d77 6974 682d 6461 7461 2e69  king-with-data.i
+00001880: 7079 6e62 290a 2d20 5b69 524f 4453 2061  pynb).- [iRODS a
+00001890: 6e64 206c 6f63 616c 2050 6174 6873 5d28  nd local Paths](
+000018a0: 7475 746f 7269 616c 732f 3033 2d69 524f  tutorials/03-iRO
+000018b0: 4453 2d50 6174 6873 2e69 7079 6e62 290a  DS-Paths.ipynb).
+000018c0: 2d20 5b4d 6574 6164 6174 615d 2874 7574  - [Metadata](tut
+000018d0: 6f72 6961 6c73 2f30 342d 4d65 7461 6461  orials/04-Metada
+000018e0: 7461 2e69 7079 6e62 290a 2d20 5b53 6861  ta.ipynb).- [Sha
+000018f0: 7269 6e67 2064 6174 615d 2874 7574 6f72  ring data](tutor
+00001900: 6961 6c73 2f30 352d 4461 7461 2d53 6861  ials/05-Data-Sha
+00001910: 7269 6e67 2e69 7079 6e62 290a 0a23 2320  ring.ipynb)..## 
+00001920: 4175 7468 6f72 730a 0a2a 2a43 6872 6973  Authors..**Chris
+00001930: 7469 6e65 2053 7461 6967 6572 2028 4d61  tine Staiger (Ma
+00001940: 696e 7461 696e 6572 2920 5b4f 5243 4944  intainer) [ORCID
+00001950: 5d28 6874 7470 733a 2f2f 6f72 6369 642e  ](https://orcid.
+00001960: 6f72 672f 3030 3030 2d30 3030 322d 3637  org/0000-0002-67
+00001970: 3534 2d37 3634 3729 2a2a 0a0a 2d20 2a57  54-7647)**..- *W
+00001980: 6167 656e 696e 6765 6e20 556e 6976 6572  ageningen Univer
+00001990: 7369 7479 2026 2052 6573 6561 7263 682a  sity & Research*
+000019a0: 2032 3032 3120 2d20 3230 3232 0a2d 202a   2021 - 2022.- *
+000019b0: 5574 7265 6368 7420 556e 6976 6572 7369  Utrecht Universi
+000019c0: 7479 2a20 3230 3232 0a0a 2a2a 5469 6d20  ty* 2022..**Tim 
+000019d0: 7661 6e20 4461 616c 656e 2a2a 2c20 2a57  van Daalen**, *W
+000019e0: 6167 656e 696e 6765 6e20 556e 6976 6572  ageningen Univer
+000019f0: 7369 7479 2026 2052 6573 6561 7263 682a  sity & Research*
+00001a00: 2032 3032 310a 0a2a 2a4d 6161 7274 656e   2021..**Maarten
+00001a10: 2053 6368 6572 6d65 7220 284d 6169 6e74   Schermer (Maint
+00001a20: 6169 6e65 7229 205b 4f52 4349 445d 2868  ainer) [ORCID](h
+00001a30: 7474 7073 3a2f 2f6f 7263 6964 2e6f 7267  ttps://orcid.org
+00001a40: 2f6d 792d 6f72 6369 643f 6f72 6369 643d  /my-orcid?orcid=
+00001a50: 3030 3030 2d30 3030 312d 3637 3730 2d33  0000-0001-6770-3
+00001a60: 3135 3529 2a2a 2c20 2a55 7472 6563 6874  155)**, *Utrecht
+00001a70: 2055 6e69 7665 7273 6974 792a 2032 3032   University* 202
+00001a80: 330a 0a2a 2a52 616f 756c 2053 6368 7261  3..**Raoul Schra
+00001a90: 6d20 284d 6169 6e74 6169 6e65 7229 205b  m (Maintainer) [
+00001aa0: 4f52 4349 445d 2868 7474 7073 3a2f 2f6f  ORCID](https://o
+00001ab0: 7263 6964 2e6f 7267 2f6d 792d 6f72 6369  rcid.org/my-orci
+00001ac0: 643f 6f72 6369 643d 3030 3030 2d30 3030  d?orcid=0000-000
+00001ad0: 312d 3636 3136 2d32 3330 5829 2a2a 2e20  1-6616-230X)**. 
+00001ae0: 0a2a 5574 7265 6368 7420 556e 6976 6572  .*Utrecht Univer
+00001af0: 7369 7479 2a20 3230 3233 0a0a 2323 2043  sity* 2023..## C
+00001b00: 6f6e 7472 6962 7574 6f72 730a 0a2a 2a4a  ontributors..**J
+00001b10: 2e50 2e20 4d63 2046 6172 6c61 6e64 2a2a  .P. Mc Farland**
+00001b20: 2c0a 2a55 6e69 7665 7273 6974 7920 6f66  ,.*University of
+00001b30: 2047 726f 6e69 6e67 656e 2c20 4365 6e74   Groningen, Cent
+00001b40: 6572 2066 6f72 2049 6e66 6f72 6d61 7469  er for Informati
+00001b50: 6f6e 2054 6563 686e 6f6c 6f67 792a 2c20  on Technology*, 
+00001b60: 3230 3232 0a0a 2323 204c 6963 656e 7365  2022..## License
+00001b70: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00001b80: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00001b90: 7468 6520 4d49 5420 6c69 6365 6e73 652e  the MIT license.
+00001ba0: 0a54 6865 2066 756c 6c20 6c69 6365 6e73  .The full licens
+00001bb0: 6520 6361 6e20 6265 2066 6f75 6e64 2069  e can be found i
+00001bc0: 6e20 5b4c 4943 454e 5345 5d28 4c49 4345  n [LICENSE](LICE
+00001bd0: 4e53 4529 2e0a                           NSE)..
```

### Comparing `ibridges-0.1.2/ibridges.egg-info/SOURCES.txt` & `ibridges-0.1.3/ibridges.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 docker-compose.yml
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/integration-tests-irods.yml
 .github/workflows/integration-tests-yoda.yml
+.github/workflows/lint.yml
 .github/workflows/main.yml
 .github/workflows/pypi_release.yml
 docker/.gitattributes
 docker/README.md
 docker/irods_catalog/Dockerfile
 docker/irods_catalog/init-user-db.sh
 docker/irods_catalog_provider/Dockerfile
@@ -47,16 +48,17 @@
 docs/source/conf.py
 docs/source/faq.rst
 docs/source/index.rst
 docs/source/quickstart.rst
 ibridges/__init__.py
 ibridges/_version.py
 ibridges/data_operations.py
+ibridges/export_metadata.py
+ibridges/icat_columns.py
 ibridges/interactive.py
-ibridges/keywords.py
 ibridges/meta.py
 ibridges/path.py
 ibridges/permissions.py
 ibridges/resources.py
 ibridges/rules.py
 ibridges/search.py
 ibridges/session.py
```

### Comparing `ibridges-0.1.2/pyproject.toml` & `ibridges-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tests/test_irodspath.py` & `ibridges-0.1.3/tests/test_irodspath.py`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tests/testdata/bunny.txt` & `ibridges-0.1.3/tests/testdata/bunny.txt`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tests/testdata/subfolder/sun.csv` & `ibridges-0.1.3/tests/testdata/subfolder/sun.csv`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/01-Setup-and-connect.ipynb` & `ibridges-0.1.3/tutorials/01-Setup-and-connect.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962993421052632%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(0, 'session.close()\\n')], delete: [0]}}, 25: {'source': "*

 * *            "{insert: [(4, 'session = Session(irods_env_path=env_file, password=password)')], "*

 * *            "delete: [4]}}, 32: {'source': {insert: [(0, 'from ibridges.path import "*

 * *            "IrodsPath\\n')], delete: [0]}}, insert: [(37, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('id', '7e49aea2'), ('metadata', OrderedDict()), "*

 * *            "('outputs', []), ('source', [] […]*

```diff
@@ -253,15 +253,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cb564f71",
             "metadata": {},
             "outputs": [],
             "source": [
-                "del session\n",
+                "session.close()\n",
                 "session = interactive_auth()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7f9dd9b3",
             "metadata": {},
@@ -292,15 +292,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges import Session\n",
                 "env_file = Path.expanduser(Path('~')).joinpath(\".irods\", \"irods_environment.json\")\n",
                 "password = <YOUR PASSWORD>\n",
                 "\n",
-                "session = Session(irods_env=ienv, password=password)"
+                "session = Session(irods_env_path=env_file, password=password)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ac22dfc7",
             "metadata": {},
             "source": [
@@ -359,15 +359,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6d06932a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges.utils.path import IrodsPath\n",
+                "from ibridges.path import IrodsPath\n",
                 "irods_path = IrodsPath(session, session.home)\n",
                 "irods_path.collection_exists()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a06f0c7d",
@@ -401,14 +401,22 @@
             "execution_count": null,
             "id": "5590a92d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "print(IrodsPath(session, \"~\"))"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7e49aea2",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ibridges-0.1.2/tutorials/02-Working-with-data.ipynb` & `ibridges-0.1.3/tutorials/02-Working-with-data.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/03-iRODS-Paths.ipynb` & `ibridges-0.1.3/tutorials/03-iRODS-Paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/04-Metadata.ipynb` & `ibridges-0.1.3/tutorials/04-Metadata.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971590909090909%*

 * *Differences: {"'cells'": "{insert: [(43, OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', "*

 * *            "'4072812e'), ('metadata', OrderedDict()), ('outputs', []), ('source', [])]))]}"}*

```diff
@@ -433,14 +433,22 @@
             "outputs": [],
             "source": [
                 "from ibridges.path import IrodsPath\n",
                 "\n",
                 "paths = [IrodsPath(session, r.get('COLL_NAME', '')).joinpath(r.get('DATA_NAME', '')) for r in result]\n",
                 "print(paths)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4072812e",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ibridges-0.1.2/tutorials/05-Data-Sharing.ipynb` & `ibridges-0.1.3/tutorials/05-Data-Sharing.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/Data_sync.ipynb` & `ibridges-0.1.3/tutorials/Data_sync.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796894728535354%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'import os\\n'), (2, 'from ibridges.interactive import "*

 * *            "interactive_auth\\n')], delete: [1]}}, 4: {'source': ['session = "*

 * *            "interactive_auth()']}, 7: {'id': '6b180cee-3753-4a1e-a10f-5cfc50fcb8b0', 'source': "*

 * *            "['print(target, target.collection_exists())\\n', 'print(source, source.is_dir())']}, "*

 * *            "8: {'source': {insert: [(6, '\\n'), (7, 'By default, checksums of all transferred "*

 * *            'files will be calculated  […]*

```diff
@@ -21,16 +21,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "de207d54",
             "metadata": {},
             "outputs": [],
             "source": [
+                "import os\n",
                 "from pathlib import Path\n",
-                "from ibridges import Session\n",
+                "from ibridges.interactive import interactive_auth\n",
                 "from ibridges.path import IrodsPath\n",
                 "from ibridges.sync import sync_data"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2bd887f2",
@@ -44,15 +45,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "648f8c49",
             "metadata": {},
             "outputs": [],
             "source": [
-                "session = Session(irods_env_path=Path.expanduser(Path('~')).joinpath(\".irods\", \"irods_environment.json\"))"
+                "session = interactive_auth()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "123e9829",
             "metadata": {},
             "source": [
@@ -61,75 +62,82 @@
                 "\n",
                 "When uploading, `source` must be an existing local folder, and `target` an existing iRODS collection, and vice versa when downloading. An exception will be raised if either doesn't exist."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d7bd4841",
+            "id": "39de2a38-2c35-48e8-9de4-cf426eaecefd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "target = IrodsPath(session, \"~\", <irods coll path>)\n",
-                "source = Path(os.path.expanduser(\"~\"), <your path>)"
+                "target = IrodsPath(session, \"~\", \"<irods path>\")\n",
+                "source = Path(os.path.expanduser(\"~\"), \"<local path>\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6b180cee-3753-4a1e-a10f-5cfc50fcb8b0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "print(target, target.collection_exists())\n",
+                "print(source, source.is_dir())"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d20dd782",
             "metadata": {},
             "source": [
                 "### Setting sync options\n",
                 "`sync` takes various options:\n",
                 "\n",
-                "- `ignore_checksum`: sync compares the checksum values and file sizes of the source and target files to determine whether synchronization is needed. If the `ignore_checksum` option is set to True, only the file size (instead of the the size and checksum value) is used for determining whether synchronization is needed. This mode gives a potentially faster operation but the result is less accurate.\n",
                 "- The `max_level` option controls the depth up to which the file tree will be synchronized. With `max_level` set to None (default), there is no limit (full recursive synchronization). A max level of 1 synchronizes only the source's root, max level 2 also includes the first set of subfolders/subcollections and their contents, etc.\n",
                 "- The `copy_empty_folders` (default False) option controls whether folders/collections that contain no files or subfolders/subcollections will be synchronized.\n",
                 "- The `dry_run` option lists all the source files and folders that need to be synchronized without actually performing the synchronization.\n",
-                "- The `verify_checksum` (default True) option will calculate and verify the checksum on the data after up- or downloading. A checksum mismatch will generate an error, but will not abort the synchronization process."
+                "\n",
+                "By default, checksums of all transferred files will be calculated and verified after up- or downloading. A checksum mismatch will generate an error, aborting the synchronization process. Should this happen, it is possible some hiccup occurred during the transfer process. Check both copies of the offending file, and retain the correct one."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "edc53ead",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ignore_checksum=True\n",
                 "max_level=None\n",
                 "copy_empty_folders=True\n",
-                "# copy_empty_folders=False\n",
                 "dry_run=True"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f9abc0ae",
             "metadata": {},
             "source": [
                 "### Dry run\n",
-                "Setting `dry_run` to True will list what will be synchronized without any actual transfers. Note that setting `verify_checksum` while performing a dry run will have no effect."
+                "Setting `dry_run` to True will list what will be synchronized without any actual transfers."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd8b1155",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ignore_checksum=False\n",
-                "sync(\n",
+                "changes = sync_data(\n",
                 "    session=session,\n",
                 "    source=source,\n",
                 "    target=target,\n",
                 "    max_level=max_level,      \n",
                 "    dry_run=dry_run,\n",
-                "    ignore_checksum=ignore_checksum,\n",
                 "    copy_empty_folders=copy_empty_folders\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ec01f5ca",
@@ -141,34 +149,40 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "20785359",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dry_run=False\n",
-                "verify_checksum=True"
+                "dry_run=False"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ed24c7bf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sync(\n",
+                "changes = sync_data(\n",
                 "    session=session,\n",
                 "    source=source,\n",
                 "    target=target,\n",
                 "    max_level=max_level,      \n",
                 "    dry_run=dry_run,\n",
-                "    verify_checksum=verify_checksum,\n",
                 "    copy_empty_folders=copy_empty_folders)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "91174060-3f3f-4460-aaae-8da9618a8933",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `ibridges-0.1.2/tutorials/QuickStart.ipynb` & `ibridges-0.1.3/tutorials/QuickStart.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928367019884876%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, 'from getpass import getpass\\n'), (3, '\\n'), (4, 'from "*

 * *            "ibridges import Session\\n'), (5, 'from ibridges.path import IrodsPath\\n')], delete: "*

 * *            "[5, 2, 1, 0]}}, 4: {'source': ['env_file = "*

 * *            'Path.expanduser(Path("~")).joinpath(".irods", "irods_environment.json")\\n\', '*

 * *            "'env_file.exists()']}, 9: {'source': ['# Close the irods session when you do not need "*

 * *            "it any longer.\\n', 'session.close()']}, 12:  […]*

```diff
@@ -19,20 +19,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b6fd51d6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from ibridges import Session\n",
-                "from ibridges.path import IrodsPath\n",
-                "\n",
                 "import json\n",
+                "from getpass import getpass\n",
                 "from pathlib import Path\n",
-                "from getpass import getpass"
+                "\n",
+                "from ibridges import Session\n",
+                "from ibridges.path import IrodsPath\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cf584f48",
             "metadata": {},
             "source": [
@@ -45,16 +45,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e8602139",
             "metadata": {},
             "outputs": [],
             "source": [
-                "env_file = Path(os.path.expanduser(\"~\")).joinpath(\".irods\", \"irods_environment.json\")\n",
-                "os.path.exists(env_file)"
+                "env_file = Path.expanduser(Path(\"~\")).joinpath(\".irods\", \"irods_environment.json\")\n",
+                "env_file.exists()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2cc48382",
             "metadata": {},
             "source": [
@@ -95,16 +95,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "241622a0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Delete the irods session when you do not need it any longer.\n",
-                "del session"
+                "# Close the irods session when you do not need it any longer.\n",
+                "session.close()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "33824686",
             "metadata": {},
             "source": [
@@ -119,19 +119,19 @@
             "source": [
                 "### Authenticate using the cached password ~/.irods/.rodsA"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "242eab2c",
+            "id": "8e5a005a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "session = Session(irods_env_path=env_file)"
+                "session = Session(irods_env=env_file)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0fb9577d",
             "metadata": {},
             "source": [
@@ -240,30 +240,75 @@
             "id": "6cd1bd28",
             "metadata": {},
             "source": [
                 "### Upload a file or folder"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "ec66ec0c",
+            "metadata": {},
+            "source": [
+                "Create a lodal file:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "08d96d6c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# create a local file\n",
                 "local_path = Path.expanduser(Path('~')).joinpath(\"demofile.txt\")\n",
                 "f = open(local_path, \"a\")\n",
                 "f.write(\"My content! Super important\")\n",
-                "f.close()\n",
-                "\n",
+                "f.close()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "9d9dee41",
+            "metadata": {},
+            "source": [
+                "Determine the iRODS path the file should be uploaded to."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "043536c3",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "irods_path = IrodsPath(session, \"~\", \"new_coll\")\n",
+                "if not irods_path.collection_exists():\n",
+                "    coll = create_collection(session, irods_path)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "d0de939a",
+            "metadata": {},
+            "source": [
+                "Upload data and get information:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "45991a0a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "# upload the file to our collection\n",
                 "upload(session, local_path, irods_path, overwrite = True)\n",
                 "\n",
                 "# list again the data object in te collection\n",
+                "coll = get_collection(session, irods_path)\n",
                 "print('data objects\\t', coll.data_objects)\n",
                 "print('cumulative size\\t', get_size(session, coll))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a0893c4b",
@@ -374,15 +419,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "a54a1dd1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
-                "local_path = Path(os.path.expanduser(\"~/Downloads\"))\n",
+                "local_path = Path(\"~/Downloads\").expanduser()\n",
                 "print(\"Download folder exists\", local_path.is_dir())\n",
                 "download(session, ipath, local_path, overwrite=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4d4cff1c",
@@ -415,16 +460,18 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "928bf82c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# upload a file\n",
-                "local_path = Path(os.path.expanduser(\"~\")).joinpath(\"demofile.txt\")\n",
+                "local_path = Path(\"~\").expanduser().joinpath(\"demofile.txt\")\n",
                 "irods_path = IrodsPath(session, \"~\", \"new_coll\")\n",
+                "if not irods_path.collection_exists():\n",
+                "    coll = create_collection(session, irods_path)\n",
                 "upload(session, local_path, irods_path, overwrite = True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "510e390a",
             "metadata": {},
@@ -713,15 +760,16 @@
             "execution_count": null,
             "id": "f1911d89",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from datetime import datetime, timedelta\n",
                 "\n",
-                "objPath = \"/nluu12p/home/research-test-christine/books/BenHur.txt\"\n",
+                "objPath = IrodsPath(session, \"~\", \"new_coll\", \"demofile.txt\")\n",
+                "objPath.dataobject_exists()\n",
                 "ticket = tickets.create_ticket(obj_path=objPath, ticket_type=\"write\", \n",
                 "                               expiry_date=datetime.today() + timedelta(days=1))  # allow write access"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -766,15 +814,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "3913b742",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ibridges.rules import execute_rule\n",
-                "rule_file = \"tutorials/example_rules/example.r\"\n",
+                "rule_file = \"example_rules/example.r\"\n",
                 "stdout, stderr = execute_rule(session, rule_file, {})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "900f8ab2",
```

### Comparing `ibridges-0.1.2/tutorials/iRODS_paths.ipynb` & `ibridges-0.1.3/tutorials/iRODS_paths.ipynb`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject1.png` & `ibridges-0.1.3/tutorials/img/DataObject1.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject2.png` & `ibridges-0.1.3/tutorials/img/DataObject2.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject3.png` & `ibridges-0.1.3/tutorials/img/DataObject3.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject4.png` & `ibridges-0.1.3/tutorials/img/DataObject4.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject5.png` & `ibridges-0.1.3/tutorials/img/DataObject5.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/DataObject6.png` & `ibridges-0.1.3/tutorials/img/DataObject6.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/Save_json.png` & `ibridges-0.1.3/tutorials/img/Save_json.png`

 * *Files identical despite different names*

### Comparing `ibridges-0.1.2/tutorials/img/Yoda_environment.png` & `ibridges-0.1.3/tutorials/img/Yoda_environment.png`

 * *Files identical despite different names*

