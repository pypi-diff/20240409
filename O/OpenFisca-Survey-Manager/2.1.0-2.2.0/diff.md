# Comparing `tmp/OpenFisca-Survey-Manager-2.1.0.tar.gz` & `tmp/OpenFisca-Survey-Manager-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-2.1.0.tar", last modified: Wed Mar 27 09:18:42 2024, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-2.2.0.tar", last modified: Tue Apr  9 14:59:17 2024, max compression
```

## Comparing `OpenFisca-Survey-Manager-2.1.0.tar` & `OpenFisca-Survey-Manager-2.2.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.964058 OpenFisca-Survey-Manager-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    23734 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.960058 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 09:18:42.000000 OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-03-27 09:18:42.964058 OpenFisca-Survey-Manager-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.956058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18253 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.956058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.956058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config_files_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config_files_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config_files_templates/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config_files_templates/raw_data_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/read_spss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.956058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32942 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/abstract_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/reform_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.956058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11066 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/simulation_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    63511 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.960058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:42.960058 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/data_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_write_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-27 09:18:42.964058 OpenFisca-Survey-Manager-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-27 09:18:22.000000 OpenFisca-Survey-Manager-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.325349 OpenFisca-Survey-Manager-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 14:59:17.000000 OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14209 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.313350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config_files_templates/raw_data_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_spss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32942 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/abstract_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/reform_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11374 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulation_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63511 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17265 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.317350 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:17.321349 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16428 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_write_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 14:59:17.325349 OpenFisca-Survey-Manager-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-09 14:59:01.000000 OpenFisca-Survey-Manager-2.2.0/setup.py
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/CHANGELOG.md` & `OpenFisca-Survey-Manager-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 ﻿# Changelog
 
-# 2.1.0 [#277](https://github.com/openfisca/openfisca-survey-manager/pull/277)
+## 2.2.0 [#295](https://github.com/openfisca/openfisca-survey-manager/pull/295)
+
+* Improve support for parquet file format :
+      - If a parquet file is provided to build-collection it will be cleaned an added to the collection as a parquet file.
+      - If the option `keep_original_parquet_file` is passed the parquet file is kept and added to the collection as is as is.
+
+## 2.1.0 [#277](https://github.com/openfisca/openfisca-survey-manager/pull/277)
 
 * New features
-  - Support parquet file format : 
-      - if a parquet file is provided to buildcollection it won't be converted in HDF5 but added to the collection as is.
+  - Support parquet file format :
+      - if a parquet file is provided to build-collection it won't be converted in HDF5 but added to the collection as is.
       - It is possible to provide a folder containing many files : each files will be used as a separate table.
   - Run a simulation on a part of the input datasets (for the moment it works only for two entities simulations) :
       - With a batch size option
-      - With a filter_by option 
+      - With a filter_by option
 
-# 2.0.10 [#285](https://github.com/openfisca/openfisca-survey-manager/pull/285)
+### 2.0.10 [#285](https://github.com/openfisca/openfisca-survey-manager/pull/285)
 
 * Technical changes
 - Some arguments for calibration were not consistently named.
 
-# 2.0.9 [#294](https://github.com/openfisca/openfisca-survey-manager/pull/294)
+### 2.0.9 [#294](https://github.com/openfisca/openfisca-survey-manager/pull/294)
 
 * Technical changes
   - Add config files directory option in `set_table_in_survey`
 
-# 2.0.8 [#292](https://github.com/openfisca/openfisca-survey-manager/pull/292)
+### 2.0.8 [#292](https://github.com/openfisca/openfisca-survey-manager/pull/292)
 
 * Technical change
   - With the security enforcement of PyPi, we have to use token instead of login/password.
 
-# 2.0.7 [#293](https://github.com/openfisca/openfisca-survey-manager/pull/293)
+### 2.0.7 [#293](https://github.com/openfisca/openfisca-survey-manager/pull/293)
 
 * Technical changes
   - Improve correction done in https://github.com/openfisca/openfisca-survey-manager/pull/286/files
 
-# 2.0.6 [#291](https://github.com/openfisca/openfisca-survey-manager/pull/291)
+### 2.0.6 [#291](https://github.com/openfisca/openfisca-survey-manager/pull/291)
 
 * Technical changes
   - Fix the script check-version-and-changelog.sh to fix issue #288
   - Upgrade CI actions
 
-# 2.0.5 [#286](https://github.com/openfisca/openfisca-survey-manager/pull/286)
+### 2.0.5 [#286](https://github.com/openfisca/openfisca-survey-manager/pull/286)
 
 * New features
   - Allows sub-annual weighted aggregates in compute_aggregate when the weights are annual.
 
-# 2.0.4 [#283](https://github.com/openfisca/openfisca-survey-manager/pull/283)
+### 2.0.4 [#283](https://github.com/openfisca/openfisca-survey-manager/pull/283)
 
 - Correction function compute_pivot_tables in ReformScenario
 
-# 2.0.3 [#282](https://github.com/openfisca/openfisca-survey-manager/pull/282)
+### 2.0.3 [#282](https://github.com/openfisca/openfisca-survey-manager/pull/282)
 
 - Correction typo error in create_data_frame_by_entity
 
-# 2.0.2 [#280](https://github.com/openfisca/openfisca-survey-manager/pull/280)
+### 2.0.2 [#280](https://github.com/openfisca/openfisca-survey-manager/pull/280)
 
 - Add a try/except for the tests config in openfisca_survey_manager/__init__.py
 
