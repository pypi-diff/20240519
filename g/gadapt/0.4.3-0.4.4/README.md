# Comparing `tmp/gadapt-0.4.3.tar.gz` & `tmp/gadapt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gadapt-0.4.3.tar", last modified: Sun May 19 10:34:54 2024, max compression
+gzip compressed data, was "gadapt-0.4.4.tar", last modified: Sun May 19 19:08:31 2024, max compression
```

## Comparing `gadapt-0.4.3.tar` & `gadapt-0.4.4.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.312925 gadapt-0.4.3/
--rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.4.3/LICENSE
--rw-rw-rw-   0        0        0    23187 2024-05-19 10:34:54.312429 gadapt-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    22848 2024-05-17 19:20:08.000000 gadapt-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.046424 gadapt-0.4.3/gadapt/
--rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.085924 gadapt-0.4.3/gadapt/adapters/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.3/gadapt/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.087924 gadapt-0.4.3/gadapt/adapters/ga_logging/
--rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/adapters/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2204 2024-05-05 22:50:27.000000 gadapt-0.4.3/gadapt/adapters/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.089924 gadapt-0.4.3/gadapt/adapters/string_operation/
--rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.4.3/gadapt/adapters/string_operation/__init__.py
--rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.4.3/gadapt/adapters/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.093924 gadapt-0.4.3/gadapt/adapters/validation/
--rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.3/gadapt/adapters/validation/__init__.py
--rw-rw-rw-   0        0        0      941 2024-05-05 18:18:08.000000 gadapt-0.4.3/gadapt/adapters/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    24756 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/adapters/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.096424 gadapt-0.4.3/gadapt/execution/
--rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     4581 2024-05-19 09:02:00.000000 gadapt-0.4.3/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.101925 gadapt-0.4.3/gadapt/factory/
--rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     6807 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/factory/ga_base_factory.py
--rw-rw-rw-   0        0        0    23242 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    32066 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.116923 gadapt-0.4.3/gadapt/ga_model/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     7865 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0     3649 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga_model/decision_variable.py
--rw-rw-rw-   0        0        0     1093 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     7797 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2258 2024-05-05 18:18:09.000000 gadapt-0.4.3/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1912 2024-05-17 22:12:01.000000 gadapt-0.4.3/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0     6785 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.4.3/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.117924 gadapt-0.4.3/gadapt/operations/
--rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.4.3/gadapt/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.126423 gadapt-0.4.3/gadapt/operations/cost_finding/
--rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/cost_finding/__init__.py
--rw-rw-rw-   0        0        0     1447 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     1830 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/cost_finding/elitism_cost_finder.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.133423 gadapt-0.4.3/gadapt/operations/crossover/
--rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/crossover/__init__.py
--rw-rw-rw-   0        0        0     8305 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1613 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/crossover/blending_crossover.py
--rw-rw-rw-   0        0        0     1734 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/crossover/blending_parent_diversity_crossover.py
--rw-rw-rw-   0        0        0     1127 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.144423 gadapt-0.4.3/gadapt/operations/exit_check/
--rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/exit_check/__init__.py
--rw-rw-rw-   0        0        0      513 2024-05-05 22:30:06.000000 gadapt-0.4.3/gadapt/operations/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1625 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      490 2024-05-05 22:30:18.000000 gadapt-0.4.3/gadapt/operations/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      584 2024-05-07 06:26:43.000000 gadapt-0.4.3/gadapt/operations/exit_check/number_of_generations_exit_checker.py
--rw-rw-rw-   0        0        0      522 2024-05-05 22:30:27.000000 gadapt-0.4.3/gadapt/operations/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.148424 gadapt-0.4.3/gadapt/operations/immigration/
--rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.152424 gadapt-0.4.3/gadapt/operations/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      993 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      370 2024-05-05 22:50:27.000000 gadapt-0.4.3/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.156423 gadapt-0.4.3/gadapt/operations/immigration/population_immigration/
--rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0     1097 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.157923 gadapt-0.4.3/gadapt/operations/mutation/
--rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.187926 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      900 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2058 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2145 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
--rw-rw-rw-   0        0        0     1472 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2049 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      591 2024-05-05 22:03:38.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1449 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
--rw-rw-rw-   0        0        0      477 2024-05-05 22:50:27.000000 gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.220924 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/
--rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
--rw-rw-rw-   0        0        0     1021 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py
--rw-rw-rw-   0        0        0     2362 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
--rw-rw-rw-   0        0        0      703 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py
--rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
--rw-rw-rw-   0        0        0      427 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.253424 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/
--rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0      815 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2647 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1485 2024-05-05 22:50:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1948 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0     1295 2024-05-05 22:50:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1189 2024-05-05 22:49:46.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     2829 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      600 2024-05-05 22:50:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
--rw-rw-rw-   0        0        0     1750 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
--rw-rw-rw-   0        0        0      541 2024-05-05 22:50:08.000000 gadapt-0.4.3/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.259426 gadapt-0.4.3/gadapt/operations/parent_selection/
--rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.4.3/gadapt/operations/parent_selection/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-05-16 06:43:45.000000 gadapt-0.4.3/gadapt/operations/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      800 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.263925 gadapt-0.4.3/gadapt/operations/population_update/
--rw-rw-rw-   0        0        0       40 2024-04-27 16:02:41.000000 gadapt-0.4.3/gadapt/operations/population_update/__init__.py
--rw-rw-rw-   0        0        0      412 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/population_update/base_population_updater.py
--rw-rw-rw-   0        0        0      961 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/operations/population_update/common_population_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.277925 gadapt-0.4.3/gadapt/operations/sampling/
--rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.4.3/gadapt/operations/sampling/__init__.py
--rw-rw-rw-   0        0        0     1104 2024-05-05 18:18:08.000000 gadapt-0.4.3/gadapt/operations/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      511 2024-05-05 18:18:09.000000 gadapt-0.4.3/gadapt/operations/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      502 2024-05-05 18:18:08.000000 gadapt-0.4.3/gadapt/operations/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     2125 2024-05-05 18:18:09.000000 gadapt-0.4.3/gadapt/operations/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2603 2024-05-05 18:18:08.000000 gadapt-0.4.3/gadapt/operations/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.280925 gadapt-0.4.3/gadapt/operations/variable_update/
--rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.4.3/gadapt/operations/variable_update/__init__.py
--rw-rw-rw-   0        0        0      377 2024-05-05 22:47:04.000000 gadapt-0.4.3/gadapt/operations/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2449 2024-05-05 22:37:22.000000 gadapt-0.4.3/gadapt/operations/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.284925 gadapt-0.4.3/gadapt/utils/
--rw-rw-rw-   0        0        0      443 2024-05-05 18:18:08.000000 gadapt-0.4.3/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.4.3/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-17 19:20:08.000000 gadapt-0.4.3/gadapt/utils/ga_decorators.py
--rw-rw-rw-   0        0        0     2916 2024-05-17 18:56:26.000000 gadapt-0.4.3/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:34:54.286926 gadapt-0.4.3/gadapt.egg-info/
--rw-rw-rw-   0        0        0    23187 2024-05-19 10:34:53.000000 gadapt-0.4.3/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5593 2024-05-19 10:34:53.000000 gadapt-0.4.3/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:34:53.000000 gadapt-0.4.3/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-19 10:34:53.000000 gadapt-0.4.3/gadapt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 10:34:53.000000 gadapt-0.4.3/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      830 2024-05-19 10:31:54.000000 gadapt-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      111 2024-05-19 10:34:54.319926 gadapt-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      495 2024-05-19 10:32:58.000000 gadapt-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.295394 gadapt-0.4.4/
+-rw-rw-rw-   0        0        0     1522 2023-05-20 09:05:31.000000 gadapt-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0    23187 2024-05-19 19:08:31.294891 gadapt-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    22848 2024-05-17 19:20:08.000000 gadapt-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:29.830884 gadapt-0.4.4/gadapt/
+-rw-rw-rw-   0        0        0       36 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:29.875882 gadapt-0.4.4/gadapt/adapters/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.4/gadapt/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:29.886381 gadapt-0.4.4/gadapt/adapters/ga_logging/
+-rw-rw-rw-   0        0        0       28 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/adapters/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2243 2024-05-19 19:04:58.000000 gadapt-0.4.4/gadapt/adapters/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:29.932882 gadapt-0.4.4/gadapt/adapters/string_operation/
+-rw-rw-rw-   0        0        0       92 2023-09-10 20:35:28.000000 gadapt-0.4.4/gadapt/adapters/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     4190 2024-04-06 20:11:32.000000 gadapt-0.4.4/gadapt/adapters/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.007888 gadapt-0.4.4/gadapt/adapters/validation/
+-rw-rw-rw-   0        0        0       33 2023-09-10 20:35:28.000000 gadapt-0.4.4/gadapt/adapters/validation/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-05-05 18:18:08.000000 gadapt-0.4.4/gadapt/adapters/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    24756 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/adapters/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.017890 gadapt-0.4.4/gadapt/execution/
+-rw-rw-rw-   0        0        0       50 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     4581 2024-05-19 09:02:00.000000 gadapt-0.4.4/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.030390 gadapt-0.4.4/gadapt/factory/
+-rw-rw-rw-   0        0        0       76 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     6807 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/factory/ga_base_factory.py
+-rw-rw-rw-   0        0        0    23242 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    32066 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.215884 gadapt-0.4.4/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     7865 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0     3649 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga_model/decision_variable.py
+-rw-rw-rw-   0        0        0     1093 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     7797 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2258 2024-05-05 18:18:09.000000 gadapt-0.4.4/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1912 2024-05-17 22:12:01.000000 gadapt-0.4.4/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0     6785 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0     1269 2024-03-05 19:39:48.000000 gadapt-0.4.4/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.223885 gadapt-0.4.4/gadapt/operations/
+-rw-rw-rw-   0        0        0      183 2024-04-09 20:23:35.000000 gadapt-0.4.4/gadapt/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.234887 gadapt-0.4.4/gadapt/operations/cost_finding/
+-rw-rw-rw-   0        0        0       66 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     1890 2024-05-19 19:06:06.000000 gadapt-0.4.4/gadapt/operations/cost_finding/elitism_cost_finder.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.265389 gadapt-0.4.4/gadapt/operations/crossover/
+-rw-rw-rw-   0        0        0       35 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/crossover/__init__.py
+-rw-rw-rw-   0        0        0     8305 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1613 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/crossover/blending_crossover.py
+-rw-rw-rw-   0        0        0     1734 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/crossover/blending_parent_diversity_crossover.py
+-rw-rw-rw-   0        0        0     1127 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.284885 gadapt-0.4.4/gadapt/operations/exit_check/
+-rw-rw-rw-   0        0        0       58 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-05-05 22:30:06.000000 gadapt-0.4.4/gadapt/operations/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1685 2024-05-19 19:06:14.000000 gadapt-0.4.4/gadapt/operations/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      490 2024-05-05 22:30:18.000000 gadapt-0.4.4/gadapt/operations/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      584 2024-05-07 06:26:43.000000 gadapt-0.4.4/gadapt/operations/exit_check/number_of_generations_exit_checker.py
+-rw-rw-rw-   0        0        0      522 2024-05-05 22:30:27.000000 gadapt-0.4.4/gadapt/operations/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.292385 gadapt-0.4.4/gadapt/operations/immigration/
+-rw-rw-rw-   0        0        0       56 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.312385 gadapt-0.4.4/gadapt/operations/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       71 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      993 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      370 2024-05-05 22:50:27.000000 gadapt-0.4.4/gadapt/operations/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.324387 gadapt-0.4.4/gadapt/operations/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       81 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0     1097 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.332885 gadapt-0.4.4/gadapt/operations/mutation/
+-rw-rw-rw-   0        0        0       40 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.375888 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       44 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      900 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2058 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2145 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0     1472 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2049 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      591 2024-05-05 22:03:38.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1449 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py
+-rw-rw-rw-   0        0        0      477 2024-05-05 22:50:27.000000 gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/strict_gene_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.674389 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/
+-rw-rw-rw-   0        0        0       25 2024-03-16 13:31:03.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py
+-rw-rw-rw-   0        0        0     1021 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py
+-rw-rw-rw-   0        0        0     2362 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py
+-rw-rw-rw-   0        0        0      703 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py
+-rw-rw-rw-   0        0        0     1678 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py
+-rw-rw-rw-   0        0        0      427 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/random_gene_mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:30.965389 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       53 2023-09-10 20:35:27.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2647 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1485 2024-05-05 22:50:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1948 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0     1295 2024-05-05 22:50:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1189 2024-05-05 22:49:46.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     2829 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      600 2024-05-05 22:50:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py
+-rw-rw-rw-   0        0        0     1750 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py
+-rw-rw-rw-   0        0        0      541 2024-05-05 22:50:08.000000 gadapt-0.4.4/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.027895 gadapt-0.4.4/gadapt/operations/parent_selection/
+-rw-rw-rw-   0        0        0       39 2023-09-10 20:35:28.000000 gadapt-0.4.4/gadapt/operations/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-05-16 06:43:45.000000 gadapt-0.4.4/gadapt/operations/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      800 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.039891 gadapt-0.4.4/gadapt/operations/population_update/
+-rw-rw-rw-   0        0        0       40 2024-04-27 16:02:41.000000 gadapt-0.4.4/gadapt/operations/population_update/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/population_update/base_population_updater.py
+-rw-rw-rw-   0        0        0      961 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/operations/population_update/common_population_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.194890 gadapt-0.4.4/gadapt/operations/sampling/
+-rw-rw-rw-   0        0        0      136 2023-09-10 20:52:27.000000 gadapt-0.4.4/gadapt/operations/sampling/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-05-05 18:18:08.000000 gadapt-0.4.4/gadapt/operations/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      511 2024-05-05 18:18:09.000000 gadapt-0.4.4/gadapt/operations/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      502 2024-05-05 18:18:08.000000 gadapt-0.4.4/gadapt/operations/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     2125 2024-05-05 18:18:09.000000 gadapt-0.4.4/gadapt/operations/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2603 2024-05-05 18:18:08.000000 gadapt-0.4.4/gadapt/operations/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.221891 gadapt-0.4.4/gadapt/operations/variable_update/
+-rw-rw-rw-   0        0        0       56 2024-04-06 20:11:32.000000 gadapt-0.4.4/gadapt/operations/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-05 22:47:04.000000 gadapt-0.4.4/gadapt/operations/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2449 2024-05-05 22:37:22.000000 gadapt-0.4.4/gadapt/operations/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.275891 gadapt-0.4.4/gadapt/utils/
+-rw-rw-rw-   0        0        0      443 2024-05-05 18:18:08.000000 gadapt-0.4.4/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       37 2023-09-10 20:35:28.000000 gadapt-0.4.4/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-17 19:20:08.000000 gadapt-0.4.4/gadapt/utils/ga_decorators.py
+-rw-rw-rw-   0        0        0     2916 2024-05-17 18:56:26.000000 gadapt-0.4.4/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:08:31.278394 gadapt-0.4.4/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    23187 2024-05-19 19:08:28.000000 gadapt-0.4.4/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5593 2024-05-19 19:08:28.000000 gadapt-0.4.4/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 19:08:28.000000 gadapt-0.4.4/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-19 19:08:28.000000 gadapt-0.4.4/gadapt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 19:08:28.000000 gadapt-0.4.4/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      830 2024-05-19 19:07:44.000000 gadapt-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2024-05-19 19:08:31.302891 gadapt-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      479 2024-05-19 19:07:40.000000 gadapt-0.4.4/setup.py
```

### Comparing `gadapt-0.4.3/LICENSE` & `gadapt-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/PKG-INFO` & `gadapt-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.4.3
+Version: 0.4.4
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
```

### Comparing `gadapt-0.4.3/README.md` & `gadapt-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/adapters/string_operation/ga_strings.py` & `gadapt-0.4.4/gadapt/adapters/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/adapters/validation/base_options_validator.py` & `gadapt-0.4.4/gadapt/adapters/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/adapters/validation/common_options_validator.py` & `gadapt-0.4.4/gadapt/adapters/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/execution/ga_executor.py` & `gadapt-0.4.4/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/factory/ga_base_factory.py` & `gadapt-0.4.4/gadapt/factory/ga_base_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/factory/ga_factory.py` & `gadapt-0.4.4/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga.py` & `gadapt-0.4.4/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/chromosome.py` & `gadapt-0.4.4/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/decision_variable.py` & `gadapt-0.4.4/gadapt/ga_model/decision_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/definitions.py` & `gadapt-0.4.4/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/ga_options.py` & `gadapt-0.4.4/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/ga_results.py` & `gadapt-0.4.4/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/gene.py` & `gadapt-0.4.4/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/population.py` & `gadapt-0.4.4/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/ga_model/ranking_model.py` & `gadapt-0.4.4/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/cost_finding/base_cost_finder.py` & `gadapt-0.4.4/gadapt/operations/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/cost_finding/elitism_cost_finder.py` & `gadapt-0.4.4/gadapt/operations/cost_finding/elitism_cost_finder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import logging
 import math
 from typing import List
 
