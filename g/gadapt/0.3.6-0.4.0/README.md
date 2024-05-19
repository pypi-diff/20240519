# Comparing `tmp/gadapt-0.3.6.tar.gz` & `tmp/gadapt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gadapt-0.3.6.tar", last modified: Tue Apr  9 20:48:05 2024, max compression
+gzip compressed data, was "gadapt-0.4.0.tar", last modified: Sun May 19 09:05:09 2024, max compression
```

## Comparing `gadapt-0.3.6.tar` & `gadapt-0.4.0.tar`

### file list

```diff
@@ -1,126 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.341575 gadapt-0.3.6/
--rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.3.6/LICENSE
--rw-rw-rw-   0        0        0    22185 2024-04-09 20:48:05.341075 gadapt-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    21860 2024-04-09 20:15:45.000000 gadapt-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.154074 gadapt-0.3.6/gadapt/
--rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.188576 gadapt-0.3.6/gadapt/adapters/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.193074 gadapt-0.3.6/gadapt/adapters/ga_logging/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/adapters/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-10-06 11:40:57.000000 gadapt-0.3.6/gadapt/adapters/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.195573 gadapt-0.3.6/gadapt/adapters/string_operation/
--rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/string_operation/__init__.py
--rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/adapters/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.199573 gadapt-0.3.6/gadapt/adapters/validation/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/adapters/validation/__init__.py
--rw-rw-rw-   0        0        0      939 2023-09-11 06:37:11.000000 gadapt-0.3.6/gadapt/adapters/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    22949 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/adapters/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.202573 gadapt-0.3.6/gadapt/execution/
--rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3254 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.206073 gadapt-0.3.6/gadapt/factory/
--rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     6432 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/factory/ga_base_factory.py
--rw-rw-rw-   0        0        0    17510 2024-04-09 20:39:00.000000 gadapt-0.3.6/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    29258 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.224075 gadapt-0.3.6/gadapt/ga_model/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     9788 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0     3739 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/ga_model/decision_variable.py
--rw-rw-rw-   0        0        0      878 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6865 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2256 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     2011 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    13440 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.225574 gadapt-0.3.6/gadapt/operations/
--rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.3.6/gadapt/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.231073 gadapt-0.3.6/gadapt/operations/cost_finding/
--rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/cost_finding/__init__.py
--rw-rw-rw-   0        0        0     1466 2024-04-09 20:26:26.000000 gadapt-0.3.6/gadapt/operations/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     1893 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/cost_finding/elitism_cost_finder.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.238075 gadapt-0.3.6/gadapt/operations/crossover/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/crossover/__init__.py
--rw-rw-rw-   0        0        0     7691 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/operations/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1474 2024-04-09 20:19:40.000000 gadapt-0.3.6/gadapt/operations/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.245074 gadapt-0.3.6/gadapt/operations/exit_check/
--rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/exit_check/__init__.py
--rw-rw-rw-   0        0        0      510 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1268 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      487 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      529 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.256075 gadapt-0.3.6/gadapt/operations/gene_combination/
--rw-rw-rw-   0        0        0       93 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      608 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1217 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.258074 gadapt-0.3.6/gadapt/operations/immigration/
--rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.262075 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      787 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      422 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.265075 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      473 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0     1045 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.266575 gadapt-0.3.6/gadapt/operations/mutation/
--rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.284074 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      838 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1522 2024-04-09 20:29:12.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1549 2024-04-09 20:31:11.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1921 2024-04-09 20:31:54.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1315 2024-04-09 20:32:04.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1969 2024-04-09 20:29:48.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      644 2024-04-09 20:32:12.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1403 2024-04-09 20:29:32.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      593 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.293575 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/
--rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/__init__.py
--rw-rw-rw-   0        0        0      391 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
--rw-rw-rw-   0        0        0     2272 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
--rw-rw-rw-   0        0        0     2388 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
--rw-rw-rw-   0        0        0      445 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.311576 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/
--rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2088 2024-04-09 20:30:21.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1372 2024-04-09 20:32:26.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1784 2024-04-09 20:30:08.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1308 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1306 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2624 2024-04-09 20:30:39.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      722 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1557 2024-04-09 20:30:49.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      663 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.319074 gadapt-0.3.6/gadapt/operations/parent_selection/
--rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/operations/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      737 2023-09-17 10:37:22.000000 gadapt-0.3.6/gadapt/operations/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1233 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.328074 gadapt-0.3.6/gadapt/operations/sampling/
--rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.3.6/gadapt/operations/sampling/__init__.py
--rw-rw-rw-   0        0        0     1102 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      509 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      500 2023-09-17 10:36:51.000000 gadapt-0.3.6/gadapt/operations/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1892 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2601 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.331075 gadapt-0.3.6/gadapt/operations/variable_update/
--rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.3.6/gadapt/operations/variable_update/__init__.py
--rw-rw-rw-   0        0        0      210 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/operations/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2565 2024-04-09 20:26:40.000000 gadapt-0.3.6/gadapt/operations/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.338075 gadapt-0.3.6/gadapt/utils/
--rw-rw-rw-   0        0        0      443 2024-03-05 19:39:48.000000 gadapt-0.3.6/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.3.6/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-04-09 20:26:27.000000 gadapt-0.3.6/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:48:05.339573 gadapt-0.3.6/gadapt.egg-info/
--rw-rw-rw-   0        0        0    22185 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5215 2024-04-09 20:48:05.000000 gadapt-0.3.6/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 20:48:04.000000 gadapt-0.3.6/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      812 2024-03-05 19:18:24.000000 gadapt-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0      111 2024-04-09 20:48:05.343575 gadapt-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-04-09 20:36:09.000000 gadapt-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.955667 gadapt-0.4.0/
+-rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    23179 2024-05-19 09:05:09.955168 gadapt-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    22848 2024-05-17 19:20:08.000000 gadapt-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.076660 gadapt-0.4.0/gadapt/
+-rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.131161 gadapt-0.4.0/gadapt/adapters/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.0/gadapt/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.169661 gadapt-0.4.0/gadapt/adapters/ga_logging/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/adapters/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2204 2024-05-05 22:50:27.000000 gadapt-0.4.0/gadapt/adapters/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.199661 gadapt-0.4.0/gadapt/adapters/string_operation/
+-rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.4.0/gadapt/adapters/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.4.0/gadapt/adapters/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.221162 gadapt-0.4.0/gadapt/adapters/validation/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.0/gadapt/adapters/validation/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-05-05 18:18:08.000000 gadapt-0.4.0/gadapt/adapters/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    24756 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/adapters/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.236161 gadapt-0.4.0/gadapt/execution/
+-rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     4581 2024-05-19 09:02:00.000000 gadapt-0.4.0/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.254162 gadapt-0.4.0/gadapt/factory/
+-rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/factory/ga_base_factory.py
+-rw-rw-rw-   0        0        0    23242 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    32066 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.328163 gadapt-0.4.0/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     7865 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0     3649 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga_model/decision_variable.py
+-rw-rw-rw-   0        0        0     1093 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     7797 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2258 2024-05-05 18:18:09.000000 gadapt-0.4.0/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1912 2024-05-17 22:12:01.000000 gadapt-0.4.0/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0     6785 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.4.0/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.340163 gadapt-0.4.0/gadapt/operations/
+-rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.4.0/gadapt/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.365663 gadapt-0.4.0/gadapt/operations/cost_finding/
+-rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     1830 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/cost_finding/elitism_cost_finder.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.409164 gadapt-0.4.0/gadapt/operations/crossover/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/crossover/__init__.py
+-rw-rw-rw-   0        0        0     8305 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1613 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/crossover/blending_crossover.py
+-rw-rw-rw-   0        0        0     1734 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/crossover/blending_parent_diversity_crossover.py
+-rw-rw-rw-   0        0        0     1127 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.509663 gadapt-0.4.0/gadapt/operations/exit_check/
+-rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-05-05 22:30:06.000000 gadapt-0.4.0/gadapt/operations/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1625 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      490 2024-05-05 22:30:18.000000 gadapt-0.4.0/gadapt/operations/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      584 2024-05-07 06:26:43.000000 gadapt-0.4.0/gadapt/operations/exit_check/number_of_generations_exit_checker.py
+-rw-rw-rw-   0        0        0      522 2024-05-05 22:30:27.000000 gadapt-0.4.0/gadapt/operations/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.517688 gadapt-0.4.0/gadapt/operations/immigration/
+-rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.538170 gadapt-0.4.0/gadapt/operations/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      993 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      370 2024-05-05 22:50:27.000000 gadapt-0.4.0/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.551686 gadapt-0.4.0/gadapt/operations/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0     1097 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.559664 gadapt-0.4.0/gadapt/operations/mutation/
+-rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.595663 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      900 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2058 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2145 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1472 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2049 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      591 2024-05-05 22:03:38.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1449 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      477 2024-05-05 22:50:27.000000 gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.615665 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/
+-rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+-rw-rw-rw-   0        0        0     1021 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py
+-rw-rw-rw-   0        0        0     2362 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+-rw-rw-rw-   0        0        0      703 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py
+-rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
+-rw-rw-rw-   0        0        0      427 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.731166 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2647 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1485 2024-05-05 22:50:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1948 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1295 2024-05-05 22:50:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1189 2024-05-05 22:49:46.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2829 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      600 2024-05-05 22:50:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1750 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      541 2024-05-05 22:50:08.000000 gadapt-0.4.0/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.780667 gadapt-0.4.0/gadapt/operations/parent_selection/
+-rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.4.0/gadapt/operations/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-05-16 06:43:45.000000 gadapt-0.4.0/gadapt/operations/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      800 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.793666 gadapt-0.4.0/gadapt/operations/population_update/
+-rw-rw-rw-   0        0        0       40 2024-04-27 16:02:41.000000 gadapt-0.4.0/gadapt/operations/population_update/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/population_update/base_population_updater.py
+-rw-rw-rw-   0        0        0      961 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/operations/population_update/common_population_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.877166 gadapt-0.4.0/gadapt/operations/sampling/
+-rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.4.0/gadapt/operations/sampling/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-05-05 18:18:08.000000 gadapt-0.4.0/gadapt/operations/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      511 2024-05-05 18:18:09.000000 gadapt-0.4.0/gadapt/operations/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      502 2024-05-05 18:18:08.000000 gadapt-0.4.0/gadapt/operations/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     2125 2024-05-05 18:18:09.000000 gadapt-0.4.0/gadapt/operations/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2603 2024-05-05 18:18:08.000000 gadapt-0.4.0/gadapt/operations/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.904665 gadapt-0.4.0/gadapt/operations/variable_update/
+-rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.4.0/gadapt/operations/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-05 22:47:04.000000 gadapt-0.4.0/gadapt/operations/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2449 2024-05-05 22:37:22.000000 gadapt-0.4.0/gadapt/operations/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.952168 gadapt-0.4.0/gadapt/utils/
+-rw-rw-rw-   0        0        0      443 2024-05-05 18:18:08.000000 gadapt-0.4.0/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.4.0/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-17 19:20:08.000000 gadapt-0.4.0/gadapt/utils/ga_decorators.py
+-rw-rw-rw-   0        0        0     2916 2024-05-17 18:56:26.000000 gadapt-0.4.0/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:05:09.953668 gadapt-0.4.0/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    23179 2024-05-19 09:05:08.000000 gadapt-0.4.0/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5593 2024-05-19 09:05:08.000000 gadapt-0.4.0/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 09:05:08.000000 gadapt-0.4.0/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-19 09:05:08.000000 gadapt-0.4.0/gadapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 09:05:08.000000 gadapt-0.4.0/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      812 2024-05-17 20:44:16.000000 gadapt-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2024-05-19 09:05:09.967667 gadapt-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-05-19 09:03:28.000000 gadapt-0.4.0/setup.py
```

### Comparing `gadapt-0.3.6/LICENSE` & `gadapt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.6/PKG-INFO` & `gadapt-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-Metadata-Version: 2.1
-Name: gadapt
-Version: 0.3.6
-Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
-Home-page: https://github.com/bpzoran/gadapt
-Author: Zoran Jankovic
-Author-email: bpzoran@yahoo.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-
 # GAdapt: Self-Adaptive Genetic Algorithm