-# 2.0.1 [#279](https://github.com/openfisca/openfisca-survey-manager/pull/279)
+### 2.0.1 [#279](https://github.com/openfisca/openfisca-survey-manager/pull/279)
 
 #### Technical changes
 
 - Fix names of ids columns when the merge option is True in create_data_frame_by_entity.
 
 # 2.0.O [#273](https://github.com/openfisca/openfisca-survey-manager/pull/273)
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-2.2.0/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-2.2.0/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/PKG-INFO` & `OpenFisca-Survey-Manager-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/README.md` & `OpenFisca-Survey-Manager-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,10 +65,8 @@
     if not private_run_with_data:
         default_config_files_directory = test_config_files_directory
 
 if default_config_files_directory is None:
     from xdg import BaseDirectory
     default_config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
 
-    log.debug('Using default_config_files_directory = {}'.format(
-        default_config_files_directory
-        ))
+    log.debug(f'Using default_config_files_directory = {default_config_files_directory}')
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/aggregates.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,24 +191,22 @@
                     'entity': 'Unknown entity',
                     'amount': 0,
                     'beneficiaries': 0,
                     },
                 index = [variable],
                 )
         weight = self.weight_variable_by_entity[column.entity.key]
-        assert weight in variables, "{} not a variable of the tax_benefit_system".format(weight)
+        assert weight in variables, f"{weight} not a variable of the tax_benefit_system"
 
         weight_array = simulation.calculate(weight, period = self.period).astype('float')
-        assert not np.isnan(np.sum(weight_array)), "The are some NaN in weights {} for entity {}".format(
-            weight, column.entity.key)
+        assert not np.isnan(np.sum(weight_array)), f"The are some NaN in weights {weight} for entity {column.entity.key}"
         # amounts and beneficiaries from current data and default data if exists
         # Build weights for each entity
         variable_array = simulation.calculate_add(variable, period = self.period).astype('float')
-        assert np.isfinite(variable_array).all(), "The are non finite values in variable {} for entity {}".format(
-            variable, column.entity.key)
+        assert np.isfinite(variable_array).all(), f"The are non finite values in variable {variable} for entity {column.entity.key}"
         data = pd.DataFrame({
             variable: variable_array,
             weight: weight_array,
             })
         if filter_by:
             filter_dummy_variable = (
                 filter_by
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Config(configparser.ConfigParser):
     config_ini = None
 
     def __init__(self, config_files_directory = None):
         configparser.ConfigParser.__init__(self)
         if config_files_directory is not None:
             config_ini = os.path.join(config_files_directory, 'config.ini')
-            assert os.path.exists(config_ini), "{} is not a valid path".format(config_ini)
+            assert os.path.exists(config_ini), f"{config_ini} is not a valid path"
             self.config_ini = config_ini
             self.read([config_ini])
 
     def save(self):
         assert self.config_ini, "configuration file path is not defined"
         assert os.path.exists(self.config_ini)
         config_file = open(self.config_ini, 'w')
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 def set_table_in_survey(input_dataframe, entity, period, collection, survey_name, survey_label = None,
         table_label = None, table_name = None, config_files_directory = default_config_files_directory,
         source_format = None, parquet_file = None):
     period = periods.period(period)
     if table_name is None:
         table_name = entity + '_' + str(period)
     if table_label is None:
-        table_label = "Input data for entity {} at period {}".format(entity, period)
+        table_label = f"Input data for entity {entity} at period {period}"
     try:
         survey_collection = SurveyCollection.load(collection = collection, config_files_directory=config_files_directory)
     except configparser.NoOptionError as e:
         log.warning(f"set_table_in_survey configparser.NoOptionError : {e}")
         survey_collection = SurveyCollection(name = collection, config_files_directory=config_files_directory)
     except configparser.NoSectionError as e:  # For tests
         log.warning(f"set_table_in_survey configparser.NoSectionError : {e}")
@@ -214,39 +214,37 @@
             survey_collection = survey_collection,
             )
 
     if survey.hdf5_file_path is None and survey.parquet_file_path is None:
         config = survey.survey_collection.config
         directory_path = config.get("data", "output_directory")
         if not os.path.isdir(directory_path):
-            log.warning("{} who should be the data directory does not exist: we create the directory".format(
-                directory_path))
+            log.warning(f"{directory_path} who should be the data directory does not exist: we create the directory")
             os.makedirs(directory_path)
         if source_format is None:
             survey.hdf5_file_path = os.path.join(directory_path, survey.name + '.h5')
         elif source_format == "parquet":
             survey.parquet_file_path = os.path.join(directory_path, survey.name)
             if not os.path.isdir(survey.parquet_file_path):
-                log.warning("{} who should be the parquet data directory does not exist: we create the directory".format(
-                    survey.parquet_file_path))
+                log.warning(f"{survey.parquet_file_path} who should be the parquet data directory does not exist: we create the directory")
                 os.makedirs(survey.parquet_file_path)
 
     assert (survey.hdf5_file_path is not None) or (survey.parquet_file_path is not None)
     if source_format == "parquet" and parquet_file is None:
         parquet_file = os.path.join(directory_path, survey.name + '.parquet')
     survey.insert_table(label = table_label, name = table_name, dataframe = input_dataframe, parquet_file = parquet_file)
     # If a survey with save name exist it will be overwritten
     survey_collection.surveys = [
         kept_survey for kept_survey in survey_collection.surveys if kept_survey.name != survey_name
         ]
     survey_collection.surveys.append(survey)
     collections_directory = survey_collection.config.get('collections', 'collections_directory')
-    assert os.path.isdir(collections_directory), """{} who should be the collections' directory does not exist.
-Fix the option collections_directory in the collections section of your config file.""".format(collections_directory)
-    collection_json_path = os.path.join(collections_directory, "{}.json".format(collection))
+    assert os.path.isdir(collections_directory), f"""{collections_directory} who should be the collections' directory does not exist.
+Fix the option collections_directory in the collections section of your config file."""
+    collection_json_path = os.path.join(collections_directory, f"{collection}.json")
     survey_collection.dump(json_file_path = collection_json_path)
 
 
 def build_input_dataframe_from_test_case(survey_scenario, test_case_scenario_kwargs, period = None,
         computed_variables = None):
     if computed_variables is None:
         computed_variables = list()
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/abstract_scenario.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/abstract_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scenarios/reform_scenario.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scenarios/reform_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/scripts/build_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,24 +71,24 @@
     csv_files = []
     parquet_files = []
 
     for root, _subdirs, files in os.walk(directory_path):
         for file_name in files:
             file_path = os.path.join(root, file_name)
             if os.path.basename(file_name).endswith(".csv"):
