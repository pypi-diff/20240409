# Comparing `tmp/gadapt-0.3.4.tar.gz` & `tmp/gadapt-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gadapt-0.3.4.tar", last modified: Sat Apr  6 20:16:33 2024, max compression
+gzip compressed data, was "gadapt-0.3.5.tar", last modified: Tue Apr  9 20:34:01 2024, max compression
```

## Comparing `gadapt-0.3.4.tar` & `gadapt-0.3.5.tar`

### file list

```diff
@@ -1,116 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.225236 gadapt-0.3.4/
--rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.4/LICENSE
--rw-rw-rw-   0        0        0    22076 2024-04-06 20:16:33.224734 gadapt-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    21751 2024-03-16 19:55:38.000000 gadapt-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:32.984740 gadapt-0.3.4/gadapt/
--rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.007232 gadapt-0.3.4/gadapt/adapters/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.010233 gadapt-0.3.4/gadapt/adapters/ga_logging/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/adapters/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.4/gadapt/adapters/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.012733 gadapt-0.3.4/gadapt/adapters/string_operation/
--rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/string_operation/__init__.py
--rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/adapters/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.021734 gadapt-0.3.4/gadapt/adapters/validation/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/adapters/validation/__init__.py
--rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.4/gadapt/adapters/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    21348 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/adapters/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.029236 gadapt-0.3.4/gadapt/execution/
--rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3396 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.034733 gadapt-0.3.4/gadapt/factory/
--rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     6349 2024-03-16 18:19:48.000000 gadapt-0.3.4/gadapt/factory/ga_base_factory.py
--rw-rw-rw-   0        0        0    17819 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    29258 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.052234 gadapt-0.3.4/gadapt/ga_model/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     9772 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0     3739 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/decision_variable.py
--rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    13275 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.053232 gadapt-0.3.4/gadapt/operations/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.056732 gadapt-0.3.4/gadapt/operations/cost_finding/
--rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/cost_finding/__init__.py
--rw-rw-rw-   0        0        0     1432 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/cost_finding/elitism_cost_finder.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.065734 gadapt-0.3.4/gadapt/operations/crossover/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/crossover/__init__.py
--rw-rw-rw-   0        0        0     7678 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1464 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.080735 gadapt-0.3.4/gadapt/operations/exit_check/
--rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/exit_check/__init__.py
--rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.089233 gadapt-0.3.4/gadapt/operations/gene_combination/
--rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.090734 gadapt-0.3.4/gadapt/operations/immigration/
--rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.099232 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.104732 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.107233 gadapt-0.3.4/gadapt/operations/mutation/
--rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.120734 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0     1240 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     1319 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      720 2024-03-16 18:15:51.000000 gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.145733 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/
--rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/__init__.py
--rw-rw-rw-   0        0        0      328 2024-03-16 18:16:05.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
--rw-rw-rw-   0        0        0     2232 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
--rw-rw-rw-   0        0        0     2287 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
--rw-rw-rw-   0        0        0      344 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.199733 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/
--rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1674 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1728 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/composed_population_mutator.py
--rw-rw-rw-   0        0        0     1813 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1738 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/cross_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     2170 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1021 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.205234 gadapt-0.3.4/gadapt/operations/parent_selection/
--rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/operations/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.4/gadapt/operations/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.213734 gadapt-0.3.4/gadapt/operations/sampling/
--rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.4/gadapt/operations/sampling/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.4/gadapt/operations/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.218733 gadapt-0.3.4/gadapt/operations/variable_update/
--rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/variable_update/__init__.py
--rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/operations/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2567 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/operations/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.221734 gadapt-0.3.4/gadapt/utils/
--rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.4/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.4/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     2901 2024-04-06 20:11:32.000000 gadapt-0.3.4/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:16:33.223234 gadapt-0.3.4/gadapt.egg-info/
--rw-rw-rw-   0        0        0    22076 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4209 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 20:16:32.000000 gadapt-0.3.4/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0      111 2024-04-06 20:16:33.227234 gadapt-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-04-06 20:15:45.000000 gadapt-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.253694 gadapt-0.3.5/
+-rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0    22185 2024-04-09 20:34:01.252693 gadapt-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    21860 2024-04-09 20:15:45.000000 gadapt-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.835191 gadapt-0.3.5/gadapt/
+-rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.875194 gadapt-0.3.5/gadapt/adapters/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.879191 gadapt-0.3.5/gadapt/adapters/ga_logging/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/adapters/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.5/gadapt/adapters/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.881191 gadapt-0.3.5/gadapt/adapters/string_operation/
+-rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/adapters/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.884691 gadapt-0.3.5/gadapt/adapters/validation/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/validation/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.5/gadapt/adapters/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    22949 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/adapters/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.888190 gadapt-0.3.5/gadapt/execution/
+-rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.892692 gadapt-0.3.5/gadapt/factory/
+-rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     6432 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/factory/ga_base_factory.py
+-rw-rw-rw-   0        0        0    17510 2024-04-09 20:31:41.000000 gadapt-0.3.5/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    29258 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.081193 gadapt-0.3.5/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     9788 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0     3739 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/ga_model/decision_variable.py
+-rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    13440 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.082192 gadapt-0.3.5/gadapt/operations/
+-rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.3.5/gadapt/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.085193 gadapt-0.3.5/gadapt/operations/cost_finding/
+-rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1466 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/operations/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/cost_finding/elitism_cost_finder.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.089693 gadapt-0.3.5/gadapt/operations/crossover/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7691 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/operations/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1474 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/operations/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.094693 gadapt-0.3.5/gadapt/operations/exit_check/
+-rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.099193 gadapt-0.3.5/gadapt/operations/gene_combination/
+-rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.100693 gadapt-0.3.5/gadapt/operations/immigration/
+-rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.105694 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.110193 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.111692 gadapt-0.3.5/gadapt/operations/mutation/
+-rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.151193 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      838 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1522 2024-04-09 20:29:12.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1549 2024-04-09 20:31:11.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1921 2024-04-09 20:31:54.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1315 2024-04-09 20:32:04.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1969 2024-04-09 20:29:48.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      644 2024-04-09 20:32:12.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1403 2024-04-09 20:29:32.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      593 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.157194 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/
+-rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/__init__.py
+-rw-rw-rw-   0        0        0      391 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+-rw-rw-rw-   0        0        0     2272 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+-rw-rw-rw-   0        0        0     2388 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
+-rw-rw-rw-   0        0        0      445 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.207694 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2088 2024-04-09 20:30:21.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1372 2024-04-09 20:32:26.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1784 2024-04-09 20:30:08.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1308 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1306 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2624 2024-04-09 20:30:39.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      722 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-09 20:30:49.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      663 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.213694 gadapt-0.3.5/gadapt/operations/parent_selection/
+-rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/operations/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.5/gadapt/operations/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.226694 gadapt-0.3.5/gadapt/operations/sampling/
+-rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.5/gadapt/operations/sampling/__init__.py
+-rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.5/gadapt/operations/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.232193 gadapt-0.3.5/gadapt/operations/variable_update/
+-rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2565 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.237194 gadapt-0.3.5/gadapt/utils/
+-rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.241195 gadapt-0.3.5/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    22185 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5215 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2024-04-09 20:34:01.267696 gadapt-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      512 2024-04-09 20:33:52.000000 gadapt-0.3.5/setup.py
```

### Comparing `gadapt-0.3.4/LICENSE` & `gadapt-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/PKG-INFO` & `gadapt-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.4
+Version: 0.3.5
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # GAdapt: Self-Adaptive Genetic Algorithm
 [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
 # What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
 
 # Installation
 To install **GAdapt**, use **pip** with the following command:
 
 ```
 pip install gadapt
@@ -162,15 +162,15 @@
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
 **gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
@@ -279,38 +279,43 @@
 
 Example of customisation of GAdapt by introducing a new class for mutation of population:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_population_mutator import BasePopulationMutator
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
 
-class BottomPopulationMutator(BasePopulationMutator):
+BaseChromosomeMutationRateDeterminator
+
+
+class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
     """
     Population mutator which selects mutating chromosomes from the bottom of
     existing unallocated chromosoms 
     """
 
     def _mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
             population, None
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-            len(unallocated_chromosomes) - number_of_mutation_chromosomes : 
-        ]
+                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   ]
         for c in chromosomes_for_mutation:
             c.mutate(population.options.number_of_mutation_genes)
 
+
 def some_func(args):
-      return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+    return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+
 
 custom_factory = GAFactory()
 custom_factory.population_mutator = BottomPopulationMutator()
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
-ga.add(-5, 5, 0.1) 
+ga.add(-5, 5, 0.1)
 
 print(ga.execute())
 ```
```

### Comparing `gadapt-0.3.4/README.md` & `gadapt-0.3.5/gadapt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+Metadata-Version: 2.1
+Name: gadapt
+Version: 0.3.5
+Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
+Home-page: https://github.com/bpzoran/gadapt
+Author: Zoran Jankovic
+Author-email: bpzoran@yahoo.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+
 # GAdapt: Self-Adaptive Genetic Algorithm
 [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
 # What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
 
 # Installation
 To install **GAdapt**, use **pip** with the following command:
 
 ```
 pip install gadapt
@@ -151,15 +162,15 @@
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
 **gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
@@ -268,38 +279,43 @@
 
 Example of customisation of GAdapt by introducing a new class for mutation of population:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_population_mutator import BasePopulationMutator
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
+
+BaseChromosomeMutationRateDeterminator
 
-class BottomPopulationMutator(BasePopulationMutator):
+
+class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
     """
     Population mutator which selects mutating chromosomes from the bottom of
     existing unallocated chromosoms 
     """
 
     def _mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
             population, None
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-            len(unallocated_chromosomes) - number_of_mutation_chromosomes : 
-        ]
+                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   ]
         for c in chromosomes_for_mutation:
             c.mutate(population.options.number_of_mutation_genes)
 
+
 def some_func(args):
-      return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+    return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+
 
 custom_factory = GAFactory()
 custom_factory.population_mutator = BottomPopulationMutator()
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
-ga.add(-5, 5, 0.1) 
+ga.add(-5, 5, 0.1)
 
 print(ga.execute())
-```
+```
```

### Comparing `gadapt-0.3.4/gadapt/adapters/ga_logging/logging_settings.py` & `gadapt-0.3.5/gadapt/adapters/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/adapters/string_operation/ga_strings.py` & `gadapt-0.3.5/gadapt/adapters/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/adapters/validation/base_options_validator.py` & `gadapt-0.3.5/gadapt/adapters/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/adapters/validation/common_options_validator.py` & `gadapt-0.3.5/gadapt/adapters/validation/common_options_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,20 +258,55 @@
             rslt &= False
         elif not isinstance(self.options.max_attempt_no, int):
             self._add_message("Max Attempt No must be type int!")
             rslt &= False
         elif self.options.max_attempt_no < 1 or self.options.max_attempt_no > 65536:
             self._add_message("Max Attempt No must be type an int between 1 and 65536!")
             rslt &= False
+        if (
+            self.options.chromosome_mutation == definitions.CROSS_DIVERSITY
+            or definitions.CROSS_DIVERSITY in self.options.chromosome_mutation
+        ):
+            if self.options.cross_diversity_mutation_gene_selection is None:
+                self._add_message(
+                    "Cross Diversity Mutation Gene Selection must not be None!"
+                )
+                rslt &= False
+            elif not isinstance(
+                self.options.cross_diversity_mutation_gene_selection, str
+            ):
+                self._add_message(
+                    "Cross Diversity Mutation Gene Selection must be type str!"
+                )
+                rslt &= False
         if self.options.chromosome_mutation is None:
             self._add_message("Chromosome Mutation must not be None!")
             rslt &= False
         elif not isinstance(self.options.chromosome_mutation, str):
             self._add_message("Chromosome Mutation must be type str!")
             rslt &= False
+        elif definitions.PARAM_SEPARATOR in self.options.chromosome_mutation:
+            mutator_strings = [
+                ms.strip()
+                for ms in self.options.chromosome_mutation.split(
+                    definitions.PARAM_SEPARATOR
+                )
+            ]
+            for mutator_string in mutator_strings:
+                if mutator_string not in definitions.CHROMOSOME_MUTATOR_STRINGS:
+                    self._add_message(
+                        "Invalid value of Chromosome Mutation:\
+                            {0}. Allowed values: {1}".format(
+                            mutator_string,
+                            self._get_allowed_values(
+                                definitions.CHROMOSOME_MUTATOR_STRINGS
+                            ),
+                        )
+                    )
+                    rslt &= False
         elif (
             self.options.chromosome_mutation
             not in definitions.CHROMOSOME_MUTATOR_STRINGS
         ):
             self._add_message(
                 "Invalid value of Chromosome Mutation: {0}. Allowed values: {1}".format(
                     self.options.chromosome_mutation,
```

### Comparing `gadapt-0.3.4/gadapt/execution/ga_executor.py` & `gadapt-0.3.5/gadapt/execution/ga_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,49 +31,49 @@
             results.messages.append(
                 (
                     message_levels.WARNING,
                     "Logging failed. Error message: {exc}".format(exc=str(ex)),
                 )
             )
             self.ga_options.logging = False
-        try:
-            chromosome_mutator = self.factory.get_chromosome_mutator()
-            population_mutator = self.factory.get_population_mutator()
-            exit_checker = self.factory.get_exit_checker()
-            cost_finder = self.factory.get_cost_finder()
-            population_immigrator = self.factory.get_population_immigrator()
-            chromosome_immigrator = self.factory.get_chromosome_immigrator()
-            selector = self.factory.get_parent_selector()
-            crossover = self.factory.get_crossover()
-            variable_updater = self.factory.get_variable_updater()
-            gene_mutator = self.factory.get_gene_mutator()
-            for dv in self.ga_options.decision_variables:
-                dv.gene_mutator = gene_mutator
-            population = Population(
-                self.ga_options,
-                chromosome_mutator=chromosome_mutator,
-                population_mutator=population_mutator,
-                exit_checker=exit_checker,
-                cost_finder=cost_finder,
-                population_immigrator=population_immigrator,
-                chromosome_immigrator=chromosome_immigrator,
-                parent_selector=selector,
-                crossover=crossover,
-                variable_updater=variable_updater,
-            )
+        # try:
+        chromosome_mutator = self.factory.get_chromosome_mutator()
+        population_mutator = self.factory.get_population_mutator()
+        exit_checker = self.factory.get_exit_checker()
+        cost_finder = self.factory.get_cost_finder()
+        population_immigrator = self.factory.get_population_immigrator()
+        chromosome_immigrator = self.factory.get_chromosome_immigrator()
+        selector = self.factory.get_parent_selector()
+        crossover = self.factory.get_crossover()
+        variable_updater = self.factory.get_variable_updater()
+        gene_mutator = self.factory.get_gene_mutator()
+        for dv in self.ga_options.decision_variables:
+            dv.gene_mutator = gene_mutator
+        population = Population(
+            self.ga_options,
+            chromosome_mutator=chromosome_mutator,
+            population_mutator=population_mutator,
+            exit_checker=exit_checker,
+            cost_finder=cost_finder,
+            population_immigrator=population_immigrator,
+            chromosome_immigrator=chromosome_immigrator,
+            parent_selector=selector,
+            crossover=crossover,
+            variable_updater=variable_updater,
+        )
+        population.find_costs()
+        while not population.exit():
+            population.immigrate()
+            population.mate()
+            population.mutate()
             population.find_costs()
-            while not population.exit():
-                population.immigrate()
-                population.mate()
-                population.mutate()
-                population.find_costs()
-            if population.timeout_expired:
-                results.messages.append((message_levels.WARNING, "Timeout expired!"))
-            best_individual = population.best_individual
-            results.min_cost = population.min_cost
-            results.number_of_iterations = population.population_generation
-            for g in best_individual:
-                results.result_values[g.decision_variable.variable_id] = g.variable_value
-        except Exception as ex:
-            results.success = False
-            results.messages.append((message_levels.ERROR, str(ex)))
+        if population.timeout_expired:
+            results.messages.append((message_levels.WARNING, "Timeout expired!"))
+        best_individual = population.best_individual
+        results.min_cost = population.min_cost
+        results.number_of_iterations = population.population_generation
+        for g in best_individual:
+            results.result_values[g.decision_variable.variable_id] = g.variable_value
+        # except Exception as ex:
+        #    results.success = False
+        #    results.messages.append((message_levels.ERROR, str(ex)))
         return results
```

### Comparing `gadapt-0.3.4/gadapt/factory/ga_base_factory.py` & `gadapt-0.3.5/gadapt/factory/ga_base_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from gadapt.operations.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.immigration.population_immigration.base_population_immigrator import (
     BasePopulationImmigrator,
 )
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
 from gadapt.operations.mutation.gene_mutation.base_gene_mutator import BaseGeneMutator
-from gadapt.operations.mutation.population_mutation.base_population_mutator import (
-    BasePopulationMutator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
 from gadapt.operations.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
 
 """
     Factory definition for creating  class instances based on GA options
 """
@@ -64,15 +64,15 @@
         """
         Chromosome Immigrator Instance
         """
         if self.chromosome_immigrator is None:
             self.chromosome_immigrator = self._get_chromosome_immigrator()
         return self.chromosome_immigrator
 
-    def get_chromosome_mutator(self) -> BaseChromosomeMutator:
+    def get_chromosome_mutator(self) -> BaseGeneMutationSelector:
         """
         Chromosome Mutator Instance
         """
         if self.chromosome_mutator is None:
             self.chromosome_mutator = self._get_chromosome_mutator()
         return self.chromosome_mutator
 
@@ -80,15 +80,15 @@
         """
         Gene Mutator Instance
         """
         if self.gene_mutator is None:
             self.gene_mutator = self._get_gene_mutator()
         return self.gene_mutator
 
-    def get_population_mutator(self) -> BasePopulationMutator:
+    def get_population_mutator(self) -> BaseChromosomeMutationRateDeterminator:
         """
         Population Mutator Instance
         """
         if self.population_mutator is None:
             self.population_mutator = self._get_population_mutator()
         return self.population_mutator
 
@@ -150,29 +150,29 @@
     def _get_chromosome_immigrator(self) -> BaseChromosomeImmigrator:
         """
         Chromosome Immigrator Instance
         """
         pass
 
     @abstractmethod
-    def _get_chromosome_mutator(self) -> BaseChromosomeMutator:
+    def _get_chromosome_mutator(self) -> BaseGeneMutationSelector:
         """
         Chromosome Mutator Instance
         """
         pass
 
     @abstractmethod
     def _get_gene_mutator(self) -> BaseGeneMutator:
         """
         Gene Mutator Instance
         """
         pass
 
     @abstractmethod
-    def _get_population_mutator(self) -> BasePopulationMutator:
+    def _get_population_mutator(self) -> BaseChromosomeMutationRateDeterminator:
         """
         Population Mutator Instance
         """
         pass
 
     @abstractmethod
     def _get_parent_selector(self) -> BaseParentSelector:
```

### Comparing `gadapt-0.3.4/gadapt/ga.py` & `gadapt-0.3.5/gadapt/ga.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         self.cross_diversity_mutation_gene_selection = (
             cross_diversity_mutation_gene_selection
         )
         self.parent_diversity_mutation_chromosome_selection = (
             parent_diversity_mutation_chromosome_selection
         )
         self.timeout = timeout
-        self._current_gv_id = 0
+        self._current_dv_id = 0
         self._factory = factory
 
     def execute(self) -> GAResults:
         """
         Executes genetic algorithm optimization base on the
         provided parameters and arguments.
         """
@@ -245,20 +245,20 @@
         """
         if step < 0.000000000000001:
             step = 0.000000000000001
         if (not isinstance(min_value, float) and not isinstance(min_value, int)) or (
             not isinstance(max_value, float) and not isinstance(max_value, int)
         ):
             raise Exception("min value, max value and step must be numerical values!")
-        decision_variable = DecisionVariable(self._current_gv_id)
+        decision_variable = DecisionVariable(self._current_dv_id)
         decision_variable.min_value = min_value
         decision_variable.max_value = max_value
         decision_variable.step = step
         self._decision_variables.append(decision_variable)
-        self._current_gv_id += 1
+        self._current_dv_id += 1
 
     @property
     def cost_function(self):
         """
         Custom function for the cost calculation (fitness). The optimisation goal
         is minimising the output of the cost function.
         cost_function must be the function with one argument -
```

### Comparing `gadapt-0.3.4/gadapt/ga_model/chromosome.py` & `gadapt-0.3.5/gadapt/ga_model/chromosome.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from typing import List
 from gadapt.ga_model.gene import Gene
 from gadapt.ga_model.decision_variable import DecisionVariable
 from gadapt.ga_model.ranking_model import RankingModel
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
 import gadapt.ga_model.definitions as definitions
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 
 
 class Chromosome(RankingModel):
     def __init__(
         self,
-        mutator: BaseChromosomeMutator,
+        mutator: BaseGeneMutationSelector,
         immigrator: BaseChromosomeImmigrator,
         population_generation: int,
     ):
         """
         Chromosome class.
         Chromosome is a part of the Population. Chromosome consists of Genes.
         Args:
@@ -94,22 +94,22 @@
 
     def _get_chromosome_string(self):
         if self._chromosome_string is None:
             self._chromosome_string = self._to_string()
         return self._chromosome_string
 
     @property
-    def mutator(self) -> BaseChromosomeMutator:
+    def mutator(self) -> BaseGeneMutationSelector:
         """
         Mutation algorithm
         """
         return self._mutator
 
     @mutator.setter
-    def mutator(self, value: BaseChromosomeMutator):
+    def mutator(self, value: BaseGeneMutationSelector):
         self._mutator = value
 
     @property
     def immigrator(self) -> BaseChromosomeImmigrator:
         """
         Immigration algorithm
         """
```

### Comparing `gadapt-0.3.4/gadapt/ga_model/decision_variable.py` & `gadapt-0.3.5/gadapt/ga_model/decision_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,19 +72,19 @@
     @step.setter
     def step(self, value: float):
         self._decimal_places = self._get_decimal_places(value)
         self._step = value
 
     def _get_decimal_places(self, num):
         num_str = str(num)
-        if 'e-' in num_str:
-            num_str = num_str.split('e-')[-1]
+        if "e-" in num_str:
+            num_str = num_str.split("e-")[-1]
             return int(num_str)
-        if '.' in num_str:
-            _, fractional_part = num_str.split('.')
+        if "." in num_str:
+            _, fractional_part = num_str.split(".")
             return len(fractional_part)
         else:
             return 0
 
     @property
     def decimal_places(self) -> int:
         """
```

### Comparing `gadapt-0.3.4/gadapt/ga_model/definitions.py` & `gadapt-0.3.5/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/ga_model/ga_options.py` & `gadapt-0.3.5/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/ga_model/ga_results.py` & `gadapt-0.3.5/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/ga_model/gene.py` & `gadapt-0.3.5/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/ga_model/population.py` & `gadapt-0.3.5/gadapt/ga_model/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,50 +12,50 @@
 from gadapt.ga_model.gene import Gene
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.immigration.population_immigration.base_population_immigrator import (
     BasePopulationImmigrator,
 )
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
-from gadapt.operations.mutation.population_mutation.base_population_mutator import (
-    BasePopulationMutator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
 from gadapt.operations.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.operations.variable_update.base_variable_updater import BaseVariableUpdater
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
 import gadapt.utils.ga_utils as ga_utils
 
 
 class Population:
     def __init__(
         self,
         options: GAOptions,
-        chromosome_mutator: BaseChromosomeMutator,
-        population_mutator: BasePopulationMutator,
+        chromosome_mutator: BaseGeneMutationSelector,
+        population_mutator: BaseChromosomeMutationRateDeterminator,
         exit_checker: BaseExitChecker,
         cost_finder: BaseCostFinder,
         population_immigrator: BasePopulationImmigrator,
         chromosome_immigrator: BaseChromosomeImmigrator,
         parent_selector: BaseParentSelector,
         crossover: BaseCrossover,
         variable_updater: BaseVariableUpdater,
     ):
         """Population for the genetic algorithm. It contains a collection of\
             chromosomes, as well as additional parameters
 
         Args:
 
             options (GAOptions): Genetic Algorithm Options
-            chromosome_mutator (BaseChromosomeMutator): Chromosome Mutator Instance
-            population_mutator (BasePopulationMutator): Population Mutator Instance
+            chromosome_mutator (BaseGeneMutationSelector): Chromosome Mutator Instance
+            population_mutator (BaseChromosomeMutationRateDeterminator): Population Mutator Instance
             exit_checker (BaseExitChecker): Exit Checker Instance
             cost_finder (BaseCostFinder): Cost Finder Instance
             population_immigrator (BasePopulationImmigrator):
             Population Immigrator Instance
             chromosome_immigrator (BaseChromosomeImmigrator):
             Chromosome Immigrator Instance
             parent_selector (BaseParentSelector): Parent Selector Instance
@@ -198,33 +198,33 @@
         return self._population_generation
 
     @population_generation.setter
     def population_generation(self, value):
         self._population_generation = value
 
     @property
-    def chromosome_mutator(self) -> BaseChromosomeMutator:
+    def chromosome_mutator(self) -> BaseGeneMutationSelector:
         """
         Chromosome mutator algorithm
         """
         return self._chromosome_mutator
 
     @chromosome_mutator.setter
-    def chromosome_mutator(self, value: BaseChromosomeMutator):
+    def chromosome_mutator(self, value: BaseGeneMutationSelector):
         self._chromosome_mutator = value
 
     @property
-    def population_mutator(self) -> BasePopulationMutator:
+    def population_mutator(self) -> BaseChromosomeMutationRateDeterminator:
         """
         Population mutator algorithm
         """
         return self._population_mutator
 
     @population_mutator.setter
-    def population_mutator(self, value: BasePopulationMutator):
+    def population_mutator(self, value: BaseChromosomeMutationRateDeterminator):
         self._population_mutator = value
 
     @property
     def cost_finder(self) -> BaseCostFinder:
         """
         Cost finding algorithm
         """
@@ -400,15 +400,19 @@
     def update_variables(self):
         """
         Updates decision variables
         """
         self.variable_updater.update_variables(self)
 
     def calculate_average_cost_step(self):
-        allocated_values = [c.cost_value for c in self.chromosomes if c.cost_value is not None and not math.isnan(c.cost_value)]        
+        allocated_values = [
+            c.cost_value
+            for c in self.chromosomes
+            if c.cost_value is not None and not math.isnan(c.cost_value)
+        ]
         if allocated_values:
             return ga_utils.average_difference(allocated_values)
         return float("NaN")
 
 
 class PopulationIterator:
     def __init__(self, population):
```

### Comparing `gadapt-0.3.4/gadapt/ga_model/ranking_model.py` & `gadapt-0.3.5/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/cost_finding/base_cost_finder.py` & `gadapt-0.3.5/gadapt/operations/cost_finding/base_cost_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,10 @@
         Finds costs for the population
 
         Args:
             population (Population): The population to find costs for each chromosome
         """
         self._find_costs_for_population(population)
         if math.isnan(population.average_cost_step_in_first_population):
-            population.average_cost_step_in_first_population = population.calculate_average_cost_step()
+            population.average_cost_step_in_first_population = (
+                population.calculate_average_cost_step()
+            )
```

### Comparing `gadapt-0.3.4/gadapt/operations/cost_finding/elitism_cost_finder.py` & `gadapt-0.3.5/gadapt/operations/cost_finding/elitism_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/crossover/base_crossover.py` & `gadapt-0.3.5/gadapt/operations/crossover/base_crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from abc import ABC, abstractmethod
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.gene import Gene
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
 from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
 import gadapt.utils.ga_utils as ga_utils
 
 
 class BaseCrossover(ABC):
     """Base Crossover Class
 
     Args:
         gene_combination (BaseGeneCombination): the algorithm
         for how genes are to be combined
-        mutator (BaseChromosomeMutator): mutation algorithm to
+        mutator (BaseGeneMutationSelector): mutation algorithm to
         be passed to offspring chromosomes
         immigrator (BaseChromosomeImmigrator): immigration algorithm
         to be passed to offspring chromosomes
         mutation_on_both_sides (bool): indicates if offspring chromosomes
         should be mutated on both sides with the same probability
     """
 
     def __init__(
         self,
         gene_combination: BaseGeneCombination,
-        mutator: BaseChromosomeMutator,
+        mutator: BaseGeneMutationSelector,
         immigrator: BaseChromosomeImmigrator,
         mutation_on_both_sides: bool = True,
     ):
         self._mutation_on_both_sides = True
         self._gene_combination = gene_combination
         self._mutator = mutator
         self._immigrator = immigrator
```

### Comparing `gadapt-0.3.4/gadapt/operations/crossover/uniform_crossover.py` & `gadapt-0.3.5/gadapt/operations/crossover/uniform_crossover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Tuple
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.gene import Gene
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
 from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
 
 
 class UniformCrossover(BaseCrossover):
     """
     Uniform Crossover.
     Genes from parents' chromosomes are combined in a uniform way
     """
 
     def __init__(
         self,
         var_combination: BaseGeneCombination,
-        mutator: BaseChromosomeMutator,
+        mutator: BaseGeneMutationSelector,
         immigrator: BaseChromosomeImmigrator,
     ):
         super(UniformCrossover, self).__init__(var_combination, mutator, immigrator)
 
     def _get_mother_father_genes(
         self, mother: Chromosome, father: Chromosome
     ) -> Tuple[Gene, Gene]:
```

### Comparing `gadapt-0.3.4/gadapt/operations/exit_check/base_exit_checker.py` & `gadapt-0.3.5/gadapt/operations/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/exit_check/requested_cost_exit_checker.py` & `gadapt-0.3.5/gadapt/operations/exit_check/requested_cost_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/gene_combination/base_gene_combination.py` & `gadapt-0.3.5/gadapt/operations/gene_combination/base_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/gene_combination/blending_gene_combination.py` & `gadapt-0.3.5/gadapt/operations/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.3.5/gadapt/operations/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-from gadapt.ga_model.chromosome import Chromosome
-import random
-from gadapt.operations.mutation.chromosome_mutation.random_chromosome_mutator import (
-    RandomChromosomeMutator,
+import gadapt.utils.ga_utils as ga_utils
+
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
+    BaseGeneMutationRateDeterminator,
 )
-from gadapt.operations.sampling.base_sampling import BaseSampling
 
 
-class CrossDiversityChromosomeMutator(RandomChromosomeMutator):
+class CrossDiversityGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
     """
-    Mutation of chromosome based on cross diversity of genetic\
-        variables in the population.
+    Determines the number of mutation genes in a chromosome based on the cross diversity coefficient of the decision variables.
     """
 
-    def __init__(self, sampling: BaseSampling) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
-        self._sampling = sampling
 
-    def _mutate_chromosome(self, c: Chromosome, number_of_mutation_genes: int):
-        if number_of_mutation_genes == 0:
-            return
-        x_genes = [g for g in c]
-        x_genes.sort(key=lambda g: -g.decision_variable.cross_diversity_coefficient)
-        if number_of_mutation_genes > len(x_genes):
-            number_of_mutation_genes = len(x_genes)
-        number_of_mutation_genes = random.randint(1, number_of_mutation_genes)
-        genes_for_mutation = self._sampling.get_sample(
-            x_genes,
-            number_of_mutation_genes,
-            lambda g: g.decision_variable.cross_diversity_coefficient,
-        )
-        for g in genes_for_mutation:
-            g.mutate()
-            self._gene_mutated(g, c)
+    def _get_number_of_mutation_genes(
+        self, chromosome, max_number_of_mutation_genes
+    ) -> int:
+        decision_variables = [g.decision_variable for g in chromosome]
+
+        def get_mutation_rate() -> float:
+            avg_rsd = ga_utils.average(
+                [dv.cross_diversity_coefficient for dv in decision_variables]
+            )
+            if avg_rsd > 1:
+                avg_rsd = 1
+            if avg_rsd < 0:
+                avg_rsd = 0
+            return 1 - avg_rsd
+
+        mutation_rate = get_mutation_rate()
+        f_return_value = mutation_rate * float(max_number_of_mutation_genes)
+        f_return_value_rounded = round(f_return_value)
+        if f_return_value_rounded == 0:
+            f_return_value_rounded = 1
+        return f_return_value_rounded
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-from gadapt.ga_model.chromosome import Chromosome
 import random
 
-from gadapt.operations.mutation.chromosome_mutation.base_chromosome_mutator import (
-    BaseChromosomeMutator,
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
+    BaseGeneMutationRateDeterminator,
 )
 
 
-class RandomChromosomeMutator(BaseChromosomeMutator):
+class RandomGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
     """
-    Random mutation of the chromosome.
+    Determines the random number of mutation genes in a chromosome between 1 and the maximum number of mutation genes specified.
     """
 
-    def _mutate_chromosome(self, c: Chromosome, number_of_mutation_genes: int):
-        if number_of_mutation_genes == 0:
-            return
-        genes_to_mutate = list(c)
-        random.shuffle(genes_to_mutate)
-        var_num = random.randint(1, number_of_mutation_genes)
-        for g in genes_to_mutate[:var_num]:
-            g.mutate()
-            self._gene_mutated(g, c)
+    def __init__(
+        self,
+    ) -> None:
+        super().__init__()
 
-        return var_num
+    def _get_number_of_mutation_genes(
+        self, chromosome, max_number_of_mutation_genes
+    ) -> int:
+        return random.randint(1, max_number_of_mutation_genes)
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 class ExtremePointedGeneMutator(RandomGeneMutator):
 
     def _make_mutated_value(self, g: Gene):
         return self._make_mutation(g)
 
     def _make_rounded_random_value_below_or_above(self, g: Gene):
         return round(
-            self._make_random_value_below_or_above(g), g.decision_variable.decimal_places
+            self._make_random_value_below_or_above(g),
+            g.decision_variable.decimal_places,
         )
 
     def _make_random_value_below_or_above(self, g: Gene):
         if get_rand_bool():
             return self._make_random_value_above(g)
         return self._make_random_value_below(g)
 
@@ -28,15 +29,17 @@
         number_of_steps = random.randint(
             0,
             round(
                 (g.variable_value - g.decision_variable.min_value)
                 / g.decision_variable.step
             ),
         )
-        return g.decision_variable.min_value + number_of_steps * g.decision_variable.step
+        return (
+            g.decision_variable.min_value + number_of_steps * g.decision_variable.step
+        )
 
     def _make_random_value_above(self, g: Gene):
         if g.variable_value == g.decision_variable.max_value:
             return g.decision_variable.make_random_value()
         number_of_steps = random.randint(
             0,
             round(
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 import math
 from gadapt.ga_model.gene import Gene
 from gadapt.operations.mutation.gene_mutation.random_gene_mutator import (
     RandomGeneMutator,
 )
 from gadapt.utils.ga_utils import (
     get_rand_bool,
-    get_rand_bool_with_probability,
     normally_distributed_random,
 )
 import numpy as np
 
+
 class NormalDistributionGeneMutator(RandomGeneMutator):
+    """
+    Generates random or normally distributed values.
+    """
 
     def _make_mutated_value(self, g: Gene):
         return self._make_random_or_normally_distributed_random_value(g)
-        
-    
+
     def _execute_function_until_value_changed(self, f, g: Gene):
-        current_gene_value = g.variable_value    
-        new_gene_value = current_gene_value    
+        current_gene_value = g.variable_value
+        new_gene_value = current_gene_value
         number_of_attempts = 5
         i = 0
         while True:
             new_gene_value = f(g)
             i += 1
             if new_gene_value != current_gene_value or i >= number_of_attempts:
                 break
         return new_gene_value
 
-
     def _make_random_or_normally_distributed_random_value(self, g: Gene):
         if get_rand_bool():
-            return self._execute_function_until_value_changed(super()._make_mutated_value, g)
+            return self._execute_function_until_value_changed(
+                super()._make_mutated_value, g
+            )
         else:
-            return self._execute_function_until_value_changed(self._make_normally_distributed_random_value, g)
-        
-    
+            return self._execute_function_until_value_changed(
+                self._make_normally_distributed_random_value, g
+            )
+
     def _calculate_nd_standard_deviation(self, g: Gene):
         min_std_dev = 0.05
         max_std_dev = 0.5
         std_dev_range = max_std_dev - min_std_dev
-        gv_rsd = np.clip(g.decision_variable.cross_diversity_coefficient, 0, 1)        
-        return min_std_dev + (std_dev_range * gv_rsd)
-    
+        dv_rsd = np.clip(g.decision_variable.cross_diversity_coefficient, 0, 1)
+        return min_std_dev + (std_dev_range * dv_rsd)
+
     def _make_normally_distributed_random_value(self, g: Gene):
         curr_value = g.variable_value
         if math.isnan(curr_value):
             curr_value = g.decision_variable.make_random_value()
         range = g.decision_variable.max_value - g.decision_variable.min_value
         mean = (curr_value - g.decision_variable.min_value) / (range)
-        normal_distribution_random_value = normally_distributed_random(mean, self._calculate_nd_standard_deviation(g), 0, 1)
+        normal_distribution_random_value = normally_distributed_random(
+            mean, self._calculate_nd_standard_deviation(g), 0, 1
+        )
         number_of_steps = round(
             (normal_distribution_random_value * range) / g.decision_variable.step
         )
-        return g.decision_variable.min_value + number_of_steps * g.decision_variable.step
+        return (
+            g.decision_variable.min_value + number_of_steps * g.decision_variable.step
+        )
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 from abc import ABC, abstractmethod
 import math
 import random
 from typing import List
 from gadapt.ga_model.chromosome import Chromosome
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
+)
 
 
-class BasePopulationMutator(ABC):
+class BaseChromosomeMutationSelector(ABC):
+    """
+    Selects and mutates the chromosomes in the population based on a specified number of mutated chromosomes.
+    """
+
     def mutate(self, population):
         """
         Mutates chromosomes in the population
         Args:
             population: Population to mutate
         """
         number_of_mutated_chromosomes = (
             population.options.number_of_mutation_chromosomes
         )
         self._mutate_population(population, number_of_mutated_chromosomes)
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+    ) -> None:
         """
         Base class for mutating chromosomes in population
         Args:
             options: genetic algorithm options
         """
         super().__init__()
+        self._chromosome_mutation_rate_determinator = (
+            chromosome_mutation_rate_determinator
+        )
 
     @abstractmethod
     def _mutate_population(self, population, number_of_mutated_chromosomes):
         pass
 
     def _get_unallocated_chromosomes(
         self, population, sort_key_function=None
@@ -43,10 +56,7 @@
         lst = [c for c in population if (unallocated_chromosomes_condition(c))]
         if sort_key_function is not None:
             lst.sort(key=sort_key_function)
         return lst
 
     def _sort_key_random(self, c: Chromosome):
         return random.random()
-    
-    def requires_continuous_execution_in_composed_mutation(self) -> bool:
-        return False
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-from ast import List
 import random
 from gadapt.ga_model.chromosome import Chromosome
-from gadapt.operations.mutation.population_mutation.base_population_mutator import (
-    BasePopulationMutator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
 from gadapt.operations.sampling.base_sampling import BaseSampling
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
+)
 
 
-class ParentDiversityPopulationMutator(BasePopulationMutator):
+class ParentDiversityChromosomeMutationSelector(BaseChromosomeMutationSelector):
     """
-    Population mutator based on parent diversity
+    Selects and mutates chromosomes in a population based on their parent diversity.
     """
 
-    def __init__(self, sampling: BaseSampling) -> None:
-        super().__init__()
+    def __init__(
+        self,
+        chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+        sampling: BaseSampling,
+    ) -> None:
+        super().__init__(chromosome_mutation_rate_determinator)
         self._sampling = sampling
 
     def _sort_key_parent_diversity_random(self, c: Chromosome):
         return (c.parent_diversity, random.random())
 
-    def _mutate_population(self, population, number_of_mutation_chromosomes):
+    def _mutate_population(self, population, max_number_of_mutation_chromosomes):
         if population is None:
             raise Exception("Population must not be null")
-        unallocated_chromosomes: List[Chromosome] = self._get_unallocated_chromosomes(
+        number_of_mutation_chromosomes = self._chromosome_mutation_rate_determinator.get_number_of_mutation_chromosomes(
+            population, max_number_of_mutation_chromosomes
+        )
+        unallocated_chromosomes: list[Chromosome] = self._get_unallocated_chromosomes(
             population, self._sort_key_parent_diversity_random
         )
-        chromosomes_for_mutation: List[Chromosome] = []
+        chromosomes_for_mutation: list[Chromosome] = []
         if population.options.must_mutate_for_same_parents:
             chromosomes_for_mutation = [
                 c for c in unallocated_chromosomes if c.parent_diversity == 0
             ]
         chromosomes_for_mutation_count = len(chromosomes_for_mutation)
         rest_number = number_of_mutation_chromosomes - chromosomes_for_mutation_count
         if rest_number > 0:
@@ -41,10 +50,7 @@
                 chromosomes_for_mutation = [c for c in unallocated_chromosomes]
             chromosomes_for_mutation = self._sampling.get_sample(
                 chromosomes_for_mutation, rest_number, lambda c: c.parent_diversity
             )
         for c in chromosomes_for_mutation:
             c.mutate(population.options.number_of_mutation_genes)
         return len(chromosomes_for_mutation)
-
-    def requires_continuous_execution_in_composed_mutation(self) -> bool:
-        return True
```

### Comparing `gadapt-0.3.4/gadapt/operations/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-from gadapt.operations.mutation.population_mutation.base_population_mutator import (
-    BasePopulationMutator,
-)
+from abc import ABC, abstractmethod
 
 
-class RandomPopulationMutator(BasePopulationMutator):
+class BaseChromosomeMutationRateDeterminator(ABC):
     """
-    Random population mutator
+    Provides a framework for determining the number of chromosomes to be mutated in a population.
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def _mutate_population(self, population, number_of_mutation_chromosomes):
+    def get_number_of_mutation_chromosomes(
+        self, population, max_number_of_mutation_chromosomes
+    ):
         if population is None:
-            raise Exception("population must not be None")
-        number_of_mutation_genes = population.options.number_of_mutation_genes
-        unallocated_chromosomes = self._get_unallocated_chromosomes(
-            population, self._sort_key_random
+            raise Exception("Population must not be null")
+        return self._get_number_of_mutation_chromosomes(
+            population, max_number_of_mutation_chromosomes
         )
-        chromosomes_for_mutation = unallocated_chromosomes[
-            :number_of_mutation_chromosomes
-        ]
-        for c in chromosomes_for_mutation:
-            c.mutate(number_of_mutation_genes)
-        return number_of_mutation_chromosomes
 
-    def requires_continuous_execution_in_composed_mutation(self) -> bool:
-        return True
+    @abstractmethod
+    def _get_number_of_mutation_chromosomes(
+        self, population, max_number_of_mutation_chromosomes
+    ) -> int:
+        pass
```

### Comparing `gadapt-0.3.4/gadapt/operations/parent_selection/base_parent_selector.py` & `gadapt-0.3.5/gadapt/operations/parent_selection/base_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/parent_selection/sampling_parent_selector.py` & `gadapt-0.3.5/gadapt/operations/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/sampling/base_sampling.py` & `gadapt-0.3.5/gadapt/operations/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/sampling/roulette_wheel_sampling.py` & `gadapt-0.3.5/gadapt/operations/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/sampling/tournament_sampling.py` & `gadapt-0.3.5/gadapt/operations/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/gadapt/operations/variable_update/common_variable_updater.py` & `gadapt-0.3.5/gadapt/operations/variable_update/common_variable_updater.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import statistics as stat
 from gadapt.ga_model.decision_variable import DecisionVariable
-import gadapt.utils.ga_utils as ga_utils
 
 
 class CommonVariableUpdater:
     """
     Common variable updater
     """
 
     def update_variables(self, population):
 
         def scale_values(dv: DecisionVariable, values):
             scaled_values = []
             if dv.min_value == dv.max_value:
-                return [0.5] * len(values)  # If min_val and max_val are the same, return a list of 0.5s
+                return [0.5] * len(
+                    values
+                )  # If min_val and max_val are the same, return a list of 0.5s
 
             for value in values:
                 scaled_value = (value - dv.min_value) / (dv.max_value - dv.min_value)
                 scaled_values.append(scaled_value)
             return scaled_values
 
         # def scale_values(data):
```

### Comparing `gadapt-0.3.4/gadapt/utils/ga_utils.py` & `gadapt-0.3.5/gadapt/utils/ga_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
 
 def normally_distributed_random(mean, std_dev, lower_bound, upper_bound):
     num = np.random.normal(mean, std_dev)
     num = np.clip(num, lower_bound, upper_bound)
     return num
 
+
 def average_difference(diff_list):
     if len(diff_list) < 2:
         return float("NaN")
     diff_list.sort()
-    differences = [diff_list[i+1] - diff_list[i] for i in range(len(diff_list)-1)]
+    differences = [diff_list[i + 1] - diff_list[i] for i in range(len(diff_list) - 1)]
     avg_difference = sum(differences) / len(differences)
-    return avg_difference
+    return avg_difference
```

### Comparing `gadapt-0.3.4/gadapt.egg-info/PKG-INFO` & `gadapt-0.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: gadapt
-Version: 0.3.4
-Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
-Home-page: https://github.com/bpzoran/gadapt
-Author: Zoran Jankovic
-Author-email: bpzoran@yahoo.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
 # GAdapt: Self-Adaptive Genetic Algorithm
 [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
 # What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
 
 # Installation
 To install **GAdapt**, use **pip** with the following command:
 
 ```
 pip install gadapt
@@ -162,15 +151,15 @@
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
 **chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this genetic variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
 **gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
 Supported values:
 - *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
 - *"random"* - Random values are assigned to genes
 
@@ -279,38 +268,43 @@
 
 Example of customisation of GAdapt by introducing a new class for mutation of population:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_population_mutator import BasePopulationMutator
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
+
+BaseChromosomeMutationRateDeterminator
 
-class BottomPopulationMutator(BasePopulationMutator):
+
+class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
     """
     Population mutator which selects mutating chromosomes from the bottom of
     existing unallocated chromosoms 
     """
 
     def _mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
             population, None
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-            len(unallocated_chromosomes) - number_of_mutation_chromosomes : 
-        ]
+                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   ]
         for c in chromosomes_for_mutation:
             c.mutate(population.options.number_of_mutation_genes)
 
+
 def some_func(args):
-      return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+    return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
+
 
 custom_factory = GAFactory()
 custom_factory.population_mutator = BottomPopulationMutator()
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
-ga.add(-5, 5, 0.1) 
+ga.add(-5, 5, 0.1)
 
 print(ga.execute())
-```
+```
```

### Comparing `gadapt-0.3.4/gadapt.egg-info/SOURCES.txt` & `gadapt-0.3.5/gadapt.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -53,29 +53,39 @@
 gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
 gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
 gadapt/operations/immigration/population_immigration/__init__.py
 gadapt/operations/immigration/population_immigration/base_population_immigrator.py
 gadapt/operations/immigration/population_immigration/common_population_immigrator.py
 gadapt/operations/mutation/__init__.py
 gadapt/operations/mutation/chromosome_mutation/__init__.py
-gadapt/operations/mutation/chromosome_mutation/base_chromosome_mutator.py
-gadapt/operations/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
-gadapt/operations/mutation/chromosome_mutation/random_chromosome_mutator.py
+gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
+gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
+gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
+gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
+gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
+gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
+gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
+gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
+gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
 gadapt/operations/mutation/gene_mutation/__init__.py
 gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
 gadapt/operations/mutation/population_mutation/__init__.py
-gadapt/operations/mutation/population_mutation/base_population_mutator.py
-gadapt/operations/mutation/population_mutation/composed_population_mutator.py
-gadapt/operations/mutation/population_mutation/cost_diversity_population_mutator.py
-gadapt/operations/mutation/population_mutation/cross_diversity_population_mutator.py
-gadapt/operations/mutation/population_mutation/parent_diversity_population_mutator.py
-gadapt/operations/mutation/population_mutation/random_population_mutator.py
+gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
+gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
+gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
+gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
+gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
+gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
+gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
+gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
+gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
+gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
 gadapt/operations/parent_selection/__init__.py
 gadapt/operations/parent_selection/base_parent_selector.py
 gadapt/operations/parent_selection/sampling_parent_selector.py
 gadapt/operations/sampling/__init__.py
 gadapt/operations/sampling/base_sampling.py
 gadapt/operations/sampling/from_top_to_bottom_sampling.py
 gadapt/operations/sampling/random_sampling.py
```

### Comparing `gadapt-0.3.4/pyproject.toml` & `gadapt-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.4/setup.py` & `gadapt-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gadapt",
-    version="0.3.4",
+    version="0.3.5",
     author="Zoran Jankovic",
     author_email="bpzoran@yahoo.com",
     url="https://github.com/bpzoran/gadapt",
     packages=find_packages(),
     long_description=open("README.md").read(),
     # Specify the content type explicitly
     long_description_content_type="text/markdown",
```