-[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
-# What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for adaptive mutation of genes and chromosomes.
+
+## What Innovations Does GAdapt Bring?
+
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost, and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation, thereby enhancing accuracy and performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
+## Installation
 
-# Installation
 To install **GAdapt**, use **pip** with the following command:
 
-```
+```bash
 pip install gadapt
 ```
 
 # Releases
-Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+The latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
 
 # Source Code
-The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
+The source code is available on GitHub: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
 
 # API Documentation
-The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
+For detailed API documentation, refer to: [GAdapt API Documentation](https://www.gadapt.com/api/)
 
 # Getting started
-The following example optimizes variable values for a complex trigonometric function.
+Below is an example optimizing variable values for a complex trigonometric function:
 ```python
 from gadapt.ga import GA
 import math
 
 #trigonometric function definition
 def trig_func(args):    
     return math.sqrt(abs(math.cos(args[0]))) + math.pow(math.cos(args[1]), 2) + math.sin(args[2]) + math.pow(args[3], 2) + math.sqrt(args[4]) + math.cos(args[5]) - (args[6]*math.sin(pow(args[6], 3)) + 1) + math.sin(args[0]) / (math.sqrt(args[0])/3 + (args[6]*math.sin(pow(args[6], 3)) + 1) ) / math.sqrt(args[4]) + math.cos(args[5])
@@ -73,15 +64,15 @@
 4: 1.0
 5: 3.14
 6: -1.0
 ```
 
 In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
 # Parameter Settings
-GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
+GAdapt genetic algorithm can receive parameters through constructor, properties, or a combination of both. Below are the supported parameters:
 
 Passing parameters through the class constructor:
 ```python
 ga = GA(cost_function=trig_func,
     population_size=32,
     population_mutation="cost_diversity,parent_diversity",
     number_of_mutation_chromosomes=6,
@@ -114,71 +105,80 @@
 ga.max_attempt_no=20
 ga.logging=True
 ga.timeout=3600
 ```
 # Parameters description
 **cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
 
-**population_size**=*64* - Number of chromosomes in the population.
+**population_size**=*32* - Number of chromosomes in the population.
 
 **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
 Supported values:
 - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
 - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations  
 - *"requested"* - The optimisation exit is triggered when the requested value reached
+- *"generations"* - The optimisation exit requested number of generations defined by "number_of_generations" parameter is reached
     
-**max_attempt_no**=*10* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
+**max_attempt_no**=*2* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
 
 **requested_cost**=*sys.float_info.max* - This parameter only takes place when *exit_check* has value *"requested"*. It determines the requested value which causes the exit from the genetic algorithm
 
+**number_of_generations**=*200* - This parameter only takes place when exit_check has value “generations”. It determines the number of generations after which the genetic algorithm exits
+
 **timeout**=*120* - A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether *exit_check* criteria is reached.
 
 **parent_selection**=*"roulette_wheel"* - The algorithm for parent selection.  
 Supported values:
 - *"roulette_wheel"* - Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes in the mating pool are inversely proportional to their cost. A chromosome with the lowest cost has the greatest probability of mating, while the chromosome with the highest cost has the lowest probability of mating.  
 - *"tournament"* - Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes from the mating pool, and chromosomes with the lowest cost in subsets become a parent. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament parent selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and pairs the chromosomes two at a time until the top kept chromosomes are selected for mating. Thus, the algorithm pairs odd rows with even rows.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes.  
+
+**crossover**=*"blending"* - The algorithm for parent selection. If the Parent Diversity mutation is used, blending crossover will be used, of the choice of this parameter.
+Supported values:
+- *"blending"* - Blending crossover combines gene values from the two parents into new variable values in offsprings. One value of the offspring variable comes from a combination of the two corresponding values of the parental genes  
+- *"uniform"* - Uniform crossover combines chromosomes in a uniform way.
     
-**percentage_of_mutation_chromosomes**=*10.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_chromosomes**=*50.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_chromosomes**=*-1* - The number of mutation chromosomes in the population. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutation_chromosomes*. This value is the upper bound - the actual number of mutated chromosomes can vary from 1 to *number_of_mutation_chromosomes*.
 
-**percentage_of_mutations_genes**=*10* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_genes**=*20* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_genes**=*-1* - The number of mutated genes in each chromosome. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutations_genes*. This value is the upper bound - the number of mutated genes can vary from 1 to *number_of_mutation_genes*.
 
 **population_mutation**=*"cost_diversity,parent_diversity"* - A type of mutation for the entire population. Based on the value of this parameter, the number of mutation chromosomes can be determined, along with how chromosomes for the mutation will be selected.
 Supported values:
 - *"cost_diversity"* - It applies to the number of mutation chromosomes. *"cost_diversity"* determines the number of mutated chromosomes adaptively, using the diversity of costs in the population. Lower cost diversity means a higher number of mutated chromosomes. The minimal value of mutated chromosomes is 0, and the maximal value is determined by the value of *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes* parameters. If *population_mutation* has a value other than *"cost_diversity"*, the number of mutation chromosomes is a random value from 1 to *number_of_mutation_chromosomes* value (or to value determined by *percentage_of_mutation_chromosomes* value). *"cost_diversity"* means that the *"parent_diversity"* method is selected to select chromosomes to be mutated. This method only determines the number of mutated chromosomes, but not how chromosomes are selected for the mutation.  
-- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_selection* parameter.  
+- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_sampling* parameter.  
 - *"random"* - It applies to the number of mutation chromosomes and to the way how mutation chromosomes will be selected. *"random"* selects chromosomes to be mutated randomly, and randomly determines the number of mutated chromosomes (with the upper bound of **number_of_mutation_chromosomes**)
 
 Population_mutation may have more values, separated by a comma. It means that more than one method can be chosen for the mutation of chromosomes in the population. For example, *"cost_diversity,parent_diversity"* means that number of mutation chromosomes will be determined by the cost diversity and the selection of chromosomes to be mutated will be defined by parent diversity. *"cost_diversity,random"* means that the cost diversity will determine the number of mutation chromosomes, and the selection of chromosomes to be mutated will be chosen randomly.
     
-**parent_diversity_mutation_chromosome_selection**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
+**parent_diversity_mutation_chromosome_sampling**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes to be mutated are proportional to the similarity of their parents (inversely proportional to the parent diversity). A chromosome with the lowest parent diversity has the greatest probability of mutation, while the chromosome with the highest parent diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes, and chromosomes with the lowest parent diversity (highest parent similarity) in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
-**chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
+**chromosome_mutation**=*"cross_diversity,random"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_sampling* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
+**gene_mutation**=*"cross_diversity,random"* - The type of assigning mutated values to genes
 Supported values:
-- *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
+- *"normal_distribution"* - assigns normally distributed random number to the variable selected for mutation
+- *"cross_diversity"* - assigns normally distributed random number to the variable selected for mutation, with standard deviation based on the cross-diversity coefficient
 - *"random"* - Random values are assigned to genes
 
-**cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
+**cross_diversity_mutation_gene_sampling**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects genes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
     
 **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
@@ -271,51 +271,50 @@
 Number of iterations: 21
 Parameter values:
 0: 0.0
 1: 0.0
 ```
 
 # GA Customisation
-GAdapt has been developed in common with clean architecture and SOLID principles and therefore it can be customized easily. Customization can be applied by creating new implementation of abstract classes and passing them to the gnetic algorithm through factory object. Abstract classes are all classes in "operation" folder with names starting with "Base". Please consult  [GAdapt API Documentation](https://www.gadapt.com/api/) for more information about GAdapt classes.
+GAdapt follows clean architecture and SOLID principles, allowing easy customization. Create new implementations of abstract classes and pass them to the genetic algorithm through the factory object.
 
-Example of customisation of GAdapt by introducing a new class for mutation of population:
+For example, customizing the chromosome mutation selector:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
+from operations.mutation.population_mutation.base_chromosome_mutation_selector import BaseChromosomeMutationSelector
+from operations.mutation.population_mutation.random_chromosome_mutation_rate_determinator import RandomChromosomeMutationRateDeterminator
 
-BaseChromosomeMutationRateDeterminator
 
-
-class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
+class BottomMutationSelector(BaseChromosomeMutationSelector):
     """
-    Population mutator which selects mutating chromosomes from the bottom of
-    existing unallocated chromosoms 
+    Chromosome mutation selector which selects mutating chromosomes from the bottom of
+    existing unallocated chromosomes sorted by the cost function value
     """
 
-    def _mutate_population(self, population, number_of_mutation_chromosomes):
-        if population is None:
+    def _mutate_population(self):
+        if self.population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
-            population, None
+            lambda chrom: (self.population.options.cost_function([g.variable_value for g in chrom]))
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   len(unallocated_chromosomes) - self.number_of_mutation_chromosomes:
                                    ]
         for c in chromosomes_for_mutation:
-            c.mutate(population.options.number_of_mutation_genes)
+            self._gene_mutation_selector.mutate(c, self.population.options.number_of_mutation_genes)
 
 
 def some_func(args):
     return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
 
 
 custom_factory = GAFactory()
-custom_factory.population_mutator = BottomPopulationMutator()
+custom_factory.chromosome_mutation_selector = BottomMutationSelector(RandomChromosomeMutationRateDeterminator())
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
 ga.add(-5, 5, 0.1)
 
 print(ga.execute())
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gadapt-0.3.6/README.md` & `gadapt-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,45 @@
+Metadata-Version: 2.1
+Name: gadapt
+Version: 0.4.0
+Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
+Home-page: https://github.com/bpzoran/gadapt
+Author: Zoran Jankovic
+Author-email: bpzoran@yahoo.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+
 # GAdapt: Self-Adaptive Genetic Algorithm
-[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
-# What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for adaptive mutation of genes and chromosomes.
+
+## What Innovations Does GAdapt Bring?
+
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost, and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation, thereby enhancing accuracy and performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
+## Installation
 
-# Installation
 To install **GAdapt**, use **pip** with the following command:
 
-```
+```bash
 pip install gadapt
 ```
 
 # Releases
-Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+The latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
 
 # Source Code
-The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
+The source code is available on GitHub: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
 
 # API Documentation
-The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
+For detailed API documentation, refer to: [GAdapt API Documentation](https://www.gadapt.com/api/)
 
 # Getting started
-The following example optimizes variable values for a complex trigonometric function.
+Below is an example optimizing variable values for a complex trigonometric function:
 ```python
 from gadapt.ga import GA
 import math
 
 #trigonometric function definition
 def trig_func(args):    
     return math.sqrt(abs(math.cos(args[0]))) + math.pow(math.cos(args[1]), 2) + math.sin(args[2]) + math.pow(args[3], 2) + math.sqrt(args[4]) + math.cos(args[5]) - (args[6]*math.sin(pow(args[6], 3)) + 1) + math.sin(args[0]) / (math.sqrt(args[0])/3 + (args[6]*math.sin(pow(args[6], 3)) + 1) ) / math.sqrt(args[4]) + math.cos(args[5])
@@ -62,15 +75,15 @@
 4: 1.0
 5: 3.14
 6: -1.0
 ```
 
 In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
 # Parameter Settings
-GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
+GAdapt genetic algorithm can receive parameters through constructor, properties, or a combination of both. Below are the supported parameters:
 
 Passing parameters through the class constructor:
 ```python
 ga = GA(cost_function=trig_func,
     population_size=32,
     population_mutation="cost_diversity,parent_diversity",
     number_of_mutation_chromosomes=6,
@@ -103,71 +116,80 @@
 ga.max_attempt_no=20
 ga.logging=True
 ga.timeout=3600
 ```
 # Parameters description
 **cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
 
-**population_size**=*64* - Number of chromosomes in the population.
+**population_size**=*32* - Number of chromosomes in the population.
 
 **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
 Supported values:
 - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
 - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations  
 - *"requested"* - The optimisation exit is triggered when the requested value reached
+- *"generations"* - The optimisation exit requested number of generations defined by "number_of_generations" parameter is reached
     
-**max_attempt_no**=*10* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
+**max_attempt_no**=*2* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
 
 **requested_cost**=*sys.float_info.max* - This parameter only takes place when *exit_check* has value *"requested"*. It determines the requested value which causes the exit from the genetic algorithm
 
+**number_of_generations**=*200* - This parameter only takes place when exit_check has value вЂњgenerationsвЂќ. It determines the number of generations after which the genetic algorithm exits
+
 **timeout**=*120* - A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether *exit_check* criteria is reached.
 
 **parent_selection**=*"roulette_wheel"* - The algorithm for parent selection.  
 Supported values:
 - *"roulette_wheel"* - Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes in the mating pool are inversely proportional to their cost. A chromosome with the lowest cost has the greatest probability of mating, while the chromosome with the highest cost has the lowest probability of mating.  
 - *"tournament"* - Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes from the mating pool, and chromosomes with the lowest cost in subsets become a parent. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament parent selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and pairs the chromosomes two at a time until the top kept chromosomes are selected for mating. Thus, the algorithm pairs odd rows with even rows.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes.  
+
+**crossover**=*"blending"* - The algorithm for parent selection. If the Parent Diversity mutation is used, blending crossover will be used, of the choice of this parameter.
+Supported values:
+- *"blending"* - Blending crossover combines gene values from the two parents into new variable values in offsprings. One value of the offspring variable comes from a combination of the two corresponding values of the parental genes  
+- *"uniform"* - Uniform crossover combines chromosomes in a uniform way.
     
-**percentage_of_mutation_chromosomes**=*10.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_chromosomes**=*50.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_chromosomes**=*-1* - The number of mutation chromosomes in the population. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutation_chromosomes*. This value is the upper bound - the actual number of mutated chromosomes can vary from 1 to *number_of_mutation_chromosomes*.
 
-**percentage_of_mutations_genes**=*10* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_genes**=*20* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_genes**=*-1* - The number of mutated genes in each chromosome. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutations_genes*. This value is the upper bound - the number of mutated genes can vary from 1 to *number_of_mutation_genes*.
 
 **population_mutation**=*"cost_diversity,parent_diversity"* - A type of mutation for the entire population. Based on the value of this parameter, the number of mutation chromosomes can be determined, along with how chromosomes for the mutation will be selected.
 Supported values:
 - *"cost_diversity"* - It applies to the number of mutation chromosomes. *"cost_diversity"* determines the number of mutated chromosomes adaptively, using the diversity of costs in the population. Lower cost diversity means a higher number of mutated chromosomes. The minimal value of mutated chromosomes is 0, and the maximal value is determined by the value of *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes* parameters. If *population_mutation* has a value other than *"cost_diversity"*, the number of mutation chromosomes is a random value from 1 to *number_of_mutation_chromosomes* value (or to value determined by *percentage_of_mutation_chromosomes* value). *"cost_diversity"* means that the *"parent_diversity"* method is selected to select chromosomes to be mutated. This method only determines the number of mutated chromosomes, but not how chromosomes are selected for the mutation.  
-- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_selection* parameter.  
+- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_sampling* parameter.  
 - *"random"* - It applies to the number of mutation chromosomes and to the way how mutation chromosomes will be selected. *"random"* selects chromosomes to be mutated randomly, and randomly determines the number of mutated chromosomes (with the upper bound of **number_of_mutation_chromosomes**)
 
 Population_mutation may have more values, separated by a comma. It means that more than one method can be chosen for the mutation of chromosomes in the population. For example, *"cost_diversity,parent_diversity"* means that number of mutation chromosomes will be determined by the cost diversity and the selection of chromosomes to be mutated will be defined by parent diversity. *"cost_diversity,random"* means that the cost diversity will determine the number of mutation chromosomes, and the selection of chromosomes to be mutated will be chosen randomly.
     
-**parent_diversity_mutation_chromosome_selection**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
+**parent_diversity_mutation_chromosome_sampling**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes to be mutated are proportional to the similarity of their parents (inversely proportional to the parent diversity). A chromosome with the lowest parent diversity has the greatest probability of mutation, while the chromosome with the highest parent diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes, and chromosomes with the lowest parent diversity (highest parent similarity) in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
-**chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
+**chromosome_mutation**=*"cross_diversity,random"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_sampling* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
+**gene_mutation**=*"cross_diversity,random"* - The type of assigning mutated values to genes
 Supported values:
-- *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
+- *"normal_distribution"* - assigns normally distributed random number to the variable selected for mutation
+- *"cross_diversity"* - assigns normally distributed random number to the variable selected for mutation, with standard deviation based on the cross-diversity coefficient
 - *"random"* - Random values are assigned to genes
 
-**cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
+**cross_diversity_mutation_gene_sampling**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects genes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
     
 **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
@@ -260,51 +282,50 @@
 Number of iterations: 21
 Parameter values:
 0: 0.0
 1: 0.0
 ```
 
 # GA Customisation
-GAdapt has been developed in common with clean architecture and SOLID principles and therefore it can be customized easily. Customization can be applied by creating new implementation of abstract classes and passing them to the gnetic algorithm through factory object. Abstract classes are all classes in "operation" folder with names starting with "Base". Please consult  [GAdapt API Documentation](https://www.gadapt.com/api/) for more information about GAdapt classes.
+GAdapt follows clean architecture and SOLID principles, allowing easy customization. Create new implementations of abstract classes and pass them to the genetic algorithm through the factory object.
 
-Example of customisation of GAdapt by introducing a new class for mutation of population:
+For example, customizing the chromosome mutation selector:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
+from operations.mutation.population_mutation.base_chromosome_mutation_selector import BaseChromosomeMutationSelector
+from operations.mutation.population_mutation.random_chromosome_mutation_rate_determinator import RandomChromosomeMutationRateDeterminator
 
-BaseChromosomeMutationRateDeterminator
 
-
-class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
+class BottomMutationSelector(BaseChromosomeMutationSelector):
     """
-    Population mutator which selects mutating chromosomes from the bottom of
-    existing unallocated chromosoms 
+    Chromosome mutation selector which selects mutating chromosomes from the bottom of
+    existing unallocated chromosomes sorted by the cost function value
     """
 
-    def _mutate_population(self, population, number_of_mutation_chromosomes):
-        if population is None:
+    def _mutate_population(self):
+        if self.population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
-            population, None
+            lambda chrom: (self.population.options.cost_function([g.variable_value for g in chrom]))
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   len(unallocated_chromosomes) - self.number_of_mutation_chromosomes:
                                    ]
         for c in chromosomes_for_mutation:
-            c.mutate(population.options.number_of_mutation_genes)
+            self._gene_mutation_selector.mutate(c, self.population.options.number_of_mutation_genes)
 
 
 def some_func(args):
     return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
 
 
 custom_factory = GAFactory()
-custom_factory.population_mutator = BottomPopulationMutator()
+custom_factory.chromosome_mutation_selector = BottomMutationSelector(RandomChromosomeMutationRateDeterminator())
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
 ga.add(-5, 5, 0.1)
 
 print(ga.execute())
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gadapt-0.3.6/gadapt/adapters/ga_logging/logging_settings.py` & `gadapt-0.4.0/gadapt/adapters/ga_logging/logging_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 from os.path import isfile, join
+
 from gadapt.utils.TimeStampFormatter import TimestampFormatter
 
 
 def init_logging(is_logging: bool):
     """
     Initializes logging for genetic algorithm
     """
@@ -21,15 +22,15 @@
             return n_last_number
         except Exception:
             return -1
 
     if not is_logging:
         logging.disable(logging.INFO)
         return
-    path = os.getcwd() + "\log"
+    path = os.getcwd() + "\\log"
     if not os.path.exists(path):
         os.mkdir(path)
     else:
         onlyfiles = [f for f in os.listdir(path) if isfile(join(path, f))]
         onlyfiles.sort(reverse=True, key=get_last_num)
         for f in onlyfiles:
             if f == "log.log":
@@ -46,15 +47,15 @@
                 n_last_number += 1
                 try:
                     os.rename(path + "\\" + f, path + "\\log.log." + str(n_last_number))
                 except Exception:
                     # print("Unable to rename log file: " + path + "\\" + f)
                     # traceback.print_exc()
                     break
-    logpath = path + "\log.log"
+    logpath = path + "\\log.log"
     logging.basicConfig(filename=logpath, level=logging.INFO)
     logger = logging.getLogger("")
     handler = logging.FileHandler(logpath)
     handler.setFormatter(
         TimestampFormatter("%(asctime)s - %(levelname)s - %(message)s")
     )
     for h in logger.handlers:
```

### Comparing `gadapt-0.3.6/gadapt/adapters/string_operation/ga_strings.py` & `gadapt-0.4.0/gadapt/adapters/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.6/gadapt/adapters/validation/base_options_validator.py` & `gadapt-0.4.0/gadapt/adapters/validation/base_options_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import List
+
 import gadapt.ga_model.message_levels as message_levels
 
 
 class BaseOptionsValidator(ABC):
     def __init__(self, options) -> None:
         """
         Base class for options validation
```

### Comparing `gadapt-0.3.6/gadapt/adapters/validation/common_options_validator.py` & `gadapt-0.4.0/gadapt/adapters/validation/common_options_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from gadapt.adapters.validation.base_options_validator import BaseOptionsValidator
 import gadapt.ga_model.definitions as definitions
+from gadapt.adapters.validation.base_options_validator import BaseOptionsValidator
 
 
 class CommonOptionsValidator(BaseOptionsValidator):
     """
     Common class for options validation
     """
 
@@ -114,14 +114,18 @@
             self._add_message("Population size type must be int!")
             rslt &= False
         elif self.options.population_size < 4 or self.options.population_size > 65536:
             self._add_message("Population size must be an int between 4 and 65536!")
             rslt &= False
         else:
             population_size = self.options.population_size
+        keep_elitism_percentage = self.options.keep_elitism_percentage
+        if not (0 <= self.options.keep_elitism_percentage <= 100):
+            self._add_message("Elitism percentage value must be between 0 and 100!")
+            rslt &= False
         immigration_number = 0
         if self.options.immigration_number is None:
             self._add_message("Immigration Number must not be None!")
             rslt &= False
         elif not isinstance(self.options.immigration_number, int):
             self._add_message("Immigration Number must be type int!")
             rslt &= False
@@ -161,15 +165,16 @@
                 (self.options.number_of_mutation_chromosomes is not None)
                 and (isinstance(self.options.number_of_mutation_chromosomes, int))
                 and (self.options.number_of_mutation_chromosomes > 0)
             ):
                 if (
                     population_size > 0
                     and self.options.number_of_mutation_chromosomes
-                    > (population_size // 2) - immigration_number
+                    > round(population_size * (keep_elitism_percentage / 100))
+                    - immigration_number
                 ):
                     self._add_message(
                         "Invalid number of mutation chromosomes: {0}".format(
                             str(self.options.number_of_mutation_chromosomes)
                         )
                     )
                     rslt &= False
@@ -262,24 +267,24 @@
         elif self.options.max_attempt_no < 1 or self.options.max_attempt_no > 65536:
             self._add_message("Max Attempt No must be type an int between 1 and 65536!")
             rslt &= False
         if (
             self.options.chromosome_mutation == definitions.CROSS_DIVERSITY
             or definitions.CROSS_DIVERSITY in self.options.chromosome_mutation
         ):
-            if self.options.cross_diversity_mutation_gene_selection is None:
+            if self.options.cross_diversity_mutation_gene_sampling is None:
                 self._add_message(
-                    "Cross Diversity Mutation Gene Selection must not be None!"
+                    "Cross Diversity Mutation Gene Sampling must not be None!"
                 )
                 rslt &= False
             elif not isinstance(
-                self.options.cross_diversity_mutation_gene_selection, str
+                self.options.cross_diversity_mutation_gene_sampling, str
             ):
                 self._add_message(
-                    "Cross Diversity Mutation Gene Selection must be type str!"
+                    "Cross Diversity Mutation Gene Sampling must be type str!"
                 )
                 rslt &= False
         if self.options.chromosome_mutation is None:
             self._add_message("Chromosome Mutation must not be None!")
             rslt &= False
         elif not isinstance(self.options.chromosome_mutation, str):
             self._add_message("Chromosome Mutation must be type str!")
@@ -288,33 +293,33 @@
             mutator_strings = [
                 ms.strip()
                 for ms in self.options.chromosome_mutation.split(
                     definitions.PARAM_SEPARATOR
                 )
             ]
             for mutator_string in mutator_strings:
-                if mutator_string not in definitions.CHROMOSOME_MUTATOR_STRINGS:
+                if mutator_string not in definitions.CHROMOSOME_MUTATION_STRINGS:
                     self._add_message(
                         "Invalid value of Chromosome Mutation:\
                             {0}. Allowed values: {1}".format(
                             mutator_string,
                             self._get_allowed_values(
-                                definitions.CHROMOSOME_MUTATOR_STRINGS
+                                definitions.CHROMOSOME_MUTATION_STRINGS
                             ),
                         )
                     )
                     rslt &= False
         elif (
             self.options.chromosome_mutation
-            not in definitions.CHROMOSOME_MUTATOR_STRINGS
+            not in definitions.CHROMOSOME_MUTATION_STRINGS
         ):
             self._add_message(
                 "Invalid value of Chromosome Mutation: {0}. Allowed values: {1}".format(
                     self.options.chromosome_mutation,
-                    self._get_allowed_values(definitions.CHROMOSOME_MUTATOR_STRINGS),
+                    self._get_allowed_values(definitions.CHROMOSOME_MUTATION_STRINGS),
                 )
             )
             rslt &= False
         if self.options.exit_check is None:
             self._add_message("Exit Check must not be None!")
             rslt &= False
         elif not isinstance(self.options.exit_check, str):
@@ -325,28 +330,28 @@
                 "Invalid value of Exit Check: {0}. Allowed values: {1}".format(
                     self.options.exit_check,
                     self._get_allowed_values(definitions.EXIT_CRITERIA_STRINGS),
                 )
             )
             rslt &= False
         if self.options.chromosome_mutation == definitions.CROSS_DIVERSITY:
-            if self.options.cross_diversity_mutation_gene_selection is None:
+            if self.options.cross_diversity_mutation_gene_sampling is None:
                 self._add_message(
                     "Cross Diversity Mutation Gene Selection must not be None!"
                 )
                 rslt &= False
             elif not isinstance(
-                self.options.cross_diversity_mutation_gene_selection, str
+                self.options.cross_diversity_mutation_gene_sampling, str
             ):
                 self._add_message(
                     "Cross Diversity Mutation Gene Selection must be type str!"
                 )
                 rslt &= False
             elif not self._validate_selection(
-                self.options.cross_diversity_mutation_gene_selection,
+                self.options.cross_diversity_mutation_gene_sampling,
                 "Cross Diversity Mutation Gene Selection",
                 self.options.number_of_mutation_genes,
                 "Group Size for Cross Diversity Mutation Gene Selection must be below\
                     or equal than the number of mutation genes!",
             ):
                 rslt &= False
         if self.options.logging is None:
@@ -361,32 +366,32 @@
         elif not isinstance(self.options.must_mutate_for_same_parents, bool):
             self._add_message("Must Mutate For Same Parents must be type bool!")
             rslt &= False
         if (
             self.options.population_mutation == definitions.COST_DIVERSITY
             or definitions.PARENT_DIVERSITY in self.options.population_mutation
         ):
-            if self.options.parent_diversity_mutation_chromosome_selection is None:
+            if self.options.parent_diversity_mutation_chromosome_sampling is None:
                 self._add_message(
-                    "Parent Diversity Mutation Chromosome Selection must not be None!"
+                    "Parent Diversity Mutation Chromosome Sampling must not be None!"
                 )
                 rslt &= False
             elif not isinstance(
-                self.options.parent_diversity_mutation_chromosome_selection, str
+                self.options.parent_diversity_mutation_chromosome_sampling, str
             ):
                 self._add_message(
-                    "Parent Diversity Mutation Chromosome Selection must be type str!"
+                    "Parent Diversity Mutation Chromosome Sampling must be type str!"
                 )
                 rslt &= False
             elif not self._validate_selection(
-                self.options.parent_diversity_mutation_chromosome_selection,
-                "Parents Diversity Mutation Chromosome Selection",
-                (population_size // 2) - self.options.immigration_number,  # type: ignore
+                self.options.parent_diversity_mutation_chromosome_sampling,
+                "Parents Diversity Mutation Chromosome Sampling",
+                round(population_size * (keep_elitism_percentage / 100)) - self.options.immigration_number,  # type: ignore
                 "Group Size for Parents Diversity Mutation Chromosome\
-                Selection cannot have the value below half population!",
+                Sampling cannot have the value below half population!",
             ):
                 rslt &= False
         if self.options.population_mutation is None:
             self._add_message("Population Mutation must not be None!")
             rslt &= False
         elif not isinstance(self.options.population_mutation, str):
             self._add_message("Population Mutation must be type str!")
@@ -395,46 +400,75 @@
             mutator_strings = [
                 ms.strip()
                 for ms in self.options.population_mutation.split(
                     definitions.PARAM_SEPARATOR
                 )
             ]
             for mutator_string in mutator_strings:
-                if mutator_string not in definitions.POPULATION_MUTATOR_STRINGS:
+                if mutator_string not in definitions.POPULATION_MUTATION_STRINGS:
                     self._add_message(
                         "Invalid value of Population Mutation:\
                             {0}. Allowed values: {1}".format(
                             mutator_string,
                             self._get_allowed_values(
-                                definitions.POPULATION_MUTATOR_STRINGS
+                                definitions.POPULATION_MUTATION_STRINGS
                             ),
                         )
                     )
                     rslt &= False
         elif (
             self.options.population_mutation
-            not in definitions.POPULATION_MUTATOR_STRINGS
+            not in definitions.POPULATION_MUTATION_STRINGS
         ):
             self._add_message(
                 "Invalid value of Population Mutation: {0}. Allowed values: {1}".format(
                     self.options.population_mutation,
-                    self._get_allowed_values(definitions.POPULATION_MUTATOR_STRINGS),
+                    self._get_allowed_values(definitions.POPULATION_MUTATION_STRINGS),
+                )
+            )
+            rslt &= False
+        if self.options.gene_mutation is None:
+            self._add_message("Gene Mutation must not be None!")
+            rslt &= False
+        elif not isinstance(self.options.gene_mutation, str):
+            self._add_message("Gene Mutation must be type str!")
+            rslt &= False
+        elif definitions.PARAM_SEPARATOR in self.options.gene_mutation:
+            mutator_strings = [
+                ms.strip()
+                for ms in self.options.gene_mutation.split(definitions.PARAM_SEPARATOR)
+            ]
+            for mutator_string in mutator_strings:
+                if mutator_string not in definitions.GENE_MUTATION_STRINGS:
+                    self._add_message(
+                        "Invalid value of Gene Mutation:\
+                            {0}. Allowed values: {1}".format(
+                            mutator_string,
+                            self._get_allowed_values(definitions.GENE_MUTATION_STRINGS),
+                        )
+                    )
+                    rslt &= False
+        elif self.options.gene_mutation not in definitions.GENE_MUTATION_STRINGS:
+            self._add_message(
+                "Invalid value of Gene Mutation: {0}. Allowed values: {1}".format(
+                    self.options.gene_mutation,
+                    self._get_allowed_values(definitions.GENE_MUTATION_STRINGS),
                 )
             )
             rslt &= False
         if self.options.parent_selection is None:
             self._add_message("Parent Selection must not be None!")
             rslt &= False
         elif not isinstance(self.options.parent_selection, str):
             self._add_message("Parent Selection must be type str!")
             rslt &= False
         elif not self._validate_selection(
             self.options.parent_selection,
             "Parent Selection",
-            (population_size // 2) - self.options.immigration_number,  # type: ignore
+            round(population_size * (keep_elitism_percentage / 100)) - self.options.immigration_number,  # type: ignore
             "Group Size for parent selection cannot have\
             the value below half population!",
         ):
             rslt &= False
         if self.options.requested_cost is None:
             self._add_message("Requested Cost must not be None!")
             rslt &= False
```

### Comparing `gadapt-0.3.6/gadapt/execution/ga_executor.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-from gadapt.factory.ga_factory import BaseGAFactory
-from gadapt.adapters.ga_logging.logging_settings import init_logging
-from gadapt.ga_model.ga_options import GAOptions
-from gadapt.ga_model.ga_results import GAResults
-from gadapt.ga_model.population import Population
-import gadapt.ga_model.message_levels as message_levels
+import random
 
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
+)
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
+)
+from gadapt.operations.sampling.base_sampling import BaseSampling
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
+)
 
-class GAExecutor:
-    """
-    Executor for the genetic algorithm
 
-    Args:
-        ga_options (GAOptions): Options for GA execution
-        factory (GAFactory): Factory for objects creation
+class ParentDiversityChromosomeMutationSelector(BaseChromosomeMutationSelector):
+    """
+    Selects and mutates chromosomes in a population based on their parent diversity.
     """
 
-    def __init__(self, ga_options: GAOptions, factory: BaseGAFactory) -> None:
-        if ga_options is not None:
-            self.ga_options = ga_options
-        self.factory = factory
-
-    def execute(self) -> GAResults:
-        """
-        Executes the genetic algorithm
-        """
-        results = GAResults()
-        try:
-            init_logging(self.ga_options.logging)
-        except Exception as ex:
-            results.messages.append(
-                (
-                    message_levels.WARNING,
-                    "Logging failed. Error message: {exc}".format(exc=str(ex)),
-                )
-            )
-            self.ga_options.logging = False
-        # try:
-        chromosome_mutator = self.factory.get_chromosome_mutator()
-        population_mutator = self.factory.get_population_mutator()
-        exit_checker = self.factory.get_exit_checker()
-        cost_finder = self.factory.get_cost_finder()
-        population_immigrator = self.factory.get_population_immigrator()
-        chromosome_immigrator = self.factory.get_chromosome_immigrator()
-        selector = self.factory.get_parent_selector()
-        crossover = self.factory.get_crossover()
-        variable_updater = self.factory.get_variable_updater()
-        gene_mutator = self.factory.get_gene_mutator()
-        for dv in self.ga_options.decision_variables:
-            dv.gene_mutator = gene_mutator
-        population = Population(
-            self.ga_options,
-            chromosome_mutator=chromosome_mutator,
-            population_mutator=population_mutator,
-            exit_checker=exit_checker,
-            cost_finder=cost_finder,
-            population_immigrator=population_immigrator,
-            chromosome_immigrator=chromosome_immigrator,
-            parent_selector=selector,
-            crossover=crossover,
-            variable_updater=variable_updater,
+    def __init__(
+        self,
+        chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+        gene_mutation_selector: BaseGeneMutationSelector,
+        sampling: BaseSampling,
+    ) -> None:
+        super().__init__(chromosome_mutation_rate_determinator, gene_mutation_selector)
+        self._sampling = sampling
+
+    def _sort_key_parent_diversity_random(self, c: Chromosome):
+        return (c.parent_diversity, random.random())
+
+    def _mutate_population(self):
+        if self.population is None:
+            raise Exception("Population must not be null")
+        unallocated_chromosomes: list[Chromosome] = self._get_unallocated_chromosomes(
+            self._sort_key_parent_diversity_random
+        )
+        chromosomes_for_mutation: list[Chromosome] = []
+        if self.population.options.must_mutate_for_same_parents:
+            chromosomes_for_mutation = [
+                c for c in unallocated_chromosomes if c.parent_diversity == 0
+            ]
+        chromosomes_for_mutation_count = len(chromosomes_for_mutation)
+        rest_number = (
+            self.number_of_mutation_chromosomes - chromosomes_for_mutation_count
         )
-        population.find_costs()
-        while not population.exit():
-            population.immigrate()
-            population.mate()
-            population.mutate()
-            population.find_costs()
-        if population.timeout_expired:
-            results.messages.append((message_levels.WARNING, "Timeout expired!"))
-        best_individual = population.best_individual
-        results.min_cost = population.min_cost
-        results.number_of_iterations = population.population_generation
-        for g in best_individual:
-            results.result_values[g.decision_variable.variable_id] = g.variable_value
-        # except Exception as ex:
-        #    results.success = False
-        #    results.messages.append((message_levels.ERROR, str(ex)))
-        return results
+        if rest_number > 0:
+            if self.population.options.must_mutate_for_same_parents:
+                other_chromosomes_for_mutation = [
+                    c for c in unallocated_chromosomes if (not c.parent_diversity == 0)
+                ]
+            else:
+                other_chromosomes_for_mutation = [c for c in unallocated_chromosomes]
+            other_chromosomes_for_mutation = self._sampling.get_sample(
+                other_chromosomes_for_mutation,
+                rest_number,
+                lambda c: c.parent_diversity,
+            )
+            chromosomes_for_mutation.extend(other_chromosomes_for_mutation)
+        for c in chromosomes_for_mutation:
+            self._gene_mutation_selector.mutate(
+                c, self.population.options.number_of_mutation_genes
+            )
+        return len(chromosomes_for_mutation)
```

### Comparing `gadapt-0.3.6/gadapt/factory/ga_base_factory.py` & `gadapt-0.4.0/gadapt/factory/ga_base_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from abc import ABC, abstractmethod
+from typing import Optional
+
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.operations.crossover.base_crossover import BaseCrossover
 from gadapt.operations.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.immigration.population_immigration.base_population_immigrator import (
     BasePopulationImmigrator,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
     BaseGeneMutationSelector,
 )
 from gadapt.operations.mutation.gene_mutation.base_gene_mutator import BaseGeneMutator
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
-    BaseChromosomeMutationRateDeterminator,
-)
 from gadapt.operations.parent_selection.base_parent_selector import BaseParentSelector
-from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
+)
 
 """
     Factory definition for creating  class instances based on GA options
 """
 
 
 class BaseGAFactory(ABC):
 
     def __init__(self) -> None:
         super().__init__()
-        self.cost_finder = None
-        self.population_immigrator = None
-        self.chromosome_immigrator = None
-        self.chromosome_mutator = None
-        self.gene_mutator = None
-        self.population_mutator = None
-        self.parent_selector = None
-        self.gene_combination = None
-        self.exit_checker = None
+        self.population_updater = None
+        self._ga = None
+        self._options = None
         self.variable_updater = None
-        self.crossover = None
+        self.cost_finder: Optional[BaseCostFinder] = None
+        self.population_immigrator: Optional[BasePopulationImmigrator] = None
+        self.chromosome_immigrator: Optional[BaseChromosomeImmigrator] = None
+        self.gene_mutator: Optional[BaseGeneMutator] = None
+        self.gene_mutation_selector: Optional[BaseGeneMutationSelector] = None
+        self.chromosome_mutation_selector: Optional[BaseChromosomeMutationSelector] = (
+            None
+        )
+        self.parent_selector: Optional[BaseParentSelector] = None
+        self.exit_checker: Optional[BaseExitChecker] = None
+        self.crossover: Optional[BaseCrossover] = None
 
     def initialize_factory(self, ga):
         self._ga = ga
         self._options = GAOptions(ga)
 
     def get_cost_finder(self) -> BaseCostFinder:
         """
@@ -64,54 +69,46 @@
         """
         Chromosome Immigrator Instance
         """
         if self.chromosome_immigrator is None:
             self.chromosome_immigrator = self._get_chromosome_immigrator()
         return self.chromosome_immigrator
 
-    def get_chromosome_mutator(self) -> BaseGeneMutationSelector:
+    def get_gene_mutation_selector(self) -> BaseGeneMutationSelector:
         """
-        Chromosome Mutator Instance
+        Gene Mutation Selector Instance
         """
-        if self.chromosome_mutator is None:
-            self.chromosome_mutator = self._get_chromosome_mutator()
-        return self.chromosome_mutator
+        if self.gene_mutation_selector is None:
+            self.gene_mutation_selector = self._get_gene_mutation_selector()
+        return self.gene_mutation_selector
 
     def get_gene_mutator(self) -> BaseGeneMutator:
         """
         Gene Mutator Instance
         """
         if self.gene_mutator is None:
             self.gene_mutator = self._get_gene_mutator()
         return self.gene_mutator
 
-    def get_population_mutator(self) -> BaseChromosomeMutationRateDeterminator:
+    def get_chromosome_mutation_selector(self) -> BaseChromosomeMutationSelector:
         """
-        Population Mutator Instance
+        Chromosome Mutation Selector Instance
         """
-        if self.population_mutator is None:
-            self.population_mutator = self._get_population_mutator()
-        return self.population_mutator
+        if self.chromosome_mutation_selector is None:
+            self.chromosome_mutation_selector = self._get_chromosome_mutation_selector()
+        return self.chromosome_mutation_selector
 
     def get_parent_selector(self) -> BaseParentSelector:
         """
         Parent Selector Instance
         """
         if self.parent_selector is None:
             self.parent_selector = self._get_parent_selector()
         return self.parent_selector
 
-    def get_gene_combination(self) -> BaseGeneCombination:
-        """
-        Gene Combination Instance
-        """
-        if self.gene_combination is None:
-            self.gene_combination = self._get_gene_combination()
-        return self.gene_combination
-
     def get_exit_checker(self) -> BaseExitChecker:
         """
         Exit Checker Instance
         """
         if self.exit_checker is None:
             self.exit_checker = self._get_exit_checker()
         return self.exit_checker
@@ -120,14 +117,22 @@
         """
         Variable Updater Instance
         """
         if self.variable_updater is None:
             self.variable_updater = self._get_variable_updater()
         return self.variable_updater
 
+    def get_population_updater(self):
+        """
+        Population Updater Instance
+        """
+        if self.population_updater is None:
+            self.population_updater = self._get_population_updater()
+        return self.population_updater
+
     def get_crossover(self) -> BaseCrossover:
         """
         Crossover Instance
         """
         if self.crossover is None:
             self.crossover = self._get_crossover()
         return self.crossover
@@ -150,61 +155,61 @@
     def _get_chromosome_immigrator(self) -> BaseChromosomeImmigrator:
         """
         Chromosome Immigrator Instance
         """
         pass
 
     @abstractmethod
-    def _get_chromosome_mutator(self) -> BaseGeneMutationSelector:
+    def _get_gene_mutation_selector(self) -> BaseGeneMutationSelector:
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
-    def _get_population_mutator(self) -> BaseChromosomeMutationRateDeterminator:
+    def _get_chromosome_mutation_selector(self) -> BaseChromosomeMutationSelector:
         """
         Population Mutator Instance
         """
         pass
 
     @abstractmethod
     def _get_parent_selector(self) -> BaseParentSelector:
         """
         Parent Selector Instance
         """
         pass
 
     @abstractmethod
-    def _get_gene_combination(self) -> BaseGeneCombination:
+    def _get_exit_checker(self) -> BaseExitChecker:
         """
-        Gene Combination Instance
+        Exit Checker Instance
         """
         pass
 
     @abstractmethod
-    def _get_exit_checker(self) -> BaseExitChecker:
+    def _get_variable_updater(self):
         """
-        Exit Checker Instance
+        Variable Updater Instance
         """
         pass
 
     @abstractmethod
-    def _get_variable_updater(self):
+    def _get_population_updater(self):
         """
-        Variable Updater Instance
+        Population Updater Instance
         """
         pass
 
     @abstractmethod
-    def _get_crossover(self):
+    def _get_crossover(self) -> BaseCrossover:
         """
         Crossover Instance
         """
         pass
```

### Comparing `gadapt-0.3.6/gadapt/factory/ga_factory.py` & `gadapt-0.4.0/gadapt/factory/ga_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from typing import Tuple, List
+
+import gadapt.ga_model.definitions as definitions
 from gadapt.factory.ga_base_factory import BaseGAFactory
+from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
+from gadapt.operations.cost_finding.elitism_cost_finder import ElitismCostFinder
+from gadapt.operations.crossover.base_crossover import BaseCrossover
+from gadapt.operations.crossover.blending_parent_diversity_crossover import (
+    BlendingParentDiversityCrossover,
+)
 from gadapt.operations.exit_check.avg_cost_exit_checker import AvgCostExitChecker
 from gadapt.operations.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.operations.exit_check.min_cost_exit_checker import MinCostExitChecker
 from gadapt.operations.exit_check.requested_cost_exit_checker import (
     RequestedCostExitChecker,
 )
-from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
-from gadapt.operations.cost_finding.elitism_cost_finder import ElitismCostFinder
-from gadapt.operations.crossover.base_crossover import BaseCrossover
-from gadapt.operations.crossover.uniform_crossover import UniformCrossover
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.immigration.chromosome_immigration.random_chromosome_immigrator import (
     RandomChromosomeImmigrator,
 )
 from gadapt.operations.immigration.population_immigration.base_population_immigrator import (
@@ -20,171 +25,215 @@
 )
 from gadapt.operations.immigration.population_immigration.common_population_immigrator import (
     CommonPopulationImmigrator,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
     BaseGeneMutationSelector,
 )
+from gadapt.operations.mutation.chromosome_mutation.composed_gene_mutation_rate_determinator import (
+    ComposedGeneMutationRateDeterminator,
+)
+from gadapt.operations.mutation.chromosome_mutation.composed_gene_mutation_selector import (
+    ComposedGeneMutationSelector,
+)
+from gadapt.operations.mutation.chromosome_mutation.cross_diversity_gene_mutation_rate_determinator import (
+    CrossDiversityGeneMutationRateDeterminator,
+)
 from gadapt.operations.mutation.chromosome_mutation.cross_diversity_gene_mutation_selector import (
     CrossDiversityGeneMutationSelector,
 )
+from gadapt.operations.mutation.chromosome_mutation.random_gene_mutation_rate_determinator import (
+    RandomGeneMutationRateDeterminator,
+)
 from gadapt.operations.mutation.chromosome_mutation.random_gene_mutation_selector import (
     RandomGeneMutationSelector,
 )
+from gadapt.operations.mutation.chromosome_mutation.strict_gene_mutation_rate_determinator import (
+    StrictGeneMutationRateDeterminator,
+)
 from gadapt.operations.mutation.gene_mutation.base_gene_mutator import BaseGeneMutator
 from gadapt.operations.mutation.gene_mutation.extreme_pointed_gene_mutator import (
     ExtremePointedGeneMutator,
 )
 from gadapt.operations.mutation.gene_mutation.normal_distribution_gene_mutator import (
     NormalDistributionGeneMutator,
 )
 from gadapt.operations.mutation.gene_mutation.random_gene_mutator import (
     RandomGeneMutator,
 )
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
+)
+from gadapt.operations.mutation.population_mutation.composed_chromosome_mutation_rate_determinator import (
+    ComposedChromosomeMutationRateDeterminator,
+)
 from gadapt.operations.mutation.population_mutation.composed_chromosome_mutation_selector import (
     ComposedChromosomeMutationSelector,
 )
 from gadapt.operations.mutation.population_mutation.cost_diversity_chromosome_mutation_rate_determinator import (
     CostDiversityChromosomeMutationRateDeterminator,
 )
 from gadapt.operations.mutation.population_mutation.cross_diversity_chromosome_mutation_rate_determinator import (
     CrossDiversityChromosomeMutationRateDeterminator,
 )
 from gadapt.operations.mutation.population_mutation.parent_diversity_chromosome_mutation_selector import (
     ParentDiversityChromosomeMutationSelector,
 )
+from gadapt.operations.mutation.population_mutation.random_chromosome_mutation_rate_determinator import (
+    RandomChromosomeMutationRateDeterminator,
+)
 from gadapt.operations.mutation.population_mutation.random_chromosome_mutation_selector import (
     RandomChromosomeMutationSelector,
 )
+from gadapt.operations.mutation.population_mutation.strict_chromosome_mutation_rate_determinator import (
+    StrictChromosomeMutationRateDeterminator,
+)
 from gadapt.operations.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.operations.parent_selection.sampling_parent_selector import (
     SamplingParentSelector,
 )
 from gadapt.operations.sampling.base_sampling import BaseSampling
 from gadapt.operations.sampling.from_top_to_bottom_sampling import (
     FromTopToBottomSampling,
 )
 from gadapt.operations.sampling.random_sampling import RandomSampling
 from gadapt.operations.sampling.roulette_wheel_sampling import RouletteWheelSampling
 from gadapt.operations.sampling.tournament_sampling import TournamentSampling
-from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
-from gadapt.operations.gene_combination.blending_gene_combination import (
-    BlendingGeneCombination,
-)
 from gadapt.operations.variable_update.common_variable_updater import (
     CommonVariableUpdater,
 )
-import gadapt.ga_model.definitions as definitions
-from gadapt.operations.mutation.chromosome_mutation.composed_gene_mutation_rate_determinator import (
-    ComposedGeneMutationRateDeterminator,
-)
-from gadapt.operations.mutation.chromosome_mutation.composed_gene_mutation_selector import (
-    ComposedGeneMutationSelector,
-)
-from gadapt.operations.mutation.chromosome_mutation.cross_diversity_gene_mutation_rate_determinator import (
-    CrossDiversityGeneMutationRateDeterminator,
-)
-from gadapt.operations.mutation.chromosome_mutation.random_gene_mutation_rate_determinator import (
-    RandomGeneMutationRateDeterminator,
+from gadapt.operations.crossover.blending_crossover import BlendingCrossover
+from gadapt.operations.crossover.uniform_crossover import UniformCrossover
+from gadapt.operations.exit_check.number_of_generations_exit_checker import (
+    NumberOfGenerationsExitChecker,
 )
-from gadapt.operations.mutation.chromosome_mutation.strict_gene_mutation_rate_determinator import (
-    StrictGeneMutationRateDeterminator,
+from gadapt.operations.mutation.gene_mutation.composed_gene_mutator import (
+    ComposedGeneMutator,
 )
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
-    BaseChromosomeMutationSelector,
+from gadapt.operations.mutation.gene_mutation.normal_distribution_cross_diversity_gene_mutator import (
+    NormalDistributionCrossDiversityGeneMutator,
 )
-from gadapt.operations.mutation.population_mutation.composed_chromosome_mutation_rate_determinator import (
-    ComposedChromosomeMutationRateDeterminator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
-from gadapt.operations.mutation.population_mutation.random_chromosome_mutation_rate_determinator import (
-    RandomChromosomeMutationRateDeterminator,
-)
-from gadapt.operations.mutation.population_mutation.strict_chromosome_mutation_rate_determinator import (
-    StrictChromosomeMutationRateDeterminator,
+from gadapt.operations.population_update.common_population_updater import (
+    CommonPopulationUpdater,
 )
 
 
 class GAFactory(BaseGAFactory):
     """
     Factory implementatiopn for creating  class instances based on GA options
     """
 
+    def __init__(self):
+        super().__init__()
+        self.gene_mutation_rate_determinator = None
+        self.chromosome_mutation_rate_determinator = None
+
     def _get_cost_finder(self) -> BaseCostFinder:
         """
         Cost Finder instance
         """
         return ElitismCostFinder()
 
     def _get_population_immigrator(self) -> BasePopulationImmigrator:
         """
         Population Immigrator Instance
         """
-        return CommonPopulationImmigrator()
+        return CommonPopulationImmigrator(self.get_chromosome_immigrator())
 
     def _get_chromosome_immigrator(self) -> BaseChromosomeImmigrator:
         """
         Chromosome Immigrator Instance
         """
         return RandomChromosomeImmigrator()
 
-    def _get_chromosome_mutator(self) -> BaseGeneMutationSelector:
+    def _get_gene_mutation_selector(self) -> BaseGeneMutationSelector:
         """
-        Chromosome Mutator Instance
+        Gene Mutation Selector Instance
         """
-        return self._get_chromosome_mutator_combined()
+        return self._get_gene_mutation_selector_combined()
+
+    def _get_gene_mutator_combined(self) -> BaseGeneMutator:
+        if self._ga is None:
+            raise Exception("_ga object must not be None!")
+        mutator_strings = [
+            gm.strip()
+            for gm in self._ga.gene_mutation.split(definitions.PARAM_SEPARATOR)
+        ]
+        gene_mutators: List[BaseGeneMutator] = []
+        if definitions.RANDOM in mutator_strings:
+            gene_mutators.append(RandomGeneMutator())
+        if definitions.EXTREME_POINTED in mutator_strings:
+            gene_mutators.append(ExtremePointedGeneMutator())
+        if definitions.CROSS_DIVERSITY in mutator_strings:
+            gene_mutators.append(NormalDistributionCrossDiversityGeneMutator())
+        elif definitions.NORMAL_DISTRIBUTION in mutator_strings:
+            gene_mutators.append(NormalDistributionGeneMutator())
+        if len(gene_mutators) == 0:
+            gene_mutators.append(NormalDistributionGeneMutator())
+            gene_mutators.append(RandomGeneMutator())
+        if len(gene_mutators) == 1:
+            return gene_mutators[0]
+        else:
+            main_gene_mutator = ComposedGeneMutator()
+            for mutator in gene_mutators:
+                main_gene_mutator.append(mutator)
+        return main_gene_mutator
 
     def _get_gene_mutator(self) -> BaseGeneMutator:
         """
         Chromosome Mutator Instance
         """
-        if self._ga.gene_mutation.strip() == definitions.EXTREME_POINTED:
-            return ExtremePointedGeneMutator()
-        elif self._ga.gene_mutation.strip() == definitions.RANDOM:
-            return RandomGeneMutator()
-        elif self._ga.gene_mutation.strip() == definitions.NORMAL_DISTRIBUTION:
-            return NormalDistributionGeneMutator()
-        else:
-            raise Exception("unknown gene mutation")
+        return self._get_gene_mutator_combined()
 
-    def _population_mutator_options_validation(self):
+    def _population_mutation_options_validation(self):
         """
         Validates population mutator options
         """
         mutator_strings = self._ga.population_mutation.split(
             definitions.PARAM_SEPARATOR
         )
         for s in mutator_strings:
-            if s.strip() not in definitions.POPULATION_MUTATOR_STRINGS:
+            if s.strip() not in definitions.POPULATION_MUTATION_STRINGS:
                 raise Exception(s + " is not defined as option for population mutation")
 
-    def _make_population_mutator(
+    def _make_chromosome_mutation_selector(
         self, population_mutator_string=None
     ) -> BaseChromosomeMutationSelector:
         """
         Population Mutator Instance
         """
-        self._population_mutator_options_validation()
-        return self._get_population_mutator_combined()
+        self._population_mutation_options_validation()
+        return self._get_chromosome_mutation_selector_combined()
 
-    def _get_population_mutator(self) -> BaseChromosomeMutationSelector:
+    def _get_chromosome_mutation_selector(self) -> BaseChromosomeMutationSelector:
         """
         Population Mutator Instance
         """
-        return self._make_population_mutator()
+        return self._make_chromosome_mutation_selector()
 
-    def _get_population_mutator_combined(self) -> BaseChromosomeMutationSelector:
-        """
-        Population Mutator Instance - combined
-        """
+    def _get_chromosome_mutation_rate_determinators(
+        self,
+    ) -> Tuple[
+        BaseChromosomeMutationRateDeterminator, BaseChromosomeMutationRateDeterminator
+    ]:
+        if self._ga is None:
+            raise Exception("_ga object must not be None!")
+        if self.chromosome_mutation_rate_determinator is not None:
+            return self.chromosome_mutation_rate_determinator
         mutator_strings = [
             ms.strip()
             for ms in self._ga.population_mutation.split(definitions.PARAM_SEPARATOR)
         ]
-        chromosome_mutation_rate_determinators = []
-        chromosome_mutation_selectors = []
+        chromosome_mutation_rate_determinators: List[
+            BaseChromosomeMutationRateDeterminator
+        ] = []
+
         if definitions.RANDOM in mutator_strings:
             chromosome_mutation_rate_determinators.append(
                 RandomChromosomeMutationRateDeterminator()
             )
         if definitions.CROSS_DIVERSITY in mutator_strings:
             chromosome_mutation_rate_determinators.append(
                 CrossDiversityChromosomeMutationRateDeterminator()
@@ -194,78 +243,106 @@
                 CostDiversityChromosomeMutationRateDeterminator()
             )
         if len(chromosome_mutation_rate_determinators) == 0:
             chromosome_mutation_rate_determinators.append(
                 CostDiversityChromosomeMutationRateDeterminator()
             )
         if len(chromosome_mutation_rate_determinators) == 1:
-            main_chromosome_mutation_rate_determinator = (
-                chromosome_mutation_rate_determinators[0]
-            )
+            main_chromosome_mutation_rate_determinator: (
+                BaseChromosomeMutationRateDeterminator
+            ) = chromosome_mutation_rate_determinators[0]
         else:
             main_chromosome_mutation_rate_determinator = (
                 ComposedChromosomeMutationRateDeterminator()
             )
             for determinator in chromosome_mutation_rate_determinators:
                 main_chromosome_mutation_rate_determinator.append(determinator)
         if (
             definitions.RANDOM in mutator_strings
             and definitions.PARENT_DIVERSITY in mutator_strings
         ):
-            helper_chromosome_mutation_rate_determinator = (
-                StrictChromosomeMutationRateDeterminator()
-            )
+            helper_chromosome_mutation_rate_determinator: (
+                BaseChromosomeMutationRateDeterminator
+            ) = StrictChromosomeMutationRateDeterminator()
         else:
             helper_chromosome_mutation_rate_determinator = (
                 main_chromosome_mutation_rate_determinator
             )
+        return (
+            main_chromosome_mutation_rate_determinator,
+            helper_chromosome_mutation_rate_determinator,
+        )
+
+    def _get_chromosome_mutation_selector_combined(
+        self,
+    ) -> BaseChromosomeMutationSelector:
+        """
+        Population Mutator Instance - combined
+        """
+        if self._ga is None:
+            raise Exception("_ga object must not be None!")
+        mutator_strings = [
+            ms.strip()
+            for ms in self._ga.population_mutation.split(definitions.PARAM_SEPARATOR)
+        ]
+        (
+            main_chromosome_mutation_rate_determinator,
+            helper_chromosome_mutation_rate_determinator,
+        ) = self._get_chromosome_mutation_rate_determinators()
+        chromosome_mutation_selectors: List[BaseChromosomeMutationSelector] = []
         if definitions.RANDOM in mutator_strings:
             chromosome_mutation_selectors.append(
                 RandomChromosomeMutationSelector(
-                    helper_chromosome_mutation_rate_determinator
+                    helper_chromosome_mutation_rate_determinator,
+                    self._get_gene_mutation_selector(),
                 )
             )
         if definitions.PARENT_DIVERSITY in mutator_strings:
             chromosome_mutation_selectors.append(
                 ParentDiversityChromosomeMutationSelector(
                     helper_chromosome_mutation_rate_determinator,
+                    self._get_gene_mutation_selector(),
                     self._get_sampling_method(
-                        self._ga.parent_diversity_mutation_chromosome_selection
+                        self._ga.parent_diversity_mutation_chromosome_sampling
                     ),
                 )
             )
         if len(chromosome_mutation_selectors) == 0:
             chromosome_mutation_selectors.append(
                 ParentDiversityChromosomeMutationSelector(
                     helper_chromosome_mutation_rate_determinator,
+                    self._get_gene_mutation_selector(),
                     self._get_sampling_method(
-                        self._ga.parent_diversity_mutation_chromosome_selection
+                        self._ga.parent_diversity_mutation_chromosome_sampling
                     ),
                 )
             )
         if len(chromosome_mutation_selectors) == 1:
-            chromosome_mutation_selector = chromosome_mutation_selectors[0]
+            return chromosome_mutation_selectors[0]
         else:
             chromosome_mutation_selector = ComposedChromosomeMutationSelector(
-                main_chromosome_mutation_rate_determinator
+                main_chromosome_mutation_rate_determinator,
+                self._get_gene_mutation_selector(),
             )
             for selector in chromosome_mutation_selectors:
                 chromosome_mutation_selector.append(selector)
         return chromosome_mutation_selector
 
-    def _get_chromosome_mutator_combined(self) -> BaseGeneMutationSelector:
-        """
-        Chromosome Mutator Instance - combined
-        """
+    def _get_gene_mutation_rate_determinators(self):
+        if self.gene_mutation_rate_determinator is not None:
+            return (
+                self.gene_mutation_rate_determinator,
+                self.gene_mutation_rate_determinator,
+            )
         mutator_strings = [
             ms.strip()
             for ms in self._ga.chromosome_mutation.split(definitions.PARAM_SEPARATOR)
         ]
         gene_mutation_rate_determinators = []
-        gene_mutation_selectors = []
+
         if definitions.RANDOM in mutator_strings:
             gene_mutation_rate_determinators.append(
                 RandomGeneMutationRateDeterminator()
             )
         if definitions.CROSS_DIVERSITY in mutator_strings:
             gene_mutation_rate_determinators.append(
                 CrossDiversityGeneMutationRateDeterminator()
@@ -292,33 +369,56 @@
             helper_gene_mutation_rate_determinator = (
                 StrictGeneMutationRateDeterminator()
             )
         else:
             helper_gene_mutation_rate_determinator = (
                 main_gene_mutation_rate_determinator
             )
+        return (
+            main_gene_mutation_rate_determinator,
+            helper_gene_mutation_rate_determinator,
+        )
+
+    def _get_gene_mutation_selector_combined(self) -> BaseGeneMutationSelector:
+        """
+        Chromosome Mutator Instance - combined
+        """
+        if self._ga is None:
+            raise Exception("_ga object must not be None!")
+        mutator_strings = [
+            ms.strip()
+            for ms in self._ga.chromosome_mutation.split(definitions.PARAM_SEPARATOR)
+        ]
+        main_gene_mutation_rate_determinator, helper_gene_mutation_rate_determinator = (
+            self._get_gene_mutation_rate_determinators()
+        )
+        gene_mutation_selectors = []
         if definitions.RANDOM in mutator_strings:
             gene_mutation_selectors.append(
-                RandomGeneMutationSelector(helper_gene_mutation_rate_determinator)
+                RandomGeneMutationSelector(
+                    helper_gene_mutation_rate_determinator, self.get_gene_mutator()
+                ),
             )
         if definitions.CROSS_DIVERSITY in mutator_strings:
             gene_mutation_selectors.append(
                 CrossDiversityGeneMutationSelector(
                     helper_gene_mutation_rate_determinator,
+                    self.get_gene_mutator(),
                     self._get_sampling_method(
-                        self._ga.cross_diversity_mutation_gene_selection
+                        self._ga.cross_diversity_mutation_gene_sampling
                     ),
                 )
             )
         if len(gene_mutation_selectors) == 0:
             gene_mutation_selectors.append(
                 CrossDiversityGeneMutationSelector(
                     helper_gene_mutation_rate_determinator,
+                    self.get_gene_mutator(),
                     self._get_sampling_method(
-                        self._ga.cross_diversity_mutation_gene_selection
+                        self._ga.cross_diversity_mutation_gene_sampling
                     ),
                 )
             )
         if len(gene_mutation_selectors) == 1:
             gene_mutation_selector = gene_mutation_selectors[0]
         else:
             gene_mutation_selector = self.get_composed_gene_mutation_selector(
@@ -334,33 +434,36 @@
         gene_mutation_selectors,
         helper_gene_mutation_rate_determinator,
     ):
         if not gene_mutation_selectors:
             gene_mutation_selectors.append(
                 CrossDiversityGeneMutationSelector(
                     helper_gene_mutation_rate_determinator,
+                    self.get_gene_mutator(),
                     self._get_sampling_method(
-                        self._ga.cross_diversity_mutation_gene_selection
+                        self._ga.cross_diversity_mutation_gene_sampling
                     ),
                 )
             )
             gene_mutation_selectors.append(
                 RandomGeneMutationSelector(helper_gene_mutation_rate_determinator)
             )
         gene_mutation_selector = ComposedGeneMutationSelector(
-            main_gene_mutation_rate_determinator
+            main_gene_mutation_rate_determinator, self.get_gene_mutator()
         )
         for selector in gene_mutation_selectors:
             gene_mutation_selector.append(selector)
         return gene_mutation_selector
 
     def _get_parent_selector(self) -> BaseParentSelector:
         """
         Parent Selector Instance
         """
+        if self._ga is None:
+            raise Exception("_ga object must not be None!")
         return SamplingParentSelector(
             self._get_sampling_method(self._ga.parent_selection)
         )
 
     def _get_sampling_method(self, str) -> BaseSampling:
         """
         Sampling Methos Instance
@@ -378,38 +481,70 @@
             return TournamentSampling(other_value)
         elif str_value == definitions.FROM_TOP_TO_BOTTOM:
             return FromTopToBottomSampling()
         elif str_value == definitions.RANDOM:
             return RandomSampling()
         return RouletteWheelSampling()
 
-    def _get_gene_combination(self) -> BaseGeneCombination:
-        """
-        Gene Combination Instance
-        """
-        return BlendingGeneCombination()
-
     def _get_exit_checker(self) -> BaseExitChecker:
         """
         Exit Checker Instance
         """
+        if self._ga is None:
+            raise Exception("ga object must not be None!")
         if self._ga.exit_check == definitions.AVG_COST:
             return AvgCostExitChecker(self._ga.max_attempt_no)
         if self._ga.exit_check == definitions.MIN_COST:
             return MinCostExitChecker(self._ga.max_attempt_no)
+        if self._ga.exit_check == definitions.GENERATIONS:
+            return NumberOfGenerationsExitChecker(self._ga.number_of_generations)
         return RequestedCostExitChecker(self._ga.requested_cost)
 
     def _get_crossover(self) -> BaseCrossover:
         """
         Crossover Instance
         """
-        return UniformCrossover(
-            self.get_gene_combination(),
-            self.get_chromosome_mutator(),
+        if self._ga is None:
+            raise Exception("ga object must not be None!")
+        mutator_strings = [
+            ms.strip()
+            for ms in self._ga.population_mutation.split(definitions.PARAM_SEPARATOR)
+        ]
+        population_mutation_selection_strings = [
+            value
+            for value in mutator_strings
+            if value in definitions.POPULATION_MUTATION_SELECTION_STRINGS
+        ]
+        if (
+            not population_mutation_selection_strings
+            or definitions.PARENT_DIVERSITY in mutator_strings
+        ):
+            return BlendingParentDiversityCrossover(
+                self.get_gene_mutation_selector(),
+                self.get_chromosome_immigrator(),
+            )
+        if self._ga.crossover == definitions.BLENDING:
+            return BlendingCrossover(
+                self.get_gene_mutation_selector(),
+                self.get_chromosome_immigrator(),
+            )
+        if self._ga.crossover == definitions.UNIFORM:
+            return UniformCrossover(
+                self.get_gene_mutation_selector(),
+                self.get_chromosome_immigrator(),
+            )
+        return BlendingParentDiversityCrossover(
+            self.get_gene_mutation_selector(),
             self.get_chromosome_immigrator(),
         )
 
     def _get_variable_updater(self):
         """
         Variable Updater Instance
         """
         return CommonVariableUpdater()
+
+    def _get_population_updater(self):
+        """
+        Population Updater Instance
+        """
+        return CommonPopulationUpdater()
```

### Comparing `gadapt-0.3.6/gadapt/ga.py` & `gadapt-0.4.0/gadapt/ga.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 """
 The main genetic algorithm module
 """
 
 import sys
-from typing import List
+from typing import List, Optional
+
+import gadapt.ga_model.definitions as definitions
+import gadapt.utils.ga_utils as ga_utils
+from gadapt.adapters.validation.common_options_validator import CommonOptionsValidator
 from gadapt.execution.ga_executor import GAExecutor
 from gadapt.factory.ga_base_factory import BaseGAFactory
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga_model.decision_variable import DecisionVariable
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
-import gadapt.utils.ga_utils as ga_utils
-import gadapt.ga_model.definitions as definitions
-from gadapt.adapters.validation.common_options_validator import CommonOptionsValidator
 
 
 class GA:
     """
     The main genetic algorithm class
     """
 
     def __init__(
         self,
         cost_function=None,
-        population_size=64,
+        population_size=32,
+        keep_elitism_percentage=50,
+        number_of_crossover_parents=-1,
         exit_check=definitions.AVG_COST,
         requested_cost=sys.float_info.max,
-        max_attempt_no=10,
+        number_of_generations=200,
+        max_attempt_no=2,
         parent_selection=definitions.ROULETTE_WHEEL,
-        population_mutation="{0}{1}{2}".format(
+        crossover=definitions.BLENDING,
+        population_mutation="{0}{1}{2}{3}{4}".format(
             definitions.COST_DIVERSITY,
             definitions.PARAM_SEPARATOR,
+            definitions.CROSS_DIVERSITY,
+            definitions.PARAM_SEPARATOR,
             definitions.PARENT_DIVERSITY,
         ),
         number_of_mutation_chromosomes=-1,
-        percentage_of_mutation_chromosomes=10.0,
-        parent_diversity_mutation_chromosome_selection=definitions.ROULETTE_WHEEL,
+        percentage_of_mutation_chromosomes=50.0,
+        parent_diversity_mutation_chromosome_sampling=definitions.ROULETTE_WHEEL,
         must_mutate_for_same_parents=True,
-        chromosome_mutation=definitions.CROSS_DIVERSITY,
-        gene_mutation=definitions.NORMAL_DISTRIBUTION,
+        chromosome_mutation=f"{definitions.CROSS_DIVERSITY}{definitions.PARAM_SEPARATOR}{definitions.RANDOM}",
+        gene_mutation=f"{definitions.CROSS_DIVERSITY}{definitions.PARAM_SEPARATOR}{definitions.RANDOM}",
         number_of_mutation_genes=-1,
-        percentage_of_mutation_genes=10.0,
-        cross_diversity_mutation_gene_selection=definitions.ROULETTE_WHEEL,
+        percentage_of_mutation_genes=20.0,
+        cross_diversity_mutation_gene_sampling=definitions.ROULETTE_WHEEL,
         immigration_number=0,
         logging=False,
         timeout=120,
-        factory: BaseGAFactory = None,
+        factory: Optional[BaseGAFactory] = None,
     ) -> None:
         """
         The constructor of the GA class accepts all parameters required to
         create an instance of the GA class. It validates such parameters.
 
         Args:
             cost_function: Custom function for the cost calculation (fitness).
@@ -67,19 +74,23 @@
 
             exit_check: A criteria for the exit for the genetic algorithm
 
             requested_cost: This parameter only takes place when exit_check
             has value “requested”. It determines the requested value
             which causes the exit from the genetic algorithm
 
+            number_of_generations: This parameter only takes place when exit_check
+            has value “generations”. It determines the number of generations
+            after which the genetic algorithm exits
+
             max_attempt_no: This parameter only takes place when exit_check
             has value “avg_cost” or “min_cost”. It determines the number of
             generations in which there is no improvement in the average/minimal cost.
 
-            parent_selection: The algorithm for parent selection.
+            parent_selection: The sampling algorithm in parent selection.
 
             population_mutation: A type of mutation for the entire population.
 
                 Based on the value of this parameter, the number of mutation
                 chromosomes can be determined, along with how
                 chromosomes for the mutation will be selected.
 
@@ -105,16 +116,16 @@
                 The calculated value is an upper bound - the actual
                 number of mutated chromosomes can vary from 1 to the calculated value.
 
                 percentage_of_mutation_chromosomes only applies if
                 number_of_mutation_chromosomes does not have a valid
                 integer value equal to or higher than 0.
 
-            parent_diversity_mutation_chromosome_selection: The
-            selection algorithm for mutating chromosomes when population_mutation
+            parent_diversity_mutation_chromosome_sampling: The
+            sampling algorithm for mutating chromosomes when population_mutation
             contains value “parent_diversity”.
                 It only applies when population_mutation has value
                 “parent_diversity”. It determines the way how chromosomes are to
                 be selected based on the diversity of their parents.
 
             must_mutate_for_same_parents: Indicates if completely the same
             parents must influence mutation for their children.
@@ -146,15 +157,15 @@
                 The calculated value is the upper bound - the actual number of
                 mutated genes can vary from 1 to the calculated value.
 
                 percentage_of_mutation_genes only applies if
                 number_of_mutations_genes does not have a valid
                 integer value equal to or higher than 0.
 
-            cross_diversity_mutation_gene_selection: The selection algorithm for
+            cross_diversity_mutation_gene_sampling: The sampling algorithm for
             mutating chromosomes when chromosome_mutation has value “cross_diversity”.
                 It only applies when chromosome_mutation has value
                 “cross_diversity” . It determines the way how genes
                 are to be selected based on the cross-diversity.
 
             immigration_number: Refers to the “Random Immigrants”
             concepts. This strategy introduces a certain number of
@@ -172,34 +183,38 @@
             optimisation will exit, regardless of whether
             exit_check criteria is reached.
 
             factory: Factory for creating object
         """
         self.cost_function = cost_function
         self.population_size = population_size
+        self.keep_elitism_percentage = keep_elitism_percentage
+        self.number_of_crossover_parents = number_of_crossover_parents
         self.exit_check = exit_check
         self.requested_cost = requested_cost
+        self.number_of_generations = number_of_generations
         self.max_attempt_no = max_attempt_no
         self.parent_selection = parent_selection
+        self.crossover = crossover
         self.population_mutation = population_mutation
         self.must_mutate_for_same_parents = must_mutate_for_same_parents
         self.number_of_mutation_chromosomes = number_of_mutation_chromosomes
         self.percentage_of_mutation_chromosomes = percentage_of_mutation_chromosomes
         self.number_of_mutation_genes = number_of_mutation_genes
         self.percentage_of_mutation_genes = percentage_of_mutation_genes
         self.chromosome_mutation = chromosome_mutation
         self.gene_mutation = gene_mutation
         self.immigration_number = immigration_number
         self.logging = logging
         self._decision_variables: List[DecisionVariable] = []
-        self.cross_diversity_mutation_gene_selection = (
-            cross_diversity_mutation_gene_selection
+        self.cross_diversity_mutation_gene_sampling = (
+            cross_diversity_mutation_gene_sampling
         )
-        self.parent_diversity_mutation_chromosome_selection = (
-            parent_diversity_mutation_chromosome_selection
+        self.parent_diversity_mutation_chromosome_sampling = (
+            parent_diversity_mutation_chromosome_sampling
         )
         self.timeout = timeout
         self._current_dv_id = 0
         self._factory = factory
 
     def execute(self) -> GAResults:
         """
@@ -230,15 +245,42 @@
         """
         return self._population_size
 
     @population_size.setter
     def population_size(self, value: int):
         self._population_size = ga_utils.try_get_int(value)
 
-    def add(self, min_value: float, max_value: float, step: float = 0.01):
+    @property
+    def keep_elitism_percentage(self) -> int:
+        """
+        Percentage number of chromosomes to be kept in the population by the cost value
+        """
+        return self._keep_elitism_percentage
+
+    @keep_elitism_percentage.setter
+    def keep_elitism_percentage(self, value: int):
+        self._keep_elitism_percentage = ga_utils.try_get_int(value)
+
+    @property
+    def number_of_crossover_parents(self) -> int:
+        """
+        Number of parents to be included in the mating pool
+        """
+        return self._number_of_crossover_parents
+
+    @number_of_crossover_parents.setter
+    def number_of_crossover_parents(self, value: int):
+        self._number_of_crossover_parents = ga_utils.try_get_int(value)
+
+    def add(
+        self,
+        min_value: float = -sys.float_info.max,
+        max_value: float = sys.float_info.max,
+        step: float = sys.float_info.min,
+    ):
         """
         Adds variables to be optimized.
         Args:
             min_value (float): lower bound of possible variable values
             max_value (float): upper bound of possible variable values
             step (float): the step that will be used in changing the
             variables values during the optimization
@@ -385,73 +427,73 @@
 
         **"parent_diversity"** - It applies to the way how mutation
         chromosomes will be selected. “parent_diversity” selects
         chromosomes to be mutated using the diversity of their parents.
         The more similar parents (lower parent diversity) mean a higher
         probability of mutation for the child. Based on the calculated
         parent diversity, chromosomes may be selected by one of the
-        selection methods, which is determined by the value of the
-        parent_diversity_mutation_chromosome_selection parameter.
+        sampling methods, which is determined by the value of the
+        parent_diversity_mutation_chromosome_sampling parameter.
 
         **"random"** - It applies to the number of mutation chromosomes
         and to the way how mutation chromosomes will be selected. “random”
         selects chromosomes to be mutated randomly, and randomly
         determines the number of mutated chromosomes (with the
         upper bound of number_of_mutation_chromosomes)
         """
         return self._population_mutation
 
     @population_mutation.setter
     def population_mutation(self, value: str):
         self._population_mutation = ga_utils.prepare_string(value)
 
     @property
-    def parent_diversity_mutation_chromosome_selection(self) -> str:
+    def parent_diversity_mutation_chromosome_sampling(self) -> str:
         """
-        The selection algorithm for mutating chromosomes when
+        The sampling algorithm for mutating chromosomes when
         population_mutation contains value “parent_diversity”.
         It only applies when population_mutation has value
         “parent_diversity”. It determines the way how chromosomes are
         to be selected based on the diversity of their parents.
 
         Supported values:
 
-        **"roulette_wheel"** - The Roulette Wheel selection algorithm
+        **"roulette_wheel"** - The Roulette Wheel sampling algorithm
         (also known as “Weighted Random Pairing”). The probabilities
         assigned to the chromosomes to be mutated are proportional
         to the similarity of their parents (inversely proportional
         to the parent diversity). A chromosome with the lowest
         parent diversity has the greatest probability of
         mutation, while the chromosome with the highest
         parent diversity has the lowest probability of mutation.
 
-        **"tournament"** - The Tournament selection algorithm.
+        **"tournament"** - The Tournament sampling algorithm.
         It randomly picks small subsets (groups) of chromosomes,
         and chromosomes with the lowest parent diversity (highest parent similarity)
         in subsets are chosen to be mutated. “tournament” can have an additional
         parameter separated from the “tournament” keyword by the comma.
         The other value represents a group size. For example, “tournament,8” means
-        that the tournament mutation selection algorithm is chosen, and
+        that the tournament mutation sampling algorithm is chosen, and
         each group contains up to 8 members. The default group size is 4.
 
-        **"from_top_to_bottom"** - From Top To Bottom selection
+        **"from_top_to_bottom"** - From Top To Bottom sampling
         algorithm starts at the top of the list and
         selects chromosomes for mutation.
 
         **"random"** - Random selection algorithm uses a
         uniform random number generator to select
         chromosomes for mutation. In this case,
-        selection for mutation will not depend
+        sampling for mutation will not depend
         on parent diversity.
         """
-        return self._parent_diversity_mutation_chromosome_selection
+        return self._parent_diversity_mutation_chromosome_sampling
 
-    @parent_diversity_mutation_chromosome_selection.setter
-    def parent_diversity_mutation_chromosome_selection(self, value: str):
-        self._parent_diversity_mutation_chromosome_selection = ga_utils.prepare_string(
+    @parent_diversity_mutation_chromosome_sampling.setter
+    def parent_diversity_mutation_chromosome_sampling(self, value: str):
+        self._parent_diversity_mutation_chromosome_sampling = ga_utils.prepare_string(
             value
         )
 
     @property
     def chromosome_mutation(self) -> str:
         """
         The type of mutation of genes in chromosomes.
@@ -460,17 +502,17 @@
 
         **"cross_diversity"** - Considers the diversity of genes of the same
         type in the population. Lower diversity can mean
         that this decision variable approaches some local
         minimums, and therefore such genes increase the
         chance for mutation. Based on the calculated
         cross-diversity, chromosomes may be selected by
-        one of the selection methods, which is
+        one of the sampling methods, which is
         determined by the value of the
-        cross_diversity_mutation_gene_selection parameter.
+        cross_diversity_mutation_gene_sampling parameter.
 
         **"random"** - Genes are randomly selected for the mutation
         """
         return self._chromosome_mutation
 
     @chromosome_mutation.setter
     def chromosome_mutation(self, value: str):
@@ -490,54 +532,54 @@
         return self._gene_mutation
 
     @gene_mutation.setter
     def gene_mutation(self, value: str):
         self._gene_mutation = ga_utils.prepare_string(value)
 
     @property
-    def cross_diversity_mutation_gene_selection(self) -> str:
+    def cross_diversity_mutation_gene_sampling(self) -> str:
         """
-        The selection algorithm for mutating chromosomes when chromosome_mutation
+        The sampling algorithm for mutating chromosomes when chromosome_mutation
         has value “cross_diversity”.
         It only applies when chromosome_mutation has value “cross_diversity” .
         It determines the way how genes are to be selected based on the cross-diversity.
 
         Supported values:
 
-        **"roulette_wheel"** - The Roulette Wheel selection algorithm
+        **"roulette_wheel"** - The Roulette Wheel sampling algorithm
         (also known as “Weighted Random Pairing”). The probabilities
         assigned to the genes to be mutated are inversely
         proportional to their cross-diversity. A gene
         with the lowest cross-diversity has the greatest
         probability of mutation, while the gene with the
         highest cross-diversity has the lowest
         probability of mutation.
 
-        **"tournament"** - The Tournament selection algorithm. It randomly picks
+        **"tournament"** - The Tournament sampling algorithm. It randomly picks
         small subsets (groups) of genes, and genes with the lowest cross-diversity
         in subsets are chosen to be mutated. “tournament” can have
         an additional parameter separated from the “tournament”
         keyword by the comma. The other value represents a group size.
         For example, “tournament,3” means that the tournament
-        mutation selection algorithm is chosen, and each group
+        mutation sampling algorithm is chosen, and each group
         contains up to 3 members. The default group size is 4.
 
-        **"from_top_to_bottom"** - From Top To Bottom selection
+        **"from_top_to_bottom"** - From Top To Bottom sampling
         algorithm starts at the top of the list and selects genes for mutation.
 
-        **"random"** - Random selection algorithm uses a
+        **"random"** - Random sampling algorithm uses a
         uniform random number generator to select genes for mutation.
-        In this case, selection for the mutation will not
+        In this case, sampling for the mutation will not
         depend on gene cross-diversity.
         """
-        return self._cross_diversity_mutation_gene_selection
+        return self._cross_diversity_mutation_gene_sampling
 
-    @cross_diversity_mutation_gene_selection.setter
-    def cross_diversity_mutation_gene_selection(self, value: str):
-        self._cross_diversity_mutation_gene_selection = ga_utils.prepare_string(value)
+    @cross_diversity_mutation_gene_sampling.setter
+    def cross_diversity_mutation_gene_sampling(self, value: str):
+        self._cross_diversity_mutation_gene_sampling = ga_utils.prepare_string(value)
 
     @property
     def max_attempt_no(self) -> int:
         """
         This parameter only takes place when exit_check has value “avg_cost”
         or “min_cost”. It determines the number of generations
         in which there is no improvement in the average/minimal cost.
@@ -568,52 +610,84 @@
         return self._exit_check
 
     @exit_check.setter
     def exit_check(self, value: str):
         self._exit_check = ga_utils.prepare_string(value)
 
     @property
+    def number_of_generations(self) -> float:
+        """
+        This parameter only takes place when exit_check
+        has value “generations”. It determines the number of generations
+        after which the genetic algorithm exits
+        """
+        return self._number_of_generations
+
+    @number_of_generations.setter
+    def number_of_generations(self, value: float):
+        self._number_of_generations = ga_utils.try_get_float(value)
+
+    @property
     def parent_selection(self) -> str:
         """
-        The algorithm for parent selection.
+        The algorithm for sampling algorithm in parent selection.
 
         Supported values:
 
-        **"roulette_wheel"** - Roulette Wheel selection algorithm
+        **"roulette_wheel"** - Roulette Wheel sampling algorithm
         (also known as “Weighted Random Pairing”).
         The probabilities assigned to the chromosomes in the mating pool are
         inversely proportional to their cost. A chromosome with the lowest
         cost has the greatest probability of mating, while the chromosome
         with the highest cost has the lowest probability of mating.
 
-        **"tournament"** - Tournament selection algorithm. It randomly picks small
+        **"tournament"** - Tournament sampling algorithm. It randomly picks small
         subsets (groups) of chromosomes from the mating pool, and chromosomes
         with the lowest cost in subsets become a parent. “tournament”
         can have an additional parameter separated from the “tournament”
         keyword by the comma. The other value represents a group size.
         For example, “tournament,8” means that the tournament
-        parent selection algorithm is chosen, and
+        sampling algorithm for parent selection is chosen, and
         each group contains up to 8 members.
         The default group size is 4.
 
-        **"from_top_to_bottom"** - From Top To Bottom selection
+        **"from_top_to_bottom"** - From Top To Bottom sampling
         algorithm starts at the top of
         the list and pairs the chromosomes two at a time until the top kept chromosomes
         are selected for mating. Thus, the algorithm pairs odd rows with even rows.
 
-        **"random"** - Random selection algorithm uses a uniform random
+        **"random"** - Random sampling algorithm uses a uniform random
         number generator to select chromosomes.
         """
         return self._parent_selection
 
     @parent_selection.setter
     def parent_selection(self, value: str):
         self._parent_selection = ga_utils.prepare_string(value)
 
     @property
+    def crossover(self) -> str:
+        """
+        The crossover algorithm
+
+        Supported values:
+
+        **"blending"** - combines gene values from the two parents into new variable values in offsprings.
+        One value of the offspring variable comes from a combination of the two
+        corresponding values of the parental genes
+
+        **"uniform"** - Genes from parents' chromosomes are combined in a uniform way.
+        """
+        return self._crossover
+
+    @crossover.setter
+    def crossover(self, value: str):
+        self._crossover = ga_utils.prepare_string(value)
+
+    @property
     def requested_cost(self) -> float:
         """
         This parameter only takes place when exit_check has value “requested”.
         It determines the requested value which causes the
         exit from the genetic algorithm
         """
         return self._requested_cost
@@ -652,17 +726,17 @@
         return self._must_mutate_for_same_parents
 
     @must_mutate_for_same_parents.setter
     def must_mutate_for_same_parents(self, value: bool):
         self._must_mutate_for_same_parents = ga_utils.try_get_bool(value)
 
     @property
-    def timeout(self) -> int:
+    def timeout(self) -> int | str:
         """
         A number of seconds after which the genetic algorithm optimisation will\
             exit, regardless of whether exit_check criteria is reached.
         """
         return self._timeout
 
     @timeout.setter
-    def timeout(self, value: int):
+    def timeout(self, value: int | str) -> None:
         self._timeout = ga_utils.try_get_int(value)
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/chromosome.py` & `gadapt-0.4.0/gadapt/ga_model/chromosome.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 """
 Chromosome
 """
 
 from typing import List
-from gadapt.ga_model.gene import Gene
+
+import gadapt.adapters.string_operation.ga_strings as ga_strings
+import gadapt.ga_model.definitions as definitions
 from gadapt.ga_model.decision_variable import DecisionVariable
+from gadapt.ga_model.gene import Gene
 from gadapt.ga_model.ranking_model import RankingModel
-from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
-    BaseChromosomeImmigrator,
-)
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
-    BaseGeneMutationSelector,
-)
-import gadapt.ga_model.definitions as definitions
-import gadapt.adapters.string_operation.ga_strings as ga_strings
 
 
 class Chromosome(RankingModel):
     def __init__(
         self,
-        mutator: BaseGeneMutationSelector,
-        immigrator: BaseChromosomeImmigrator,
         population_generation: int,
     ):
         """
         Chromosome class.
         Chromosome is a part of the Population. Chromosome consists of Genes.
         Args:
-            immigrator (BaseChromosomeImmigrator): Immigration algorithm
-            population_generation (int): Generation in which the\
-                chromosome is created in the population
+            population_generation: population generation
         """
         super().__init__()
-        self._mutator = mutator
-        self._immigrator = immigrator
         self._cost_value = definitions.FLOAT_NAN
         self._is_immigrant = False
         self._population_generation = population_generation
         self._chromosome_id = None
         self._mutated_variables_id_list: List[int] = []
         self._first_mutant_generation = 0
         self._first_immigrant_generation = 0
@@ -94,36 +83,14 @@
 
     def _get_chromosome_string(self):
         if self._chromosome_string is None:
             self._chromosome_string = self._to_string()
         return self._chromosome_string
 
     @property
-    def mutator(self) -> BaseGeneMutationSelector:
-        """
-        Mutation algorithm
-        """
-        return self._mutator
-
-    @mutator.setter
-    def mutator(self, value: BaseGeneMutationSelector):
-        self._mutator = value
-
-    @property
-    def immigrator(self) -> BaseChromosomeImmigrator:
-        """
-        Immigration algorithm
-        """
-        return self._immigrator
-
-    @immigrator.setter
-    def immigrator(self, value: BaseChromosomeImmigrator):
-        self._immigrator = value
-
-    @property
     def number_of_mutation_genes(self):
         """
         The number of mutated genes in the chromosome.
         """
         return self._number_of_mutation_genes
 
     @number_of_mutation_genes.setter
@@ -280,51 +247,24 @@
         return self._last_immigrant_generation
 
     @last_immigrant_generation.setter
     def last_immigrant_generation(self, value: int):
         self._last_immigrant_generation = value
 
     @property
-    def mutation_on_both_sides(self) -> bool:
-        """
-        Indicates if mutation should be applied on both sides
-        """
-        return self._mutation_on_both_sides
-
-    @mutation_on_both_sides.setter
-    def mutation_on_both_sides(self, value: bool):
-        """
-        Indicates if mutation of the chromosome shouls be applied with the\
-            same probability of lower and higher value comparing with the current value
-        """
-        self._mutation_on_both_sides = value
-
-    @property
     def succ(self) -> bool:
         """
         Indicates if cost function execution succeded
         """
         return self._succ
 
     @succ.setter
     def succ(self, value: bool):
         self._succ = value
 
-    def mutate(self, number_of_mutation_genes: int):
-        """
-        Mutates chromosome
-        """
-        self.mutator.mutate(self, number_of_mutation_genes)
-
-    def immigrate(self):
-        """
-        Immigrates chromosome
-        """
-        self.immigrator.immigrate(self)
-
     @property
     def mutated_variables_id_list(self) -> List[int]:
         """
         List of mutated variables
         """
         return self._mutated_variables_id_list
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/decision_variable.py` & `gadapt-0.4.0/gadapt/ga_model/decision_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Decision variable
 """
 
 import random
+import sys
+
 import gadapt.ga_model.definitions as definitions
 
 
 class DecisionVariable:
     def __init__(self, id: int) -> None:
         """
         Decision variable class defines genes.
         Each gene has a reference to one decision variable.
         Decision variable contains common values for genes: variable id, maximal\
             value, minimal value, step.
         Args:
             id (int): identifier of the decision variable
         """
+        self._max_value = sys.float_info.min
+        self._decimal_places = -1
+        self._stacked = False
         self.variable_id = id
         self._standard_deviation = definitions.FLOAT_NAN
-        self._gene_mutator = None
         self._initial_st_dev = -1.0
 
     def __eq__(self, other):
         if not isinstance(other, DecisionVariable):
             return False
         return self.variable_id == other.variable_id
 
@@ -110,22 +114,14 @@
         """
         return self._standard_deviation
 
     @cross_diversity_coefficient.setter
     def cross_diversity_coefficient(self, value: float):
         self._standard_deviation = value
 
-    @property
-    def gene_mutator(self):
-        return self._gene_mutator
-
-    @gene_mutator.setter
-    def gene_mutator(self, value):
-        self._gene_mutator = value
-
     def make_random_value(self):
         """
         Makes random value, based on min value, max value, and step
         """
         number_of_steps = random.randint(
             0, round((self.max_value - self.min_value) / self.step)
         )
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/definitions.py` & `gadapt-0.4.0/gadapt/ga_model/definitions.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,31 @@
 RANDOM = "random"
 COST_DIVERSITY = "cost_diversity"
 PARENT_DIVERSITY = "parent_diversity"
 CROSS_DIVERSITY = "cross_diversity"
 TOURNAMENT = "tournament"
 FROM_TOP_TO_BOTTOM = "from_top_to_bottom"
 ROULETTE_WHEEL = "roulette_wheel"
+UNIFORM = "uniform"
+BLENDING = "blending"
 AVG_COST = "avg_cost"
 MIN_COST = "min_cost"
 REQUESTED = "requested"
+GENERATIONS = "generations"
 AVG = "avg"
 MIN = "min"
 PARAM_SEPARATOR = ","
 FLOAT_NAN = float("NaN")
 NOT_IMPLEMENTED = "not implemented"
 EXTREME_POINTED = "extreme_pointed"
 NORMAL_DISTRIBUTION = "normal_distribution"
-POPULATION_MUTATOR_STRINGS = [COST_DIVERSITY, PARENT_DIVERSITY, RANDOM, CROSS_DIVERSITY]
-CHROMOSOME_MUTATOR_STRINGS = [RANDOM, CROSS_DIVERSITY]
-GENE_MUTATOR_STRINGS = [RANDOM, NORMAL_DISTRIBUTION]
+POPULATION_MUTATION_STRINGS = [
+    COST_DIVERSITY,
+    PARENT_DIVERSITY,
+    RANDOM,
+    CROSS_DIVERSITY,
+]
+POPULATION_MUTATION_SELECTION_STRINGS = [RANDOM, PARENT_DIVERSITY]
+CHROMOSOME_MUTATION_STRINGS = [RANDOM, CROSS_DIVERSITY]
+GENE_MUTATION_STRINGS = [RANDOM, NORMAL_DISTRIBUTION, CROSS_DIVERSITY, EXTREME_POINTED]
 SELECTION_STRINGS = [RANDOM, FROM_TOP_TO_BOTTOM, ROULETTE_WHEEL, TOURNAMENT]
-EXIT_CRITERIA_STRINGS = [AVG_COST, MIN_COST, REQUESTED]
+EXIT_CRITERIA_STRINGS = [AVG_COST, MIN_COST, REQUESTED, GENERATIONS]
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/ga_options.py` & `gadapt-0.4.0/gadapt/ga_model/ga_options.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Genetic algorithm options
 """
 
 from typing import List
+
 from gadapt.ga_model.decision_variable import DecisionVariable
 
 
 class GAOptions:
     def __init__(self, ga) -> None:
         """
         Genetic algorithm options class
         Args:
             ga: Genetic algorithm class, containing data to initialize options
         """
         super().__init__()
         self._population_size = ga.population_size
+        self._keep_elitism_percentage = ga.keep_elitism_percentage
+        self._number_of_crossover_parents = ga.number_of_crossover_parents
         self._cost_function = ga.cost_function
         self._immigration_number = ga.immigration_number
         self._set_number_of_mutation_chromosomes(ga)
         self._max_attempt_no = ga.max_attempt_no
         self._requested_cost = ga.requested_cost
         self._logging = ga.logging
         self._decision_variables = ga._decision_variables
@@ -32,21 +35,25 @@
             and isinstance(ga.number_of_mutation_chromosomes, int)
             and ga.number_of_mutation_chromosomes >= 0
         ):
             self._number_of_mutation_chromosomes = ga.number_of_mutation_chromosomes
         elif (
             (ga.percentage_of_mutation_chromosomes is not None)
             and isinstance(ga.percentage_of_mutation_chromosomes, float)
-            and ga.percentage_of_mutation_chromosomes >= 0.0
-            and ga.percentage_of_mutation_chromosomes <= 100
+            and 0.0 <= ga.percentage_of_mutation_chromosomes <= 100
         ):
             nomc = round(
-                self.population_size * (ga.percentage_of_mutation_chromosomes / 100)
+                (self.population_size / 2)
+                * (ga.percentage_of_mutation_chromosomes / 100)
             )
-            while nomc >= self.population_size // 2 - self.immigration_number:
+            while (
+                nomc
+                >= round(self.population_size * (self.keep_elitism_percentage / 100))
+                - self.immigration_number
+            ):
                 nomc -= 1
             if nomc < 0:
                 raise Exception(
                     "Invalid percentage of mutation chromosomes and immigration number"
                 )
             self._number_of_mutation_chromosomes = nomc
         else:
@@ -58,16 +65,15 @@
             and isinstance(ga.number_of_mutation_genes, int)
             and ga.number_of_mutation_genes >= 0
         ):
             self._number_of_mutation_genes = ga.number_of_mutation_genes
         elif (
             (ga.percentage_of_mutation_genes is not None)
             and isinstance(ga.percentage_of_mutation_genes, float)
-            and ga.percentage_of_mutation_genes >= 0.0
-            and ga.percentage_of_mutation_genes <= 100
+            and 0.0 <= ga.percentage_of_mutation_genes <= 100
         ):
             self._number_of_mutation_genes = round(
                 float(len(self._decision_variables))
                 * (ga.percentage_of_mutation_genes / 100)
             )
         else:
             self._number_of_mutation_genes = ga.number_of_mutation_genes
@@ -147,28 +153,50 @@
         return self._population_size
 
     @population_size.setter
     def population_size(self, value: int):
         self._population_size = value
 
     @property
+    def keep_elitism_percentage(self) -> int:
+        """
+        Percentage number of chromosomes to be kept in the population by the cost value
+        """
+        return self._keep_elitism_percentage
+
+    @keep_elitism_percentage.setter
+    def keep_elitism_percentage(self, value: int):
+        self._keep_elitism_percentage = value
+
+    @property
+    def number_of_crossover_parents(self) -> int:
+        """
+        Number of parents to be included in the mating pool
+        """
+        if self._number_of_crossover_parents > 1:
+            return self._number_of_crossover_parents
+        return self.keep_number
+
+    @number_of_crossover_parents.setter
+    def number_of_crossover_parents(self, value: int):
+        self._number_of_crossover_parents = value
+
+    @property
     def decision_variables(self) -> List[DecisionVariable]:
         """
         Collection of decision variables
         """
         return self._decision_variables
 
     @property
     def _abandon_number(self) -> int:
         return self._get_abandon_number()
 
     def _get_abandon_number(self) -> int:
-        if self.population_size % 2 == 0:
-            return self.population_size // 2
-        return self.population_size // 2 - 1
+        return round(self.population_size * (1 - self.keep_elitism_percentage / 100))
 
     @property
     def keep_number(self) -> int:
         return self.population_size - self._abandon_number
 
     @property
     def logging(self) -> bool:
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/ga_results.py` & `gadapt-0.4.0/gadapt/ga_model/ga_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Results for the genetic algorithm execution
 """
 
 from typing import List
+
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 
 
 class GAResults:
     def __init__(self) -> None:
         """
         Results class for the genetic algorithm execution
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/gene.py` & `gadapt-0.4.0/gadapt/ga_model/gene.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Gene
 """
 
 import math
-from gadapt.ga_model.decision_variable import DecisionVariable
-from gadapt.ga_model.ranking_model import RankingModel
+
 import gadapt.adapters.string_operation.ga_strings as ga_strings
 import gadapt.ga_model.definitions as definitions
+from gadapt.ga_model.decision_variable import DecisionVariable
+from gadapt.ga_model.ranking_model import RankingModel
 
 
 class Gene(RankingModel):
     def __init__(self, gen_variable, var_value=None):
         """
         Gene class. Gene is a part of chromosome.
         It contains concrete values for decision variables.
@@ -38,30 +39,26 @@
         Decision variable which defines the gene
         """
         return self._decision_variable
 
     @decision_variable.setter
     def decision_variable(self, value: DecisionVariable):
         if not isinstance(value, DecisionVariable):
-            pass
             raise
         self._decision_variable = value
 
     @property
     def variable_value(self):
         """
         Value of the gene
         """
         return self._variable_value
 
     @variable_value.setter
     def variable_value(self, value):
         self._variable_value = value
 
-    def mutate(self):
-        self.decision_variable.gene_mutator.mutate(self)
-
     def set_random_value(self):
         """
         Sets a random value for the variable_value property
         """
         self.variable_value = self.decision_variable.make_random_value()
```

### Comparing `gadapt-0.3.6/gadapt/ga_model/ranking_model.py` & `gadapt-0.4.0/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.3.6/gadapt/operations/cost_finding/base_cost_finder.py` & `gadapt-0.4.0/gadapt/operations/cost_finding/base_cost_finder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from abc import ABC, abstractmethod
-import math
 import sys
 import traceback
+from abc import ABC, abstractmethod
+from typing import Optional
+
+from gadapt.ga_model.population import Population
 from gadapt.ga_model.chromosome import Chromosome
 
 
 class BaseCostFinder(ABC):
     """
     Base class for cost finding
     """
 
+    def __init__(self):
+        super().__init__()
+        self.population: Optional[Population] = None
+
     def _execute_function(self, cost_function, c: Chromosome):
         """
         Executes the cost function
 
         Args:
             cost_function: Function to execute
             c (Chromosome): The chromosome with
@@ -28,22 +34,19 @@
         except Exception:
             print(Exception)
             traceback.print_exc()
             c.succ = False
             c.cost_value = sys.float_info.max
 
     @abstractmethod
-    def _find_costs_for_population(self, population):
+    def _find_costs_for_population(self):
         pass
 
     def find_costs(self, population):
         """
         Finds costs for the population
 
         Args:
             population (Population): The population to find costs for each chromosome
         """
-        self._find_costs_for_population(population)
-        if math.isnan(population.average_cost_step_in_first_population):
-            population.average_cost_step_in_first_population = (
-                population.calculate_average_cost_step()
-            )
+        self.population = population
+        self._find_costs_for_population()
```

### Comparing `gadapt-0.3.6/gadapt/operations/cost_finding/elitism_cost_finder.py` & `gadapt-0.4.0/gadapt/operations/cost_finding/elitism_cost_finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import logging
 import math
 from typing import List
-from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
+
 from gadapt.ga_model.chromosome import Chromosome
-from gadapt.ga_model.population import Population
+from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
 
 
 class ElitismCostFinder(BaseCostFinder):
     """
     Finding costs for a better half of the population
     """
 
-    def _find_costs_for_population(self, population: Population):
-        if population is None:
+    def _find_costs_for_population(self):
+        if self.population is None:
             raise Exception("population must not be null!")
         chromosomes_for_execution: List[Chromosome] = [
             c
-            for c in population
+            for c in self.population
             if (math.isnan(c.cost_value))
             or (
                 c.is_immigrant
-                and c.population_generation == population.population_generation
+                and c.population_generation == self.population.population_generation
             )
         ]
         for c in chromosomes_for_execution:
-            self._execute_function(population.options.cost_function, c)
-        better_chromosomes: List[Chromosome] = population.get_sorted(
+            self._execute_function(self.population.options.cost_function, c)
+        better_chromosomes: List[Chromosome] = self.population.get_sorted(
             key=lambda x: x.cost_value
-        )[: population.options.keep_number]
-        population.best_individual = better_chromosomes[0]
-        population.min_cost = (
+        )[: self.population.options.keep_number]
+        self.population.best_individual = better_chromosomes[0]
+        self.population.min_cost = (
             min(better_chromosomes, key=lambda x: x.cost_value)
         ).cost_value
         better_chromosomes_without_immigrants = better_chromosomes[
-            : population.options.keep_number - population.options.immigration_number
+            : self.population.options.keep_number
+            - self.population.options.immigration_number
         ]
-        population.avg_cost = sum(
+        self.population.avg_cost = sum(
             [c.cost_value for c in better_chromosomes_without_immigrants]
         ) / len(better_chromosomes_without_immigrants)
-        self._log_population(population)
-        population.clear_and_add_chromosomes(better_chromosomes)
-        population.update_variables()
+        self._log_population()
+        self.population.clear_and_add_chromosomes(better_chromosomes)
 
-    def _log_population(self, population: Population):
-        if population.options.logging:
-            logging.info(str(population))
+    def _log_population(self):
+        if self.population.options.logging:
+            logging.info(str(self.population))
```

### Comparing `gadapt-0.3.6/gadapt/operations/crossover/base_crossover.py` & `gadapt-0.4.0/gadapt/operations/crossover/base_crossover.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,169 +1,198 @@
+import math
 from abc import ABC, abstractmethod
-from gadapt.ga_model.chromosome import Chromosome
+from typing import Tuple, List
+
 from gadapt.ga_model.gene import Gene
+from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
     BaseGeneMutationSelector,
 )
-from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
-import gadapt.utils.ga_utils as ga_utils
 
 
 class BaseCrossover(ABC):
     """Base Crossover Class
 
     Args:
-        gene_combination (BaseGeneCombination): the algorithm
-        for how genes are to be combined
         mutator (BaseGeneMutationSelector): mutation algorithm to
         be passed to offspring chromosomes
         immigrator (BaseChromosomeImmigrator): immigration algorithm
         to be passed to offspring chromosomes
-        mutation_on_both_sides (bool): indicates if offspring chromosomes
         should be mutated on both sides with the same probability
     """
 
     def __init__(
         self,
-        gene_combination: BaseGeneCombination,
         mutator: BaseGeneMutationSelector,
         immigrator: BaseChromosomeImmigrator,
-        mutation_on_both_sides: bool = True,
     ):
-        self._mutation_on_both_sides = True
-        self._gene_combination = gene_combination
         self._mutator = mutator
         self._immigrator = immigrator
-        self._mutation_on_both_sides = mutation_on_both_sides
+        self._current_gene_number = -1
+
+    def mate(self, chromosome_pairs: List[Tuple[Chromosome, Chromosome]], population):
+        """
+        Returns list of chromosome pairs using parents' genetic material
+
+        Args:
+            chromosome_pairs (List[Tuple[Chromosome, Chromosome]]) : List of chromosome pairs for mating
+            population: Population
+        """
+        for chromosome1, chromosome2 in chromosome_pairs:
+            offspring1, offspring2 = self._mate_pair(
+                chromosome1, chromosome2, population.population_generation
+            )
+            population.add_chromosomes((offspring1, offspring2))
+        current_len = len(population)
+        chromosome_surplus = current_len - population.options.population_size
+        if chromosome_surplus > 0:
+            sorted_by_cost_value = sorted(
+                population, key=lambda chrom: chrom.cost_value, reverse=True
+            )
+            i = 0
+            for c in sorted_by_cost_value:
+                if i >= chromosome_surplus:
+                    break
+                if not math.isnan(c.cost_value):
+                    population.chromosomes.remove(c)
 
-    def mate(self, mother: Chromosome, father: Chromosome, population_generation: int):
+    def _mate_pair(
+        self, mother: Chromosome, father: Chromosome, population_generation: int
+    ):
         """Returns two offspring chromosomes using parents' genetic material
 
         Args:
             mother (Chromosome): The first chromosome for mating
             father (Chromosome): The second chromosome for mating
             population_generation (int): Current generation in the population
 
         Returns:
             Chromosome: the first offspring chromosome
             Chromosome: the second offspring chromosome
         """
-
-        def get_genetic_diversity(g_m: Gene, g_f: Gene) -> float:
-            return abs(g_m.variable_value - g_f.variable_value) / (
-                g_f.decision_variable.max_value - g_f.decision_variable.min_value
-            )
-
         if len(mother) != len(father):
             raise Exception("Mother and father must have the same number of genes!")
-        offspring1 = Chromosome(self._mutator, self._immigrator, population_generation)
-        offspring2 = Chromosome(self._mutator, self._immigrator, population_generation)
-        self.number_of_genes = len(father)
-        genetic_diversity = []
-        for self._current_gene_number in range(self.number_of_genes):
-            mother_gene, father_gene = self._get_mother_father_genes(mother, father)
-            decision_variable_father = father_gene.decision_variable
-            decision_variable_mother = mother_gene.decision_variable
+        self._mother = mother
+        self._father = father
+        self._offspring1 = Chromosome(population_generation)
+        self._offspring2 = Chromosome(population_generation)
+        self._cross_genetic_material()
+        self._increase_generation()
+        return self._offspring1, self._offspring2
+
+    def _cross_genetic_material(self):
+        number_of_genes = len(self._father)
+        for self._current_gene_number in range(number_of_genes):
+            self._mother_gene, self._father_gene = self._get_mother_father_genes()
+            decision_variable_father = self._mother_gene.decision_variable
+            decision_variable_mother = self._father_gene.decision_variable
             if decision_variable_father != decision_variable_mother:
                 decision_variable_mother = next(
                     (
                         item.decision_variable
-                        for item in mother
+                        for item in self._mother
                         if item.decision_variable == decision_variable_father
                     ),
                     None,
                 )
             if decision_variable_mother is None:
                 raise Exception(
                     "chromosomes in crossover do not have the same structure!"
                 )
-            genetic_diversity.append(get_genetic_diversity(mother_gene, father_gene))
-            var1, var2 = self._combine(mother_gene, father_gene)
-            offspring1.add_gene(decision_variable_father, var1)
-            offspring2.add_gene(decision_variable_father, var2)
-        parrents_diversity = round(ga_utils.average(genetic_diversity), 2)
-        offspring1.parent_diversity = parrents_diversity
-        offspring2.parent_diversity = parrents_diversity
-        offspring1.mutation_on_both_sides = self._mutation_on_both_sides
-        offspring2.mutation_on_both_sides = self._mutation_on_both_sides
-        offspring1.mother_id = mother.chromosome_id
-        offspring2.mother_id = mother.chromosome_id
-        offspring1.father_id = father.chromosome_id
-        offspring2.father_id = father.chromosome_id
-        self._increase_generation(offspring1, offspring2, mother, father)
-        return offspring1, offspring2
+            self._decision_variable_crossed()
+            var1, var2 = self._combine()
+            self._offspring1.add_gene(decision_variable_father, var1)
+            self._offspring2.add_gene(decision_variable_father, var2)
+        self._all_decision_variable_crossed()
+        self._offspring1.mother_id = self._mother.chromosome_id
+        self._offspring2.mother_id = self._mother.chromosome_id
+        self._offspring1.father_id = self._father.chromosome_id
+        self._offspring2.father_id = self._father.chromosome_id
+
+    def _get_mother_father_genes(self) -> Tuple[Gene, Gene]:
+        if self._current_gene_number == -1:
+            raise Exception("_current_gene_number not set")
+        father_gene = self._father[self._current_gene_number]
+        mother_gene = self._mother[self._current_gene_number]
+        return mother_gene, father_gene
 
     @abstractmethod
-    def _get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
+    def _combine(self):
         pass
 
-    @abstractmethod
-    def _combine(self, mother_gene: Gene, father_gene: Gene):
-        pass
-
-    def _increase_generation(
-        self,
-        offspring1: Chromosome,
-        offspring2: Chromosome,
-        mother: Chromosome,
-        father: Chromosome,
-    ):
-        current_generation = mother.chromosome_generation
-        if current_generation == 0 or current_generation < father.chromosome_generation:
-            current_generation = father.chromosome_generation
+    def _increase_generation(self):
+        current_generation = self._mother.chromosome_generation
+        if (
+            current_generation == 0
+            or current_generation < self._father.chromosome_generation
+        ):
+            current_generation = self._father.chromosome_generation
         current_generation += 1
-        offspring1.chromosome_generation = current_generation
-        offspring2.chromosome_generation = current_generation
+        self._offspring1.chromosome_generation = current_generation
+        self._offspring2.chromosome_generation = current_generation
 
         current_generation = 0
-        if mother.first_mutant_generation > 0 or father.first_mutant_generation > 0:
-            current_generation = mother.first_mutant_generation
+        if (
+            self._mother.first_mutant_generation > 0
+            or self._father.first_mutant_generation > 0
+        ):
+            current_generation = self._mother.first_mutant_generation
             if (
                 current_generation == 0
-                or father.first_mutant_generation > current_generation
+                or self._father.first_mutant_generation > current_generation
             ):
-                current_generation = father.first_mutant_generation
+                current_generation = self._father.first_mutant_generation
             current_generation += 1
-        offspring1.first_mutant_generation = current_generation
-        offspring2.first_mutant_generation = current_generation
+        self._offspring1.first_mutant_generation = current_generation
+        self._offspring2.first_mutant_generation = current_generation
 
         current_generation = 0
-        if mother.last_mutant_generation > 0 or father.last_mutant_generation > 0:
-            current_generation = mother.last_mutant_generation
+        if (
+            self._mother.last_mutant_generation > 0
+            or self._father.last_mutant_generation > 0
+        ):
+            current_generation = self._mother.last_mutant_generation
             if current_generation == 0 or (
-                father.last_mutant_generation > 0
-                and father.last_mutant_generation < current_generation
+                0 < self._father.last_mutant_generation < current_generation
             ):
-                current_generation = father.last_mutant_generation
+                current_generation = self._father.last_mutant_generation
             current_generation += 1
-        offspring1.last_mutant_generation = current_generation
-        offspring2.last_mutant_generation = current_generation
+        self._offspring1.last_mutant_generation = current_generation
+        self._offspring2.last_mutant_generation = current_generation
 
         current_generation = 0
         if (
-            mother.first_immigrant_generation > 0
-            or father.first_immigrant_generation > 0
+            self._mother.first_immigrant_generation > 0
+            or self._father.first_immigrant_generation > 0
         ):
-            current_generation = mother.first_immigrant_generation
+            current_generation = self._mother.first_immigrant_generation
             if (
                 current_generation == 0
-                or father.first_immigrant_generation > current_generation
+                or self._father.first_immigrant_generation > current_generation
             ):
-                current_generation = father.first_immigrant_generation
+                current_generation = self._father.first_immigrant_generation
             current_generation += 1
-        offspring1.first_immigrant_generation = current_generation
-        offspring2.first_immigrant_generation = current_generation
+        self._offspring1.first_immigrant_generation = current_generation
+        self._offspring2.first_immigrant_generation = current_generation
 
         current_generation = 0
-        if mother.last_immigrant_generation > 0 or father.last_immigrant_generation > 0:
-            current_generation = mother.last_immigrant_generation
+        if (
+            self._mother.last_immigrant_generation > 0
+            or self._father.last_immigrant_generation > 0
+        ):
+            current_generation = self._mother.last_immigrant_generation
             if current_generation == 0 or (
-                father.last_immigrant_generation > 0
-                and father.last_immigrant_generation < current_generation
+                0 < self._father.last_immigrant_generation < current_generation
             ):
-                current_generation = father.last_immigrant_generation
+                current_generation = self._father.last_immigrant_generation
             current_generation += 1
-        offspring1.last_immigrant_generation = current_generation
-        offspring2.last_immigrant_generation = current_generation
+        self._offspring1.last_immigrant_generation = current_generation
+        self._offspring2.last_immigrant_generation = current_generation
+
+    def _decision_variable_crossed(self):
+        pass
+
+    def _all_decision_variable_crossed(self):
+        pass
```

### Comparing `gadapt-0.3.6/gadapt/operations/crossover/uniform_crossover.py` & `gadapt-0.4.0/gadapt/operations/crossover/blending_parent_diversity_crossover.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-from typing import Tuple
-from gadapt.ga_model.chromosome import Chromosome
-from gadapt.operations.crossover.base_crossover import BaseCrossover
-from gadapt.ga_model.gene import Gene
 from gadapt.operations.immigration.chromosome_immigration.base_chromosome_immigrator import (
     BaseChromosomeImmigrator,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
     BaseGeneMutationSelector,
 )
-from gadapt.operations.gene_combination.base_gene_combination import BaseGeneCombination
+from gadapt.operations.crossover.uniform_crossover import UniformCrossover
+from gadapt.utils import ga_utils
 
 
-class UniformCrossover(BaseCrossover):
+class BlendingParentDiversityCrossover(UniformCrossover):
     """
-    Uniform Crossover.
-    Genes from parents' chromosomes are combined in a uniform way
+    Blending Crossover. Genes from parents' chromosomes are combined in a blending way.
+    Calculates diversity of parents and save it to chromosomes.
     """
 
     def __init__(
         self,
-        var_combination: BaseGeneCombination,
         mutator: BaseGeneMutationSelector,
         immigrator: BaseChromosomeImmigrator,
     ):
-        super(UniformCrossover, self).__init__(var_combination, mutator, immigrator)
+        super(BlendingParentDiversityCrossover, self).__init__(mutator, immigrator)
+        self._genetic_diversity = None
 
-    def _get_mother_father_genes(
-        self, mother: Chromosome, father: Chromosome
-    ) -> Tuple[Gene, Gene]:
-        father_gene = father[self._current_gene_number]
-        mother_gene = mother[self._current_gene_number]
-        return mother_gene, father_gene
-
-    def _combine(self, mother_gene: Gene, father_gene: Gene):
-        if self._gene_combination is None:
-            raise Exception("gene_combination must not be null!")
-        return self._gene_combination.combine(mother_gene, father_gene)
+    def _get_genetic_diversity(self) -> float:
+        return abs(
+            self._mother_gene.variable_value - self._father_gene.variable_value
+        ) / (
+            self._father_gene.decision_variable.max_value
+            - self._father_gene.decision_variable.min_value
+        )
+
+    def _get_parent_diversity(self):
+        return round(ga_utils.average(self._genetic_diversity), 2)
+
+    def _decision_variable_crossed(self):
+        self._genetic_diversity.append(self._get_genetic_diversity())
+
+    def _all_decision_variable_crossed(self):
+        parent_diversity = self._get_parent_diversity()
+        self._offspring1.parent_diversity = parent_diversity
+        self._offspring2.parent_diversity = parent_diversity
+
+    def _cross_genetic_material(self):
+        self._genetic_diversity = []
+        super()._cross_genetic_material()
```

### Comparing `gadapt-0.3.6/gadapt/operations/exit_check/base_exit_checker.py` & `gadapt-0.4.0/gadapt/operations/exit_check/base_exit_checker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from abc import ABC, abstractmethod
 import logging
+from abc import ABC, abstractmethod
 from datetime import datetime
+from typing import Optional
+
+from gadapt.ga_model.population import Population
 
 
 class BaseExitChecker(ABC):
     """
     Base class for exit check
     Args:
         max_attempt_no (int): Maximal number of attempts with no improvement,
@@ -12,33 +15,39 @@
 
             After this number of attempts with no improvements, the GA exits
     """
 
     def __init__(self, max_attempt_no: int) -> None:
         self.max_attempt_no = max_attempt_no
         self.attempt_no = 0
+        self.population: Optional[Population] = None
 
     @property
     def attempt_no(self) -> int:
         return self._attempt_no
 
     @attempt_no.setter
     def attempt_no(self, value: int):
         self._attempt_no = value
 
-    def check(self, population):
-        time_diff = (datetime.now() - population.start_time).total_seconds()
-        if time_diff >= population.options.timeout:
-            population.timeout_expired = True
+    def check(self, population: Population):
+        self.population = population
+        if self.population is None:
+            raise Exception("Population is None!")
+        if self.population is None:
+            raise Exception("Population is None!")
+        time_diff = (datetime.now() - self.population.start_time).total_seconds()
+        if time_diff >= self.population.options.timeout:
+            self.population.timeout_expired = True
             return True
-        if self._is_exit(population):
+        if self._is_exit():
             self.attempt_no += 1
         else:
             self.attempt_no = 0
         if self.attempt_no >= self.max_attempt_no:
             logging.info("function exit.")
             return True
         return False
 
     @abstractmethod
-    def _is_exit(self, population) -> bool:
+    def _is_exit(self) -> bool:
         pass
```

### Comparing `gadapt-0.3.6/gadapt/operations/exit_check/requested_cost_exit_checker.py` & `gadapt-0.4.0/gadapt/operations/exit_check/requested_cost_exit_checker.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,11 +7,11 @@
     The GA exits when the minimum cost reaches a defined value.
     """
 
     def __init__(self, requested_cost: float) -> None:
         super().__init__(1)
         self.requested_cost = requested_cost
 
-    def _is_exit(self, population):
-        if population.min_cost <= self.requested_cost:
+    def _is_exit(self):
+        if self.population.min_cost <= self.requested_cost:
             return True
         return False
```

### Comparing `gadapt-0.3.6/gadapt/operations/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.4.0/gadapt/operations/immigration/population_immigration/common_population_immigrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import List
+
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.immigration.population_immigration.base_population_immigrator import (
     BasePopulationImmigrator,
 )
 
 
 class CommonPopulationImmigrator(BasePopulationImmigrator):
     """
-    Common class for the population immigration.
-    In kept part of the population lower ranked chromosomes are replaced with new ones
+    Common class for the self.population immigration.
+    In kept part of the self.population lower ranked chromosomes are replaced with new ones
     """
 
-    def _immigrate_population(self, population):
-        if population.options.immigration_number < 1:
+    def _immigrate_population(self):
+        if self.population.options.immigration_number < 1:
             return
-        keep_number = population.options.keep_number
+        keep_number = self.population.options.keep_number
         chromosome_list: List[Chromosome] = list(
-            population.get_sorted(key=lambda c: c.cost_value)
+            self.population.get_sorted(key=lambda c: c.cost_value)
         )[:keep_number]
         chromosome_list = sorted(
             chromosome_list, key=lambda c: (-c.cost_value, -c.chromosome_id)
-        )[: population.options.immigration_number]
+        )[: self.population.options.immigration_number]
         for c in chromosome_list:
-            c.immigrate()
-            c.population_generation = population.population_generation
+            self._chromosome_immigrator.immigrate(c)
+            c.population_generation = self.population.population_generation
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 class BaseGeneMutationRateDeterminator(ABC):
     def __init__(self) -> None:
         """
         Provides a framework for determining the number of mutation genes in a chromosome.
         """
         super().__init__()
+        self.max_number_of_mutation_genes: int = -1
 
-    def get_number_of_mutation_genes(self, chromosome, max_number_of_mutation_genes):
+    def get_number_of_mutation_genes(
+        self, chromosome, max_number_of_mutation_genes: int
+    ):
         if max_number_of_mutation_genes is None:
             raise Exception("max_number_of_mutation_genes must not be None")
         if not chromosome:
             raise Exception("chromosome must not be None")
-
-        return self._get_number_of_mutation_genes(
-            chromosome, max_number_of_mutation_genes
-        )
+        self.chromosome = chromosome
+        self.max_number_of_mutation_genes = max_number_of_mutation_genes
+        return self._get_number_of_mutation_genes()
 
     @abstractmethod
-    def _get_number_of_mutation_genes(
-        self, chromosome, max_number_of_mutation_genes
-    ) -> int:
+    def _get_number_of_mutation_genes(self) -> int:
         pass
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-from abc import ABC, abstractmethod
-
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
+import gadapt.utils.ga_utils as ga_utils
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
 
 
-class BaseGeneMutationSelector(ABC):
+class CrossDiversityChromosomeMutationRateDeterminator(
+    BaseChromosomeMutationRateDeterminator
+):
     """
-    Provides a framework for selecting and mutating genes in a chromosome.
+    Determining the number of chromosomes to be mutated in a population based on the cross-diversity coefficient of the decision variables.
     """
 
     def __init__(
-        self, gene_mutation_rate_determinator: BaseGeneMutationRateDeterminator
-    ):
-        """
-        Initializes an instance of the class by setting the gene_mutation_rate_determinator attribute.
-        """
-        self._gene_mutation_rate_determinator = gene_mutation_rate_determinator
-
-    def mutate(self, c, number_of_mutation_genes: int):
-        """
-        Selects and mutates genes in the chromosome
-        Args:
-            c: Chromosome to mutate
-            number_of_mutation_genes: Number of mutation genes
-        """
-        self._before_mutated(c)
-        self._mutate_chromosome(c, number_of_mutation_genes)
-        self._chromosome_mutated(c)
-
-    @abstractmethod
-    def _mutate_chromosome(self, c, number_of_mutation_genes: int):
-        pass
-
-    def _gene_mutated(self, g, c):
-        c.mutated_variables_id_list.append(g.decision_variable.variable_id)
-
-    def _chromosome_mutated(self, c):
-        c.is_mutated = True
-        if c.first_mutant_generation == 0:
-            c.first_mutant_generation += 1
-        c.last_mutant_generation = 1
-
-    def _before_mutated(self, c):
-        c.mutated_variables_id_list.clear()
+        self,
+    ) -> None:
+        super().__init__()
+
+    def _get_number_of_mutation_chromosomes(self) -> int:
+        def get_mutation_rate() -> float:
+            avg_rsd = ga_utils.average(
+                [
+                    dv.cross_diversity_coefficient
+                    for dv in self.population.options.decision_variables
+                ]
+            )
+            if avg_rsd > 1:
+                avg_rsd = 1
+            if avg_rsd < 0:
+                avg_rsd = 0
+            return 1 - avg_rsd
+
+        mutation_rate = get_mutation_rate()
+        f_return_value = mutation_rate * float(self.max_number_of_mutation_chromosomes)
+        return round(f_return_value)
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 import random
 from typing import List
 
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
     BaseGeneMutationRateDeterminator,
 )
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
+)
+from gadapt.operations.mutation.gene_mutation.base_gene_mutator import BaseGeneMutator
 
 
-class ComposedGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
+class ComposedGeneMutationSelector(BaseGeneMutationSelector):
     """
-    Provides a way to combine multiple gene mutation rate determinators into a single determinator. It randomly selects one of the determinators to determine the number of mutation genes in a chromosome.
+    Allows for the composition of multiple mutation selectors and applies them sequentially to the chromosome.
     """
 
-    def __init__(self) -> None:
-        super().__init__()
-        self.determinators: List[BaseGeneMutationRateDeterminator] = []
+    def __init__(
+        self,
+        gene_mutation_rate_determinator: BaseGeneMutationRateDeterminator,
+        gene_mutator: BaseGeneMutator,
+    ) -> None:
+        super().__init__(gene_mutation_rate_determinator, gene_mutator)
+        self.selectors: List[BaseGeneMutationSelector] = []
 
-    def append(self, determinator: BaseGeneMutationRateDeterminator):
+    def append(self, selector: BaseGeneMutationSelector):
         """
-        Adds a gene mutation rate determinator to the list of determinators.
+        Appends mutation selectors to a list of selectors.
         Args:
-            determinator: A BaseGeneMutationRateDeterminator object representing a gene mutation rate determinator.
+            selector: An instance of the BaseGeneMutationSelector class that will be added to the list of selectors.
         """
-        self.determinators.append(determinator)
+        self.selectors.append(selector)
 
-    def _get_number_of_mutation_genes(self, chromosome, max_number_of_mutation_genes):
-        if chromosome is None:
+    def _mutate_chromosome(self):
+        if self.chromosome is None:
             raise Exception("Chromosome must not be null")
-        if len(self.determinators) == 0:
+        if len(self.selectors) == 0:
             raise Exception("at least one mutator must be added")
-        if len(self.determinators) > 1:
-            random.shuffle(self.determinators)
-        current_determinator = self.determinators[0]
-        return current_determinator.get_number_of_mutation_genes(
-            chromosome, max_number_of_mutation_genes
+        if len(self.selectors) > 1:
+            random.shuffle(self.selectors)
+        nmg = 0
+        number_of_mutation_genes = (
+            self._gene_mutation_rate_determinator.get_number_of_mutation_genes(
+                self.chromosome, self.number_of_mutation_genes
+            )
         )
+        if number_of_mutation_genes == 0:
+            number_of_mutation_genes = 1
+        for s in self.selectors:
+            if nmg < number_of_mutation_genes:
+                s.number_of_mutation_genes = number_of_mutation_genes - nmg
+                s.chromosome = self.chromosome
+                mg = s._mutate_chromosome()
+                nmg += mg
+        return nmg
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 import random
 from typing import List
 
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
+)
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
 )
 from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
     BaseGeneMutationSelector,
 )
 
 
-class ComposedGeneMutationSelector(BaseGeneMutationSelector):
-    """
-    Allows for the composition of multiple mutation selectors and applies them sequentially to the chromosome.
-    """
-
+class ComposedChromosomeMutationSelector(BaseChromosomeMutationSelector):
     def __init__(
-        self, gene_mutation_rate_determinator: BaseGeneMutationRateDeterminator
+        self,
+        chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+        gene_mutation_selector: BaseGeneMutationSelector,
     ) -> None:
-        super().__init__(gene_mutation_rate_determinator)
-        self.selectors: List[BaseGeneMutationSelector] = []
+        super().__init__(chromosome_mutation_rate_determinator, gene_mutation_selector)
+        self.selectors: List[BaseChromosomeMutationSelector] = []
 
-    def append(self, selector: BaseGeneMutationSelector):
+    def append(self, selector: BaseChromosomeMutationSelector):
         """
-        Appends mutation selectors to a list of selectors.
-        Args:
-            selector: An instance of the BaseGeneMutationSelector class that will be added to the list of selectors.
+        Appends selector to the composition of selectors
         """
         self.selectors.append(selector)
 
-    def _mutate_chromosome(self, chromosome, max_number_of_mutation_genes):
-        if chromosome is None:
-            raise Exception("Chromosome must not be null")
+    def _mutate_population(self):
+        if self.population is None:
+            raise Exception("Population must not be null")
         if len(self.selectors) == 0:
             raise Exception("at least one mutator must be added")
         if len(self.selectors) > 1:
             random.shuffle(self.selectors)
-        nmg = 0
-        number_of_mutation_genes = (
-            self._gene_mutation_rate_determinator.get_number_of_mutation_genes(
-                chromosome, max_number_of_mutation_genes
-            )
-        )
-        if number_of_mutation_genes == 0:
+        nmc = 0
+        limit_number_of_mutation_chromosomes = self.number_of_mutation_chromosomes
+        if limit_number_of_mutation_chromosomes == 0:
             return 0
         for m in self.selectors:
-            if nmg < number_of_mutation_genes:
-                mg = m._mutate_chromosome(chromosome, number_of_mutation_genes - nmg)
-                nmg += mg
-        return nmg
+            if nmc < limit_number_of_mutation_chromosomes:
+                m.population = self.population
+                m.number_of_mutation_chromosomes = (
+                    limit_number_of_mutation_chromosomes - nmc
+                )
+                mc = m._mutate_population()
+                nmc += mc
+        return nmc
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-import gadapt.utils.ga_utils as ga_utils
+import random
 
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
+from gadapt.ga_model.chromosome import Chromosome
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
+)
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_selector import (
+    BaseChromosomeMutationSelector,
+)
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
 )
 
 
-class CrossDiversityGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
+class RandomChromosomeMutationSelector(BaseChromosomeMutationSelector):
     """
-    Determines the number of mutation genes in a chromosome based on the cross diversity coefficient of the decision variables.
+    Implements the mutation of chromosomes in a population based on a random selection of chromosomes
     """
 
     def __init__(
         self,
+        chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+        gene_mutation_selector: BaseGeneMutationSelector,
     ) -> None:
-        super().__init__()
+        super().__init__(chromosome_mutation_rate_determinator, gene_mutation_selector)
 
-    def _get_number_of_mutation_genes(
-        self, chromosome, max_number_of_mutation_genes
-    ) -> int:
-        decision_variables = [g.decision_variable for g in chromosome]
-
-        def get_mutation_rate() -> float:
-            avg_rsd = ga_utils.average(
-                [dv.cross_diversity_coefficient for dv in decision_variables]
+    def _mutate_population(self):
+        if self.population is None:
+            raise Exception("population must not be None")
+        unallocated_chromosomes = self._get_unallocated_chromosomes(
+            self._sort_key_random
+        )
+        mutation_chromosome_number = self.number_of_mutation_chromosomes
+        if mutation_chromosome_number == 0:
+            return 0
+        chromosomes_for_mutation = unallocated_chromosomes[:mutation_chromosome_number]
+        for c in chromosomes_for_mutation:
+            self._gene_mutation_selector.mutate(
+                c, self.population.options.number_of_mutation_genes
             )
-            if avg_rsd > 1:
-                avg_rsd = 1
-            if avg_rsd < 0:
-                avg_rsd = 0
-            return 1 - avg_rsd
-
-        mutation_rate = get_mutation_rate()
-        f_return_value = mutation_rate * float(max_number_of_mutation_genes)
-        f_return_value_rounded = round(f_return_value)
-        if f_return_value_rounded == 0:
-            f_return_value_rounded = 1
-        return f_return_value_rounded
+        return mutation_chromosome_number
+
+    def _sort_key_random(self, _: Chromosome):
+        return random.random()
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py` & `gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-from gadapt.ga_model.chromosome import Chromosome
 import random
+
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
+    BaseGeneMutationRateDeterminator,
+)
 from gadapt.operations.mutation.chromosome_mutation.random_gene_mutation_selector import (
     RandomGeneMutationSelector,
 )
 from gadapt.operations.sampling.base_sampling import BaseSampling
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
-)
+from gadapt.operations.mutation.gene_mutation.base_gene_mutator import BaseGeneMutator
 
 
 class CrossDiversityGeneMutationSelector(RandomGeneMutationSelector):
     """
     Selects and mutates a chromosome based on the cross diversity of decision variables in the population.
     """
 
     def __init__(
         self,
         gene_mutation_rate_determinator: BaseGeneMutationRateDeterminator,
+        gene_mutator: BaseGeneMutator,
         sampling: BaseSampling,
     ) -> None:
-        super().__init__(gene_mutation_rate_determinator)
+        super().__init__(gene_mutation_rate_determinator, gene_mutator)
         self._sampling = sampling
 
-    def _mutate_chromosome(self, c: Chromosome, max_number_of_mutation_genes: int):
-        if max_number_of_mutation_genes == 0:
-            return
-        x_genes = [g for g in c]
+    def _mutate_chromosome(self):
+        if self.number_of_mutation_genes == 0:
+            self.number_of_mutation_genes = 1
+        x_genes = [g for g in self.chromosome]
         x_genes.sort(key=lambda g: -g.decision_variable.cross_diversity_coefficient)
         number_of_mutation_genes = (
             self._gene_mutation_rate_determinator.get_number_of_mutation_genes(
-                c, max_number_of_mutation_genes
+                self.chromosome, self.number_of_mutation_genes
             )
         )
         if number_of_mutation_genes > len(x_genes):
             number_of_mutation_genes = len(x_genes)
         if number_of_mutation_genes == 0:
-            max_number_of_mutation_genes = 0
+            max_number_of_mutation_genes = 1
         else:
             max_number_of_mutation_genes = random.randint(1, number_of_mutation_genes)
         genes_for_mutation = self._sampling.get_sample(
             x_genes,
             max_number_of_mutation_genes,
             lambda g: g.decision_variable.cross_diversity_coefficient,
         )
         for g in genes_for_mutation:
-            g.mutate()
-            self._gene_mutated(g, c)
+            self._gene_mutator.mutate(g)
         return len(genes_for_mutation)
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-import random
-
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
+from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
+    BaseChromosomeMutationRateDeterminator,
 )
 
 
-class RandomGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
+class StrictChromosomeMutationRateDeterminator(BaseChromosomeMutationRateDeterminator):
     """
-    Determines the random number of mutation genes in a chromosome between 1 and the maximum number of mutation genes specified.
+    Provides a strict determination of the number of chromosomes to be mutated in a population.
     """
 
-    def __init__(
-        self,
-    ) -> None:
+    def __init__(self) -> None:
         super().__init__()
 
-    def _get_number_of_mutation_genes(
-        self, chromosome, max_number_of_mutation_genes
-    ) -> int:
-        return random.randint(1, max_number_of_mutation_genes)
+    def _get_number_of_mutation_chromosomes(self) -> int:
+        return self.max_number_of_mutation_chromosomes
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py` & `gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-from gadapt.ga_model.chromosome import Chromosome
-import random
-
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
-    BaseGeneMutationSelector,
-)
-from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
-    BaseGeneMutationRateDeterminator,
+import gadapt.utils.ga_utils as ga_utils
+from gadapt.operations.mutation.chromosome_mutation.random_gene_mutation_rate_determinator import (
+    RandomGeneMutationRateDeterminator,
 )
 
 
-class RandomGeneMutationSelector(BaseGeneMutationSelector):
+class CrossDiversityGeneMutationRateDeterminator(RandomGeneMutationRateDeterminator):
     """
-    Selects and mutates genes in a chromosome using a random mutation strategy.
+    Determines the number of mutation genes in a chromosome based on the cross diversity coefficient of the decision variables.
     """
 
     def __init__(
-        self, gene_mutation_rate_determinator: BaseGeneMutationRateDeterminator
-    ):
-        super().__init__(gene_mutation_rate_determinator)
-
-    def _mutate_chromosome(self, c: Chromosome, max_number_of_mutation_genes: int):
-        if max_number_of_mutation_genes <= 1:
-            return max_number_of_mutation_genes
-        genes_to_mutate = list(c)
-        random.shuffle(genes_to_mutate)
-        number_of_mutation_genes = (
-            self._gene_mutation_rate_determinator.get_number_of_mutation_genes(
-                c, max_number_of_mutation_genes
+        self,
+    ) -> None:
+        super().__init__()
+
+    def _get_number_of_mutation_genes(self) -> int:
+        decision_variables = [g.decision_variable for g in self.chromosome]
+
+        def get_mutation_rate() -> float:
+            avg_rsd = ga_utils.average(
+                [dv.cross_diversity_coefficient for dv in decision_variables]
             )
+            if avg_rsd > 1:
+                avg_rsd = 1
+            if avg_rsd < 0:
+                avg_rsd = 0
+            return avg_rsd
+
+        mutation_rate = get_mutation_rate()
+        limit_number_of_mutation_genes = mutation_rate * float(
+            self.max_number_of_mutation_genes
         )
-        if number_of_mutation_genes <= 1:
-            return number_of_mutation_genes
-        var_num = random.randint(1, number_of_mutation_genes)
-        for g in genes_to_mutate[:var_num]:
-            g.mutate()
-            self._gene_mutated(g, c)
-
-        return var_num
+        limit_number_of_mutation_genes_rounded = round(limit_number_of_mutation_genes)
+        if limit_number_of_mutation_genes_rounded == 0:
+            limit_number_of_mutation_genes_rounded = 1
+        self.max_number_of_mutation_genes = limit_number_of_mutation_genes_rounded
+        return super()._get_number_of_mutation_genes()
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 class BaseChromosomeMutationRateDeterminator(ABC):
     """
     Provides a framework for determining the number of chromosomes to be mutated in a population.
     """
 
     def __init__(self) -> None:
         super().__init__()
+        self.max_number_of_mutation_chromosomes = -1
 
     def get_number_of_mutation_chromosomes(
         self, population, max_number_of_mutation_chromosomes
     ):
         if population is None:
             raise Exception("Population must not be null")
-        return self._get_number_of_mutation_chromosomes(
-            population, max_number_of_mutation_chromosomes
-        )
+        self.population = population
+        self.max_number_of_mutation_chromosomes = max_number_of_mutation_chromosomes
+        return self._get_number_of_mutation_chromosomes()
 
     @abstractmethod
-    def _get_number_of_mutation_chromosomes(
-        self, population, max_number_of_mutation_chromosomes
-    ) -> int:
+    def _get_number_of_mutation_chromosomes(self) -> int:
         pass
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,70 @@
-from abc import ABC, abstractmethod
 import math
-import random
+from abc import ABC, abstractmethod
 from typing import List
+
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
     BaseChromosomeMutationRateDeterminator,
 )
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_selector import (
+    BaseGeneMutationSelector,
+)
 
 
 class BaseChromosomeMutationSelector(ABC):
     """
     Selects and mutates the chromosomes in the population based on a specified number of mutated chromosomes.
     """
 
-    def mutate(self, population):
-        """
-        Mutates chromosomes in the population
-        Args:
-            population: Population to mutate
-        """
-        number_of_mutated_chromosomes = (
-            population.options.number_of_mutation_chromosomes
-        )
-        self._mutate_population(population, number_of_mutated_chromosomes)
-
     def __init__(
         self,
         chromosome_mutation_rate_determinator: BaseChromosomeMutationRateDeterminator,
+        gene_mutation_selector: BaseGeneMutationSelector,
     ) -> None:
         """
-        Base class for mutating chromosomes in population
+        Base class for selecting mating chromosomes in population
         Args:
-            options: genetic algorithm options
+            chromosome_mutation_rate_determinator: chromosome mutation rate determinator
         """
         super().__init__()
         self._chromosome_mutation_rate_determinator = (
             chromosome_mutation_rate_determinator
         )
+        self.number_of_mutation_chromosomes = -1
+        self._gene_mutation_selector = gene_mutation_selector
+
+    def mutate(self, population):
+        """
+        Mutates chromosomes in the population
+        Args:
+            population: Population to mutate
+        """
+        self.population = population
+        max_number_of_mutated_chromosomes = (
+            population.options.number_of_mutation_chromosomes
+        )
+        self.number_of_mutation_chromosomes = self._chromosome_mutation_rate_determinator.get_number_of_mutation_chromosomes(
+            self.population, max_number_of_mutated_chromosomes
+        )
+        self._mutate_population()
 
     @abstractmethod
-    def _mutate_population(self, population, number_of_mutated_chromosomes):
+    def _mutate_population(self):
         pass
 
-    def _get_unallocated_chromosomes(
-        self, population, sort_key_function=None
-    ) -> List[Chromosome]:
+    def mutate_chromosome(self, c: Chromosome, number_of_mutated_chromosomes: int):
+        self._gene_mutation_selector.mutate(c, number_of_mutated_chromosomes)
+
+    def _get_unallocated_chromosomes(self, sort_key_function=None) -> List[Chromosome]:
         def unallocated_chromosomes_condition(c: Chromosome) -> bool:
             return (
                 math.isnan(c.cost_value)
                 and (not c.is_immigrant)
-                and c.population_generation == population.population_generation
+                and c.population_generation == self.population.population_generation
                 and not c.is_mutated
             )
 
-        lst = [c for c in population if (unallocated_chromosomes_condition(c))]
+        lst = [c for c in self.population if (unallocated_chromosomes_condition(c))]
         if sort_key_function is not None:
             lst.sort(key=sort_key_function)
         return lst
-
-    def _sort_key_random(self, c: Chromosome):
-        return random.random()
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
     def append(self, determinator: BaseChromosomeMutationRateDeterminator):
         """
         Appends determinator to the composition of determinators
         """
         self.determinators.append(determinator)
 
-    def _get_number_of_mutation_chromosomes(
-        self, population, max_number_of_mutation_chromosomes
-    ):
-        if population is None:
+    def _get_number_of_mutation_chromosomes(self):
+        if self.population is None:
             raise Exception("Population must not be null")
         if len(self.determinators) == 0:
             raise Exception("at least one mutator must be added")
+        for determinator in self.determinators:
+            determinator.population = self.population
+            determinator.max_number_of_mutation_chromosomes = (
+                self.max_number_of_mutation_chromosomes
+            )
         if len(self.determinators) > 1:
             random.shuffle(self.determinators)
         current_determinator = self.determinators[0]
-        return current_determinator.get_number_of_mutation_chromosomes(
-            population, max_number_of_mutation_chromosomes
-        )
+        return current_determinator._get_number_of_mutation_chromosomes()
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
     BaseChromosomeMutationRateDeterminator,
 )
 
 
 class CostDiversityChromosomeMutationRateDeterminator(
     BaseChromosomeMutationRateDeterminator
@@ -12,26 +13,25 @@
     """
 
     def __init__(
         self,
     ) -> None:
         super().__init__()
 
-    def _get_number_of_mutation_chromosomes(
-        self, population, max_number_of_mutation_chromosomes
-    ) -> int:
+    def _get_number_of_mutation_chromosomes(self) -> int:
         def get_mutation_rate() -> float:
-            if not population.average_cost_step_in_first_population or math.isnan(
-                population.average_cost_step_in_first_population
+            if (
+                self.population.average_cost_step_in_first_population is None
+                or math.isnan(self.population.average_cost_step_in_first_population)
             ):
-                return 1
-            cost_step_ratio = (
-                population.calculate_average_cost_step()
-                / population.average_cost_step_in_first_population
+                return 1.0
+            cost_step_ratio = float(
+                self.population.average_cost_step
+                / self.population.average_cost_step_in_first_population
             )
-            if cost_step_ratio > 1:
-                cost_step_ratio = 1
-            return 1 - cost_step_ratio
+            if cost_step_ratio > 1.0:
+                cost_step_ratio = 1.0
+            return 1.0 - cost_step_ratio
 
         mutation_rate = get_mutation_rate()
-        f_return_value = mutation_rate * float(max_number_of_mutation_chromosomes)
+        f_return_value = mutation_rate * float(self.max_number_of_mutation_chromosomes)
         return round(f_return_value)
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import random
 
-from gadapt.ga_model.population import Population
 from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
     BaseChromosomeMutationRateDeterminator,
 )
 
 
 class RandomChromosomeMutationRateDeterminator(BaseChromosomeMutationRateDeterminator):
     """
@@ -12,11 +11,9 @@
     """
 
     def __init__(
         self,
     ) -> None:
         super().__init__()
 
-    def _get_number_of_mutation_chromosomes(
-        self, population: Population, max_number_of_mutation_chromosomes
-    ) -> int:
-        return random.randint(1, max_number_of_mutation_chromosomes)
+    def _get_number_of_mutation_chromosomes(self) -> int:
+        return random.randint(1, self.max_number_of_mutation_chromosomes)
```

### Comparing `gadapt-0.3.6/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.0/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from gadapt.ga_model.population import Population
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import (
-    BaseChromosomeMutationRateDeterminator,
+import random
+
+from gadapt.operations.mutation.chromosome_mutation.base_gene_mutation_rate_determinator import (
+    BaseGeneMutationRateDeterminator,
 )
 
 
-class StrictChromosomeMutationRateDeterminator(BaseChromosomeMutationRateDeterminator):
+class RandomGeneMutationRateDeterminator(BaseGeneMutationRateDeterminator):
     """
-    Provides a strict determination of the number of chromosomes to be mutated in a population.
+    Determines the random number of mutation genes in a chromosome between 1 and the maximum number of mutation genes specified.
     """
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+    ) -> None:
         super().__init__()
 
-    def _get_number_of_mutation_chromosomes(
-        self, population: Population, max_number_of_mutation_chromosomes
-    ) -> int:
-        return max_number_of_mutation_chromosomes
+    def _get_number_of_mutation_genes(self) -> int:
+        return random.randint(1, self.max_number_of_mutation_genes)
```

### Comparing `gadapt-0.3.6/gadapt/operations/sampling/base_sampling.py` & `gadapt-0.4.0/gadapt/operations/sampling/base_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import List
-from gadapt.ga_model.ranking_model import RankingModel
 from typing import TypeVar
 
+from gadapt.ga_model.ranking_model import RankingModel
+
 T = TypeVar("T", bound=RankingModel)
 
 
 class BaseSampling(ABC):
     """
     The algorithm for extracting a sample from the population.
     """
```

### Comparing `gadapt-0.3.6/gadapt/operations/sampling/roulette_wheel_sampling.py` & `gadapt-0.4.0/gadapt/operations/sampling/roulette_wheel_sampling.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import random
 from typing import List
+
 from gadapt.operations.sampling.base_sampling import T, BaseSampling
 
 
 class RouletteWheelSampling(BaseSampling):
     """
     "RouletteWheel" (also known as "Weighted Random Pairing") algorithm for\
         extracting a sample from the population.
     """
 
     def _prepare_sample(self, lst: List[T]) -> List[T]:
+        """
+        Prepares a sample from a list of objects.
+        It calculates the cumulative probabilities for each object based on their rank
+        and uses these probabilities to select objects for the sample.
+        """
         rank_sum = sum(range(1, len(lst) + 1))
-        cummultative_probability_list: List[float] = []
+        cumulative_probability_list: List[float] = []
         action_probability = 0.0
         n_keep = len(lst)
         for j in range(len(lst)):
             n = n_keep - j
             probability_for_action = float(n_keep - n + 1) / float(rank_sum)
             action_probability += probability_for_action
-            cummultative_probability_list.append(action_probability)
+            cumulative_probability_list.append(action_probability)
         rank = 0
         unallocated_members = [rm for rm in lst]
         unallocated_members.sort(key=self._sort_key, reverse=True)
         members_for_action = []
         for j in range(self.max_num):
             if len(unallocated_members) == 0:
                 continue
             for i_c_p_l, m in enumerate(unallocated_members):
-                m.action_probability = cummultative_probability_list[i_c_p_l]
+                m.action_probability = cumulative_probability_list[i_c_p_l]
             rnd_value = random.random()
             max_prob = (
                 max(unallocated_members, key=lambda m: m.action_probability)
             ).action_probability
             rnd_value = rnd_value * max_prob
             mem = next(
                 mb for mb in unallocated_members if mb.action_probability >= rnd_value
```

### Comparing `gadapt-0.3.6/gadapt/operations/sampling/tournament_sampling.py` & `gadapt-0.4.0/gadapt/operations/sampling/tournament_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 from typing import List
+
 from gadapt.operations.sampling.base_sampling import T, BaseSampling
 
 
 class TournamentSampling(BaseSampling):
     """
     "Tournament" algorithm for extracting a sample from the population.
     """
```

### Comparing `gadapt-0.3.6/gadapt/operations/variable_update/common_variable_updater.py` & `gadapt-0.4.0/gadapt/operations/variable_update/common_variable_updater.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import statistics as stat
+
 from gadapt.ga_model.decision_variable import DecisionVariable
+from gadapt.operations.variable_update.base_variable_updater import BaseVariableUpdater
 
 
-class CommonVariableUpdater:
+class CommonVariableUpdater(BaseVariableUpdater):
     """
     Common variable updater
     """
 
-    def update_variables(self, population):
+    def _update_variables(self):
 
         def scale_values(dv: DecisionVariable, values):
             scaled_values = []
             if dv.min_value == dv.max_value:
                 return [0.5] * len(
                     values
                 )  # If min_val and max_val are the same, return a list of 0.5s
 
             for value in values:
                 scaled_value = (value - dv.min_value) / (dv.max_value - dv.min_value)
                 scaled_values.append(scaled_value)
             return scaled_values
 
-        # def scale_values(data):
-        #     min_val = min(data)
-        #     max_val = max(data)
-        #     scaled_data = [(x - min_val) / (max_val - min_val) for x in data]
-        #     return scaled_data
-
         unique_values_per_variables = {}
         values_per_variables = {}
-        for c in population:
+        for c in self.population:
             if c.is_immigrant:
                 continue
             for g in c:
                 unique_var_values = unique_values_per_variables.get(
                     g.decision_variable, None
                 )
                 var_values = values_per_variables.get(g.decision_variable, None)
```

### Comparing `gadapt-0.3.6/gadapt/utils/ga_utils.py` & `gadapt-0.4.0/gadapt/utils/ga_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from functools import reduce
 import random
+from functools import reduce
 from typing import List
-import numpy as np
 
+import numpy as np
 
 """
 Genetic algorithm utility
 """
 
 
 def get_rand_bool():
@@ -113,9 +113,9 @@
 
 
 def average_difference(diff_list):
     if len(diff_list) < 2:
         return float("NaN")
     diff_list.sort()
     differences = [diff_list[i + 1] - diff_list[i] for i in range(len(diff_list) - 1)]
-    avg_difference = sum(differences) / len(differences)
+    avg_difference = float(sum(differences) / len(differences))
     return avg_difference
```

### Comparing `gadapt-0.3.6/gadapt.egg-info/PKG-INFO` & `gadapt-0.4.0/gadapt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.3.6
+Version: 0.4.0
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # GAdapt: Self-Adaptive Genetic Algorithm
-[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
-# What innovations does GAdapt bring?
-**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for adaptive mutation of genes and chromosomes.
 
+## What Innovations Does GAdapt Bring?
+
+**GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost, and cross-diversity of decision variables in the population. Less diversity increases the probability of mutation, thereby enhancing accuracy and performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
+
+## Installation
 
-# Installation
 To install **GAdapt**, use **pip** with the following command:
 
-```
+```bash
 pip install gadapt
 ```
 
 # Releases
-Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+The latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
 
 # Source Code
-The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
+The source code is available on GitHub: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
 
 # API Documentation
-The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
+For detailed API documentation, refer to: [GAdapt API Documentation](https://www.gadapt.com/api/)
 
 # Getting started
-The following example optimizes variable values for a complex trigonometric function.
+Below is an example optimizing variable values for a complex trigonometric function:
 ```python
 from gadapt.ga import GA
 import math
 
 #trigonometric function definition
 def trig_func(args):    
     return math.sqrt(abs(math.cos(args[0]))) + math.pow(math.cos(args[1]), 2) + math.sin(args[2]) + math.pow(args[3], 2) + math.sqrt(args[4]) + math.cos(args[5]) - (args[6]*math.sin(pow(args[6], 3)) + 1) + math.sin(args[0]) / (math.sqrt(args[0])/3 + (args[6]*math.sin(pow(args[6], 3)) + 1) ) / math.sqrt(args[4]) + math.cos(args[5])
@@ -73,15 +75,15 @@
 4: 1.0
 5: 3.14
 6: -1.0
 ```
 
 In this example, the genetic algorithm searches for the combination of seven parameters, bringing the lowest value for the passed function. The only mandatory attribute to the genetic algorithm is *cost_function*, and other attributes in this example took default values. Parameters to be optimized are added by the "add" method. There are seven parameters to be optimized in this example.
 # Parameter Settings
-GAdapt genetic algorithm can receive parameters using constructor, properties, or combined.
+GAdapt genetic algorithm can receive parameters through constructor, properties, or a combination of both. Below are the supported parameters:
 
 Passing parameters through the class constructor:
 ```python
 ga = GA(cost_function=trig_func,
     population_size=32,
     population_mutation="cost_diversity,parent_diversity",
     number_of_mutation_chromosomes=6,
@@ -114,71 +116,80 @@
 ga.max_attempt_no=20
 ga.logging=True
 ga.timeout=3600
 ```
 # Parameters description
 **cost_function**=*None* - Custom function for the cost calculation (fitness). The optimisation goal is minimising the output of the cost function. *cost_function* must be the function with one argument - a dictionary of values, where the key is an index (the ordinal of adding parameters) and the key is the parameter's value to be optimised. When adding parameters, there should be as many parameters as the function uses. The *cost_function* is the only mandatory parameter.
 
-**population_size**=*64* - Number of chromosomes in the population.
+**population_size**=*32* - Number of chromosomes in the population.
 
 **exit_check**=*"avg_cost"* - A criteria for the exit for the genetic algorithm.  
 Supported values:
 - *"avg_cost"* - The optimisation exit is triggered when the average cost of the upper half of the population is not improved in the specified number of generations  
 - *"min_cost"* - The optimisation exit is triggered when the minimal cost in the population is not improved in the specified number of generations  
 - *"requested"* - The optimisation exit is triggered when the requested value reached
+- *"generations"* - The optimisation exit requested number of generations defined by "number_of_generations" parameter is reached
     
-**max_attempt_no**=*10* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
+**max_attempt_no**=*2* - This parameter only takes place when *exit_check* has value *"avg_cost"* or *"min_cost"*. It determines the number of generations in which there is no improvement in the average/minimal cost.
 
 **requested_cost**=*sys.float_info.max* - This parameter only takes place when *exit_check* has value *"requested"*. It determines the requested value which causes the exit from the genetic algorithm
 
+**number_of_generations**=*200* - This parameter only takes place when exit_check has value вЂњgenerationsвЂќ. It determines the number of generations after which the genetic algorithm exits
+
 **timeout**=*120* - A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether *exit_check* criteria is reached.
 
 **parent_selection**=*"roulette_wheel"* - The algorithm for parent selection.  
 Supported values:
 - *"roulette_wheel"* - Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes in the mating pool are inversely proportional to their cost. A chromosome with the lowest cost has the greatest probability of mating, while the chromosome with the highest cost has the lowest probability of mating.  
 - *"tournament"* - Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes from the mating pool, and chromosomes with the lowest cost in subsets become a parent. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament parent selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and pairs the chromosomes two at a time until the top kept chromosomes are selected for mating. Thus, the algorithm pairs odd rows with even rows.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes.  
+
+**crossover**=*"blending"* - The algorithm for parent selection. If the Parent Diversity mutation is used, blending crossover will be used, of the choice of this parameter.
+Supported values:
+- *"blending"* - Blending crossover combines gene values from the two parents into new variable values in offsprings. One value of the offspring variable comes from a combination of the two corresponding values of the parental genes  
+- *"uniform"* - Uniform crossover combines chromosomes in a uniform way.
     
-**percentage_of_mutation_chromosomes**=*10.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_chromosomes**=*50.0* - The percentage of mutated chromosomes in the population. This value is applied to the *population_size* value and rounded to an integer value, giving the number of mutation chromosomes. For example, if *population_size* has a value of 32, and *percentage_of_mutation_chromosomes* has a value of 10, the number of mutation chromosomes will be 3. The calculated value is an upper bound - the actual number of mutated chromosomes can vary from 1 to the calculated value. *percentage_of_mutation_chromosomes* only applies if *number_of_mutation_chromosomes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_chromosomes**=*-1* - The number of mutation chromosomes in the population. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutation_chromosomes*. This value is the upper bound - the actual number of mutated chromosomes can vary from 1 to *number_of_mutation_chromosomes*.
 
-**percentage_of_mutations_genes**=*10* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
+**percentage_of_mutation_genes**=*20* - The percentage of mutated genes in each chromosome. It applies to the chromosome size (number of genes in each chromosome), and the calculated value rounds to an integer value. The calculated value is the upper bound - the actual number of mutated genes can vary from 1 to the calculated value. *percentage_of_mutations_genes* only applies if *number_of_mutations_genes* does not have a valid integer value equal to or higher than 0.
 
 **number_of_mutation_genes**=*-1* - The number of mutated genes in each chromosome. In case it's value is equal to or higher than 0, it overrides *percentage_of_mutations_genes*. This value is the upper bound - the number of mutated genes can vary from 1 to *number_of_mutation_genes*.
 
 **population_mutation**=*"cost_diversity,parent_diversity"* - A type of mutation for the entire population. Based on the value of this parameter, the number of mutation chromosomes can be determined, along with how chromosomes for the mutation will be selected.
 Supported values:
 - *"cost_diversity"* - It applies to the number of mutation chromosomes. *"cost_diversity"* determines the number of mutated chromosomes adaptively, using the diversity of costs in the population. Lower cost diversity means a higher number of mutated chromosomes. The minimal value of mutated chromosomes is 0, and the maximal value is determined by the value of *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes* parameters. If *population_mutation* has a value other than *"cost_diversity"*, the number of mutation chromosomes is a random value from 1 to *number_of_mutation_chromosomes* value (or to value determined by *percentage_of_mutation_chromosomes* value). *"cost_diversity"* means that the *"parent_diversity"* method is selected to select chromosomes to be mutated. This method only determines the number of mutated chromosomes, but not how chromosomes are selected for the mutation.  
-- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_selection* parameter.  
+- *"parent_diversity"* - It applies to the way how mutation chromosomes will be selected. *"parent_diversity"* selects chromosomes to be mutated using the diversity of their parents. The more similar parents (lower parent diversity) mean a higher probability of mutation for the child. Based on the calculated parent diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *parent_diversity_mutation_chromosome_sampling* parameter.  
 - *"random"* - It applies to the number of mutation chromosomes and to the way how mutation chromosomes will be selected. *"random"* selects chromosomes to be mutated randomly, and randomly determines the number of mutated chromosomes (with the upper bound of **number_of_mutation_chromosomes**)
 
 Population_mutation may have more values, separated by a comma. It means that more than one method can be chosen for the mutation of chromosomes in the population. For example, *"cost_diversity,parent_diversity"* means that number of mutation chromosomes will be determined by the cost diversity and the selection of chromosomes to be mutated will be defined by parent diversity. *"cost_diversity,random"* means that the cost diversity will determine the number of mutation chromosomes, and the selection of chromosomes to be mutated will be chosen randomly.
     
-**parent_diversity_mutation_chromosome_selection**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
+**parent_diversity_mutation_chromosome_sampling**=*"roulette_wheel"* - The selection algorithm for mutating chromosomes when *population_mutation* contains value *"parent_diversity"*. It only applies when *population_mutation* has value *"parent_diversity"*. It determines the way how chromosomes are to be selected based on the diversity of their parents.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the chromosomes to be mutated are proportional to the similarity of their parents (inversely proportional to the parent diversity). A chromosome with the lowest parent diversity has the greatest probability of mutation, while the chromosome with the highest parent diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of chromosomes, and chromosomes with the lowest parent diversity (highest parent similarity) in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,8"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 8 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects chromosomes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select chromosomes for mutation. In this case, selection for mutation will not depend on parent diversity.  
     
 **must_mutate_for_same_parents**=*True* - Indicates if completely the same parents must influence mutation for their children. In other words, each child will be mutated if it has parents with a diversity value of 0. If *must_mutate_for_same_parents* has the value True, the number of mutated chromosomes can outreach value determined by *number_of_mutation_chromosomes* or *percentage_of_mutation_chromosomes*
 
-**chromosome_mutation**=*"cross_diversity"* - The type of gene selection in chromosomes for mutation  
+**chromosome_mutation**=*"cross_diversity,random"* - The type of gene selection in chromosomes for mutation  
 Supported values:
-- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_selection* parameter.  
+- *"cross_diversity"* - Considers the diversity of genes of the same type in the population. Lower diversity can mean that this decision variable approaches some local minimums, and therefore such genes increase the chance for mutation. Based on the calculated cross-diversity, chromosomes may be selected by one of the selection methods, which is determined by the value of the *cross_diversity_mutation_gene_sampling* parameter.  
 - *"random"* - Genes are randomly selected for the mutation
 
-**gene_mutation**=*"normal_distribution"* - The type of assigning mutated values to genes
+**gene_mutation**=*"cross_diversity,random"* - The type of assigning mutated values to genes
 Supported values:
-- *"normal_distribution"* - assignes normally distributed random number to the variable selected for mutation
+- *"normal_distribution"* - assigns normally distributed random number to the variable selected for mutation
+- *"cross_diversity"* - assigns normally distributed random number to the variable selected for mutation, with standard deviation based on the cross-diversity coefficient
 - *"random"* - Random values are assigned to genes
 
-**cross_diversity_mutation_gene_selection**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
+**cross_diversity_mutation_gene_sampling**=*"roulette_wheel"* - the selection algorithm for mutating chromosomes when *chromosome_mutation* has value *"cross_diversity"*. It only applies when *chromosome_mutation* has value *"cross_diversity"* . It determines the way how genes are to be selected based on the cross-diversity.  
 Supported values:
 - *"roulette_wheel"* - The Roulette Wheel selection algorithm (also known as "Weighted Random Pairing"). The probabilities assigned to the genes to be mutated are inversely proportional to their cross-diversity. A gene with the lowest cross-diversity has the greatest probability of mutation, while the gene with the highest cross-diversity has the lowest probability of mutation.  
 - *"tournament"* - The Tournament selection algorithm. It randomly picks small subsets (groups) of genes, and genes with the lowest cross-diversity in subsets are chosen to be mutated. *"tournament"* can have an additional parameter separated from the *"tournament"* keyword by the comma. The other value represents a group size. For example, *"tournament,3"* means that the tournament mutation selection algorithm is chosen, and each group contains up to 3 members. The default group size is 4.  
 - *"from_top_to_bottom"* - From Top To Bottom selection algorithm starts at the top of the list and selects genes for mutation.  
 - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
     
 **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
@@ -271,51 +282,50 @@
 Number of iterations: 21
 Parameter values:
 0: 0.0
 1: 0.0
 ```
 
 # GA Customisation
-GAdapt has been developed in common with clean architecture and SOLID principles and therefore it can be customized easily. Customization can be applied by creating new implementation of abstract classes and passing them to the gnetic algorithm through factory object. Abstract classes are all classes in "operation" folder with names starting with "Base". Please consult  [GAdapt API Documentation](https://www.gadapt.com/api/) for more information about GAdapt classes.
+GAdapt follows clean architecture and SOLID principles, allowing easy customization. Create new implementations of abstract classes and pass them to the genetic algorithm through the factory object.
 
-Example of customisation of GAdapt by introducing a new class for mutation of population:
+For example, customizing the chromosome mutation selector:
 
 ```python
 import math
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga import GA
-from gadapt.operations.mutation.population_mutation.base_chromosome_mutation_rate_determinator import
-
-BaseChromosomeMutationRateDeterminator
+from operations.mutation.population_mutation.base_chromosome_mutation_selector import BaseChromosomeMutationSelector
+from operations.mutation.population_mutation.random_chromosome_mutation_rate_determinator import RandomChromosomeMutationRateDeterminator
 
 
-class BottomPopulationMutator(BaseChromosomeMutationRateDeterminator):
+class BottomMutationSelector(BaseChromosomeMutationSelector):
     """
-    Population mutator which selects mutating chromosomes from the bottom of
-    existing unallocated chromosoms 
+    Chromosome mutation selector which selects mutating chromosomes from the bottom of
+    existing unallocated chromosomes sorted by the cost function value
     """
 
-    def _mutate_population(self, population, number_of_mutation_chromosomes):
-        if population is None:
+    def _mutate_population(self):
+        if self.population is None:
             raise Exception("population must not be None")
         unallocated_chromosomes = self._get_unallocated_chromosomes(
-            population, None
+            lambda chrom: (self.population.options.cost_function([g.variable_value for g in chrom]))
         )
         chromosomes_for_mutation = unallocated_chromosomes[
-                                   len(unallocated_chromosomes) - number_of_mutation_chromosomes:
+                                   len(unallocated_chromosomes) - self.number_of_mutation_chromosomes:
                                    ]
         for c in chromosomes_for_mutation:
-            c.mutate(population.options.number_of_mutation_genes)
+            self._gene_mutation_selector.mutate(c, self.population.options.number_of_mutation_genes)
 
 
 def some_func(args):
     return math.sqrt(abs(args[0])) + math.pow(args[1], 2)
 
 
 custom_factory = GAFactory()
-custom_factory.population_mutator = BottomPopulationMutator()
+custom_factory.chromosome_mutation_selector = BottomMutationSelector(RandomChromosomeMutationRateDeterminator())
 ga = GA(cost_function=some_func, factory=custom_factory)
 ga.add(-25, 25, 1)
 ga.add(-5, 5, 0.1)
 
 print(ga.execute())
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gadapt-0.3.6/gadapt.egg-info/SOURCES.txt` & `gadapt-0.4.0/gadapt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 gadapt/ga_model/ranking_model.py
 gadapt/operations/__init__.py
 gadapt/operations/cost_finding/__init__.py
 gadapt/operations/cost_finding/base_cost_finder.py
 gadapt/operations/cost_finding/elitism_cost_finder.py
 gadapt/operations/crossover/__init__.py
 gadapt/operations/crossover/base_crossover.py
+gadapt/operations/crossover/blending_crossover.py
+gadapt/operations/crossover/blending_parent_diversity_crossover.py
 gadapt/operations/crossover/uniform_crossover.py
 gadapt/operations/exit_check/__init__.py
 gadapt/operations/exit_check/avg_cost_exit_checker.py
 gadapt/operations/exit_check/base_exit_checker.py
 gadapt/operations/exit_check/min_cost_exit_checker.py
+gadapt/operations/exit_check/number_of_generations_exit_checker.py
 gadapt/operations/exit_check/requested_cost_exit_checker.py
-gadapt/operations/gene_combination/__init__.py
-gadapt/operations/gene_combination/base_gene_combination.py
-gadapt/operations/gene_combination/blending_gene_combination.py
 gadapt/operations/immigration/__init__.py
 gadapt/operations/immigration/chromosome_immigration/__init__.py
 gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
 gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
 gadapt/operations/immigration/population_immigration/__init__.py
 gadapt/operations/immigration/population_immigration/base_population_immigrator.py
 gadapt/operations/immigration/population_immigration/common_population_immigrator.py
@@ -64,15 +64,17 @@
 gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
 gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
 gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
 gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
 gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
 gadapt/operations/mutation/gene_mutation/__init__.py
 gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
 gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
 gadapt/operations/mutation/population_mutation/__init__.py
 gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
 gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
 gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
 gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
@@ -81,19 +83,23 @@
 gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
 gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
 gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
 gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
 gadapt/operations/parent_selection/__init__.py
 gadapt/operations/parent_selection/base_parent_selector.py
 gadapt/operations/parent_selection/sampling_parent_selector.py
+gadapt/operations/population_update/__init__.py
+gadapt/operations/population_update/base_population_updater.py
+gadapt/operations/population_update/common_population_updater.py
 gadapt/operations/sampling/__init__.py
 gadapt/operations/sampling/base_sampling.py
 gadapt/operations/sampling/from_top_to_bottom_sampling.py
 gadapt/operations/sampling/random_sampling.py
 gadapt/operations/sampling/roulette_wheel_sampling.py
 gadapt/operations/sampling/tournament_sampling.py
 gadapt/operations/variable_update/__init__.py
 gadapt/operations/variable_update/base_variable_updater.py
 gadapt/operations/variable_update/common_variable_updater.py
 gadapt/utils/TimeStampFormatter.py
 gadapt/utils/__init__.py
+gadapt/utils/ga_decorators.py
 gadapt/utils/ga_utils.py
```

### Comparing `gadapt-0.3.6/pyproject.toml` & `gadapt-0.4.0/pyproject.toml`

 * *Files identical despite different names*