-                log.info("Found csv file {}".format(file_path))
+                log.info(f"Found csv file {file_path}")
                 csv_files.append(file_path)
             if os.path.basename(file_name).endswith(".dta"):
-                log.info("Found stata file {}".format(file_path))
+                log.info(f"Found stata file {file_path}")
                 stata_files.append(file_path)
             if os.path.basename(file_name).endswith(".sas7bdat"):
-                log.info("Found sas file {}".format(file_path))
+                log.info(f"Found sas file {file_path}")
                 sas_files.append(file_path)
             if os.path.basename(file_name).endswith(".parquet"):
-                log.info("Found parquet file {}".format(file_path))
+                log.info(f"Found parquet file {file_path}")
                 relative = file_name[file_name.find(directory_path):]
                 if ("/" in relative or "\\" in relative) and re.match(r".*-\d$", file_name):
                     # Keep only the folder name if parquet files are in subfolders and name contains "-<number>"
                     file_path = os.path.dirname(file_name)
                 parquet_files.append(file_path)
     return {'csv': csv_files, 'stata': stata_files, 'sas': sas_files, 'parquet': parquet_files}
 
@@ -96,14 +96,15 @@
 def build_survey_collection(
         config_files_directory: str,
         collection_name = None,
         replace_metadata = False,
         replace_data = False,
         data_directory_path_by_survey_suffix = None,
         source_format = 'sas',
+        keep_original_parquet_file = False,
         ):
 
     assert collection_name is not None
     assert data_directory_path_by_survey_suffix is not None
     surveys_name = list(data_directory_path_by_survey_suffix.keys())
     assert surveys_name is not None, "A list of surveys to process is needed"
 
@@ -148,15 +149,15 @@
             os.mkdir(collections_directory)
         collection_json_path = os.path.join(collections_directory, "{}.json".format(collection_name))
         survey_collection.dump(json_file_path = collection_json_path)
         surveys = []
         for survey in survey_collection.surveys:
             if survey.name.endswith(str(survey_suffix)) and survey.name.startswith(collection_name):
                 surveys.append(survey)
-        survey_collection.fill_hdf(source_format = source_format, surveys = surveys, overwrite = replace_data)
+        survey_collection.fill_store(source_format = source_format, surveys = surveys, overwrite = replace_data, keep_original_parquet_file = keep_original_parquet_file)
     return survey_collection
 
 
 def check_template_config_files(config_files_directory: str):
     """
     Create template config files if they do not exist.
     """
@@ -200,15 +201,17 @@
     parser.add_argument('-c', '--collection', help = "name of collection to build or update", required = True)
     parser.add_argument('-d', '--replace-data', action = 'store_true', default = False,
         help = "erase existing survey data HDF5 file (instead of failing when HDF5 file already exists)")
     parser.add_argument('-m', '--replace-metadata', action = 'store_true', default = False,
         help = "erase existing collection metadata JSON file (instead of just adding new surveys)")
     parser.add_argument('-p', '--path', help = f'path to the config files directory (default = {default_config_files_directory})')
     parser.add_argument('-s', '--survey', help = 'name of survey to build or update (default = all)')
+    parser.add_argument('-k', '--keep_original_parquet_file', action = 'store_true', default = False, help = "Keep original and point to original parquet files")
     parser.add_argument('-v', '--verbose', action = 'store_true', default = False, help = "increase output verbosity")
+
     args = parser.parse_args()
     logging.basicConfig(level = logging.DEBUG if args.verbose else logging.WARNING, stream = sys.stdout)
 
     if args.path:
         config_files_directory = args.path
     else:
         config_files_directory = default_config_files_directory
@@ -234,14 +237,15 @@
         build_survey_collection(
             collection_name = args.collection,
             data_directory_path_by_survey_suffix = data_directory_path_by_survey_suffix,
             replace_metadata = args.replace_metadata,
             replace_data = args.replace_data,
             source_format = 'sas',
             config_files_directory = config_files_directory,
+            keep_original_parquet_file = args.keep_original_parquet_file,
             )
     except Exception as e:
         log.info(e)
         pdb.post_mortem(sys.exc_info()[2])
         raise e
 
     log.info("The program has been executed in {}".format(datetime.datetime.now() - start_time))
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/simulation_builder.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulation_builder.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/simulations.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/simulations.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/survey_collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,22 +76,19 @@
             self.json_file_path = json_file_path
 
         config.set("collections", self.name, self.json_file_path)
         config.save()
         with codecs.open(self.json_file_path, 'w', encoding = 'utf-8') as _file:
             json.dump(self.to_json(), _file, ensure_ascii = False, indent = 2)
 
-    def fill_hdf(self, source_format = None, surveys = None, tables = None, overwrite = False):
-        if source_format is not None:
-            assert source_format in ["csv", "Rdata", "sas", "spss", "stata", "parquet"], \
-                "Data source format {} is unknown".format(source_format)
+    def fill_store(self, source_format = None, surveys = None, tables = None, overwrite = False, keep_original_parquet_file = False):
         if surveys is None:
             surveys = self.surveys
         for survey in surveys:
