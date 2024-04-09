# Comparing `tmp/gadapt-0.3.5.tar.gz` & `tmp/gadapt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gadapt-0.3.5.tar", last modified: Tue Apr  9 20:34:01 2024, max compression
+gzip compressed data, was "gadapt-0.3.6.tar", last modified: Tue Apr  9 20:48:05 2024, max compression
```

## Comparing `gadapt-0.3.5.tar` & `gadapt-0.3.6.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.253694 gadapt-0.3.5/
--rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.5/LICENSE
--rw-rw-rw-   0        0        0    22185 2024-04-09 20:34:01.252693 gadapt-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    21860 2024-04-09 20:15:45.000000 gadapt-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.835191 gadapt-0.3.5/gadapt/
--rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.875194 gadapt-0.3.5/gadapt/adapters/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.879191 gadapt-0.3.5/gadapt/adapters/ga_logging/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/adapters/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.5/gadapt/adapters/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.881191 gadapt-0.3.5/gadapt/adapters/string_operation/
--rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/string_operation/__init__.py
--rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/adapters/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.884691 gadapt-0.3.5/gadapt/adapters/validation/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/adapters/validation/__init__.py
--rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.5/gadapt/adapters/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    22949 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/adapters/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.888190 gadapt-0.3.5/gadapt/execution/
--rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3254 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:00.892692 gadapt-0.3.5/gadapt/factory/
--rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     6432 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/factory/ga_base_factory.py
--rw-rw-rw-   0        0        0    17510 2024-04-09 20:31:41.000000 gadapt-0.3.5/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    29258 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.081193 gadapt-0.3.5/gadapt/ga_model/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     9788 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0     3739 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/ga_model/decision_variable.py
--rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    13440 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.082192 gadapt-0.3.5/gadapt/operations/
--rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.3.5/gadapt/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.085193 gadapt-0.3.5/gadapt/operations/cost_finding/
--rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/cost_finding/__init__.py
--rw-rw-rw-   0        0        0     1466 2024-04-09 20:26:26.000000 gadapt-0.3.5/gadapt/operations/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/cost_finding/elitism_cost_finder.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.089693 gadapt-0.3.5/gadapt/operations/crossover/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/crossover/__init__.py
--rw-rw-rw-   0        0        0     7691 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/operations/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1474 2024-04-09 20:19:40.000000 gadapt-0.3.5/gadapt/operations/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.094693 gadapt-0.3.5/gadapt/operations/exit_check/
--rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/exit_check/__init__.py
--rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.099193 gadapt-0.3.5/gadapt/operations/gene_combination/
--rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.100693 gadapt-0.3.5/gadapt/operations/immigration/
--rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.105694 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.110193 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.111692 gadapt-0.3.5/gadapt/operations/mutation/
--rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.151193 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      838 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1522 2024-04-09 20:29:12.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1549 2024-04-09 20:31:11.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1921 2024-04-09 20:31:54.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1315 2024-04-09 20:32:04.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1969 2024-04-09 20:29:48.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      644 2024-04-09 20:32:12.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1403 2024-04-09 20:29:32.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      593 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.157194 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/
--rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/__init__.py
--rw-rw-rw-   0        0        0      391 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
--rw-rw-rw-   0        0        0     2272 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
--rw-rw-rw-   0        0        0     2388 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
--rw-rw-rw-   0        0        0      445 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.207694 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/
--rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2088 2024-04-09 20:30:21.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1372 2024-04-09 20:32:26.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1784 2024-04-09 20:30:08.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1308 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1306 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2624 2024-04-09 20:30:39.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      722 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1557 2024-04-09 20:30:49.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      663 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.213694 gadapt-0.3.5/gadapt/operations/parent_selection/
--rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/operations/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.5/gadapt/operations/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.226694 gadapt-0.3.5/gadapt/operations/sampling/
--rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.5/gadapt/operations/sampling/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.5/gadapt/operations/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.232193 gadapt-0.3.5/gadapt/operations/variable_update/
--rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.5/gadapt/operations/variable_update/__init__.py
--rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/operations/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2565 2024-04-09 20:26:40.000000 gadapt-0.3.5/gadapt/operations/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.237194 gadapt-0.3.5/gadapt/utils/
--rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.5/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.5/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-04-09 20:26:27.000000 gadapt-0.3.5/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:34:01.241195 gadapt-0.3.5/gadapt.egg-info/
--rw-rw-rw-   0        0        0    22185 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5215 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 20:34:00.000000 gadapt-0.3.5/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      111 2024-04-09 20:34:01.267696 gadapt-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-04-09 20:33:52.000000 gadapt-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.341575 gadapt-0.3.6/
+-rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0    22185 2024-04-09 20:48:05.341075 gadapt-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21860 2024-04-09 20:15:45.000000 gadapt-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.154074 gadapt-0.3.6/gadapt/
+-rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.188576 gadapt-0.3.6/gadapt/adapters/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.193074 gadapt-0.3.6/gadapt/adapters/ga_logging/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/adapters/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.6/gadapt/adapters/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.195573 gadapt-0.3.6/gadapt/adapters/string_operation/
+-rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/adapters/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.199573 gadapt-0.3.6/gadapt/adapters/validation/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/validation/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.6/gadapt/adapters/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    22949 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/adapters/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.202573 gadapt-0.3.6/gadapt/execution/
+-rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3254 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.206073 gadapt-0.3.6/gadapt/factory/
+-rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     6432 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/factory/ga_base_factory.py
+-rw-rw-rw-   0        0        0    17510 2024-04-09 20:39:00.000000 gadapt-0.3.6/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    29258 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.224075 gadapt-0.3.6/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     9788 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0     3739 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/ga_model/decision_variable.py
+-rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    13440 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.225574 gadapt-0.3.6/gadapt/operations/
+-rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.3.6/gadapt/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.231073 gadapt-0.3.6/gadapt/operations/cost_finding/
+-rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1466 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/operations/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/cost_finding/elitism_cost_finder.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.238075 gadapt-0.3.6/gadapt/operations/crossover/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7691 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/operations/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1474 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/operations/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.245074 gadapt-0.3.6/gadapt/operations/exit_check/
+-rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.256075 gadapt-0.3.6/gadapt/operations/gene_combination/
+-rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.258074 gadapt-0.3.6/gadapt/operations/immigration/
+-rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.262075 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.265075 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.266575 gadapt-0.3.6/gadapt/operations/mutation/
+-rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.284074 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      838 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1522 2024-04-09 20:29:12.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1549 2024-04-09 20:31:11.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1921 2024-04-09 20:31:54.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1315 2024-04-09 20:32:04.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1969 2024-04-09 20:29:48.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      644 2024-04-09 20:32:12.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1403 2024-04-09 20:29:32.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      593 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.293575 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/
+-rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/__init__.py
+-rw-rw-rw-   0        0        0      391 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+-rw-rw-rw-   0        0        0     2272 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+-rw-rw-rw-   0        0        0     2388 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
+-rw-rw-rw-   0        0        0      445 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.311576 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2088 2024-04-09 20:30:21.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1372 2024-04-09 20:32:26.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1784 2024-04-09 20:30:08.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1308 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1306 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2624 2024-04-09 20:30:39.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      722 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-09 20:30:49.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      663 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.319074 gadapt-0.3.6/gadapt/operations/parent_selection/
+-rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/operations/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.6/gadapt/operations/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.328074 gadapt-0.3.6/gadapt/operations/sampling/
+-rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.6/gadapt/operations/sampling/__init__.py
+-rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.6/gadapt/operations/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.331075 gadapt-0.3.6/gadapt/operations/variable_update/
+-rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2565 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.338075 gadapt-0.3.6/gadapt/utils/
+-rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.339573 gadapt-0.3.6/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    22185 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5215 2024-04-09 20:48:05.000000 gadapt-0.3.6/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2024-04-09 20:48:05.343575 gadapt-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      512 2024-04-09 20:36:09.000000 gadapt-0.3.6/setup.py
```

### Comparing `gadapt-0.3.5/LICENSE` & `gadapt-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/PKG-INFO` & `gadapt-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.5
+Version: 0.3.6
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `gadapt-0.3.5/README.md` & `gadapt-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/adapters/ga_logging/logging_settings.py` & `gadapt-0.3.6/gadapt/adapters/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/adapters/string_operation/ga_strings.py` & `gadapt-0.3.6/gadapt/adapters/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/adapters/validation/base_options_validator.py` & `gadapt-0.3.6/gadapt/adapters/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/adapters/validation/common_options_validator.py` & `gadapt-0.3.6/gadapt/adapters/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/execution/ga_executor.py` & `gadapt-0.3.6/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/factory/ga_base_factory.py` & `gadapt-0.3.6/gadapt/factory/ga_base_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/factory/ga_factory.py` & `gadapt-0.3.6/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga.py` & `gadapt-0.3.6/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/chromosome.py` & `gadapt-0.3.6/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/decision_variable.py` & `gadapt-0.3.6/gadapt/ga_model/decision_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/definitions.py` & `gadapt-0.3.6/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/ga_options.py` & `gadapt-0.3.6/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/ga_results.py` & `gadapt-0.3.6/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/gene.py` & `gadapt-0.3.6/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/population.py` & `gadapt-0.3.6/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/ga_model/ranking_model.py` & `gadapt-0.3.6/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/cost_finding/base_cost_finder.py` & `gadapt-0.3.6/gadapt/operations/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/cost_finding/elitism_cost_finder.py` & `gadapt-0.3.6/gadapt/operations/cost_finding/elitism_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/crossover/base_crossover.py` & `gadapt-0.3.6/gadapt/operations/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/crossover/uniform_crossover.py` & `gadapt-0.3.6/gadapt/operations/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/exit_check/base_exit_checker.py` & `gadapt-0.3.6/gadapt/operations/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/exit_check/requested_cost_exit_checker.py` & `gadapt-0.3.6/gadapt/operations/exit_check/requested_cost_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/gene_combination/base_gene_combination.py` & `gadapt-0.3.6/gadapt/operations/gene_combination/base_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/gene_combination/blending_gene_combination.py` & `gadapt-0.3.6/gadapt/operations/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.3.6/gadapt/operations/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py` & `gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py` & `gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py` & `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/parent_selection/base_parent_selector.py` & `gadapt-0.3.6/gadapt/operations/parent_selection/base_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/parent_selection/sampling_parent_selector.py` & `gadapt-0.3.6/gadapt/operations/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/sampling/base_sampling.py` & `gadapt-0.3.6/gadapt/operations/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/sampling/roulette_wheel_sampling.py` & `gadapt-0.3.6/gadapt/operations/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/sampling/tournament_sampling.py` & `gadapt-0.3.6/gadapt/operations/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/operations/variable_update/common_variable_updater.py` & `gadapt-0.3.6/gadapt/operations/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt/utils/ga_utils.py` & `gadapt-0.3.6/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/gadapt.egg-info/PKG-INFO` & `gadapt-0.3.6/gadapt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.5
+Version: 0.3.6
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `gadapt-0.3.5/gadapt.egg-info/SOURCES.txt` & `gadapt-0.3.6/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/pyproject.toml` & `gadapt-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.5/setup.py` & `gadapt-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gadapt",
-    version="0.3.5",
+    version="0.3.6",
     author="Zoran Jankovic",
     author_email="bpzoran@yahoo.com",
     url="https://github.com/bpzoran/gadapt",
     packages=find_packages(),
     long_description=open("README.md").read(),
     # Specify the content type explicitly
     long_description_content_type="text/markdown",
```