+from gadapt.adapters.ga_logging.logging_settings import gadapt_log_info
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.operations.cost_finding.base_cost_finder import BaseCostFinder
 
 
 class ElitismCostFinder(BaseCostFinder):
     """
     Finding costs for a better half of the population
@@ -40,8 +40,8 @@
             [c.cost_value for c in better_chromosomes_without_immigrants]
         ) / len(better_chromosomes_without_immigrants)
         self._log_population()
         self.population.clear_and_add_chromosomes(better_chromosomes)
 
     def _log_population(self):
         if self.population.options.logging:
-            logging.info(str(self.population))
+            gadapt_log_info(str(self.population))
```

### Comparing `gadapt-0.4.3/gadapt/operations/crossover/base_crossover.py` & `gadapt-0.4.4/gadapt/operations/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/crossover/blending_crossover.py` & `gadapt-0.4.4/gadapt/operations/crossover/blending_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/crossover/blending_parent_diversity_crossover.py` & `gadapt-0.4.4/gadapt/operations/crossover/blending_parent_diversity_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/crossover/uniform_crossover.py` & `gadapt-0.4.4/gadapt/operations/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/exit_check/avg_cost_exit_checker.py` & `gadapt-0.4.4/gadapt/operations/exit_check/avg_cost_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/exit_check/base_exit_checker.py` & `gadapt-0.4.4/gadapt/operations/exit_check/base_exit_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import logging
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Optional
 
+from gadapt.adapters.ga_logging.logging_settings import gadapt_log_info
 from gadapt.ga_model.population import Population
 
 
 class BaseExitChecker(ABC):
     """
     Base class for exit check
     Args:
@@ -40,14 +40,14 @@
             self.population.timeout_expired = True
             return True
         if self._is_exit():
             self.attempt_no += 1
         else:
             self.attempt_no = 0
         if self.attempt_no >= self.max_attempt_no:
-            logging.info("function exit.")
+            gadapt_log_info("function exit.")
             return True
         return False
 
     @abstractmethod
     def _is_exit(self) -> bool:
         pass
```

### Comparing `gadapt-0.4.3/gadapt/operations/exit_check/number_of_generations_exit_checker.py` & `gadapt-0.4.4/gadapt/operations/exit_check/number_of_generations_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/exit_check/requested_cost_exit_checker.py` & `gadapt-0.4.4/gadapt/operations/exit_check/requested_cost_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.4.4/gadapt/operations/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/immigration/population_immigration/base_population_immigrator.py` & `gadapt-0.4.4/gadapt/operations/immigration/population_immigration/base_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.4.4/gadapt/operations/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/base_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/composed_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/cross_diversity_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/chromosome_mutation/random_gene_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py` & `gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/base_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py` & `gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/composed_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py` & `gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/extreme_pointed_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py` & `gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/normal_distribution_cross_diversity_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py` & `gadapt-0.4.4/gadapt/operations/mutation/gene_mutation/normal_distribution_gene_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/base_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/composed_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/cost_diversity_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/cross_diversity_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/parent_diversity_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/random_chromosome_mutation_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py` & `gadapt-0.4.4/gadapt/operations/mutation/population_mutation/strict_chromosome_mutation_rate_determinator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/parent_selection/base_parent_selector.py` & `gadapt-0.4.4/gadapt/operations/parent_selection/base_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/parent_selection/sampling_parent_selector.py` & `gadapt-0.4.4/gadapt/operations/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/population_update/common_population_updater.py` & `gadapt-0.4.4/gadapt/operations/population_update/common_population_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/sampling/base_sampling.py` & `gadapt-0.4.4/gadapt/operations/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/sampling/roulette_wheel_sampling.py` & `gadapt-0.4.4/gadapt/operations/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/sampling/tournament_sampling.py` & `gadapt-0.4.4/gadapt/operations/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/operations/variable_update/common_variable_updater.py` & `gadapt-0.4.4/gadapt/operations/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/utils/ga_decorators.py` & `gadapt-0.4.4/gadapt/utils/ga_decorators.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt/utils/ga_utils.py` & `gadapt-0.4.4/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/gadapt.egg-info/PKG-INFO` & `gadapt-0.4.4/gadapt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.4.3
+Version: 0.4.4
 Summary: GAdapt: A Python Library for        Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
```

### Comparing `gadapt-0.4.3/gadapt.egg-info/SOURCES.txt` & `gadapt-0.4.4/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gadapt-0.4.3/pyproject.toml` & `gadapt-0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gadapt"
-version = "0.4.3"
+version = "0.4.4"
 description = "Self-Adaptive Genetic Algorithm"
 authors = ["Zoran Jankovic <bpzoran@yahoo.com>"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