-            survey.fill_hdf(source_format = source_format, tables = tables, overwrite = overwrite)
+            survey.fill_store(source_format = source_format, tables = tables, overwrite = overwrite, keep_original_parquet_file = keep_original_parquet_file)
         self.dump()
 
     def get_survey(self, survey_name):
         available_surveys_names = [survey.name for survey in self.surveys]
         assert survey_name in available_surveys_names, \
             'Survey {} cannot be found for survey collection {}.\nAvailable surveys are :{}'.format(
                 survey_name, self.name, available_surveys_names)
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/surveys.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     sas7bdat = "sas",
     dta = 'stata',
     Rdata = 'Rdata',
     spss = 'sav',
     parquet = 'parquet',
     )
 
+admissible_source_formats = list(source_format_by_extension.values())
+
 
 class NoMoreDataError(Exception):
     # Exception when the user ask for more data than available in file
     pass
 
 
 class Survey(object):
@@ -62,16 +64,16 @@
 
         if survey_collection is not None:
             self.survey_collection = survey_collection
 
         self.informations = kwargs
 
     def __repr__(self):
-        header = """{} : survey data {}
-Contains the following tables : \n""".format(self.name, self.label)
+        header = f"""{self.name} : survey data {self.label}
+Contains the following tables : \n"""
         tables = yaml.safe_dump(
             list(self.tables.keys()),
             default_flow_style = False)
         informations = yaml.safe_dump(self.informations, default_flow_style = False)
         return header + tables + informations
 
     @classmethod
@@ -86,55 +88,54 @@
         self.tables = survey_json.get('tables')
         return self
 
     def dump(self):
         assert self.survey_collection is not None
         self.survey_collection.dump()
 
-    def fill_hdf(self, source_format = None, tables = None, overwrite = True):
+    def fill_store(self, source_format = None, tables = None, overwrite = True, keep_original_parquet_file = False,
+            store_format = "hdf5"):
         """
-        Convert data from the source files to hdf5.
+        Convert data from the source files to store format either hdf5 or parquet.
         If the source is in parquet, the data is not converted.
         """
         assert self.survey_collection is not None
         assert isinstance(overwrite, bool) or isinstance(overwrite, list)
         survey = self
-        if survey.hdf5_file_path is None and 'parquet' not in source_format:
-            # Create folder if it does not exist
-            config = survey.survey_collection.config
-            directory_path = config.get("data", "output_directory")
-            if not os.path.isdir(directory_path):
-                log.warn("{} who should be the HDF5 data directory does not exist: we create the directory".format(
-                    directory_path))
-                os.makedirs(directory_path)
+        # Create folder if it does not exist
+        config = survey.survey_collection.config
+        directory_path = config.get("data", "output_directory")
+        if not os.path.isdir(directory_path):
+            log.warn(f"{directory_path} who should be the store data directory does not exist: we create the directory")
+            os.makedirs(directory_path)
+
+        if source_format == "parquet":
+            store_format = "parquet"
 
+        if store_format == "hdf5" and survey.hdf5_file_path is None:
             survey.hdf5_file_path = os.path.join(directory_path, survey.name + '.h5')
-        if source_format is None:
-            source_formats = ['csv', 'stata', 'sas', 'spss', 'Rdata', 'parquet']
-        else:
+
+        if store_format == "parquet" and survey.parquet_file_path is None:
+            survey.parquet_file_path = os.path.join(directory_path, survey.name)
+
+        self.store_format = store_format
+
+        if source_format is not None:
+            assert source_format in admissible_source_formats, f"Data source format {source_format} is unknown"
             source_formats = [source_format]
+        else:
+            source_formats = admissible_source_formats
+
         for source_format in source_formats:
-            files = "{}_files".format(source_format)
+            files = f"{source_format}_files"
             for data_file in survey.informations.get(files, []):
                 path_name, extension = os.path.splitext(data_file)
                 name = os.path.basename(path_name)
                 if tables is None or name in tables:
-                    if source_format != "parquet":
-                        table = Table(
-                            label = name,
-                            name = name,
-                            source_format = source_format_by_extension[extension[1:]],
-                            survey = survey,
-                            )
-                        table.fill_hdf(
-                            data_file = data_file,
-                            clean = True,
-                            overwrite = overwrite if isinstance(overwrite, bool) else table.name in overwrite,
-                            )
-                    else:
+                    if keep_original_parquet_file:
                         # Use folder instead of files if numeric at end of file
                         if re.match(r".*-\d$", name):
                             name = name.split("-")[0]
                             parquet_file = os.path.dirname(data_file)
                             # Get the parent folder
                             survey.parquet_file_path = "/".join(os.path.dirname(data_file).split(os.sep)[:-1])
                         else:
@@ -144,14 +145,27 @@
                             label = name,
                             name = name,
                             source_format = source_format_by_extension[extension[1:]],
                             survey = survey,
                             parquet_file = parquet_file,
                             )
                         table.read_parquet_columns(data_file)
+
+                    else:
+                        table = Table(
+                            label = name,
+                            name = name,
+                            source_format = source_format_by_extension[extension[1:]],
+                            survey = survey,
+                            )
+                        table.fill_store(
+                            data_file,
+                            clean = True,
+                            overwrite = overwrite if isinstance(overwrite, bool) else table.name in overwrite,
+                            )
         self.dump()
 
     def find_tables(self, variable, tables = None, rename_ident = True):
         """Find tables containing a given variable."""
         container_tables = []
 
         assert variable is not None
@@ -170,26 +184,26 @@
         """
         Get columns of a table.
         """
         assert table is not None
         if self.hdf5_file_path is not None:
             store = pandas.HDFStore(self.hdf5_file_path, "r")
             if table in store:
-                log.debug("Building columns index for table {}".format(table))
+                log.debug(f"Building columns index for table {table}")
                 data_frame = store[table]
                 if rename_ident is True:
                     for column_name in data_frame:
                         if ident_re.match(column_name) is not None:
                             data_frame.rename(columns = {column_name: "ident"}, inplace = True)
-                            log.info("{} column have been replaced by ident".format(column_name))
+                            log.info(f"{column_name} column have been replaced by ident")
                             break
                 store.close()
                 return list(data_frame.columns)
             else:
-                log.info('table {} was not found in {}'.format(table, store.filename))
+                log.info(f'table {table} was not found in {store.filename}')
                 store.close()
                 return list()
         elif self.parquet_file_path is not None:
             parquet_schema = pq.read_schema(self.parquet_file_path)
             column_names = parquet_schema.names
             return column_names
 
@@ -224,18 +238,17 @@
           pd.DataFrame: dataframe containing the variables
 
         Raises:
           Exception:
 
         """
         if self.parquet_file_path is None and self.hdf5_file_path is None:
-            raise Exception("No data file found for survey {}".format(self.name))
+            raise Exception(f"No data file found for survey {self.name}")
         if self.hdf5_file_path is not None:
-            assert os.path.exists(self.hdf5_file_path), '{} is not a valid path. This could happen because your data were not builded yet. Please consider using a rebuild option in your code.'.format(
-                self.hdf5_file_path)
+            assert os.path.exists(self.hdf5_file_path), f'{self.hdf5_file_path} is not a valid path. This could happen because your data were not builded yet. Please consider using a rebuild option in your code.'
             store = pandas.HDFStore(self.hdf5_file_path, "r")
             if ignorecase:
                 keys = store.keys()
                 eligible_tables = []
                 for string in keys:
                     match = re.findall(table, string, re.IGNORECASE)
                     if match:
@@ -311,41 +324,41 @@
                         #         df = batch.to_pandas()
                         #         break
                         #     index += 1
                     else:
                         df = pq.ParquetDataset(parquet_file).read(columns=columns).to_pandas()
                     break
             else:
-                raise Exception("No table {} found in {}".format(table, self.parquet_file_path))
+                raise Exception(f"No table {table} found in {self.parquet_file_path}")
 
         if lowercase:
             columns = dict((column_name, column_name.lower()) for column_name in df)
             df.rename(columns = columns, inplace = True)
 
         if rename_ident is True:
             for column_name in df:
                 if ident_re.match(str(column_name)) is not None:
                     df.rename(columns = {column_name: "ident"}, inplace = True)
-                    log.info("{} column have been replaced by ident".format(column_name))
+                    log.info(f"{column_name} column have been replaced by ident")
                     break
 
         if variables is None:
             return df
         else:
             diff = set(variables) - set(df.columns)
             if diff:
-                raise Exception("The following variable(s) {} are missing".format(diff))
+                raise Exception(f"The following variable(s) {diff} are missing")
             variables = list(set(variables).intersection(df.columns))
             df = df[variables]
             return df
 
     def insert_table(self, label = None, name = None, **kwargs):
         """
         Inserts a table in the Survey object
-        If a pandas dataframe is provided, it is saved in the hdf5 file
+        If a pandas dataframe is provided, it is saved in the store file
         """
         parquet_file = kwargs.pop('parquet_file', None)
         data_frame = kwargs.pop('data_frame', None)
         if data_frame is None:
             # Try without underscore
             data_frame = kwargs.pop('dataframe', None)
 
@@ -357,20 +370,20 @@
             else:
                 variables = list(data_frame.columns)
             if label is None:
                 label = name
             table = Table(label = label, name = name, survey = self, variables = variables, parquet_file = parquet_file)
             assert (table.survey.hdf5_file_path is not None) or (table.survey.parquet_file_path is not None)
             if parquet_file is not None:
-                log.debug("Saving table {} in {}".format(name, table.survey.parquet_file_path))
+                log.debug(f"Saving table {name} in {table.survey.parquet_file_path}")
                 data_frame.to_parquet(parquet_file)
             else:
-                log.debug("Saving table {} in {}".format(name, table.survey.hdf5_file_path))
+                log.debug(f"Saving table {name} in {table.survey.hdf5_file_path}")
                 to_hdf_kwargs = kwargs.pop('to_hdf_kwargs', dict())
-                table.save_data_frame(data_frame, **to_hdf_kwargs)
+                table.save_data_frame_to_hdf5(data_frame, **to_hdf_kwargs)
 
         if name not in self.tables:
             self.tables[name] = dict()
         for key, val in kwargs.items():
             self.tables[name][key] = val
 
     def to_json(self):
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tables.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tables."""
 
 from chardet.universaldetector import UniversalDetector
 import collections
 import csv
 import datetime
+import errno
 import gc
 import logging
 import os
 import pandas
 from pyarrow import parquet as pq
 
 
@@ -18,14 +19,24 @@
 except ImportError:
     read_spss = None
 
 
 log = logging.getLogger(__name__)
 
 
+reader_by_source_format = dict(
+    # Rdata = pandas.rpy.common.load_data,
+    csv = pandas.read_csv,
+    sas = read_sas.read_sas,
+    spss = read_spss,
+    stata = pandas.read_stata,
+    parquet = pandas.read_parquet,
+    )
+
+
 class Table(object):
     """A table of a survey."""
     label = None
     name = None
     source_format = None
     survey = None
     variables = None
@@ -38,227 +49,254 @@
         self.label = label
         self.source_format = source_format
         self.variables = variables
         self.parquet_file = parquet_file
         self.informations = kwargs
 
         from .surveys import Survey  # Keep it here to avoid infinite recursion
-        assert isinstance(survey, Survey), 'survey is of type {} and not {}'.format(type(survey), Survey)
+        assert isinstance(survey, Survey), f'survey is of type {type(survey)} and not {Survey}'
         self.survey = survey
         if not survey.tables:
             survey.tables = collections.OrderedDict()
 
         survey.tables[name] = collections.OrderedDict(
             source_format = source_format,
             variables = variables,
             parquet_file = parquet_file,
             )
 
-    def _check_and_log(self, data_file_path):
-        """Check if the file exists and log the insertion."""
+    def _check_and_log(self, data_file_path, store_file_path):
+        """
+        Check if the file exists and log the insertion.
+
+        Args:
+            data_file_path: Data file path
+            store_file_path: Store file or dir path
+
+        Raises:
+            Exception: File not found
+        """
+        assert store_file_path is not None, "Store file path cannot be None"
         if not os.path.isfile(data_file_path):
-            raise Exception("file_path {} do not exists".format(data_file_path))
-        log.info("Inserting table {} from file {} in HDF file {} at point {}".format(
-            self.name,
-            data_file_path,
-            self.survey.hdf5_file_path,
-            self.name,
-            ))
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), data_file_path)
+
+        log.info(f"Inserting table {self.name} from file {data_file_path} in store file {store_file_path} at point {self.name}")
 
-    def _save(self, data_frame: pandas.DataFrame = None):
+    def _is_stored(self):
+        if self.survey.hdf5_file_path is not None:
+            store = pandas.HDFStore(self.survey.hdf5_file_path)
+            if self.name in store:
+                log.info(f'Exiting without overwriting {self.name} in {self.survey.hdf5_file_path}')
+                store.close()
+                return True
+
+            store.close()
+            return False
+        else:
+            return False
+
+    def _save(self, data_frame: pandas.DataFrame = None, store_format = "hdf5"):
         """
-        Save a data frame in the HDF5 file format.
+        Save a data frame in the store according to is format (HDF5 or Parque).
         """
         assert data_frame is not None
-        table = self
-        hdf5_file_path = table.survey.hdf5_file_path
-        variables = table.variables
-        log.info("Inserting table {} in HDF file {}".format(table.name, hdf5_file_path))
+        variables = self.variables
+
         if variables:
             stored_variables = list(set(variables).intersection(set(data_frame.columns)))
-            log.info('The folloging variables are stored: {}'.format(stored_variables))
+            log.info(f'The folloging variables are stored: {stored_variables}')
             if set(stored_variables) != set(variables):
-                log.info('variables wanted by the user that were not available: {}'.format(
-                    list(set(variables) - set(stored_variables))
-                    ))
+                log.info(f'variables wanted by the user that were not available: {list(set(variables) - set(stored_variables))}')
             data_frame = data_frame[stored_variables].copy()
 
-        self.save_data_frame(data_frame)
+        assert store_format in ["hdf5", "parquet"], f"invalid store_format: {store_format}"
+        if store_format == "hdf5":
+            self.save_data_frame_to_hdf5(data_frame)
+        else:
+            parquet_file_path = self.survey.parquet_file_path
+            log.info(f"Inserting table {self.name} in Parquet file {parquet_file_path}")
+            self.save_data_frame_to_parquet(data_frame)
         gc.collect()
 
+    def fill_store(self, data_file, overwrite: bool = False, clean: bool = False, **kwargs):
+        """
+        Fill the store (HDF5 or parquet file) with the table.
+        Read the `data_file` in parameter and save it to the store.
+
+        Args:
+            data_file (_type_, optional): The data file path. Defaults to None.
+            overwrite (bool, optional): Overwrite the data. Defaults to False.
+            clean (bool, optional): Clean the raw data befoe saving. Defaults to False.
+            store_format (str, optional): _description_. Defaults to "hdf5".
+
+        Raises:
+            e: Skip file if error
+        """
+        if not overwrite and self._is_stored():
+            log.info(
+                f'Exiting without overwriting {self.name} in {self.survey.hdf5_file_path}'
+                )
+            return
+
+        start_table_time = datetime.datetime.now()
+        data_frame = self.read_source(data_file, **kwargs)
+        try:
+            if clean:
+                clean_data_frame(data_frame)
+            self._save(data_frame = data_frame, store_format = self.survey.store_format)
+            log.info(f"File {data_file} has been processed in {datetime.datetime.now() - start_table_time}")
+        except Exception as e:
+            log.info(f'Skipping file {data_file} because of following error \n {e}')
+            raise e
+
     def read_parquet_columns(self, parquet_file = None) -> list:
         """
         Initialize the table from a parquet file.
         """
         if parquet_file is None:
             parquet_file = self.parquet_file
         log.info(f"Initializing table {self.name} from parquet file {parquet_file}")
         self.source_format = 'parquet'
         parquet_schema = pq.read_schema(parquet_file)
         self.variables = parquet_schema.names
         self.survey.tables[self.name]["variables"] = self.variables
         return self.variables
 
-    def fill_hdf(self, **kwargs):
-        """
-        Fill the HDF5 file with the table.
-        Read the `data_file` in parameter and save it in the HDF5 file.
-        """
+    def read_source(self, data_file, **kwargs):
         source_format = self.source_format
-
-        reader_by_source_format = dict(
-            # Rdata = pandas.rpy.common.load_data,
-            csv = pandas.read_csv,
-            sas = read_sas.read_sas,
-            spss = read_spss,
-            stata = pandas.read_stata,
-            parquet = pandas.read_parquet,
+        store_file_path = (
+            self.survey.hdf5_file_path
+            if self.survey.store_format == "hdf5"
+            else self.survey.parquet_file_path
             )
-        start_table_time = datetime.datetime.now()
-        data_file = kwargs.pop("data_file")
-        overwrite = kwargs.pop('overwrite')
-        clean = kwargs.pop("clean")
-
-        # if source_format == 'stata':
-        #     kwargs[]
-        if not overwrite:
-            store = pandas.HDFStore(self.survey.hdf5_file_path)
-            if self.name in store:
-                log.info(
-                    'Exiting without overwriting {} in {}'.format(
-                        self.name, self.survey.hdf5_file_path))
-            store.close()
-            return
-        else:
-            self._check_and_log(data_file)
-            reader = reader_by_source_format[source_format]
-            try:
 
-                if source_format == 'csv':
-                    try:
-                        data_frame = reader(data_file, **kwargs)
+        self._check_and_log(data_file, store_file_path = store_file_path)
+        reader = reader_by_source_format[source_format]
+        try:
+            if source_format == 'csv':
+                try:
+                    data_frame = reader(data_file, **kwargs)
 
-                        if len(data_frame.columns) == 1 and ";" in len(data_frame.columns[0]):
-                            raise ValueError("A ';' is presennt in the unique column name. Looks like we got the wrong separator.")
+                    if len(data_frame.columns) == 1 and ";" in len(data_frame.columns[0]):
+                        raise ValueError("A ';' is present in the unique column name. Looks like we got the wrong separator.")
 
-                    except Exception:
-                        log.debug(f"Failing to read {data_file}, Trying to infer econding and dialect/sperator")
+                except Exception:
+                    log.debug(f"Failing to read {data_file}, Trying to infer encoding and dialect/separator")
+
+                    # Detect encoding
+                    detector = UniversalDetector()
+                    with open(data_file, 'rb') as csvfile:
+                        for line in csvfile:
+                            detector.feed(line)
+                            if detector.done:
+                                break
+                        detector.close()
 
-                        # Detect encoding
-                        detector = UniversalDetector()
-                        with open(data_file, 'rb') as csvfile:
-                            for line in csvfile:
-                                detector.feed(line)
-                                if detector.done:
-                                    break
-                            detector.close()
-
-                        encoding = detector.result['encoding']
-                        confidence = detector.result['confidence']
-
-                        # Sniff dialect
-                        try:
-                            with open(data_file, 'r', newline = "", encoding = encoding) as csvfile:
-                                dialect = csv.Sniffer().sniff(csvfile.read(1024), delimiters=";,")
-                        except Exception:
-                            # Sometimes the sniffer fails, we switch back to the default ... of french statistical data
-                            dialect = None
-                            delimiter = ";"
-
-                        log.debug(
-                            f"dialect.delimiter = {dialect.delimiter if dialect is not None else delimiter}, encoding = {encoding}, confidence = {confidence}"
-                            )
-                        kwargs['engine'] = "python"
-                        if dialect:
-                            kwargs['dialect'] = dialect
-                        else:
-                            kwargs['delimiter'] = delimiter
-                        kwargs['encoding'] = encoding
-                        data_frame = reader(data_file, **kwargs)
+                    encoding = detector.result['encoding']
+                    confidence = detector.result['confidence']
 
-                else:
+                    # Sniff dialect
+                    try:
+                        with open(data_file, 'r', newline = "", encoding = encoding) as csvfile:
+                            dialect = csv.Sniffer().sniff(csvfile.read(1024), delimiters=";,")
+                    except Exception:
+                        # Sometimes the sniffer fails, we switch back to the default ... of french statistical data
+                        dialect = None
+                        delimiter = ";"
+
+                    log.debug(
+                        f"dialect.delimiter = {dialect.delimiter if dialect is not None else delimiter}, encoding = {encoding}, confidence = {confidence}"
+                        )
+                    kwargs['engine'] = "python"
+                    if dialect:
+                        kwargs['dialect'] = dialect
+                    else:
+                        kwargs['delimiter'] = delimiter
+                    kwargs['encoding'] = encoding
                     data_frame = reader(data_file, **kwargs)
 
-            except Exception as e:
-                log.info('Error while reading {}'.format(data_file))
-                raise e
-            gc.collect()
-            try:
-                if clean:
-                    clean_data_frame(data_frame)
-                self._save(data_frame = data_frame)
-                log.info("File {} has been processed in {}".format(
-                    data_file, datetime.datetime.now() - start_table_time))
-            except Exception as e:
-                log.info('Skipping file {} because of following error \n {}'.format(data_file, e))
-                raise e
+            else:
+                data_frame = reader(data_file, **kwargs)
 
-    def save_data_frame(self, data_frame, **kwargs):
+        except Exception as e:
+            log.info(f'Error while reading {data_file}')
+            raise e
+
+        gc.collect()
+        return data_frame
+
+    def save_data_frame_to_hdf5(self, data_frame, **kwargs):
         """Save a data frame in the HDF5 file format."""
         hdf5_file_path = self.survey.hdf5_file_path
+        log.info(f"Inserting table {self.name} in HDF file {hdf5_file_path}")
         store_path = self.name
         try:
             data_frame.to_hdf(hdf5_file_path, store_path, append = False, **kwargs)
         except (TypeError, NotImplementedError):
-            log.info("Type problem(s) when creating {} in {}".format(store_path, hdf5_file_path))
+            log.info(f"Type problem(s) when creating {store_path} in {hdf5_file_path}")
             dtypes = data_frame.dtypes
             # Checking for strings
             converted_dtypes = dtypes.isin(['mixed', 'unicode'])
             if converted_dtypes.any():
-                log.info("The following types are converted to strings \n {}".format(dtypes[converted_dtypes]))
+                log.info(f"The following types are converted to strings \n {dtypes[converted_dtypes]}")
                 # Conversion to strings
                 for column in dtypes[converted_dtypes].index:
                     data_frame[column] = data_frame[column].copy().astype(str)
 
             # Checking for remaining categories
             dtypes = data_frame.dtypes
             converted_dtypes = dtypes.isin(['category'])
             if not converted_dtypes.empty:  # With category table format is needed
-                log.info("The following types are added as category using the table format\n {}".format(dtypes[converted_dtypes]))
+                log.info(f"The following types are added as category using the table format\n {dtypes[converted_dtypes]}")
                 data_frame.to_hdf(hdf5_file_path, store_path, append = False, format = 'table', **kwargs)
 
         self.variables = list(data_frame.columns)
 
+    def save_data_frame_to_parquet(self, data_frame):
+        """Save a data frame in the Parquet file format."""
+        parquet_file_path = self.survey.parquet_file_path
+
+        if not os.path.isdir(parquet_file_path):
+            log.warn(f"{parquet_file_path} where to store table {self.name} data does not exist: we create the directory")
+            os.makedirs(parquet_file_path)
+        self.parquet_file = parquet_file_path + "/" + self.name
+        data_frame.to_parquet(self.parquet_file)
+        self.variables = list(data_frame.columns)
+
+        self.survey.tables[self.name]["parquet_file"] = self.parquet_file
+        self.survey.tables[self.name]["variables"] = self.variables
+
 
 def clean_data_frame(data_frame):
     """Clean a data frame.
+
+    The following steps are executed:
     - drop empty columns
     - replace empty strings with zeros
     - convert string columns to integers
     """
     data_frame.columns = data_frame.columns.str.lower()
     object_column_names = list(data_frame.select_dtypes(include=["object"]).columns)
-    log.info(
-        "The following variables are to be cleaned or left as strings : \n {}".format(object_column_names)
-        )
+    log.info(f"The following variables are to be cleaned or left as strings : \n {object_column_names}")
     for column_name in object_column_names:
         if data_frame[column_name].isnull().all():  #
-            log.info("Drop empty column {}".format(column_name))
+            log.info(f"Drop empty column {column_name}")
             data_frame.drop(column_name, axis = 1, inplace = True)
             continue
 
         values = [str(value) for value in data_frame[column_name].value_counts().keys()]
         empty_string_present = "" in values
         if empty_string_present:
             values.remove("")
         all_digits = all([value.strip().isdigit() for value in values])
         no_zero = all([value != 0 for value in values])
         if all_digits and no_zero:
-            log.info(
-                "Replacing empty string with zero for variable {}".format(column_name)
-                )
+            log.info(f"Replacing empty string with zero for variable {column_name}")
             data_frame.replace(
-                to_replace = {
-                    column_name: {"": 0},
-                    },
+                to_replace = {column_name: {"": 0}},
                 inplace = True,
                 )
-            log.info(
-                "Converting string variable {} to integer".format(column_name)
-                )
+            log.info(f"Converting string variable {column_name} to integer")
             try:
                 data_frame[column_name] = data_frame[column_name].astype("int")
             except OverflowError:
-                log.info(
-                    'OverflowError when converting {} to int. Keeping as {}'.format(
-                        column_name, data_frame[column_name].dtype)
-                    )
+                log.info(f'OverflowError when converting {column_name} to int. Keeping as {data_frame[column_name].dtype}')
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/__init__.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_aggregates.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_calibration.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_aggregate.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_aggregate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_pivot_table.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_compute_winners_loosers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     df_by_entity = survey_scenario.create_data_frame_by_entity(
         variables = ['salary', 'rent'],
         period = period,
         )
     salary = survey_scenario.calculate_variable('salary', period = period)
     rent = survey_scenario.calculate_variable('rent', period = period)
     for entity, df in df_by_entity.items():
-        assert not df.empty, "{} dataframe is empty".format(entity)
+        assert not df.empty, f"{entity} dataframe is empty"
     assert (df_by_entity['person']['salary'] == salary).all().all()
     assert (df_by_entity['household']['rent'] == rent).all().all()
 
 
 def test_create_data_frame_by_entity_with_index():
     survey_scenario = create_randomly_initialized_survey_scenario()
     period = '2017-01'
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_parquet.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_surveys.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     survey = Survey(
         hdf5_file_path = saved_fake_survey_hdf5_file_path,
         name = 'fake_survey',
         sas_files = [saved_fake_survey_file_path],
         survey_collection = survey_collection,
         )
     survey.insert_table(name = 'test_parquet')
-    survey.fill_hdf(source_format = 'parquet')
+    survey.fill_store(source_format = 'parquet')
 
 
 def test_survey():
     name = 'fake'
     data_dir = os.path.join(
         openfisca_survey_manager_location,
         'openfisca_survey_manager',
@@ -53,15 +53,15 @@
     survey = Survey(
         hdf5_file_path = saved_fake_survey_hdf5_file_path,
         name = 'fake_survey',
         sas_files = [saved_fake_survey_file_path],
         survey_collection = survey_collection,
         )
     survey.insert_table(name = 'help')
-    survey.fill_hdf(source_format = 'sas')
+    survey.fill_store(source_format = 'sas')
 
 
 def test_survey_load():
     survey_name = 'test_set_table_in_survey_2021'
     collection = 'fake'
     data_dir = os.path.join(
         openfisca_survey_manager_location,
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from openfisca_core.parameters import ParameterNode, Scale
 from openfisca_country_template import CountryTaxBenefitSystem
 from openfisca_survey_manager.utils import parameters_asof, variables_asof
 
 
 def check_max_instant_leaf(sub_parameter, instant):
     for parameter_at_instant in sub_parameter.values_list:
-        assert periods.instant(parameter_at_instant.instant_str) <= instant, "Error for {}: \n {}".format(
-            sub_parameter.name, sub_parameter.values_list)
+        assert periods.instant(parameter_at_instant.instant_str) <= instant, f"Error for {sub_parameter.name}: \n {sub_parameter.values_list}"
 
 
 def check_max_instant(parameters, instant):
     for _, sub_parameter in parameters.children.items():
         if isinstance(sub_parameter, ParameterNode):
             check_max_instant(sub_parameter, instant)
         else:
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/tests/test_write_parquet.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/tests/test_write_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,8 +93,9 @@
         build_survey_collection(
             collection_name=collection_name,
             data_directory_path_by_survey_suffix=data_directory_path_by_survey_suffix,
             replace_metadata=False,
             replace_data=False,
             source_format="parquet",
             config_files_directory=data_dir,
+            keep_original_parquet_file=True,
             )
```

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-2.2.0/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/setup.cfg` & `OpenFisca-Survey-Manager-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-2.1.0/setup.py` & `OpenFisca-Survey-Manager-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '2.1.0',
+    version = '2.2.0',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

