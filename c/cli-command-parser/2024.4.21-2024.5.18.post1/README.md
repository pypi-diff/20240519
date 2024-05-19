# Comparing `tmp/cli_command_parser-2024.4.21.tar.gz` & `tmp/cli_command_parser-2024.5.18.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2024.4.21.tar", last modified: Sun Apr 21 18:50:10 2024, max compression
+gzip compressed data, was "cli_command_parser-2024.5.18.post1.tar", last modified: Sat May 18 19:53:14 2024, max compression
```

## Comparing `cli_command_parser-2024.4.21.tar` & `cli_command_parser-2024.5.18.post1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.755294 cli_command_parser-2024.4.21/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.21/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.21/MANIFEST.in
--rw-rw-rw-   0        0        0     5947 2024-04-21 18:50:10.755294 cli_command_parser-2024.4.21/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/entry_points.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.556295 cli_command_parser-2024.4.21/lib/
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.631295 cli_command_parser-2024.4.21/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1172 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2024-04-21 18:50:01.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0     2876 2024-04-21 18:49:52.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19229 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    17763 2024-04-21 18:49:52.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     5101 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    18605 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    19931 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.671296 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12711 2023-05-08 11:55:32.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0     2047 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/cli.py
--rw-rw-rw-   0        0        0    24279 2023-05-08 11:55:32.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     8927 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0    12518 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 19:45:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     8297 2024-04-21 18:49:52.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.688295 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     9550 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    21528 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     9377 2023-05-13 19:45:03.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5306 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.719295 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6695 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     9096 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     8341 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0     7596 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/patterns.py
--rw-rw-rw-   0        0        0    22732 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0    17663 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     8144 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.753296 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    17329 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/actions.py
--rw-rw-rw-   0        0        0    26658 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    16689 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    11219 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     8253 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    25510 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11295 2023-05-21 20:53:58.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    16866 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0    12374 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1999 2023-10-14 13:44:15.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     5864 2024-04-20 20:55:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 18:50:10.754294 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     5947 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-21 18:50:10.000000 cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2024.4.21/pyproject.toml
--rw-rw-rw-   0        0        0     4428 2023-10-14 13:44:15.000000 cli_command_parser-2024.4.21/readme.rst
--rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2024.4.21/requirements-dev.txt
--rw-rw-rw-   0        0        0     1500 2024-04-21 18:50:10.756293 cli_command_parser-2024.4.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.144151 cli_command_parser-2024.5.18.post1/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.18.post1/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.18.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6008 2024-05-18 19:53:14.144151 cli_command_parser-2024.5.18.post1/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.18.post1/entry_points.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.012194 cli_command_parser-2024.5.18.post1/lib/
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.063356 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1172 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      297 2024-05-18 19:53:01.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0     2876 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    19242 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    17746 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5113 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    21162 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    19894 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.101153 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12662 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0     2047 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/cli.py
+-rw-rw-rw-   0        0        0    24268 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     8941 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    12490 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    15347 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6781 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8297 2024-04-21 18:49:52.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.108152 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     9786 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    21375 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     9358 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     7927 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.127152 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 19:11:26.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-20 18:50:11.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6695 2024-04-20 20:55:10.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     9029 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     8339 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0     7625 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/patterns.py
+-rw-rw-rw-   0        0        0    22730 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6523 2023-05-20 18:50:11.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    17645 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     8144 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.142152 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      313 2023-06-14 11:32:55.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    17323 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/actions.py
+-rw-rw-rw-   0        0        0    26713 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    16751 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    11206 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     8230 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25503 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 16:32:28.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4543 2023-07-30 20:03:01.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11277 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    16870 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    12374 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     2117 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     5858 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 19:53:14.143151 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     6008 2024-05-18 19:53:13.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2024-05-18 19:53:14.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 19:53:13.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-18 19:53:13.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2024-05-18 19:53:13.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-18 19:53:13.000000 cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1991 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/pyproject.toml
+-rw-rw-rw-   0        0        0     4483 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/readme.rst
+-rw-rw-rw-   0        0        0      116 2024-05-18 19:49:30.000000 cli_command_parser-2024.5.18.post1/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1500 2024-05-18 19:53:14.145151 cli_command_parser-2024.5.18.post1/setup.cfg
```

### Comparing `cli_command_parser-2024.4.21/LICENSE` & `cli_command_parser-2024.5.18.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/PKG-INFO` & `cli_command_parser-2024.5.18.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2024.4.21
+Version: 2024.5.18.post1
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
@@ -30,27 +30,27 @@
 Requires-Dist: wcwidth; extra == "wcwidth"
 Provides-Extra: conversion
 Requires-Dist: astunparse; python_version < "3.9" and extra == "conversion"
 
 CLI Command Parser
 ##################
 
-|downloads| |py_version| |coverage_badge| |build_status| |Blue|
+|downloads| |py_version| |coverage_badge| |build_status| |Ruff|
 
 .. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
 
-.. |Blue| image:: https://img.shields.io/badge/code%20style-blue-blue.svg
-    :target: https://blue.readthedocs.io/
+.. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://docs.astral.sh/ruff/
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/cli-command-parser
     :target: https://pypistats.org/packages/cli-command-parser
 
 
 CLI Command Parser is a class-based CLI argument parser that defines parameters with descriptors.  It provides the
 tools to quickly and easily get started with basic CLIs, and it scales well to support even very large and complex
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/__init__.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/annotations.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/annotations.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/command_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,48 +8,50 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import cached_property
-from typing import TYPE_CHECKING, Optional, Collection, Iterator, List, Dict, Set, Tuple
+from typing import TYPE_CHECKING, Collection, Iterator, Optional
 
-from .config import CommandConfig, AmbiguousComboMode
-from .exceptions import CommandDefinitionError, ParameterDefinitionError, AmbiguousShortForm, AmbiguousCombo
-from .parameters.base import ParamBase, Parameter, BaseOption, BasePositional
-from .parameters import SubCommand, PassThru, ActionFlag, ParamGroup, Action, help_action
+from .config import AmbiguousComboMode, CommandConfig
+from .exceptions import AmbiguousCombo, AmbiguousShortForm, CommandDefinitionError, ParameterDefinitionError
+from .parameters import Action, ActionFlag, ParamGroup, PassThru, SubCommand, help_action
+from .parameters.base import BaseOption, BasePositional, ParamBase, Parameter
 
 if TYPE_CHECKING:
     from .context import Context
     from .formatting.commands import CommandHelpFormatter
     from .typing import CommandCls, Strings
 
-__all__ = ['CommandParameters']
+    OptionMap = dict[str, BaseOption]
+    ActionFlags = list[ActionFlag]
 
-OptionMap = Dict[str, BaseOption]
-ActionFlags = List[ActionFlag]
+__all__ = ['CommandParameters']
 
 
 class CommandParameters:
+    # fmt: off
     command: CommandCls                                  #: The Command associated with this CommandParameters object
     formatter: CommandHelpFormatter                      #: The formatter used for this Command's help text
     command_parent: Optional[CommandCls]                 #: The parent Command, if any
     parent: Optional[CommandParameters]                  #: The parent Command's CommandParameters
     action: Optional[Action] = None                      #: An Action Parameter, if specified
     _pass_thru: Optional[PassThru] = None                #: A PassThru Parameter, if specified
     sub_command: Optional[SubCommand] = None             #: A SubCommand Parameter, if specified
     action_flags: ActionFlags                            #: List of action flags
-    split_action_flags: Tuple[ActionFlags, ActionFlags]  #: Action flags split by before/after main
-    options: List[BaseOption]                            #: List of optional Parameters
+    split_action_flags: tuple[ActionFlags, ActionFlags]  #: Action flags split by before/after main
+    options: list[BaseOption]                            #: List of optional Parameters
     combo_option_map: OptionMap                          #: Mapping of {short opt: Parameter} (no dash characters)
-    groups: List[ParamGroup]                             #: List of ParamGroup objects
-    positionals: List[BasePositional]                    #: List of positional Parameters
-    _deferred_positionals: List[BasePositional] = ()     #: Positional Parameters that are deferred to sub commands
+    groups: list[ParamGroup]                             #: List of ParamGroup objects
+    positionals: list[BasePositional]                    #: List of positional Parameters
+    _deferred_positionals: list[BasePositional] = ()     #: Positional Parameters that are deferred to sub commands
     option_map: OptionMap                                #: Mapping of {--opt / -opt: Parameter}
+    # fmt: on
 
     def __init__(
         self,
         command: CommandCls,
         command_parent: Optional[CommandCls],
         parent_params: Optional[CommandParameters],
         config: CommandConfig,
@@ -79,23 +81,23 @@
     @property
     def has_nested_pass_thru(self) -> bool:
         return any(params._pass_thru for params in self._iter_nested_params())
 
     # endregion
 
     @cached_property
-    def all_positionals(self) -> List[BasePositional]:
+    def all_positionals(self) -> list[BasePositional]:
         try:
             if not self.parent.sub_command:
                 return self.parent.all_positionals + self.positionals
         except AttributeError:
             pass
         return self.positionals
 
-    def get_positionals_to_parse(self, ctx: Context) -> List[BasePositional]:
+    def get_positionals_to_parse(self, ctx: Context) -> list[BasePositional]:
         if self.all_positionals:
             for i, param in enumerate(self.all_positionals):
                 if not ctx.num_provided(param):
                     return [p for p in self.all_positionals[i:]]
 
         return []
 
@@ -166,21 +168,21 @@
         if self.config.add_help and self.command_parent is not None and (not self.parent or not self.parent._has_help):
             options.append(help_action)
 
         self._process_positionals(positionals)
         self._process_options(options)
         self._process_groups(groups)
 
-    def _process_groups(self, groups: Set[ParamGroup]):
+    def _process_groups(self, groups: set[ParamGroup]):
         if self.parent:
             self.groups = sorted((*self.parent.groups, *groups)) if groups else self.parent.groups.copy()
         else:
             self.groups = sorted(groups) if groups else []
 
-    def _process_positionals(self, params: List[BasePositional]):
+    def _process_positionals(self, params: list[BasePositional]):
         unfollowable = action_or_sub_cmd = split_index = None
         if self.parent and (deferred := self.parent._deferred_positionals):
             params = deferred + params
 
         for i, param in enumerate(params):
             if unfollowable:
                 if 0 in unfollowable.nargs:
@@ -212,15 +214,15 @@
             if self.sub_command.has_local_choices:
                 self._deferred_positionals = params[split_index:]
             else:
                 params, self._deferred_positionals = params[:split_index], params[split_index:]
 
         self.positionals = params
 
-    def _process_options(self, params: List[BaseOption]):
+    def _process_options(self, params: list[BaseOption]):
         if parent := self.parent:
             option_map = parent.option_map.copy()
             combo_option_map = parent.combo_option_map.copy()
             self.options = parent.options + params
         else:
             option_map = {}
             combo_option_map = {}
@@ -294,25 +296,25 @@
         self.split_action_flags = action_flags[:n_before], action_flags[n_before:]
 
     # endregion
 
     # region Ambiguous Short Combo Handling
 
     @cached_property
-    def _classified_combo_options(self) -> Tuple[OptionMap, OptionMap]:
+    def _classified_combo_options(self) -> tuple[OptionMap, OptionMap]:
         multi_char_combos = {}
         items = self.combo_option_map.items()
         for combo, param in items:
             if len(combo) == 1:  # combo_option_map is sorted in reverse length order, so all following will be 1 char
                 return dict([(combo, param), *items]), multi_char_combos
             multi_char_combos[combo] = param
         return {}, multi_char_combos
 
     @cached_property
-    def _potentially_ambiguous_combo_opts(self) -> Dict[str, Tuple[BaseOption, OptionMap]]:
+    def _potentially_ambiguous_combo_opts(self) -> dict[str, tuple[BaseOption, OptionMap]]:
         return _find_ambiguous_combos(*self._classified_combo_options)
 
     @cached_property
     def _nested_potentially_ambiguous_combo_options(self):
         single_char_combos, multi_char_combos = (xcc.copy() for xcc in self._classified_combo_options)
         for params in self._iter_nested_params():
             nested_single_char_combos, nested_multi_char_combos = params._classified_combo_options
@@ -353,15 +355,15 @@
                 yield params
                 yield from params._iter_nested_params()
 
     # region Option Processing
 
     def short_option_to_param_value_pairs(
         self, option: str
-    ) -> Tuple[List[Tuple[str, BaseOption, Optional[str]]], bool]:
+    ) -> tuple[list[tuple[str, BaseOption, Optional[str]]], bool]:
         option, eq, value = option.partition('=')
         if eq:  # An `=` was present in the string
             # Note: if the option is not in this Command's option_map, the KeyError is handled by CommandParser
             return [(option, self.option_map[option], value)], True
         else:
             value = None
 
@@ -400,15 +402,15 @@
         yield from (p for p in self.options if p.required and not p.group)
         if self._pass_thru and self._pass_thru.required and not self._pass_thru.group:
             yield self._pass_thru
 
 
 def _find_ambiguous_combos(
     single_char_combos: OptionMap, multi_char_combos: OptionMap
-) -> Dict[str, Tuple[BaseOption, OptionMap]]:
+) -> dict[str, tuple[BaseOption, OptionMap]]:
     ambiguous_combo_options = {}
     for combo, param in multi_char_combos.items():
         if singles := {c: single_char_combos[c] for c in combo if c in single_char_combos}:
             ambiguous_combo_options[combo] = (param, singles)
 
     return ambiguous_combo_options
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/commands.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 """
 
 from __future__ import annotations
 
 import logging
 from abc import ABC
 from contextlib import ExitStack
-from typing import TYPE_CHECKING, Type, Sequence, Optional, overload
+from typing import TYPE_CHECKING, Optional, Sequence, Type, overload
 
-from .core import CommandMeta, get_top_level_commands, get_params
-from .context import Context, ActionPhase, get_or_create_context
+from .context import ActionPhase, Context, get_or_create_context
+from .core import CommandMeta, get_params, get_top_level_commands
 from .exceptions import ParamConflict
 from .parser import parse_args_and_get_next_cmd
 from .utils import maybe_await
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandObj
 
@@ -50,20 +50,20 @@
         return f'<{cls.__name__} in prog={cls.__class__.meta(cls).prog!r}>'
 
     # region Parse & Run
 
     @classmethod
     @overload
     def parse_and_run(cls: Type[CommandObj], argv: Argv = None, **kwargs) -> Optional[CommandObj]:
-        ...  # These overloads indicate that an instance of the same type or another may be returned
+        # These overloads indicate that an instance of the same type or another may be returned
+        ...
 
     @classmethod
     @overload
-    def parse_and_run(cls, argv: Argv = None, **kwargs) -> Optional[CommandObj]:
-        ...
+    def parse_and_run(cls, argv: Argv = None, **kwargs) -> Optional[CommandObj]: ...
 
     @classmethod
     def parse_and_run(cls, argv=None, **kwargs):
         """
         Primary entry point for parsing arguments, resolving subcommands, and running a command.
 
         Calls :meth:`.parse` to parse arguments and resolve subcommands, then calls :meth:`.__call__` on the resulting
@@ -90,21 +90,19 @@
 
     # endregion
 
     # region Parse
 
     @classmethod
     @overload
-    def parse(cls: Type[CommandObj], argv: Argv = None) -> CommandObj:
-        ...
+    def parse(cls: Type[CommandObj], argv: Argv = None) -> CommandObj: ...
 
     @classmethod
     @overload
-    def parse(cls, argv: Argv = None) -> CommandObj:
-        ...
+    def parse(cls, argv: Argv = None) -> CommandObj: ...
 
     @classmethod
     def parse(cls, argv=None):
         """
         Parses the specified arguments (or :data:`sys.argv`), and resolves the final subcommand class based on the
         parsed arguments, if necessary.  Initializes the Command, but does not call any of its other methods.
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/compat.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 Contains stdlib CPython functions / classes from Python 3.8 and 3.10.
 
 The :class:`WCTextWrapper` in this module extends the stdlib :class:`python:textwrap.TextWrapper` to support wide
 characters.
 """
 
+from __future__ import annotations
+
 from textwrap import TextWrapper
-from typing import List
 
 from .utils import wcswidth
 
 __all__ = ['WCTextWrapper']
 
 # region textwrap
 
 
 class WCTextWrapper(TextWrapper):
     """
     Patches the ``_wrap_chunks`` method to use :func:`wcwidth:wcwidth.wcswidth` instead of :func:`python:len` (when the
     optional ``wcwidth`` dependency is available).  Minimal formatting changes are applied.  No logic has been changed.
     """
 
-    def _wrap_chunks(self, chunks: List[str]) -> List[str]:
+    def _wrap_chunks(self, chunks: list[str]) -> list[str]:
         """
         _wrap_chunks(chunks : [string]) -> [string]
 
         Wrap a sequence of text chunks and return a list of lines of length 'self.width' or less.  (If
         'break_long_words' is false, some lines may be longer than this.)  Chunks correspond roughly to words and the
         whitespace between them: each chunk is indivisible (modulo 'break_long_words'), but a line break can come
         between any two chunks.  Chunks should not have internal whitespace; ie. a chunk is either all whitespace or a
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/config.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from collections import ChainMap
 from enum import Enum
-from typing import TYPE_CHECKING, Optional, Any, Union, Callable, Type, TypeVar, Generic, overload, Dict
+from string import whitespace
+from typing import TYPE_CHECKING, Any, Callable, Generic, Optional, Sequence, Type, TypeVar, Union, overload
 
+from .exceptions import CommandDefinitionError
 from .utils import FixedFlag, MissingMixin, _NotSet, positive_int
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .error_handling import ErrorHandler
     from .formatting.commands import CommandHelpFormatter
     from .formatting.params import ParamHelpFormatter
-    from .typing import Bool, ParamOrGroup, CommandType
+    from .typing import Bool, CommandType, ParamOrGroup
 
 __all__ = [
     'CommandConfig',
     'ShowDefaults',
     'OptionNameMode',
     'SubcommandAliasHelpMode',
     'AmbiguousComboMode',
@@ -45,19 +47,21 @@
     If ``TRUTHY`` / ``NON_EMPTY`` / ``ANY`` are combined, then the most permissive (rightmost / highest value)
     option will be used.
 
     The ``MISSING`` option must be combined with one of ``TRUTHY`` / ``NON_EMPTY`` / ``ANY`` - using ``MISSING`` alone
     is equivalent to ``ShowDefaults.MISSING | ShowDefaults.NEVER``, which will result in no default values being shown.
     """
 
+    # fmt: off
     NEVER = 1       #: Never include the default value in help text
     MISSING = 2     #: Only include the default value if ``default:`` is not already present
     TRUTHY = 4      #: Only include the default value if it is treated as True in a boolean context
     NON_EMPTY = 8   #: Only include the default value if it is not ``None`` or an empty container
     ANY = 16        #: Any default value, regardless of truthiness, will be included
+    # fmt: on
 
     @classmethod
     def _missing_(cls, value: Union[str, int]) -> ShowDefaults:
         if isinstance(value, str):
             try:
                 return cls._member_map_[value.upper().replace('-', '_')]  # noqa
             except KeyError:
@@ -100,21 +104,23 @@
 
         - ``'_'`` or ``'-'`` or ``'*'`` or ``'*_'`` or ``'*-'`` or ``'_*'`` or ``'-*'`` or ``None``
         - ``OptionNameMode.UNDERSCORE`` or ``OptionNameMode.DASH`` or ``OptionNameMode.BOTH``
           or ``OptionNameMode.BOTH_UNDERSCORE`` or ``OptionNameMode.BOTH_DASH`` or ``OptionNameMode.NONE``
         - ``'underscore'`` or ``'dash'`` or ``'both'`` or ``'both_underscore'`` or ``'both_dash'`` or ``'none'``
     """
 
+    # fmt: off
     UNDERSCORE = 1
     DASH = 2
     BOTH = 3                # = 1|2
     #                         & 4  -> display options set
     BOTH_UNDERSCORE = 15    # & 8  -> show only underscore version
     BOTH_DASH = 23          # & 16 -> show only dash version
     NONE = 32
+    # fmt: on
 
     @classmethod
     def _missing_(cls, value: Union[str, int, None]) -> OptionNameMode:
         try:
             return OPT_NAME_MODE_ALIASES[value]
         except KeyError:
             pass
@@ -149,17 +155,19 @@
     :COMBINE: All of the aliases will be combined on the same line in the ``Subcommands:`` section, with the values
       displayed in a way that is similar to the way that the ``choices=`` values for other Parameters are displayed.
     :ALIAS: Each alias will be on a separate line in the ``Subcommands:`` section, but only the first choice/value will
       have the description (if defined for the target Command).  Subsequent aliases' descriptions will be replaced by
       ``Alias of: <first choice/alias value>``.
     """
 
+    # fmt: off
     REPEAT = 'repeat'       # Repeat the description as if it was a separate subcommand
     COMBINE = 'combine'     # Combine aliases onto a single line
     ALIAS = 'alias'         # Indicate the subcommand that it is an alias for; do not repeat the description
+    # fmt: on
 
 
 CmdAliasMode = Union[SubcommandAliasHelpMode, str]
 
 
 class AmbiguousComboMode(MissingMixin, Enum):
     """
@@ -172,34 +180,38 @@
     :PERMISSIVE: Allow multi-char short options that overlap with a single char one for exact matches, but reject any
       user input that combines multiple short options when the combination contains a sequence that could be
       interpreted as a multi-char short option.
     :STRICT: Reject multi-char short options that overlap with a single char one before parsing, regardless of user
       input.
     """
 
+    # fmt: off
     IGNORE = 'ignore'           # Ignore potentially ambiguous combinations of short options entirely
     PERMISSIVE = 'permissive'   # Allow multi-char short options that overlap with a single char one for exact matches
     STRICT = 'strict'           # Reject multi-char short options that overlap with a single char one before parsing
+    # fmt: on
 
 
 class AllowLeadingDash(Enum):
     """
     How a given Parameter should handle values with a leading dash (``-``).  Only configurable at the Parameter level,
     not the Command level.
 
     The behavior based on each supported option:
 
     :NUMERIC: Allow numeric values like ``-5`` and ``-1.3``, but reject values like ``-d``.
     :ALWAYS: Always allow values with a leading dash.
     :NEVER: Never allow values with a leading dash.
     """
 
+    # fmt: off
     NUMERIC = 'numeric'     # Allow a leading dash when the value is numeric
     ALWAYS = 'always'       # Always allow a leading dash
     NEVER = 'never'         # Never allow a leading dash
+    # fmt: on
 
     @classmethod
     def _missing_(cls, value):
         if isinstance(value, str):
             try:
                 return cls._member_map_[value.upper()]  # noqa
             except KeyError:
@@ -214,36 +226,42 @@
 # endregion
 
 
 # region Config Item Descriptors / Decorators
 
 
 class ConfigItem(Generic[CV, DV]):
+    """
+    A single configurable setting in the :class:`CommandConfig`.
+
+    :param default: Default config value to use if no explicit value is provided
+    :param type: A class or other callable that will be called to validate/normalize provided values
+    """
+
     __slots__ = ('default', 'type', 'name')
 
     def __init__(self, default: DV, type: Callable[..., CV] = None):  # noqa
         self.default = default
         self.type = type
 
     def __set_name__(self, owner: Type[CommandConfig], name: str):
         self.name = name
         owner.FIELDS.add(name)
 
     @overload
-    def __get__(self, instance: None, owner: Type[CommandConfig]) -> ConfigItem[CV, DV]:
-        ...
+    def __get__(self, instance: None, owner: Type[CommandConfig]) -> ConfigItem[CV, DV]: ...
 
     @overload
-    def __get__(self, instance: CommandConfig, owner: Type[CommandConfig]) -> ConfigValue:
-        ...
+    def __get__(self, instance: CommandConfig, owner: Type[CommandConfig]) -> ConfigValue: ...
 
     def __get__(self, instance, owner):
-        if instance is None:
+        try:
+            return instance._data.get(self.name, self.default)
+        except AttributeError:  # instance is None
             return self
-        return instance._data.get(self.name, self.default)
 
     def __set__(self, instance: CommandConfig, value: ConfigValue):
         if instance._read_only:
             raise AttributeError(f'Unable to set attribute {self.name}={value!r} because {instance} is read-only')
         elif self.type is not None:
             value = self.type(value)
         instance._data[self.name] = value
@@ -257,14 +275,16 @@
             raise AttributeError(f'No {self.name!r} config was stored for {instance}') from e
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.default!r}, type={self.type!r})>'
 
 
 class DynamicConfigItem(ConfigItem):
+    # A ConfigItem with a setter :paramref:`.ConfigItem.type` defined as a method in :class:`CommandConfig`.
+
     __slots__ = ('__doc__',)
 
     def __init__(self, default: DV, type: Callable[..., CV]):  # noqa
         super().__init__(default, type)
         self.__doc__ = type.__doc__
 
     def __set__(self, instance: CommandConfig, value: ConfigValue):
@@ -368,38 +388,68 @@
 
     #: Delimiter to use between choices in usage / help text
     choice_delim: str = ConfigItem('|', str)
 
     #: Whether there should be a visual indicator in help text for the parameters that are members of a given group
     show_group_tree: Bool = ConfigItem(False, bool)
 
+    @config_item(('\u00a6 ', '\u2551 ', '\u2502 '))
+    def group_tree_spacers(self, value: tuple[str, str, str] | Sequence[str]) -> tuple[str, str, str]:
+        """
+        The spacer characters to use at the beginning of each line when :attr:`.show_group_tree` is True.
+
+        The default spacers:
+
+        +--------------------+-----------+------------------------------+
+        | Parameter Type     | Character | Character Name               |
+        +====================+===========+==============================+
+        | Mutually Exclusive | \u00a6         | BROKEN BAR                   |
+        +--------------------+-----------+------------------------------+
+        | Mutually dependent | \u2551         | BOX DRAWINGS DOUBLE VERTICAL |
+        +--------------------+-----------+------------------------------+
+        | Other              | \u2502         | BOX DRAWINGS LIGHT VERTICAL  |
+        +--------------------+-----------+------------------------------+
+
+        :param value: A 3-tuple (or other sequence with 3 items) of spacer strings to be used for
+          (mutually exclusive, mutually dependent, other) group members, respectively.
+        :return: The validated and normalized value (or the default value if this property is accessed without
+          providing explicit values)
+        """
+        # Note: extra spaces in the docstring table are intentional - the escape sequences each collapse to one char
+        if isinstance(value, Sequence) and len(value) == 3 and all(isinstance(v, str) for v in value):
+            return tuple(f'{v} ' if v and v[-1] not in whitespace else v for v in value)  # noqa
+        raise CommandDefinitionError(
+            f'Invalid group_tree_spacers={value!r} - expected a 3-tuple of 2-character strings'
+        )
+
     #: Whether mutually exclusive / dependent groups should include that fact in their descriptions
     show_group_type: Bool = ConfigItem(True, bool)
 
     #: A callable that accepts 2 arguments, a :class:`.Command` class (not object) and a :class:`.CommandParameters`
     #: object, and returns a :class:`.CommandHelpFormatter`
     command_formatter: Callable[[CommandType, CommandParameters], CommandHelpFormatter] = ConfigItem(None)
 
     #: A callable that accepts a :class:`.Parameter` or :class:`.ParamGroup` and returns a :class:`.ParamHelpFormatter`
     param_formatter: Callable[[ParamOrGroup], ParamHelpFormatter] = ConfigItem(None)
 
     #: Whether the program version, author email, and documentation URL should be included in the help text epilog, if
     #: they were successfully detected
     extended_epilog: Bool = ConfigItem(True, bool)
 
-    #: Width (in characters) for the usage column in help text
+    #: Width (in characters) for the usage column in help text, after which the parameter descriptions begin.
     usage_column_width: int = ConfigItem(30, int)
 
-    #: Min width (in chars) for the usage column in help text after adjusting for group indentation / terminal width
-    min_usage_column_width: int = ConfigItem(20, int)
+    #: Whether the :attr:`.usage_column_width` should be enforced for parameters with usage text parts that exceed it.
+    #: By default, that setting only defines where the parameter descriptions begin.
+    strict_usage_column_width: bool = ConfigItem(False, bool)
 
     @config_item(False)
     def wrap_usage_str(self, value: Any) -> Union[int, bool]:
         """
-        Wrap the basic usage string after the specified number of characters, or automatically based on terminal size
+        Wrap the basic usage line after the specified number of characters, or automatically based on terminal size
         if ``True`` is specified instead.
         """
         if value is True or value is False:
             return value
         return positive_int(value, 'a bool or a positive integer', min_val=1)
 
     # endregion
@@ -428,15 +478,15 @@
                 bad = set(kwargs).difference(self.FIELDS)
                 raise TypeError(f'Invalid configuration - unsupported options: {", ".join(sorted(bad))}') from None
 
     def __repr__(self) -> str:
         settings = ', '.join(f'{k}={v!r}' for k, v in self.as_dict(False).items())
         return f'<{self.__class__.__name__}[depth={len(self._data.maps)}]({settings})>'
 
-    def as_dict(self, full: Bool = True) -> Dict[str, Any]:
+    def as_dict(self, full: Bool = True) -> dict[str, Any]:
         """Return a dict representing the configured options."""
         if full:
             return {key: getattr(self, key) for key in self.FIELDS}
         return {key: val for key, val in self._data.items() if key in self.FIELDS}
 
 
 DEFAULT_CONFIG: CommandConfig = CommandConfig(read_only=True)
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/context.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 
 import sys
 from collections import defaultdict
 from contextlib import AbstractContextManager
 from contextvars import ContextVar
 from enum import Enum
 from functools import cached_property
-from inspect import Signature, Parameter as _Parameter
-from typing import TYPE_CHECKING, Any, Callable, Union, Sequence, Optional, Iterator, Collection, cast
-from typing import Dict, Tuple, List
+from inspect import Parameter as _Parameter, Signature
+from typing import TYPE_CHECKING, Any, Callable, Collection, Iterator, Optional, Sequence, Union, cast
 
-from .config import CommandConfig, DEFAULT_CONFIG
+from .config import DEFAULT_CONFIG, CommandConfig
 from .error_handling import ErrorHandler, NullErrorHandler, extended_error_handler
 from .exceptions import NoActiveContext
-from .utils import _NotSet, Terminal
+from .utils import Terminal, _NotSet
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .commands import Command
-    from .parameters import Parameter, Option, ActionFlag
-    from .typing import Bool, ParamOrGroup, CommandType, CommandObj, AnyConfig, OptStr, StrSeq, PathLike  # noqa
+    from .parameters import ActionFlag, Option, Parameter
+    from .typing import AnyConfig, Bool, CommandObj, CommandType, OptStr, ParamOrGroup, PathLike, StrSeq  # noqa
 
 __all__ = ['Context', 'ctx', 'get_current_context', 'get_or_create_context', 'get_context', 'get_parsed', 'get_raw_arg']
 
 _context_stack = ContextVar('cli_command_parser.context.stack')
 _TERMINAL = Terminal()
 
 Argv = Optional['StrSeq']
@@ -45,15 +44,15 @@
     """
 
     config: CommandConfig
     prog: OptStr = None
     allow_argv_prog: Bool = True
     _command_obj: CommandObj = None
     _terminal_width: Optional[int]
-    _provided: Dict[ParamOrGroup, int]
+    _provided: dict[ParamOrGroup, int]
 
     def __init__(
         self,
         argv: Argv = None,
         command_cls: Optional[CommandType] = None,
         *,
         parent: Optional[Context] = None,
@@ -154,15 +153,15 @@
         self,
         command: Command = None,
         *,
         exclude: Collection[Parameter] = (),
         recursive: Bool = True,
         default: Any = None,
         include_defaults: Bool = True,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """
         Returns all of the parsed arguments as a dictionary.
 
         The :ref:`get_parsed() <advanced:Parsed Args as a Dictionary>` helper function provides an easier way to access
         this functionality.
 
         :param command: An initialized Command object for which arguments were already parsed.
@@ -243,28 +242,28 @@
         """
         self._provided[param] += val_count
 
     def num_provided(self, param: ParamOrGroup) -> int:
         """Not intended to be called by users.  Used by Parameters during parsing to handle nargs."""
         return self._provided[param]
 
-    def get_missing(self) -> List[Parameter]:
+    def get_missing(self) -> list[Parameter]:
         """Not intended to be called by users.  Used during parsing to determine if any Parameters are missing."""
         return [p for p in self.params.required_check_params() if not self._provided[p]]
 
     def missing_options_with_env_var(self) -> Iterator[Option]:
         """Yields Option parameters that have an environment variable configured, and did not have any CLI values."""
         yield from (p for p in self.params.options if p.env_var and not self._provided[p])
 
     # endregion
 
     # region Actions
 
     @cached_property
-    def _parsed_action_flags(self) -> Tuple[int, List[ActionFlag], List[ActionFlag]]:
+    def _parsed_action_flags(self) -> tuple[int, list[ActionFlag], list[ActionFlag]]:
         """
         Not intended to be accessed by users.  Returns a tuple containing the total number of action flags provided, the
         action flags to run before main, and the action flags to run after main.
         """
         try:
             before_main, after_main = self.params.split_action_flags  # Each part is already sorted
         except AttributeError:  # self.command_cls is None
@@ -277,21 +276,21 @@
 
     @property
     def action_flag_count(self) -> int:
         """Not intended to be accessed by users.  Returns the count of parsed action flags."""
         return self._parsed_action_flags[0]
 
     @cached_property
-    def all_action_flags(self) -> List[ActionFlag]:
+    def all_action_flags(self) -> list[ActionFlag]:
         """Not intended to be accessed by users.  Returns all parsed action flags."""
         _, before_main, after_main = self._parsed_action_flags
         return before_main + after_main
 
     @cached_property
-    def categorized_action_flags(self) -> Dict[ActionPhase, Sequence[ActionFlag]]:
+    def categorized_action_flags(self) -> dict[ActionPhase, Sequence[ActionFlag]]:
         """
         Not intended to be accessed by users.  Returns a dict of parsed action flags, categorized by the
         :class:`ActionPhase` during which they will run.
         """
         _, before_main, after_main = self._parsed_action_flags
         init_actions, before_actions = [], []
         for flag in before_main:
@@ -317,15 +316,15 @@
             self.actions_taken += 1
             yield action_flag
 
     # endregion
 
 
 def _normalize_config(
-    config: AnyConfig, kwargs: Dict[str, Any], parent: Context | None, command: CommandType | None
+    config: AnyConfig, kwargs: dict[str, Any], parent: Context | None, command: CommandType | None
 ) -> CommandConfig:
     if config is not None:
         if kwargs:
             raise TypeError(f'Cannot combine {config=} with keyword config arguments={kwargs}')
         elif isinstance(config, CommandConfig):
             return config
         kwargs = config
@@ -465,15 +464,15 @@
         return command._Command__ctx  # noqa
     except AttributeError as e:
         raise TypeError('get_context only supports Command objects') from e
 
 
 def get_parsed(
     command: Command, to_call: Callable = None, default: Any = None, include_defaults: Bool = True
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """
     Provides a way to obtain all of the arguments that were parsed for the given Command as a dictionary.
 
     If the parsed arguments are intended to be used to call a particular function/method, or to initialize a particular
     class, then that callable can be provided as the ``to_call`` parameter to filter the parsed arguments to only the
     ones that would be accepted by it.  It will not be called by this function.
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
 
 import ast
 import logging
 import sys
 from argparse import ArgumentParser
 from ast import AST, Assign, Call, withitem
-from functools import partial, cached_property
-from inspect import Signature, BoundArguments
+from functools import cached_property, partial
+from inspect import BoundArguments, Signature
 from pathlib import Path
-from typing import TYPE_CHECKING, Union, Optional, Callable, Collection, TypeVar, Generic, Type, Iterator
-from typing import List, Tuple, Dict, Set
+from typing import TYPE_CHECKING, Callable, Collection, Generic, Iterator, Type, TypeVar, Union
 
 from .argparse_utils import ArgumentParser as _ArgumentParser, SubParsersAction as _SubParsersAction
 from .utils import get_name_repr, iter_module_parents, unparse
 
 if TYPE_CHECKING:
     from cli_command_parser.typing import PathLike
-    from .visitor import TrackedRefMap, TrackedRef
+
+    from .visitor import TrackedRef, TrackedRefMap
 
 __all__ = ['ParserArg', 'ArgGroup', 'MutuallyExclusiveGroup', 'AstArgumentParser', 'SubParser', 'Script']
 log = logging.getLogger(__name__)
 
 InitNode = Union[Call, Assign, withitem]
-OptCall = Optional[Call]
+OptCall = Union[Call, None]
 ParserCls = Type['AstArgumentParser']
 ParserObj = TypeVar('ParserObj', bound='AstArgumentParser')
 RepresentedCallable = TypeVar('RepresentedCallable', bound=Callable)
 AC = TypeVar('AC', bound='AstCallable')
 D = TypeVar('D')
 _NotSet = object()
 
 
 class Script:
     _parser_classes = {}
-    path: Optional[Path]
+    path: Union[Path, None]
 
     def __init__(self, src_text: str, smart_loop_handling: bool = True, path: PathLike = None):
         self.smart_loop_handling = smart_loop_handling
         self._parsers = []
         self.path = Path(path) if path else None
         self.src_text = src_text
         parse_args = (self.src_text, self.path.as_posix()) if self.path else (self.src_text,)
@@ -45,15 +45,15 @@
 
     def __repr__(self) -> str:
         parsers = len(self.parsers)
         location = f' @ {self.path.as_posix()}' if self.path else ''
         return f'<{self.__class__.__name__}[{parsers=}{location}]>'
 
     @property
-    def mod_cls_to_ast_cls_map(self) -> Dict[str, Dict[str, ParserCls]]:
+    def mod_cls_to_ast_cls_map(self) -> dict[str, dict[str, ParserCls]]:
         return self._parser_classes
 
     @classmethod
     def _register_parser(cls, module: str, name: str, ast_cls: ParserCls):
         # Identify package-level exports that may have been defined for a custom ArgumentParser subclass
         modules = [module, *(parent for parent in iter_module_parents(module) if name in vars(sys.modules[parent]))]
         for module in modules:
@@ -68,15 +68,15 @@
 
     def add_parser(self, ast_cls: ParserCls, node: InitNode, call: OptCall, tracked_refs: TrackedRefMap) -> ParserObj:
         parser = ast_cls(node, self, tracked_refs, call)
         self._parsers.append(parser)
         return parser
 
     @cached_property
-    def parsers(self) -> List[ParserObj]:
+    def parsers(self) -> list[ParserObj]:
         from .visitor import ScriptVisitor, TrackedRef  # noqa: F811
 
         track_refs = (TrackedRef('argparse.REMAINDER'), TrackedRef('argparse.SUPPRESS'))
         visitor = ScriptVisitor(self.smart_loop_handling, track_refs=track_refs)
         for module, name_cls_map in self.mod_cls_to_ast_cls_map.items():
             for name, ast_cls in name_cls_map.items():
                 visitor.track_callable(module, name, partial(self.add_parser, ast_cls))
@@ -93,15 +93,15 @@
 
     __slots__ = ('func',)
 
     def __init__(self, func):
         self.func = func
 
     def __set_name__(self, owner: Type[AstCallable], name: str):
-        if owner._add_visit_func(name):      # This check is only to enable a low-value unit test...
+        if owner._add_visit_func(name):  # This check is only to enable a low-value unit test...
             setattr(owner, name, self.func)  # There's no need to keep the descriptor - replace self with func
 
     def __get__(self, instance, owner):
         # This will never actually be called, but it makes PyCharm happy
         return self if instance is None else partial(self.func, instance)
 
 
@@ -158,15 +158,15 @@
         self.call_kwargs = call.keywords
         self._tracked_refs = tracked_refs
         self.parent = parent
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}[{self.init_call_repr()}]>'
 
-    def get_tracked_refs(self, module: str, name: str, default: D = _NotSet) -> Union[Set[str], D]:
+    def get_tracked_refs(self, module: str, name: str, default: D = _NotSet) -> Union[set[str], D]:
         for tracked_ref, refs in self._tracked_refs.items():
             if tracked_ref.module == module and tracked_ref.name == name:
                 return refs
         if default is not _NotSet:
             return default
         raise KeyError(f'No tracked ref found for {module}.{name}')
 
@@ -189,41 +189,41 @@
 
     @cached_property
     def _init_func_bound(self) -> BoundArguments:
         args = self.call_args if isinstance(self.represents, type) else ('self', *self.call_args)
         return self.signature.bind(*args, **{kw.arg: kw.value for kw in self.call_kwargs})
 
     @cached_property
-    def init_func_args(self) -> List[str]:
+    def init_func_args(self) -> list[str]:
         try:
             args = self._init_func_bound.args[1:]
         except (TypeError, AttributeError):  # No represents func
             args = self.call_args
         return [unparse(arg) for arg in args]
 
     @cached_property
-    def init_func_raw_kwargs(self) -> Dict[str, AST]:
+    def init_func_raw_kwargs(self) -> dict[str, AST]:
         try:
             kwargs = self._init_func_bound.arguments
         except (TypeError, AttributeError):  # No represents func
             return {kw.arg: kw.value for kw in self.call_kwargs}
         else:
             kwargs = kwargs.copy()
             kwargs.pop('self', None)
             if isinstance(kwargs.get('args'), tuple):
                 kwargs.pop('args')
             if isinstance(kwargs.get('kwargs'), dict):
                 kwargs.update(kwargs.pop('kwargs'))
             return kwargs
 
-    def _init_func_kwargs(self) -> Dict[str, str]:
+    def _init_func_kwargs(self) -> dict[str, str]:
         return {key: unparse(val) for key, val in self.init_func_raw_kwargs.items()}
 
     @cached_property
-    def init_func_kwargs(self) -> Dict[str, str]:
+    def init_func_kwargs(self) -> dict[str, str]:
         return self._init_func_kwargs()
 
     def init_call_repr(self) -> str:
         arg_str = ', '.join(self.init_func_args)
         if kw_str := ', '.join(f'{k}={v}' for k, v in self.init_func_kwargs.items()):
             arg_str = kw_str if not arg_str else (arg_str + ', ' + kw_str)
         return f'{self.init_func_name}({arg_str})'
@@ -240,16 +240,16 @@
 class ParserArg(AstCallable, represents=ArgumentParser.add_argument):
     parent: ArgCollection
 
 
 class ArgCollection(AstCallable):
     parent: ArgCollection | Script
     _children = ('args', 'groups')
-    args: List[ParserArg]
-    groups: List[ArgGroup]
+    args: list[ParserArg]
+    groups: list[ArgGroup]
     add_argument = AddVisitedChild(ParserArg, 'args')
 
     def __init_subclass__(cls, children: Collection[str] = (), **kwargs):
         super().__init_subclass__(**kwargs)
         if children:
             cls._children = (*cls._children, *children)
 
@@ -257,28 +257,28 @@
         super().__init__(node, parent, tracked_refs, call)
         self.args = []
         self.groups = []
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}: ``{self.init_call_repr()}``>'
 
-    def _add_child(self, cls: Type[AC], container: List[AC], node: InitNode, call: Call, refs: TrackedRefMap) -> AC:
+    def _add_child(self, cls: Type[AC], container: list[AC], node: InitNode, call: Call, refs: TrackedRefMap) -> AC:
         child = cls(node, self, refs, call)
         container.append(child)
         return child
 
     @visit_func
     def add_mutually_exclusive_group(self, node: InitNode, call: Call, tracked_refs: TrackedRefMap):
         return self._add_child(MutuallyExclusiveGroup, self.groups, node, call, tracked_refs)
 
     @visit_func
     def add_argument_group(self, node: InitNode, call: Call, tracked_refs: TrackedRefMap):
         return self._add_child(ArgGroup, self.groups, node, call, tracked_refs)
 
-    def grouped_children(self) -> Iterator[Tuple[Type[AC], List[AC]]]:
+    def grouped_children(self) -> Iterator[tuple[Type[AC], list[AC]]]:
         yield ParserArg, self.args
         yield ArgGroup, self.groups
 
     # region Output Methods
 
     def pprint(self, indent: int = 0):
         print(f'{" " * indent} + {self!r}:')
@@ -307,15 +307,15 @@
         sub_parser = self.parent._add_subparser(node, call, tracked_refs)
         sub_parser.sp_parent = self
         return sub_parser
 
 
 @Script.register_parser
 class AstArgumentParser(ArgCollection, represents=ArgumentParser, children=('sub_parsers',)):
-    sub_parsers: List[SubParser]
+    sub_parsers: list[SubParser]
     add_subparsers = AddVisitedChild(SubparsersAction, '_subparsers_actions')
 
     def __init__(self, node: InitNode, parent: AstCallable | Script, tracked_refs: TrackedRefMap, call: Call = None):
         super().__init__(node, parent, tracked_refs, call)
         self._subparsers_actions = []
         # Note: sub_parsers aren't included in grouped_children since they need different handling during conversion
         self.sub_parsers = []
@@ -329,14 +329,14 @@
         return self._add_child(sub_parser_cls or SubParser, self.sub_parsers, node, call, tracked_refs)
 
 
 class SubParser(AstArgumentParser, represents=_SubParsersAction.add_parser):
     sp_parent: SubparsersAction
 
     @cached_property
-    def init_func_kwargs(self) -> Dict[str, str]:
+    def init_func_kwargs(self) -> dict[str, str]:
         kwargs = self.sp_parent.init_func_kwargs.copy()
         kwargs.update(self._init_func_kwargs())
         return kwargs
 
 
 # endregion
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/cli.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/command_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 
 import keyword
 import logging
 from abc import ABC, abstractmethod
-from ast import literal_eval, Attribute, Name, GeneratorExp, Subscript, DictComp, ListComp, SetComp, Constant, Str
+from ast import Attribute, Constant, DictComp, GeneratorExp, ListComp, Name, SetComp, Str, Subscript, literal_eval
 from dataclasses import dataclass, fields
 from functools import cached_property
 from itertools import count
-from typing import TYPE_CHECKING, Union, Optional, Iterator, Iterable, Type, TypeVar, Generic, List, Tuple
+from typing import TYPE_CHECKING, Generic, Iterable, Iterator, Optional, Type, TypeVar, Union
 
 from cli_command_parser.nargs import Nargs
-from .argparse_ast import AC, ParserArg, ArgGroup, MutuallyExclusiveGroup, AstArgumentParser, Script
+
+from .argparse_ast import AC, ArgGroup, AstArgumentParser, MutuallyExclusiveGroup, ParserArg, Script
 from .utils import collection_contents, unparse
 
 if TYPE_CHECKING:
     from cli_command_parser.typing import OptStr
+
     from .argparse_ast import ArgCollection
 
 __all__ = ['convert_script']
 log = logging.getLogger(__name__)
 
 C = TypeVar('C', bound='Converter')
 
@@ -61,29 +63,29 @@
         raise TypeError(f'No Converter is registered for {ast_obj.__class__.__name__} objects')
 
     @classmethod
     def init_for_ast_callable(cls, ast_obj: AC, *args, **kwargs) -> Converter[AC]:
         return cls.for_ast_callable(ast_obj)(ast_obj, *args, **kwargs)
 
     @classmethod
-    def init_group(cls: Type[C], parent: CollectionConverter, ast_objs: List[AC]) -> ConverterGroup[C]:
+    def init_group(cls: Type[C], parent: CollectionConverter, ast_objs: list[AC]) -> ConverterGroup[C]:
         return ConverterGroup(parent, cls, [cls(ast_obj, parent) for ast_obj in ast_objs])
 
     def convert(self, indent: int = 0) -> str:
         return '\n'.join(self.format_lines(indent))
 
     @abstractmethod
     def format_lines(self, indent: int = 0) -> Iterator[str]:
         raise NotImplementedError
 
 
 class ConverterGroup(Generic[C]):
     __slots__ = ('parent', 'member_type', 'members')
 
-    def __init__(self, parent: CollectionConverter, member_type: Type[C], members: List[C]):
+    def __init__(self, parent: CollectionConverter, member_type: Type[C], members: list[C]):
         self.parent = parent
         self.member_type = member_type
         self.members = members
 
     def __len__(self) -> int:
         return len(self.members)
 
@@ -123,15 +125,15 @@
     _name_mode = None
 
     @cached_property
     def name_mode(self) -> str | None:
         return self._name_mode or (self.parent.name_mode if self.parent else None)
 
     @cached_property
-    def grouped_children(self) -> List[ConverterGroup[ParamConverter | GroupConverter | Converter]]:
+    def grouped_children(self) -> list[ConverterGroup[ParamConverter | GroupConverter | Converter]]:
         return [self.for_ast_callable(cg_cls).init_group(self, cg) for cg_cls, cg in self.ast_obj.grouped_children()]
 
     def descendant_args(self) -> Iterator[ParamConverter]:
         for child_group in self.grouped_children:
             if not child_group.members:
                 continue
             elif hasattr(child_group[0], 'descendant_args'):
@@ -169,15 +171,15 @@
         add_methods: bool = False,
     ):
         super().__init__(parser, parent)
         self.counter = count() if counter is None else counter
         self.add_methods = add_methods
 
     @cached_property
-    def sub_parser_converters(self) -> List[ParserConverter]:
+    def sub_parser_converters(self) -> list[ParserConverter]:
         cls, add_methods = self.__class__, self.add_methods
         return [cls(sub_parser, self, self.counter, add_methods=add_methods) for sub_parser in self.ast_obj.sub_parsers]
 
     def descendant_args(self) -> Iterator[ParamConverter]:
         yield from super().descendant_args()
         for sp_converter in self.sub_parser_converters:
             yield from sp_converter.descendant_args()
@@ -246,15 +248,15 @@
             return None
         name = literal_eval_or_none(self.ast_obj.init_func_kwargs.get('name'))
         if not name or not name[0].isalpha():
             return None
         return name.title().replace(' ', '').replace('_', '').replace('-', '')
 
     @cached_property
-    def _choices(self) -> Tuple[OptStr, OptStr]:
+    def _choices(self) -> tuple[OptStr, OptStr]:
         if not self.is_sub_parser:
             return None, None
         name = self.ast_obj.init_func_kwargs.get('name')
         aliases = self.ast_obj.init_func_raw_kwargs.get('aliases')
         if not aliases:
             if name and (not self._custom_name or '-' in name or ' ' in name):
                 return 'choice', name
@@ -335,15 +337,15 @@
         if self.is_positional and not other.is_positional:
             return True
         if self.is_pass_thru and not other.is_pass_thru:
             return False
         return self.num < other.num
 
     @classmethod
-    def init_group(cls, parent: CollectionConverter, args: List[ParserArg]) -> ParamConverterGroup:
+    def init_group(cls, parent: CollectionConverter, args: list[ParserArg]) -> ParamConverterGroup:
         return ParamConverterGroup(parent, cls, [cls(arg, parent, i) for i, arg in enumerate(args)])
 
     def format_lines(self, indent: int = 4) -> Iterator[str]:
         yield self.format(indent)
 
     def format(self, indent: int = 4) -> str:
         param_cls, args_obj = self.get_cls_and_kwargs()
@@ -387,15 +389,15 @@
             yield f'param_{next(self._counter)}'
 
     # endregion
 
     # region Arg Processing
 
     @cached_property
-    def cmd_option_strs(self) -> List[str]:
+    def cmd_option_strs(self) -> list[str]:
         if not self.is_option:
             return []
         long, short, plain = self._grouped_opt_strs
         return short if self.use_auto_long_opt_str else (long + short)
 
     @cached_property
     def use_auto_long_opt_str(self) -> bool:
@@ -403,15 +405,15 @@
             return False
         long, short, plain = self._grouped_opt_strs
         return len(long) == 1 and long[0][2:] == self._attr_name
 
     def get_pos_args(self) -> Iterable[str]:
         return (repr(arg) for arg in self.cmd_option_strs)
 
-    def get_cls_and_kwargs(self) -> Tuple[str, BaseArgs]:
+    def get_cls_and_kwargs(self) -> tuple[str, BaseArgs]:
         kwargs = self.ast_obj.init_func_kwargs.copy()
         if (help_arg := kwargs.get('help')) and help_arg in self.ast_obj.get_tracked_refs('argparse', 'SUPPRESS', ()):
             kwargs.update({'hide': 'True', 'help': None})
 
         if self.is_pass_thru:
             return 'PassThru', PassThruArgs.from_kwargs(**kwargs)
 
@@ -458,15 +460,15 @@
     def is_option(self) -> bool:
         long, short, plain = self._grouped_opt_strs
         return (long or short) and not plain
 
     # endregion
 
     @cached_property
-    def _grouped_opt_strs(self) -> Tuple[List[str], List[str], List[str]]:
+    def _grouped_opt_strs(self) -> tuple[list[str], list[str], list[str]]:
         option_strs = (literal_eval(opt) for opt in self.ast_obj.init_func_args)
         long, short, plain = [], [], []
         for opt in option_strs:
             if opt.startswith('--'):
                 long.append(opt)
             elif opt.startswith('-'):
                 short.append(opt)
@@ -512,15 +514,15 @@
 # region Arg Containers
 
 
 @dataclass
 class BaseArgs:
     help: OptStr = None
 
-    def _to_str(self, args: Tuple[str, ...], end_fields: List[str]) -> str:
+    def _to_str(self, args: tuple[str, ...], end_fields: list[str]) -> str:
         skip = set(end_fields)
         keys = [f.name for f in fields(self) if f.name not in skip] + end_fields
         kv_iter = ((key, getattr(self, key)) for key in keys)
         return ', '.join((*args, *(f'{key}={val}' for key, val in kv_iter if val is not None)))
 
     def to_str(self, *args: str) -> str:
         return self._to_str(args, ['help'])
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/conversion/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import logging
 import re
-from ast import NodeVisitor, AST, Assign, Call, For, Attribute, Name, Import, ImportFrom, expr
+from ast import AST, Assign, Attribute, Call, For, Import, ImportFrom, Name, NodeVisitor, expr
 from collections import ChainMap, defaultdict
 from functools import partial, wraps
-from typing import Iterator, Union, Callable, Collection, Tuple, List, Dict, Set
+from typing import TYPE_CHECKING, Callable, Collection, Iterator, Union
 
 from .argparse_ast import AstArgumentParser
 from .utils import get_name_repr
 
+if TYPE_CHECKING:
+    TrackedRefMap = dict['TrackedRef', set[str]]
+
 __all__ = ['ScriptVisitor', 'TrackedRef']
 log = logging.getLogger(__name__)
 
-TrackedRefMap = Dict['TrackedRef', Set[str]]
 _NoCall = object()
 
 
 def scoped(func):
     @wraps(func)
     def _scoped_method(self: ScriptVisitor, *args, **kwargs):
         self.scopes = self.scopes.new_child()
@@ -119,15 +121,15 @@
             else:
                 self._visit_for_elements(node, node.target.id, ele_names)
         else:
             self.generic_visit(node)
 
     visit_AsyncFor = visit_For
 
-    def _visit_for_smart(self, node: For, loop_var: str, ele_names: List[str]):
+    def _visit_for_smart(self, node: For, loop_var: str, ele_names: list[str]):
         log.debug(f'Attempting smart for loop visit for {loop_var=} in {ele_names=}')
         refs = [ref for ref in (self.scopes.get(name) for name in ele_names) if ref]
         # log.debug(f'  > Found {len(refs)=}, {len(ele_names)=}')
 
         if len(refs) == len(ele_names) and all(isinstance(ref, AstArgumentParser) for ref in refs):
             parents = set(ref.parent for ref in refs)
             log.debug(f'  > Found parents={len(parents)}')
@@ -137,15 +139,15 @@
                     self.scopes[loop_var] = parent
                     self.generic_visit(node)
                     return
 
         log.debug('Falling back to generic loop handling')
         self._visit_for_elements(node, loop_var, ele_names)
 
-    def _visit_for_elements(self, node: For, loop_var: str, ele_names: List[str]):
+    def _visit_for_elements(self, node: For, loop_var: str, ele_names: list[str]):
         visited_any = False
         for name in ele_names:
             if ref := self.scopes.get(name):
                 visited_any = True
                 self.scopes[loop_var] = ref
                 self.generic_visit(node)
 
@@ -214,12 +216,12 @@
     def __hash__(self) -> int:
         return hash(self.__class__) ^ hash(self.module) ^ hash(self.name)
 
     def __eq__(self, other: TrackedRef) -> bool:
         return self.name == other.name and self.module == other.module
 
 
-def imp_names(imp: Import | ImportFrom) -> Iterator[Tuple[str, str]]:
+def imp_names(imp: Import | ImportFrom) -> Iterator[tuple[str, str]]:
     for alias in imp.names:
         name = alias.name
         as_name = alias.asname or name
         yield name, as_name
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/core.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from abc import ABC, ABCMeta
-from typing import TYPE_CHECKING, Optional, Union, TypeVar, Callable, Iterable, Collection, Any, Mapping, Iterator
-from typing import Dict, Tuple, List
+from typing import TYPE_CHECKING, Any, Callable, Collection, Iterable, Iterator, Mapping, Optional, TypeVar, Union
 from warnings import warn
 from weakref import WeakSet
 
 from .command_parameters import CommandParameters
-from .config import CommandConfig, DEFAULT_CONFIG
+from .config import DEFAULT_CONFIG, CommandConfig
 from .exceptions import CommandDefinitionError
 from .metadata import ProgramMetadata
 
 if TYPE_CHECKING:
-    from .typing import Config, AnyConfig, CommandCls, CommandAny, OptStr
+    from .typing import AnyConfig, CommandAny, CommandCls, Config, OptStr
 
-__all__ = ['CommandMeta', 'get_parent', 'get_config', 'get_params', 'get_metadata', 'get_top_level_commands']
+    Bases = Union[tuple[type, ...], Iterable[type]]
+    Choices = Union[Mapping[str, Optional[str]], Collection[str]]
+    OptChoices = Optional[Choices]
+    T = TypeVar('T')
 
-Bases = Union[Tuple[type, ...], Iterable[type]]
-Choices = Union[Mapping[str, Optional[str]], Collection[str]]
-OptChoices = Optional[Choices]
-T = TypeVar('T')
+__all__ = ['CommandMeta', 'get_parent', 'get_config', 'get_params', 'get_metadata', 'get_top_level_commands']
 
 _NotSet = object()
 META_KEYS = {'prog', 'usage', 'description', 'epilog', 'doc_name'}
 
 
 class CommandMeta(ABCMeta, type):
     # noinspection PyUnresolvedReferences
@@ -65,28 +64,28 @@
     :param bool always_run_after_main: Whether :meth:`Command._after_main_` should always be called, even if an
       exception was raised in :meth:`Command.main`
     """
 
     _commands = WeakSet()
 
     @classmethod
-    def __prepare__(mcs, name: str, bases: Bases, **kwargs) -> Dict[str, Any]:
+    def __prepare__(mcs, name: str, bases: Bases, **kwargs) -> dict[str, Any]:
         """Called before ``__new__`` and before evaluating the contents of a class."""
         return {
             '_CommandMeta__params': None,  # Prevent commands from inheriting parent params
             '_CommandMeta__metadata': None,  # Prevent commands from inheriting parent metadata directly
             '_CommandMeta__parents': None,  # Prevent commands from inheriting parents directly
             '_is_subcommand_': False,
         }
 
     def __new__(
         mcs,
         name: str,
         bases: Bases,
-        namespace: Dict[str, Any],
+        namespace: dict[str, Any],
         *,
         choice: str = _NotSet,
         choices: Choices = None,
         help: str = None,  # noqa
         config: AnyConfig = None,
         **kwargs,
     ) -> CommandCls:
@@ -137,15 +136,15 @@
             if isinstance(base, mcs):
                 return meth(base)
         return None
 
     # region Config Methods
 
     @classmethod
-    def _prepare_config(mcs, bases: Bases, config: AnyConfig, kwargs: Dict[str, Any]) -> Config:
+    def _prepare_config(mcs, bases: Bases, config: AnyConfig, kwargs: dict[str, Any]) -> Config:
         if config is not None:
             if kwargs:
                 raise CommandDefinitionError(f'Cannot combine {config=} with keyword config arguments={kwargs}')
             elif isinstance(config, CommandConfig):
                 return config
             kwargs = config  # It was a dict
 
@@ -155,16 +154,16 @@
             return CommandConfig(parent=parent_config, **cfg_kwargs)
 
         return None
 
     @classmethod
     def config(mcs, cls: CommandAny, default: T = None) -> Union[CommandConfig, T]:
         try:
-            return cls.__config     # This attr is not overwritten for every subclass
-        except AttributeError:      # This means that the Command and all of its parents have no custom config
+            return cls.__config  # This attr is not overwritten for every subclass
+        except AttributeError:  # This means that the Command and all of its parents have no custom config
             return default
 
     # endregion
 
     # region Metaclass-Managed Command Attributes
 
     @classmethod
@@ -226,15 +225,15 @@
     try:
         return cmd_cls, type.mro(cmd_cls)[1:-1]  # 0 is always the class itself, -1 is always object
     except TypeError:  # a Command object was provided instead of a Command class
         cmd_cls = cmd_cls.__class__
         return cmd_cls, type.mro(cmd_cls)[1:-1]
 
 
-def _choice_items(choice: OptStr, choices: OptChoices) -> Iterator[Tuple[OptStr, OptStr]]:
+def _choice_items(choice: OptStr, choices: OptChoices) -> Iterator[tuple[OptStr, OptStr]]:
     if not choices:
         # Automatic use of the subcommand class name is handled by SubCommand.register_command when choice is None
         if choice is not None:  # Allow an explicit None to be used to prevent registration
             yield (None if choice is _NotSet else choice), None
     else:
         try:
             items = choices.items()
@@ -256,15 +255,15 @@
 
 get_parent = CommandMeta.parent
 get_config = CommandMeta.config
 get_metadata = CommandMeta.meta
 get_params = CommandMeta.params
 
 
-def get_top_level_commands() -> List[CommandCls]:
+def get_top_level_commands() -> list[CommandCls]:
     """
     Returns a list of Command subclasses that are inferred to be direct subclasses of :class:`~commands.Command`.
 
     This was implemented because ``Command.__subclasses__()`` does not release dead references to subclasses quickly
     enough for tests.
     """
     return [cmd for cmd in CommandMeta._commands if not cmd._is_subcommand_]
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/documentation.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 import logging
 import sys
 from abc import ABC
 from collections import defaultdict
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Mapping, Any, List, Dict
+from typing import TYPE_CHECKING, Any, Iterable, Mapping
 
 from .commands import Command
 from .context import Context
-from .core import CommandMeta, get_params, get_parent, get_metadata
-from .formatting.commands import get_formatter, NameFunc
+from .core import CommandMeta, get_metadata, get_params, get_parent
+from .formatting.commands import NameFunc, get_formatter
 from .formatting.restructured_text import MODULE_TEMPLATE, rst_header, rst_toc_tree
 
 if TYPE_CHECKING:
-    from .typing import Bool, PathLike, CommandCls, Strings
+    from .typing import Bool, CommandCls, PathLike, Strings
 
-    Commands = Dict[str, CommandCls]
+    Commands = dict[str, CommandCls]
 
 __all__ = ['render_script_rst', 'render_command_rst', 'load_commands', 'RstWriter']
 log = logging.getLogger(__name__)
 
 
 # region Render Script / Command RST
 
@@ -94,15 +94,15 @@
     if doc_str := module.__doc__:
         for command in commands.values():
             get_metadata(command).pkg_doc_str = doc_str
 
     return commands
 
 
-def filtered_commands(obj_map: Dict[str, Any], top_only: Bool = False, include_abc: Bool = False) -> Commands:
+def filtered_commands(obj_map: dict[str, Any], top_only: Bool = False, include_abc: Bool = False) -> Commands:
     commands = {key: val for key, val in obj_map.items() if not key.startswith('__') and _is_command(val, include_abc)}
     if top_only:
         commands = top_level_commands(commands)
 
     return commands
 
 
@@ -272,15 +272,15 @@
         *,
         name: str = None,
         header: str = None,
         index: Bool = True,
         empty: Bool = False,
         caption: str = None,
         max_depth: int = 4,
-    ) -> List[str]:
+    ) -> list[str]:
         """
         :param pkg_name: The name of the package to document
         :param pkg_path: The path to the package
         :param subdir: The output subdirectory for package contents
         :param name: The name to use for the index file
         :param header: Header text to use in the index (default is based on the package name)
         :param index: Whether the index file should be created
@@ -310,15 +310,15 @@
             content_subdir=index_subdir,
             caption=caption,
             subdir=subdir,
             max_depth=max_depth,
         )
         return contents
 
-    def _generate_code_rsts(self, pkg_name: str, pkg_path: Path, subdir: str = None, max_depth: int = 4) -> List[str]:
+    def _generate_code_rsts(self, pkg_name: str, pkg_path: Path, subdir: str = None, max_depth: int = 4) -> list[str]:
         contents = []
         for path in pkg_path.iterdir():
             if path.is_dir():
                 sub_pkg_name = f'{pkg_name}.{path.name}'
                 if self.document_package(sub_pkg_name, path, subdir, max_depth=max_depth):
                     contents.append(sub_pkg_name)
             elif path.is_file() and path.suffix == '.py' and not path.name.startswith('__'):
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/error_handling.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/error_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 """
 
 from __future__ import annotations
 
 import platform
 import sys
 from collections import ChainMap
-from typing import Type, Callable, Union, Optional, Iterator, Dict
+from typing import Callable, Iterator, Optional, Type, Union
 
 from .exceptions import CommandParserException
 
 __all__ = ['ErrorHandler', 'error_handler', 'extended_error_handler', 'no_exit_handler', 'NullErrorHandler']
 
 WINDOWS = platform.system().lower() == 'windows'
 HandlerFunc = Callable[[BaseException], Optional[bool]]
 
 
 class ErrorHandler:
     __slots__ = ('exc_handler_map',)
-    _exc_handler_map: Dict[Type[BaseException], Handler] = {}
-    exc_handler_map: Dict[Type[BaseException], Handler]
+    _exc_handler_map: dict[Type[BaseException], Handler] = {}
+    exc_handler_map: dict[Type[BaseException], Handler]
 
     def __init__(self):
         self.exc_handler_map = {}
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}[handlers={len(self.exc_handler_map)}]>'
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from functools import cached_property
 from textwrap import TextWrapper
-from typing import TYPE_CHECKING, Union, Type, Callable, Iterator, Iterable, Optional
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator, Optional, Type, Union
 
-from ..context import ctx, NoActiveContext
-from ..core import get_params, get_metadata
+from ..context import NoActiveContext, ctx
+from ..core import get_metadata, get_params
 from ..parameters.groups import ParamGroup
-from ..utils import camel_to_snake_case, _NotSet
+from ..utils import _NotSet, camel_to_snake_case
 from .restructured_text import RstTable, spaced_rst_header
-from .utils import combine_and_wrap
+from .utils import PartWrapper
 
 if TYPE_CHECKING:
-    from ..core import CommandMeta
     from ..command_parameters import CommandParameters
     from ..config import CommandConfig
+    from ..core import CommandMeta
     from ..metadata import ProgramMetadata
-    from ..parameters import Parameter, BasePositional, BaseOption, SubCommand, PassThru
-    from ..typing import Bool, CommandType, CommandCls, CommandAny
+    from ..parameters import BaseOption, BasePositional, Parameter, PassThru, SubCommand
+    from ..typing import Bool, CommandAny, CommandCls, CommandType
 
 __all__ = ['CommandHelpFormatter', 'get_formatter']
 
 NameFunc = Callable[[str], str]
 
 
 class CommandHelpFormatter:
@@ -65,15 +65,18 @@
     def maybe_add_options(self, params: Iterable[BaseOption]):
         for param in params:
             self.maybe_add_option(param)
 
     def _iter_params(self) -> Iterator[Union[BasePositional, BaseOption, PassThru]]:
         params = self.params
         yield from params.all_positionals
+        # TODO: Add configurable option to reduce usage line noise, so something like [options] is displayed instead of
+        #  every option+metavar, while positionals are retained?
         yield from params.options
+        # TODO: Should groups be respected for the usage line?
         if params.pass_thru is not None:
             yield params.pass_thru
 
     def _usage_parts(self, sub_cmd_choice: str = None, allow_sys_argv: Bool = True) -> Iterator[str]:
         yield 'usage:'
         yield self._meta.get_prog(allow_sys_argv)
         if sub_cmd_choice:
@@ -96,15 +99,15 @@
         if usage := self._meta.usage:
             if wrap_usage_str:
                 return '\n'.join(TextWrapper(width=wrap_usage_str, subsequent_indent=' ' * cont_indent).wrap(usage))
             return usage
 
         parts = self._usage_parts(sub_cmd_choice, allow_sys_argv)
         if wrap_usage_str:
-            return '\n'.join(combine_and_wrap(parts, wrap_usage_str, cont_indent, delim))
+            return PartWrapper(wrap_usage_str, cont_indent, delim).join('', parts)
         return delim.join(parts)
 
     def format_help(self, allow_sys_argv: Bool = True) -> str:
         parts = [self.format_usage(allow_sys_argv=allow_sys_argv), '']
         if description := self._meta.description:
             parts += [description, '']
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 :author: Doug Skrypa
 """
 # pylint: disable=W0613
 
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Type, Callable, Iterator, Iterable, Tuple, Dict
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator, Type
 
-from ..config import SubcommandAliasHelpMode, CmdAliasMode
+from ..config import CmdAliasMode, SubcommandAliasHelpMode
 from ..context import ctx
 from ..core import get_config
-from ..parameters.base import BasePositional, BaseOption
-from ..parameters.choice_map import ChoiceMap, Choice
 from ..parameters import ParamGroup, PassThru, TriFlag
+from ..parameters.base import BaseOption, BasePositional
+from ..parameters.choice_map import Choice, ChoiceMap
 from .restructured_text import RstTable
-from .utils import format_help_entry, _should_add_default
+from .utils import _should_add_default, format_help_entry
 
 if TYPE_CHECKING:
     from ..nargs import Nargs
     from ..parameters.option_strings import TriFlagOptionStrings
-    from ..typing import Bool, ParamOrGroup, OptStr
+    from ..typing import Bool, OptStr, ParamOrGroup
 
-BoolFormatterMap = Dict[bool, Callable[[str], str]]
+    BoolFormatterMap = dict[bool, Callable[[str], str]]
 
 
 class ParamHelpFormatter:
     __slots__ = ('param',)
     _param_cls_fmt_cls_map = {}
     required_formatter_map: BoolFormatterMap = {False: '[{}]'.format}
 
@@ -70,15 +70,15 @@
         param = self.param
         if param.metavar and param.action.accepts_values:
             return param.metavar
 
         config = ctx.config
         if (t := param.type) is not None:
             try:
-                metavar = t.format_metavar(config.choice_delim, config.sort_choices)
+                metavar = t.format_metavar(config.choice_delim, config.sort_choices)  # noqa
             except Exception:  # noqa  # pylint: disable=W0703
                 pass
             else:
                 if metavar is not NotImplemented:
                     return metavar
 
         if config.use_type_metavar and t is not None:
@@ -110,42 +110,41 @@
         return self.maybe_wrap_usage(self.format_usage(True))
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         """Format the Parameter for use in both the ``usage:`` line and in the list of Parameters"""
         return self.format_metavar()
 
     def iter_usage_parts(self, include_meta: Bool = False, full: Bool = False) -> Iterator[str]:
+        """Format the Parameter for use in the list of Parameters with their ``help='...'`` descriptions"""
         yield self.format_usage(include_meta=include_meta, full=full)
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         param = self.param
         if description is None:
             description = param.help or ''
         if _should_add_default(param.default, description, param.show_default):
             pad, quote = _pad_and_quote(description, rst)
             description += f'{pad}(default: {quote}{param.default!r}{quote})'
 
         return description
 
-    def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
+    def format_help(self, prefix: str = '') -> str:
         usage_iter = self.iter_usage_parts(include_meta=True, full=True)
-        description = self.format_description()
-        return format_help_entry(usage_iter, description, prefix, tw_offset)
+        return format_help_entry(usage_iter, self.format_description(), prefix)
 
     # region RST
 
     def rst_usage(self) -> str:
-        usage = self.format_usage(include_meta=True, full=True)
-        return f'``{usage}``'
+        return '``' + self.format_usage(include_meta=True, full=True) + '``'
 
-    def rst_row(self) -> Tuple[str, str]:
+    def rst_row(self) -> tuple[str, str]:
         """Returns a tuple of (usage, description)"""
         return self.rst_usage(), self.format_description(rst=True)
 
-    def rst_rows(self) -> Iterator[Tuple[str, str]]:
+    def rst_rows(self) -> Iterator[tuple[str, str]]:
         yield self.rst_row()
 
     # endregion
 
 
 class PositionalHelpFormatter(ParamHelpFormatter, param_cls=BasePositional):
     param: BasePositional
@@ -155,17 +154,20 @@
 
 
 class OptionHelpFormatter(ParamHelpFormatter, param_cls=BaseOption):
     param: BaseOption
 
     def iter_usage_parts(self, include_meta: Bool = False, full: Bool = False) -> Iterator[str]:
         opts = self.param.option_strs
-        if self.param.nargs == 0:
+        if self.param.nargs == 0:  # It's a flag, so no metavar to represent a value
             yield from opts.option_strs()
         else:
+            # TODO: Config option for short before long?
+            # TODO: Config option to combine as `-f, --foo METAVAR` or `--foo, -f METAVAR` instead of repeating the
+            #  metavar as `--foo METAVAR, -f METAVAR`
             metavar = self._format_usage_metavar()
             yield from (f'{opt} {metavar}' for opt in opts.option_strs())
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         description = super().format_description(rst, description)
         param: BaseOption = self.param
         if param.env_var and (param.show_env_var or (param.show_env_var is None and ctx.config.show_env_vars)):
@@ -191,35 +193,33 @@
         return ', '.join(f'``{part}``' for part in self.iter_usage_parts())
 
 
 class TriFlagHelpFormatter(OptionHelpFormatter, param_cls=TriFlag):
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         opts: TriFlagOptionStrings = self.param.option_strs
         if full:
-            primary = delim.join(opts.primary_option_strs())
-            alts = delim.join(opts.alt_option_strs())
-            return f'{primary} | {alts}'
+            return f'{delim.join(opts.primary_option_strs())} | {delim.join(opts.alt_option_strs())}'
         else:
             return f'{opts.get_usage_opt(False)} | {opts.get_usage_opt(True)}'
 
     def format_description(self, rst: Bool = False, alt: bool = False) -> str:
         if not alt:
             return super().format_description(rst=rst)
         elif self.param.alt_help:
             return super().format_description(rst=rst, description=self.param.alt_help)
         return ''
 
-    def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
+    def format_help(self, prefix: str = '') -> str:
         opts: TriFlagOptionStrings = self.param.option_strs
-        primary = format_help_entry(opts.primary_option_strs(), self.format_description(), prefix, tw_offset)
+        primary = format_help_entry(opts.primary_option_strs(), self.format_description(), prefix)
         alt_desc = self.format_description(alt=True)
-        alt_entry = format_help_entry(opts.alt_option_strs(), alt_desc, prefix, tw_offset, lpad=2 if alt_desc else 4)
+        alt_entry = format_help_entry(opts.alt_option_strs(), alt_desc, prefix, lpad=2 if alt_desc else 4)
         return f'{primary}\n{alt_entry}'
 
-    def rst_rows(self) -> Iterator[Tuple[str, str]]:
+    def rst_rows(self) -> Iterator[tuple[str, str]]:
         opts: TriFlagOptionStrings = self.param.option_strs
         for alt in (False, True):
             usage = ', '.join(f'``{part}``' for part in opts.option_strs(alt))
             yield usage, self.format_description(rst=True, alt=alt)
 
 
 class ChoiceMapHelpFormatter(ParamHelpFormatter, param_cls=ChoiceMap):
@@ -235,55 +235,54 @@
             choices = (str(c) for c in (c.choice for cg in self.choice_groups for c in cg.choices) if c is not None)
             if config.sort_choices:
                 choices = sorted(choices)
             return f'{{{config.choice_delim.join(choices)}}}'
         else:
             return self.param.metavar or self.param.name.upper()
 
-    def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
-        return self.format_metavar()
-
-    def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
-        help_entry = format_help_entry(self.iter_usage_parts(), self.param.description, prefix, tw_offset, lpad=2)
-        choices = self._format_choices(prefix, tw_offset)
+    def format_help(self, prefix: str = '') -> str:
+        help_entry = format_help_entry(self.iter_usage_parts(), self.param.description, prefix, lpad=2)
+        choices = self._format_choices(prefix)
         if ctx.config.sort_choices:
             choices = sorted(choices)
 
         parts = (
             f'{prefix}{self.param.title or self.param._default_title}:',
             help_entry,
             *choices,
             prefix.rstrip(),
         )
         return '\n'.join(parts)
 
-    def _format_choices(self, prefix: str = '', tw_offset: int = 0) -> Iterator[str]:
+    def _format_choices(self, prefix: str = '') -> Iterator[str]:
         mode = ctx.config.cmd_alias_mode or SubcommandAliasHelpMode.ALIAS
         for choice_group in self.choice_groups:
-            yield from choice_group.format(mode, tw_offset, prefix)
+            yield from choice_group.format(mode, prefix)
 
     def rst_table(self) -> RstTable:
         rows = self._format_rst_rows()
         if ctx.config.sort_choices:
             rows = sorted(rows)
 
         table = RstTable(self.param.title or self.param._default_title, self.param.description)
         table.add_rows(rows)
         return table
 
-    def _format_rst_rows(self) -> Iterator[Tuple[str, OptStr]]:
+    def _format_rst_rows(self) -> Iterator[tuple[str, OptStr]]:
         mode = ctx.config.cmd_alias_mode or SubcommandAliasHelpMode.ALIAS
         for choice_group in self.choice_groups:
             for choice, usage, description in choice_group.prepare(mode):
                 yield f'``{usage}``', description
 
 
 class ChoiceGroup:
     """
-    A group of :class:`.Choice` objects from a given :class:`~.choice_map.ChoiceMap` that point to the same target.
+    A group of :class:`.Choice` objects from a given :class:`~.choice_map.ChoiceMap`, representing the positional
+    argument values that may be provided, that point to the same target.
+
     The first discovered Choice for a given target is considered the canonical one.  Subsequent Choices for that target
     are considered aliases.
 
     Used for formatting help text based on the configured :attr:`.CommandConfig.cmd_alias_mode`.
     """
 
     __slots__ = ('choice_strs', 'choices')
@@ -312,26 +311,25 @@
         return target_choice_map.values()
 
     def add(self, choice: Choice):
         self.choices.append(choice)
         if choice.choice:
             self.choice_strs.append(choice.choice)
 
-    def format(self, default_mode: CmdAliasMode, tw_offset: int = 0, prefix: str = '') -> Iterator[str]:
+    def format(self, default_mode: CmdAliasMode, prefix: str = '') -> Iterator[str]:
         """
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
           or the format string to use for subcommand aliases.
-        :param tw_offset: Terminal width offset for text width calculations.
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups).
         :return: Generator that yields formatted help text entries (strings) for the Choices in this group.
         """
         for choice, usage, description in self.prepare(default_mode):
-            yield format_help_entry((usage,), description, lpad=4, tw_offset=tw_offset, prefix=prefix)
+            yield format_help_entry((usage,), description, lpad=4, prefix=prefix)
 
-    def prepare(self, default_mode: CmdAliasMode) -> Iterator[Tuple[Choice, OptStr, OptStr]]:
+    def prepare(self, default_mode: CmdAliasMode) -> Iterator[tuple[Choice, OptStr, OptStr]]:
         """
         Prepares the choice values and descriptions to use for each Choice in this group based on the configured alias
         mode.
 
         :param default_mode: The default :class:`.SubcommandAliasHelpMode` to use if no mode was explicitly configured,
           or the format string to use for subcommand aliases.
         :return: Generator that yields 3-tuples containing the :class:`.Choice` object, the choice string value, and
@@ -350,15 +348,15 @@
         elif mode == SubcommandAliasHelpMode.REPEAT:
             yield from self.prepare_repeated()
         elif mode == SubcommandAliasHelpMode.COMBINE:
             yield self.prepare_combined()
         else:  # Treat as a format string
             yield from self.prepare_aliases(mode)
 
-    def prepare_combined(self) -> Tuple[Choice, OptStr, OptStr]:
+    def prepare_combined(self) -> tuple[Choice, OptStr, OptStr]:
         """
         Prepare this group's Choices for inclusion in help text / documentation by combining all aliases into a single
         entry.
         """
         first, choice_strs = self.choices[0], self.choice_strs
         try:
             usage, *additional = choice_strs
@@ -366,15 +364,15 @@
             return first, first.format_usage(), first.help
 
         if additional:
             usage = f'{{{"|".join(choice_strs)}}}'
 
         return first, usage, first.help
 
-    def prepare_aliases(self, format_str: str = 'Alias of: {choice}') -> Iterator[Tuple[Choice, OptStr, OptStr]]:
+    def prepare_aliases(self, format_str: str = 'Alias of: {choice}') -> Iterator[tuple[Choice, OptStr, OptStr]]:
         """
         Prepare this group's Choices for inclusion in help text / documentation using an alternate description for
         aliases.
 
         Variables supported in the :paramref:`.format_str`:
 
         - ``{choice}``: The first ("canonical") choice string for this group
@@ -398,15 +396,15 @@
             yield first, first.format_usage(), first.help
         else:
             help_str = first.help
             yield first, first_str, help_str
             for choice_str in choice_strs:
                 yield first, choice_str, format_str.format(choice=first_str, alias=choice_str, help=help_str)
 
-    def prepare_repeated(self) -> Iterator[Tuple[Choice, OptStr, OptStr]]:
+    def prepare_repeated(self) -> Iterator[tuple[Choice, OptStr, OptStr]]:
         """
         Prepare this group's Choices for inclusion in help text / documentation with no modifications.  Choices that
         are considered aliases are simply repeated as if they were not aliases.
         """
         for choice in self.choices:
             yield choice, choice.format_usage(), choice.help
 
@@ -424,14 +422,15 @@
             return ' + '
         elif self.param.mutually_exclusive:
             return ' | '
         else:
             return ', '
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
+        # This is currently (as of 2024-05-18) only used for error messages
         members = (mem.formatter.format_usage(include_meta, full, delim) for mem in self.param.members)
         return self.maybe_wrap_usage(self._get_choice_delim().join(members))
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         if description:
             return description
         group = self.param
@@ -443,49 +442,47 @@
         elif ctx.config.show_group_type and (group.mutually_exclusive or group.mutually_dependent):
             return f'Mutually {"exclusive" if group.mutually_exclusive else "dependent"} options'
 
         adjective = 'Required' if group.required else 'Other' if group.contains_required else 'Optional'
         return f'{adjective} arguments'
 
     def _get_spacer(self) -> str:
-        # TODO: Config option to set these chars OR to have them just be spaces
+        spacers = ctx.config.group_tree_spacers
         if self.param.mutually_exclusive:
-            return '\u00A6 '  # BROKEN BAR
+            return spacers[0]  # default: \u00a6 (BROKEN BAR)
         elif self.param.mutually_dependent:
-            return '\u2551 '  # BOX DRAWINGS DOUBLE VERTICAL
+            return spacers[1]  # default: \u2551 (BOX DRAWINGS DOUBLE VERTICAL)
         else:
-            return '\u2502 '  # BOX DRAWINGS LIGHT VERTICAL
+            return spacers[2]  # default: \u2502 (BOX DRAWINGS LIGHT VERTICAL)
 
-    def format_help(self, prefix: str = '', tw_offset: int = 0, clean: Bool = True) -> str:
+    def format_help(self, prefix: str = '', clean: Bool = True) -> str:
         """
         Prepare the help text for this group.
 
         :param prefix: Prefix to add to every line (primarily intended for use with nested groups)
-        :param tw_offset: Terminal width offset for text width calculations
         :param clean: If this group only contains other groups or Action or SubCommand parameters, then omit the
           description.
         :return: The formatted help text.
         """
         if ctx.config.show_group_tree:
             spacer = prefix + self._get_spacer()
-            tw_offset += 2
         else:
             spacer = prefix
 
         parts = [f'{prefix}{self.format_description()}:']
         nested = params = 0
         for member in self.param.members:
             if not member.show_in_help:
                 continue
             elif isinstance(member, (ChoiceMap, ParamGroup)):
                 nested += 1
                 parts.append(spacer.rstrip())  # Add space for readability
             else:
                 params += 1
-            parts.append(member.formatter.format_help(prefix=spacer, tw_offset=tw_offset))
+            parts.append(member.formatter.format_help(prefix=spacer))
 
         if clean and nested and not params:
             parts = parts[2:]  # remove description and the first spacer
 
         if not parts[-1].endswith('\n'):  # ensure a new line separates sections, but avoid extra lines
             parts.append(spacer.rstrip())
 
@@ -497,18 +494,17 @@
         for member in self.param.members:
             if member.show_in_help:
                 formatter = member.formatter
                 try:
                     sub_table: RstTable = formatter.rst_table()  # noqa
                 except AttributeError:
                     table.add_rows(formatter.rst_rows())
-                    # table.add_row(*formatter.rst_row())
                 else:
                     sub_table.show_title = False
                     table.add_row(sub_table.title, str(sub_table))
 
         return table
 
 
-def _pad_and_quote(description: str, rst: bool) -> Tuple[str, str]:
+def _pad_and_quote(description: str, rst: bool) -> tuple[str, str]:
     """Returns a 2-tuple of ``(pad char, quote string)``"""
     return ' ' if description else '', '``' if rst else ''
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from itertools import starmap
-from typing import TYPE_CHECKING, Union, Iterator, Iterable, Any, TypeVar, Sequence, Mapping, Dict, Tuple, List
+from typing import TYPE_CHECKING, Any, Iterable, Iterator, Mapping, Sequence, TypeVar, Union
 
 from .utils import line_iter
 
 if TYPE_CHECKING:
-    from ..typing import OptStr, Bool, Strings
+    from ..typing import Bool, OptStr, Strings
 
 __all__ = ['rst_bar', 'rst_list_table', 'RstTable']
 
 T = TypeVar('T')
 RowMaps = Sequence[Mapping[T, 'OptStr']]
 
 # region Constants & Templates
@@ -58,26 +58,26 @@
     if before:
         yield ''
     yield f'{text}\n{rst_bar(text, level)}'
     yield ''
 
 
 def _rst_directive(
-    directive: str, args: str = None, options: Dict[str, Any] = None, indent: int = 4, check: Bool = False
+    directive: str, args: str = None, options: dict[str, Any] = None, indent: int = 4, check: Bool = False
 ) -> Iterator[str]:
     yield f'.. {directive}:: {args}' if args else f'.. {directive}::'
     if options:
         pre = ' ' * indent
         for key, val in options.items():
             if not check or val is not None:
                 yield f'{pre}:{key}: {val}'
 
 
 def rst_directive(
-    directive: str, args: str = None, options: Dict[str, Any] = None, indent: int = 4, check: Bool = False
+    directive: str, args: str = None, options: dict[str, Any] = None, indent: int = 4, check: Bool = False
 ) -> str:
     return '\n'.join(_rst_directive(directive, args, options, indent, check))
 
 
 def _rst_toc_tree(name: str, content_fmt: str, contents: Strings, max_depth: int = 4, **kwargs) -> Iterator[str]:
     options = {'maxdepth': max_depth, **kwargs}
     yield rst_header(name, 1)
@@ -96,15 +96,15 @@
     :param max_depth: The maximum depth of the table of contents tree.  Use ``-1`` to allow unlimited depth.
     :param kwargs: Keyword arguments to be included as ``:key: <value>`` options to the ``toctree`` directive.
     :return: The RST header and table of contents directive as a string.
     """
     return '\n'.join(_rst_toc_tree(name, content_fmt, contents, max_depth, **kwargs))
 
 
-def rst_list_table(data: Dict[str, str], value_pad: int = 20) -> str:
+def rst_list_table(data: dict[str, str], value_pad: int = 20) -> str:
     max_key = max(map(len, data))
     max_val = max(map(len, data.values()))
     widths = f'{max_key} {max_val + value_pad}'
     entries = '\n'.join(f'    * - | {key}\n      - | {value}' for key, value in data.items())
     return LIST_TABLE_TMPL.format(widths=widths, entries=entries)
 
 
@@ -248,15 +248,15 @@
 
         yield ''
 
     def __str__(self) -> str:
         return '\n'.join(self.iter_build())
 
 
-def _widths(columns: Iterable[OptStr]) -> Tuple[bool, List[int]]:
+def _widths(columns: Iterable[OptStr]) -> tuple[bool, list[int]]:
     widths = []
     any_new_line = False
     for column in columns:
         if not column:
             widths.append(0)
         elif '\n' in column:
             any_new_line = True
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 
 from __future__ import annotations
 
 import os
 from abc import ABC
 from pathlib import Path as _Path
-from typing import Union, Optional
+from typing import Optional, Union
 
-from ..typing import Bool, T, PathLike, Converter
+from ..typing import Bool, Converter, PathLike, T
 from .base import InputType
 from .exceptions import InputValidationError
-from .utils import InputParam, StatMode, FileWrapper, allows_write, fix_windows_path
+from .utils import FileWrapper, InputParam, StatMode, allows_write, fix_windows_path
 
 __all__ = ['Path', 'File', 'Serialized', 'Json', 'Pickle']
 
 
 class FileInput(InputType[T], ABC):
     exists: bool = InputParam(None)
     expand: bool = InputParam(True)
@@ -197,15 +197,14 @@
     :param kwargs: Additional keyword arguments to pass to :class:`.File`
     """
 
     def __init__(self, *, mode: str = 'rb', **kwargs):
         import json
 
         # TODO: catch JSONDecodeError and provide a standardized cleaner error message (with a way to disable this error handling)
-        # TODO: Update docs to not suggest importing `inputs as i`
 
         write = allows_write(mode, True)
         kwargs['pass_file'] = write  # json.load just calls loads with f.read()
         super().__init__(json.dump if write else json.loads, mode=mode, **kwargs)
 
 
 class Pickle(Serialized):
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 :author: Doug Skrypa
 """
 # pylint: disable=W0622
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Union, Optional
+from typing import Optional, Union
 
-from ..typing import Bool, NT, Number, NumType, RngType
+from ..typing import NT, Bool, Number, NumType, RngType
 from .base import InputType
 from .exceptions import InputValidationError
 
 __all__ = ['Range', 'NumRange']
 
 _range = range
 
@@ -157,16 +157,16 @@
             if real_min >= real_max:
                 raise ValueError(
                     f'Invalid {min=} >= {max=} with snap=True, {include_min=},'
                     f' {include_max=} - snap would produce invalid values'
                 )
 
         self.snap = snap
-        self.min = self.type(min) if min is not None else min   # for floats especially, such as a range like 0~1, this
-        self.max = self.type(max) if max is not None else max   # helps to highlight the type in reprs
+        self.min = self.type(min) if min is not None else min  # for floats especially, such as a range like 0~1, this
+        self.max = self.type(max) if max is not None else max  # helps to highlight the type in reprs
         self.include_min = include_min
         self.include_max = include_max
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.type!r}, snap={self.snap!r})[{self._range_str()}]>'
 
     def _range_str(self, var: str = 'N') -> str:
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/patterns.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 from __future__ import annotations
 
 import os
 import re
 from abc import ABC
 from enum import Enum
 from fnmatch import translate
-from typing import TypeVar, Union, Collection, Sequence, Pattern, Match, Tuple, Dict
+from typing import Collection, Dict, Match, Pattern, Sequence, Tuple, TypeVar, Union
 
 from ..utils import MissingMixin
 from .base import InputType, T
 from .exceptions import InputValidationError
 
 __all__ = ['Regex', 'RegexMode', 'Glob']
 
 RegexResult = TypeVar('RegexResult', str, Match, Tuple[str, ...], Dict[str, str])
 
 
 class PatternInput(InputType[T], ABC):
     __slots__ = ('patterns',)
-    patterns: Tuple[Pattern, ...]
+    patterns: tuple[Pattern, ...]
 
     def _pattern_strings(self, sort: bool = False) -> Sequence[str]:
         patterns = [p.pattern for p in self.patterns]
         if sort:
             patterns.sort()
         return patterns
 
@@ -41,19 +41,21 @@
             return f'this pattern: {patterns[0]}'
         return 'any of the following patterns:\n' + '\n'.join(f'  - {p}' for p in patterns)
 
 
 class RegexMode(MissingMixin, Enum):
     """The RegexMode for a given Regex input governs the type of value it returns during parsing."""
 
+    # fmt: off
     STRING = 'string'   #: Return the full original string if it matches a given pattern
     MATCH = 'match'     #: Return a :ref:`Match <python:match-objects>` object
     GROUP = 'group'     #: Return the string from the specified capturing group
     GROUPS = 'groups'   #: Return a tuple containing all captured groups, or specific captured groups
     DICT = 'dict'       #: Return a dictionary containing all named capturing groups and their captured values
+    # fmt: on
 
     @classmethod
     def normalize(cls, value: Union[str, RegexMode, None], group, groups) -> RegexMode:
         if value is None:
             if group is not None:
                 return cls.GROUP
             elif groups:
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from calendar import day_name, day_abbr, month_name, month_abbr
-from datetime import datetime, date, time, timedelta
+from calendar import day_abbr, day_name, month_abbr, month_name
+from datetime import date, datetime, time, timedelta
 from enum import Enum
 from locale import LC_ALL, setlocale
 from threading import RLock
-from typing import Union, Iterator, Collection, Sequence, Optional, TypeVar, Type, Literal, overload
-from typing import Tuple, Dict
+from typing import Collection, Iterator, Literal, Optional, Sequence, Type, TypeVar, Union, overload
 
-from ..typing import T, Bool, Locale, TimeBound
+from ..typing import Bool, Locale, T, TimeBound
 from ..utils import MissingMixin
 from .base import InputType
 from .exceptions import InputValidationError, InvalidChoiceError
 
 __all__ = ['DTFormatMode', 'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time']
 
 DT = TypeVar('DT')
@@ -99,23 +98,25 @@
         return self(value)
 
 
 # region Calendar Unit Inputs
 
 
 class DTFormatMode(MissingMixin, Enum):
+    # fmt: off
     FULL = 'full'                   #: The full name of a given date/time unit
     ABBREVIATION = 'abbreviation'   #: The abbreviation of a given date/time unit
     NUMERIC = 'numeric'             #: The numeric representation of a given date/time unit
     NUMERIC_ISO = 'numeric_iso'     #: The ISO numeric representation of a given date/time unit
+    # fmt: on
 
 
 class CalendarUnitInput(DTInput[Union[str, int]], ABC):
     __slots__ = ('full', 'abbreviation', 'numeric', 'out_format', 'out_locale')
-    _formats: Dict[DTFormatMode, Sequence[Union[str, int]]]
+    _formats: dict[DTFormatMode, Sequence[Union[str, int]]]
     _min_index: int = 0
 
     def __init_subclass__(cls, min_index: int = 0, **kwargs):
         super().__init_subclass__(**kwargs)
         cls._min_index = min_index
 
     def __init__(
@@ -147,15 +148,15 @@
         self.abbreviation = abbreviation
         self.numeric = numeric
         self.out_format = DTFormatMode(out_format)
         self.out_locale = out_locale or self.locale
         if self.out_format not in self._formats:
             raise ValueError(f'Unsupported out_format={self.out_format} for {self.__class__.__name__} inputs')
 
-    def _values(self) -> Iterator[Tuple[int, str]]:
+    def _values(self) -> Iterator[tuple[int, str]]:
         if not self.full and not self.abbreviation:
             return
         min_index = self._min_index
         with different_locale(self.locale):
             if self.full:
                 yield from enumerate(self._formats[DTFormatMode.FULL][min_index:], min_index)
             if self.abbreviation:
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/metadata.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 """
 # pylint: disable=R0801
 
 from __future__ import annotations
 
 from collections import defaultdict
 from functools import cached_property
-from importlib.metadata import entry_points, EntryPoint, Distribution
+from importlib.metadata import Distribution, EntryPoint, entry_points
 from inspect import getmodule
 from pathlib import Path
 from sys import modules
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Type, Callable, Optional, Union, Iterator, Tuple, Dict, Set
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, Type, Union
 from urllib.parse import urlparse
 
-from .context import ctx, NoActiveContext
+from .context import NoActiveContext, ctx
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandType, OptStr
 
 __all__ = ['ProgramMetadata']
 
 DEFAULT_FILE_NAME: str = 'UNKNOWN'
@@ -54,15 +54,15 @@
     def __set__(self, instance: ProgramMetadata, value: Union[str, Path, None]):
         if value is not None:
             instance.__dict__[self.name] = value
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({", ".join(f"{a}={v}" for a, v in self._attrs())})'
 
-    def _attrs(self) -> Iterator[Tuple[str, Any]]:
+    def _attrs(self) -> Iterator[tuple[str, Any]]:
         for base in self.__class__.mro()[:-1]:
             for attr in base.__slots__:  # noqa
                 if attr != 'name':
                     value = getattr(self, attr)
                     yield attr, (getattr(value, '__qualname__', value) if attr == 'func' else repr(value))
 
     def get_parent(self, instance: ProgramMetadata) -> Optional[ProgramMetadata]:
@@ -182,33 +182,33 @@
 
     def __repr__(self) -> str:
         return _repr(self)
 
     # region Program Name Properties
 
     @cached_property
-    def _prog_and_src(self) -> Tuple[str, str]:
+    def _prog_and_src(self) -> tuple[str, str]:
         if prog := self.__dict__.get('prog'):
             return prog, 'class kwargs'
         return _prog_finder.normalize(self.path, self.parent, None, self.cmd_module, self.command)
 
     @dynamic_metadata
     def prog(self) -> str:
         return self._prog_and_src[0]
 
     @cached_property
-    def _doc_prog_and_src(self) -> Tuple[str, str]:
+    def _doc_prog_and_src(self) -> tuple[str, str]:
         if prog := self.__dict__.get('prog'):
             return prog, 'class kwargs'
         return _prog_finder.normalize(self.path, self.parent, False, self.cmd_module, self.command)
 
     def get_prog(self, allow_sys_argv: Bool = None) -> str:
         return self._get_prog(allow_sys_argv)[0]
 
-    def _get_prog(self, allow_sys_argv: Bool = None) -> Tuple[str, str]:
+    def _get_prog(self, allow_sys_argv: Bool = None) -> tuple[str, str]:
         return self._prog_and_src if allow_sys_argv or allow_sys_argv is None else self._doc_prog_and_src
 
     @dynamic_metadata(inheritable=False)
     def doc_name(self) -> str:
         # TODO: Bug: Explicitly provided value not used in rst page title sometimes?
         return Path(self._doc_prog_and_src[0]).stem
 
@@ -283,39 +283,39 @@
     indent_str = ' ' * indent
     fields_str = '\n'.join(f'{indent_str}{k}={_repr(v, indent)},' for k, v in field_dict.items())
     return f'<{obj.__class__.__name__}(\n{fields_str}\n{prev_str})>'
 
 
 class ProgFinder:
     @cached_property
-    def mod_obj_prog_map(self) -> Dict[str, Dict[str, str]]:
+    def mod_obj_prog_map(self) -> dict[str, dict[str, str]]:
         mod_obj_prog_map = defaultdict(dict)
         for entry_point in self._get_console_scripts():
             module, obj = map(str.strip, entry_point.value.split(':', 1))
             obj = obj.split('[', 1)[0].strip()  # Strip extras, if any
             mod_obj_prog_map[module][obj] = entry_point.name
 
         mod_obj_prog_map.default_factory = None  # Disable automatic defaults
         return mod_obj_prog_map
 
     @classmethod
-    def _get_console_scripts(cls) -> Tuple[EntryPoint, ...]:
+    def _get_console_scripts(cls) -> tuple[EntryPoint, ...]:
         try:
             return entry_points(group='console_scripts')  # noqa
         except TypeError:  # Python 3.8 or 3.9
             return entry_points()['console_scripts']  # noqa
 
     def normalize(
         self,
         cmd_path: Path,
         parent: Optional[ProgramMetadata],
         allow_sys_argv: Bool,
         cmd_module: str,
         cmd_name: str,
-    ) -> Tuple[OptStr, str]:
+    ) -> tuple[OptStr, str]:
         if ep_name := self._from_entry_point(cmd_module, cmd_name):
             return ep_name, 'entry_points'
 
         if allow_sys_argv is None:
             try:
                 allow_sys_argv = ctx.allow_argv_prog
             except NoActiveContext:
@@ -383,15 +383,15 @@
         self._dist_urls = {}
 
     @cached_property
     def _distributions(self) -> dict[str, Distribution]:
         # Note: Distribution.name was not added until 3.10, and it returns `self.metadata['Name']`
         return {dist.metadata['Name']: dist for dist in Distribution.discover()}
 
-    def _get_top_levels(self, dist_name: str, dist: Distribution) -> Set[str]:
+    def _get_top_levels(self, dist_name: str, dist: Distribution) -> set[str]:
         # dist_name = dist.metadata['Name']  # Distribution.name was not added until 3.10, and it returns this
         if (top_levels := self._dist_top_levels.get(dist_name)) is not None:
             return top_levels
         elif raw := dist.read_text('top_level.txt'):
             self._dist_top_levels[dist_name] = top_levels = {pkg for pkg in map(str.strip, raw.split()) if pkg}
             return top_levels
 
@@ -424,15 +424,15 @@
 
         # The package name may have a prefix like `lib` not included in top_level when interactive
         for part in module.__package__.split('.'):
             if (dist := self.dist_for_pkg(part)) is not None:
                 return dist
         return None
 
-    def get_urls(self, dist: Distribution) -> Dict[str, str]:
+    def get_urls(self, dist: Distribution) -> dict[str, str]:
         metadata = dist.metadata
         dist_name = metadata['Name']
         if (urls := self._dist_urls.get(dist_name)) is not None:
             return urls
 
         urls = {}
         for key, val in metadata.items():
@@ -444,15 +444,15 @@
         self._dist_urls[dist_name] = urls
         return urls
 
 
 _dist_finder = DistributionFinder()
 
 
-def _path_and_globals(command: CommandType, path: Path = None) -> Tuple[Path, Dict[str, Any]]:
+def _path_and_globals(command: CommandType, path: Path = None) -> tuple[Path, dict[str, Any]]:
     module = getmodule(command)  # Returns the module object (obj.__module__ just provides the name of the module)
     if path is None:
         try:
             path = Path(module.__file__).resolve()
         except AttributeError:  # module is None
             path = Path.cwd().joinpath(DEFAULT_FILE_NAME)
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/nargs.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/nargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Helpers for handling ``nargs=...`` for Parameters.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import Any, Union, Optional, Sequence, Collection, Iterable, Tuple, Set, FrozenSet
+from typing import Any, Collection, FrozenSet, Iterable, Optional, Sequence, Set, Tuple, Union
 
 __all__ = ['Nargs', 'NargsValue', 'REMAINDER', 'nargs_min_and_max_sums']
 
 REMAINDER = type('REMAINDER', (), {})()
 _UNBOUND = (None, REMAINDER)
 NARGS_STR_RANGES = {'?': (0, 1), '*': (0, None), '+': (1, None), 'REMAINDER': (0, REMAINDER)}
 SET_ERROR_FMT = 'Invalid nargs={!r} set - expected non-empty set where all values are integers >= 0'
@@ -175,15 +175,15 @@
         return self._has_upper_bound
 
     @property
     def upper_bound(self) -> Union[int, float]:
         return self.max if self._has_upper_bound else float('inf')
 
 
-def nargs_min_and_max_sums(nargs_objects: Iterable[Nargs]) -> Tuple[int, Union[int, float]]:
+def nargs_min_and_max_sums(nargs_objects: Iterable[Nargs]) -> tuple[int, Union[int, float]]:
     min_sum, max_sum = 0, 0
     iter_nargs = iter(nargs_objects)
     for obj in iter_nargs:
         min_sum += obj.min
         if obj._has_upper_bound:
             max_sum += obj.max
         else:
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/actions.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Parameter actions define how Parameters behave when processing values that were provided via CLI or environment
 variables.
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Iterator, Iterable, Callable, Union, Sequence, TypeVar, NoReturn, List
+from typing import TYPE_CHECKING, Callable, Iterable, Iterator, NoReturn, Sequence, TypeVar, Union
 
 from ..context import ctx
-from ..exceptions import BadArgument, MissingArgument, InvalidChoice, TooManyArguments, ParamUsageError, ParamConflict
+from ..exceptions import BadArgument, InvalidChoice, MissingArgument, ParamConflict, ParamUsageError, TooManyArguments
 from ..inputs import InputType
 from ..nargs import Nargs
 from ..utils import _NotSet, camel_to_snake_case
 
 if TYPE_CHECKING:
-    from ..typing import CommandObj, Param, Bool, T_co
+    from ..typing import Bool, CommandObj, Param, T_co
 
 __all__ = [
     'ParamAction',
     'Store',
     'Append',
     'StoreConst',
     'AppendConst',
@@ -119,15 +119,15 @@
     #         validate(value)
     #         yield value
 
     # endregion
 
     # region Backtracking
 
-    def get_maybe_poppable_counts(self) -> List[int]:
+    def get_maybe_poppable_counts(self) -> list[int]:
         """
         :return: The indexes on which the parsed values may be split such that the remaining number of values will
           still be acceptable for the Parameter's nargs.
         """
         return []
 
     def can_reset(self) -> bool:
@@ -314,15 +314,15 @@
             return False
         return super().would_accept(value, combo)
 
     # endregion
 
     # region Backtracking
 
-    def get_maybe_poppable_counts(self) -> List[int]:
+    def get_maybe_poppable_counts(self) -> list[int]:
         """
         :return: The indexes on which the parsed values may be split such that the remaining number of values will
           still be acceptable for the Parameter's nargs.
         """
         if not self.param.nargs.variable or self.param.type not in (None, str):
             return []
         elif (values := ctx.get_parsed_value(self.param)) is not _NotSet:
@@ -521,15 +521,15 @@
 
 class StoreAll(Store):
     __slots__ = ()
     default_nargs = Nargs('REMAINDER')
 
     # region Add Parsed Value / Constant Methods
 
-    def add_values(self, values: List[str], *, opt: str = None, combo: bool = False) -> Found:
+    def add_values(self, values: list[str], *, opt: str = None, combo: bool = False) -> Found:
         param = self.param
         ctx.record_action(param)
 
         if (value := ctx.get_parsed_value(param)) is not _NotSet:
             raise ParamUsageError(
                 param, f'can only be specified once - found {values=} but a stored {value=} already exists'
             )
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """
 Base classes and helpers for Parameters and Groups
 
 :author: Doug Skrypa
 """
-# pylint: disable=R0801
 
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from contextvars import ContextVar
 from functools import cached_property
 from itertools import chain
-from typing import TYPE_CHECKING, Any, Type, Generic, Optional, Callable, Collection, Union, Iterator, TypeVar, overload
-from typing import NoReturn, Dict, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Collection, Generic, Iterator, NoReturn, Type, TypeVar, Union, overload
 
 from ..annotations import get_descriptor_value_type
-from ..config import CommandConfig, OptionNameMode, AllowLeadingDash, DEFAULT_CONFIG
+from ..config import DEFAULT_CONFIG, AllowLeadingDash, CommandConfig, OptionNameMode
 from ..context import Context, ctx, get_current_context
-from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice
+from ..exceptions import BadArgument, InvalidChoice, MissingArgument, ParameterDefinitionError
 from ..inputs import InputType, normalize_input_type
 from ..inputs.choices import _ChoicesBase
 from ..inputs.exceptions import InputValidationError, InvalidChoiceError
-from ..nargs import Nargs, REMAINDER
-from ..typing import T_co, DefaultFunc, CommandMethod
+from ..nargs import REMAINDER, Nargs
+from ..typing import CommandMethod, DefaultFunc, T_co
 from ..utils import _NotSet
 from .option_strings import OptionStrings
 
 if TYPE_CHECKING:
     from ..formatting.params import ParamHelpFormatter
-    from ..typing import OptStr, OptStrs, Strings, Bool, CommandCls, CommandObj, CommandAny, Param, LeadingDash
+    from ..typing import Bool, CommandAny, CommandCls, CommandObj, LeadingDash, OptStr, OptStrs, Param, Strings
     from .actions import ParamAction
     from .groups import ParamGroup
 
 __all__ = ['Parameter', 'BasePositional', 'BaseOption']
 
 _group_stack = ContextVar('cli_command_parser.parameters.base.group_stack')
 _is_numeric = re.compile(r'^-\d+$|^-\d*\.\d+?$').match
@@ -47,24 +45,26 @@
     :param name: The name to use for this parameter.  Defaults to the name assigned to this parameter.
     :param required: Whether this parameter is required or not.  If it is required, then an exception will be
       raised if the user did not provide a value for this parameter.  Defaults to ``False``.
     :param help: A brief description of this parameter that will appear in ``--help`` text.
     :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
     """
 
+    # fmt: off
     # Class Attributes
     missing_hint: str = None        #: Hint to provide if this param/group is missing
     # Instance Attributes
     _attr_name: str = None          #: Always the name of the attr that points to this object
     _name: str = None               #: An explicitly provided name, or the name of the attr that points to this object
     group: ParamGroup = None        #: The group this object is a member of, if any
     command: CommandCls = None      #: The :class:`.Command` this object is a member of
     required: Bool                  #: Whether this param/group is required
     help: str                       #: The description for this param/group that will appear in ``--help`` text
     hide: Bool                      #: Whether this param/group should be hidden in ``--help`` text
+    # fmt: on
 
     def __init__(self, name: str = None, required: Bool = False, help: str = None, hide: Bool = False):  # noqa
         self.__doc__ = help  # Prevent this class's docstring from showing up for params in generated documentation
         self.required = required
         self.help = help
         self.hide = hide
         # TODO: Make the --help flag a counter and allow some `hide=True` params to be shown with `-hh` or similar?
@@ -77,15 +77,15 @@
     @property
     def name(self) -> str:
         if self._name is not None:
             return self._name
         return self._default_name()
 
     @name.setter
-    def name(self, value: Optional[str]):
+    def name(self, value: Union[str, None]):
         if value is not None:
             self._name = value
 
     def _default_name(self) -> str:
         return f'{self.__class__.__name__}#{id(self)}'
 
     def __set_name__(self, command: CommandCls, name: str):
@@ -95,15 +95,15 @@
         self._attr_name = name
 
     # endregion
 
     def __hash__(self) -> int:
         return hash(self.__class__) ^ hash(self._attr_name) ^ hash(self._name) ^ hash(self.command)
 
-    def _ctx(self, command: CommandAny = None) -> Optional[Context]:
+    def _ctx(self, command: CommandAny = None) -> Union[Context, None]:
         if context := get_current_context(True):
             return context
         if command is None:
             command = self.command
         try:
             return command._Command__ctx
         except AttributeError:
@@ -172,26 +172,28 @@
     :param show_default: Override the :attr:`.CommandConfig.show_defaults` setting for this parameter to always or
       never include the default value in usage / help messages.  Default: follow the ``show_defaults`` setting.
     :param hide: If ``True``, this parameter will not be included in usage / help messages.  Defaults to ``False``.
     """
 
     # region Attributes & Initialization
 
+    # fmt: off
     # Class attributes
-    _action_map: Dict[str, Type[ParamAction]] = {}
-    _repr_attrs: Optional[Strings] = None           #: Attributes to include in ``repr()`` output
+    _action_map: dict[str, Type[ParamAction]] = {}
+    _repr_attrs: Union[Strings, None] = None                            #: Attributes to include in ``repr()`` output
     # Instance attributes with class defaults
     metavar: str = None
-    nargs: Nargs                                    # Expected to be set in subclasses
-    type: Optional[Callable[[str], T_co]] = None    # Expected to be set in subclasses
-    allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC  # Set in some subclasses
+    nargs: Nargs                                                        # Expected to be set in subclasses
+    type: Union[Callable[[str], T_co], None] = None                     # Expected to be set in subclasses
+    allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC     # Set in some subclasses
     default = _NotSet
     default_cb: DefaultCallback | None = None
     show_default: Bool = None
     strict_default: Bool = False
+    # fmt: on
 
     def __init_subclass__(cls, repr_attrs: Strings = None, actions: Collection[Type[ParamAction]] = None, **kwargs):
         """
         :param repr_attrs: Additional attributes to include in the repr.
         :param actions: Collection of ParamAction classes that this type of Parameter supports
         """
         super().__init_subclass__(**kwargs)
@@ -316,15 +318,15 @@
         return f'{self.__class__.__name__}({self.name!r}, {kwargs})'
 
     # region Parsing / Argument Handling
 
     def get_const(self, opt_str: OptStr = None):
         return _NotSet
 
-    def get_env_const(self, value: str, env_var: str) -> Tuple[T_co, bool]:
+    def get_env_const(self, value: str, env_var: str) -> tuple[T_co, bool]:
         return _NotSet, False
 
     def prepare_value(self, value: str, short_combo: Bool = False, pre_action: Bool = False) -> T_co:
         type_func = self.type
         if type_func is None or (pre_action and isinstance(type_func, InputType) and type_func.is_valid_type(value)):
             return value
         try:
@@ -334,15 +336,15 @@
         except InputValidationError as e:
             raise BadArgument(self, str(e)) from e
         except (TypeError, ValueError) as e:
             raise BadArgument(self, f'bad {value=} for type={type_func!r}: {e}') from e
         except Exception as e:
             raise BadArgument(self, f'unable to cast {value=} to type={type_func!r}') from e
 
-    def validate(self, value: Optional[T_co], joined: Bool = False):
+    def validate(self, value: Union[T_co, None], joined: Bool = False):
         if not isinstance(value, str) or not value or not value[0] == '-':
             return
         elif self.allow_leading_dash == AllowLeadingDash.NUMERIC:
             if not joined and len(value) > 1 and not _is_numeric(value):
                 raise BadArgument(self, f'invalid {value=}')
         elif self.allow_leading_dash == AllowLeadingDash.NEVER:
             raise BadArgument(self, f'invalid {value=}')
@@ -356,20 +358,18 @@
             return True
 
     # endregion
 
     # region Parse Results / Argument Value Handling
 
     @overload
-    def __get__(self: Param, command: None, owner: CommandCls) -> Param:
-        ...
+    def __get__(self: Param, command: None, owner: CommandCls) -> Param: ...
 
     @overload
-    def __get__(self, command: CommandObj, owner: CommandCls) -> Optional[T_co]:
-        ...
+    def __get__(self, command: CommandObj, owner: CommandCls) -> Union[T_co, None]: ...
 
     def __get__(self, command, owner):
         if command is None:
             return self
 
         with self._ctx(command):
             value = self.result(command)
@@ -541,15 +541,15 @@
 
     def __init__(self, default: AllowLeadingDash = AllowLeadingDash.NUMERIC):
         self.default = default
 
     def __set_name__(self, owner, name: str):
         self.name = name
 
-    def __get__(self, instance: Optional[Parameter], owner) -> Union[AllowLeadingDash, AllowLeadingDashProperty]:
+    def __get__(self, instance: Union[Parameter, None], owner) -> Union[AllowLeadingDash, AllowLeadingDashProperty]:
         if instance is None:
             return self
         return instance.__dict__.get(self.name, self.default)
 
     def __set__(self, instance: Parameter, value: LeadingDash):
         if value is not None:
             value = AllowLeadingDash(value)
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from functools import partial
-from string import whitespace, printable
-from typing import Type, TypeVar, Generic, Optional, Callable, Union, Collection, Mapping, NoReturn, Dict
+from string import printable, whitespace
 from types import MethodType
+from typing import Callable, Collection, Generic, Mapping, NoReturn, Optional, Type, TypeVar, Union
 
 from ..context import ctx
-from ..exceptions import ParameterDefinitionError, BadArgument, InvalidChoice, CommandDefinitionError
+from ..exceptions import BadArgument, CommandDefinitionError, InvalidChoice, ParameterDefinitionError
 from ..formatting.utils import format_help_entry
 from ..nargs import Nargs
 from ..typing import Bool, CommandCls, CommandObj
 from ..utils import _NotSet, camel_to_snake_case, short_repr
 from .actions import Concatenate
 from .base import BasePositional
 
@@ -47,17 +47,17 @@
         help_str = f', help={short_repr(self.help)}' if self.help else ''
         target_str = f', target={self.target}' if self.choice != self.target else ''
         return f'{self.__class__.__name__}({self.choice!r}{target_str}{help_str})'
 
     def format_usage(self) -> str:
         return '(default)' if self.choice is None else self.choice
 
-    def format_help(self, lpad: int = 4, tw_offset: int = 0, prefix: str = '') -> str:
+    def format_help(self, lpad: int = 4, prefix: str = '') -> str:
         # Note: no longer called by formatters
-        return format_help_entry((self.format_usage(),), self.help, prefix, tw_offset, lpad=lpad)
+        return format_help_entry((self.format_usage(),), self.help, prefix, lpad=lpad)
 
 
 class ChoiceMap(BasePositional[str], Generic[T], actions=(Concatenate,)):
     """
     Base class for :class:`SubCommand` and :class:`Action`.  It is not meant to be used directly.
 
     Allows choices to be defined and provided as a string that may contain spaces, without requiring users to escape or
@@ -74,15 +74,15 @@
     :param description: The description to be used in help text for this parameter.
     :param kwargs: Additional keyword arguments to pass to :class:`.BasePositional`.
     """
 
     _choice_validation_exc = ParameterDefinitionError
     _default_title: str = 'Choices'
     nargs = Nargs('+')
-    choices: Dict[str, Choice[T]]
+    choices: dict[str, Choice[T]]
     title: OptStr
     description: OptStr
 
     def __init_subclass__(  # pylint: disable=W0222
         cls, title: str = None, choice_validation_exc: Type[Exception] = None, **kwargs
     ):
         """
@@ -131,15 +131,19 @@
             raise cls._choice_validation_exc(f'Invalid {cls.__name__} {prefix}={value!r} - invalid characters: {bad}')
 
     def register_choice(self, choice: str, target: T = _NotSet, help: str = None):  # noqa
         self._validate_positional(choice)
         self._register_choice(choice, target, help)
 
     def _register_choice(
-        self, choice: OptStr, target: Optional[T] = _NotSet, help: str = None, local: bool = False  # noqa
+        self,
+        choice: OptStr,
+        target: Optional[T] = _NotSet,
+        help: str = None,  # noqa
+        local: bool = False,
     ):
         try:
             existing = self.choices[choice]
         except KeyError:
             self.choices[choice] = Choice(choice, target, help, local)
             self._update_nargs()
         else:
@@ -252,15 +256,19 @@
             msg = f'Invalid {choice=} for {command} with {parent=} - already assigned to {self.choices[choice].target}'
             raise CommandDefinitionError(msg) from None
 
         command._is_subcommand_ = True  # This is used indirectly by ``main()`` to filter out non-top-level Commands
         return command
 
     def register(
-        self, command_or_choice: Union[str, CommandCls] = None, *, choice: str = None, help: str = None  # noqa
+        self,
+        command_or_choice: Union[str, CommandCls] = None,
+        *,
+        choice: str = None,
+        help: str = None,  # noqa
     ) -> Callable[[CommandCls], CommandCls]:
         """
         Class decorator version of :meth:`.register_command`.  Registers the wrapped :class:`.Command` as the
         subcommand class to be used for further parsing when the given choice is specified for this parameter.
 
         This is only necessary for subcommands that do not extend their parent Command class.  When extending a parent
         Command, it is automatically registered as a subcommand during Command subclass initialization.
@@ -293,15 +301,19 @@
 
     Actions are better suited for use cases where all of the target functions accept the same arguments.  If target
     functions require different / additional parameters, then using a :class:`.SubCommand` with separate sub
     :class:`.Command` classes may make more sense.
     """
 
     def register_action(
-        self, choice: OptStr, method: MethodType, help: str = None, default: Bool = False  # noqa
+        self,
+        choice: OptStr,
+        method: MethodType,
+        help: str = None,  # noqa
+        default: Bool = False,
     ) -> MethodType:
         if help is None:
             try:
                 help = method.__doc__  # noqa
             except AttributeError:
                 pass
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from itertools import count
-from typing import TYPE_CHECKING, Optional, Iterable, Iterator, Tuple, List
+from typing import TYPE_CHECKING, Iterable, Iterator, Optional
 
 from ..context import ctx
-from ..exceptions import ParameterDefinitionError, CommandDefinitionError, ParamConflict, ParamsMissing
-from .base import ParamBase, BasePositional, BaseOption, _group_stack
+from ..exceptions import CommandDefinitionError, ParamConflict, ParameterDefinitionError, ParamsMissing
+from .base import BaseOption, BasePositional, ParamBase, _group_stack
 from .pass_thru import PassThru
 
 if TYPE_CHECKING:
     from ..typing import Bool, ParamList, ParamOrGroup
 
 __all__ = ['ParamGroup']
 
@@ -41,15 +41,15 @@
       ``False``.
     :param hide: If ``True``, this group of parameters will not be included in usage / help messages.  Defaults to
       ``False``.
     """
 
     _num: int
     description: Optional[str]
-    members: List[ParamOrGroup]
+    members: list[ParamOrGroup]
     mutually_exclusive: Bool = False
     mutually_dependent: Bool = False
 
     def __init__(
         self,
         name: str = None,
         *,
@@ -173,15 +173,15 @@
         for param in params:
             self.register(param)
 
     # endregion
 
     # region Argument Handling
 
-    def _categorize_params(self) -> Tuple[ParamList, ParamList]:
+    def _categorize_params(self) -> tuple[ParamList, ParamList]:
         """Called after parsing to group this group's members by whether they were provided or not."""
         provided = []
         missing = []
         for obj in self.members:
             if ctx.num_provided(obj):
                 provided.append(obj)
             else:
@@ -234,15 +234,15 @@
         req_any, req_all = self._classify_required()
         if not provided and req_any:
             raise ParamsMissing(missing, partial=not req_all)
         elif provided or not self.in_mutually_exclusive_group:
             if req_missing := [p for p in missing if p.required]:
                 raise ParamsMissing(req_missing)
 
-    def _classify_required(self) -> Tuple[bool, bool]:
+    def _classify_required(self) -> tuple[bool, bool]:
         """Returns a tuple of (req_any, req_all)"""
         if self.mutually_dependent and (self.required or any(p.required for p in self.members)):
             return True, True
         elif self.required:
             return True, False
         else:
             return False, False
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/option_strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 Containers for option strings
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Collection, Union, Iterator, List, Set, Tuple
+from typing import TYPE_CHECKING, Collection, Iterator, Optional, Union
 
-from ..config import OptionNameMode, DEFAULT_CONFIG
+from ..config import DEFAULT_CONFIG, OptionNameMode
 from ..exceptions import ParameterDefinitionError
 from ..utils import _NotSet
 
 if TYPE_CHECKING:
     from ..typing import Bool
 
 __all__ = ['OptionStrings', 'TriFlagOptionStrings']
 
 
 class OptionStrings:
     """Container for the option strings registered for a given BaseOption (or subclass thereof)."""
 
     __slots__ = ('name_mode', '_long', '_short', 'combinable', '_display_long')
     name_mode: Optional[OptionNameMode]
-    combinable: Set[str]
-    _display_long: Set[str]
-    _long: Set[str]
-    _short: Set[str]
+    combinable: set[str]
+    _display_long: set[str]
+    _long: set[str]
+    _short: set[str]
 
     def __init__(self, option_strs: Collection[str], name_mode: Union[OptionNameMode, str, None] = _NotSet):
         self.name_mode = OptionNameMode(name_mode) if name_mode is not _NotSet else None
         long_opts, short_opts = _split_options(option_strs)
         self._display_long = self._long = long_opts
         self._short = short_opts
         self.combinable = {opt[1:] for opt in short_opts if len(opt) == 2}
@@ -65,27 +65,27 @@
                 self._display_long.add(option)
         if mode & OptionNameMode.UNDERSCORE:
             option = f'--{name}'
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
-    def get_sets(self) -> Tuple[Set[str], Set[str]]:
+    def get_sets(self) -> tuple[set[str], set[str]]:
         return self._long, self._short
 
     @property
-    def long(self) -> List[str]:
+    def long(self) -> list[str]:
         return sorted(self._long, key=_options_sort_key)
 
     @property
-    def short(self) -> List[str]:
+    def short(self) -> list[str]:
         return sorted(self._short, key=_options_sort_key)
 
     @property
-    def display_long(self) -> List[str]:
+    def display_long(self) -> list[str]:
         return sorted(self._display_long, key=_options_sort_key)
 
     def get_usage_opt(self) -> str:
         return next(self.option_strs())
 
     def option_strs(self) -> Iterator[str]:
         yield from self.display_long
@@ -96,15 +96,15 @@
 
 class TriFlagOptionStrings(OptionStrings):
     """Container for the option strings registered for a given TriFlag."""
 
     __slots__ = ('_alt_prefix', '_alt_long', '_alt_short')
     _alt_prefix: Optional[str]
     _alt_short: Optional[str]
-    _alt_long: Union[Set[str], Tuple[str]]
+    _alt_long: Union[set[str], tuple[str]]
 
     def has_long(self) -> Bool:
         """Whether any primary / non-alternate long option strings were defined"""
         return self._long.difference(self._alt_long)
 
     def has_min_opts(self) -> Bool:
         return next(self.option_strs(False), None) and next(self.option_strs(True), None)
@@ -133,43 +133,43 @@
             option = f'--{self._alt_prefix}_{name}'
             self._alt_long.add(option)
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
     @property
-    def alt_allowed(self) -> Set[str]:
+    def alt_allowed(self) -> set[str]:
         allowed = set(self._alt_long)
         if self._alt_short:
             allowed.add(self._alt_short)
             allowed.add(self._alt_short[1:])
         return allowed
 
     # @property
     # def long_primary(self) -> List[str]:
     #     return [opt for opt in self.long if opt not in self._alt_long]
 
     @property
-    def display_long_primary(self) -> List[str]:
+    def display_long_primary(self) -> list[str]:
         return [opt for opt in self.display_long if opt not in self._alt_long]
 
     @property
-    def short_primary(self) -> List[str]:
+    def short_primary(self) -> list[str]:
         return [opt for opt in self.short if opt != self._alt_short]
 
     # @property
     # def long_alt(self) -> List[str]:
     #     return sorted(self._alt_long, key=_options_sort_key)
 
     @property
-    def display_long_alt(self) -> List[str]:
+    def display_long_alt(self) -> list[str]:
         return [opt for opt in self.display_long if opt in self._alt_long]
 
     @property
-    def short_alt(self) -> List[str]:
+    def short_alt(self) -> list[str]:
         return [self._alt_short] if self._alt_short else []
 
     def primary_option_strs(self) -> Iterator[str]:
         yield from self.display_long_primary
         yield from self.short_primary
 
     def alt_option_strs(self) -> Iterator[str]:
@@ -191,20 +191,20 @@
 
 
 def _options_sort_key(opt: str):
     """Used to sort option strings in descending length order (alphanumeric order for options with the same length)"""
     return -len(opt), opt
 
 
-def _split_options(opt_strs: Collection[str]) -> Tuple[Set[str], Set[str]]:
+def _split_options(opt_strs: Collection[str]) -> tuple[set[str], set[str]]:
     """Split long and short option strings and ensure that all of the provided option strings are valid."""
     long_opts, short_opts, bad_opts, bad_short = set(), set(), [], []
     for opt in opt_strs:
-        if not opt:     # Ignore None / empty strings / etc
-            continue    # Only raise an exception if invalid values that were intended to be used were provided
+        if not opt:  # Ignore None / empty strings / etc
+            continue  # Only raise an exception if invalid values that were intended to be used were provided
         elif not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt:
             bad_opts.append(opt)
         elif opt.startswith('--'):
             long_opts.add(opt)
         elif '-' in opt[2:]:
             bad_short.append(opt)
         else:
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 """
 
 from __future__ import annotations
 
 import logging
 from abc import ABC
 from functools import partial, update_wrapper
-from typing import TYPE_CHECKING, Any, Optional, Callable, Union, TypeVar, NoReturn, Literal, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Literal, NoReturn, Optional, TypeVar, Union
 
-from ..exceptions import ParameterDefinitionError, BadArgument, CommandDefinitionError, ParamUsageError, ParserExit
+from ..exceptions import BadArgument, CommandDefinitionError, ParameterDefinitionError, ParamUsageError, ParserExit
 from ..inputs import normalize_input_type
 from ..nargs import Nargs, NargsValue
 from ..typing import T_co, TypeFunc
 from ..utils import _NotSet, str_to_bool
-from .actions import Store, StoreConst, Append, AppendConst, Count
-from .base import BaseOption, AllowLeadingDashProperty
+from .actions import Append, AppendConst, Count, Store, StoreConst
+from .base import AllowLeadingDashProperty, BaseOption
 from .option_strings import TriFlagOptionStrings
 
 if TYPE_CHECKING:
-    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, LeadingDash, CommandMethod
+    from ..typing import Bool, ChoicesType, CommandCls, CommandMethod, CommandObj, InputTypeFunc, LeadingDash, OptStr
 
 __all__ = [
     'Option',
     'Flag',
     'TriFlag',
     'ActionFlag',
     'Counter',
@@ -184,15 +184,15 @@
         self.const = const
         if type is not None:
             self.type = type
 
     def register_default_cb(self, method):
         raise ParameterDefinitionError(f'{self.__class__.__name__}s do not support default callback methods')
 
-    def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TD], bool]:
+    def get_env_const(self, value: str, env_var: str) -> tuple[Union[TC, TD], bool]:
         try:
             parsed = self.type(value)
         except Exception as e:
             raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
         if self.use_env_value and parsed != self.const and parsed != self.default:
             raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
         return parsed, self.use_env_value
@@ -237,20 +237,20 @@
     type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
     use_env_value: bool = False
     _default_cb_ok = True
     _opt_str_cls = TriFlagOptionStrings
     option_strs: TriFlagOptionStrings
     alt_help: OptStr = None
     default: TD
-    consts: Tuple[TC, TA]
+    consts: tuple[TC, TA]
 
     def __init__(
         self,
         *option_strs: str,
-        consts: Tuple[TC, TA] = (True, False),
+        consts: tuple[TC, TA] = (True, False),
         alt_prefix: str = None,
         alt_long: str = None,
         alt_short: str = None,
         alt_help: str = None,
         action: ConstAct = 'store_const',
         default: TD = _NotSet,
         default_cb: Callable[[], TD] = None,
@@ -300,15 +300,15 @@
 
     def get_const(self, opt_str: OptStr = None) -> Union[TC, TA]:
         if opt_str in self.option_strs.alt_allowed:
             return self.consts[1]
         else:
             return self.consts[0]
 
-    def get_env_const(self, value: str, env_var: str) -> Tuple[Union[TC, TA, TD], bool]:
+    def get_env_const(self, value: str, env_var: str) -> tuple[Union[TC, TA, TD], bool]:
         try:
             parsed = self.type(value)
         except Exception as e:
             raise ParamUsageError(self, f'unable to parse {value=} from {env_var=}: {e}') from e
         if self.use_env_value:
             if parsed not in self.consts and parsed != self.default:
                 raise BadArgument(self, f'invalid value={parsed!r} from {env_var=}')
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parameters/positionals.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parse_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union, Optional, Collection, Iterable, Iterator, MutableMapping, Dict, Set, Tuple
+from typing import TYPE_CHECKING, Collection, Iterable, Iterator, MutableMapping, Optional, Union
 
 from .exceptions import AmbiguousParseTree
 from .nargs import nargs_min_and_max_sums
 from .utils import _parse_tree_target_repr
 
 if TYPE_CHECKING:
     from .nargs import Nargs
     from .parameters.base import BasePositional
     from .parameters.choice_map import Choice
-    from .typing import OptStr, CommandCls
+    from .typing import CommandCls, OptStr
 
 __all__ = ['PosNode']
 
 
 class AnyWord:
     __slots__ = ('nargs', 'n', 'remaining')
 
@@ -56,15 +56,15 @@
 Word = Union[str, AnyWord, None]
 Target = Union['BasePositional', 'CommandCls', None]
 
 
 class PosNode(MutableMapping[Word, 'PosNode']):
     __slots__ = ('links', 'param', 'parent', 'target', 'word', '_any_word', '_any_node')
 
-    links: Dict[Word, PosNode]
+    links: dict[Word, PosNode]
     param: Optional[BasePositional]
     parent: Optional[PosNode]
     target: Target
     word: Word
 
     def __init__(
         self, word: Word, param: Optional[BasePositional], target: Target = None, parent: Optional[PosNode] = None
@@ -75,25 +75,25 @@
         self.target = target
         self.word = word
         try:
             parent[word] = self
         except TypeError:  # parent was None
             pass
 
-    def link_params(self, recursive: bool = False) -> Set[BasePositional]:
+    def link_params(self, recursive: bool = False) -> set[BasePositional]:
         return set(self._link_params(recursive))
 
     def _link_params(self, recursive: bool = False) -> Iterator[BasePositional]:
         for node in self.values():
             yield node.param
         if recursive:
             for node in self.values():
                 yield from node._link_params(_has_upper_bound(node))
 
-    def nargs_min_and_max(self) -> Tuple[int, Union[int, float]]:
+    def nargs_min_and_max(self) -> tuple[int, Union[int, float]]:
         return nargs_min_and_max_sums(p.nargs for p in self.link_params(True))
 
     # region AnyWord Methods
 
     @property
     def any_word(self) -> AnyWord:
         try:
@@ -130,15 +130,15 @@
         return PosNode(word, self.param, self.target, self)
 
     # endregion
 
     # region Introspection
 
     @property
-    def raw_path(self) -> Tuple[Word, ...]:
+    def raw_path(self) -> tuple[Word, ...]:
         word = self.word
         if not word:
             return ()
         return (*self.parent.raw_path, word)  # noqa
 
     def path_repr(self) -> str:
         return '({})'.format(', '.join(str(n) if isinstance(n, AnyWord) else repr(n) for n in self.raw_path))
@@ -321,25 +321,25 @@
 def _has_upper_bound(node) -> bool:
     try:
         return node.word.nargs.has_upper_bound
     except AttributeError:
         return True
 
 
-def process_params(command: CommandCls, nodes: Iterable[PosNode], params: Iterable[BasePositional]) -> Set[PosNode]:
+def process_params(command: CommandCls, nodes: Iterable[PosNode], params: Iterable[BasePositional]) -> set[PosNode]:
     for param in params:
         nodes = process_param(command, nodes, param)
 
     return nodes
 
 
-def process_param(command: CommandCls, nodes: Iterable[PosNode], param: BasePositional) -> Set[PosNode]:
+def process_param(command: CommandCls, nodes: Iterable[PosNode], param: BasePositional) -> set[PosNode]:
     # At each step, the number of branches grows
     try:
-        choices: Dict[OptStr, Choice] = param.choices  # noqa
+        choices: dict[OptStr, Choice] = param.choices  # noqa
     except AttributeError:  # It was not a ChoiceMap param
         pass
     else:
         get_params = command.__class__.params
 
         new_nodes = set()
         for choice in choices.values():
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/parser.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,45 +5,52 @@
 """
 
 from __future__ import annotations
 
 import logging
 from collections import deque
 from os import environ
-from typing import TYPE_CHECKING, Optional, Iterable, Deque, List
+from typing import TYPE_CHECKING, Deque, Iterable, Optional
 
-from .core import get_parent
 from .context import ActionPhase, Context
-from .exceptions import UsageError, ParamUsageError, NoSuchOption, MissingArgument, ParamsMissing
-from .exceptions import Backtrack, NextCommand
+from .core import get_parent
+from .exceptions import (
+    Backtrack,
+    MissingArgument,
+    NextCommand,
+    NoSuchOption,
+    ParamsMissing,
+    ParamUsageError,
+    UsageError,
+)
 from .nargs import REMAINDER, nargs_min_and_max_sums
+from .parameters.base import BaseOption, BasePositional, Parameter
 from .parse_tree import PosNode
-from .parameters.base import Parameter, BasePositional, BaseOption
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .config import CommandConfig
-    from .typing import CommandType, OptStr, Bool
+    from .typing import Bool, CommandType, OptStr
 
 __all__ = ['CommandParser', 'parse_args_and_get_next_cmd']
 log = logging.getLogger(__name__)
 
 _PRE_INIT = ActionPhase.PRE_INIT
 
 
 class CommandParser:
     """Stateful parser used for a single pass of argument parsing"""
 
     __slots__ = ('_last', 'arg_deque', 'ctx', 'config', 'deferred', 'params', 'positionals')
 
     arg_deque: Optional[Deque[str]]
     config: CommandConfig
-    deferred: Optional[List[str]]
+    deferred: Optional[list[str]]
     params: CommandParameters
-    positionals: List[BasePositional]
+    positionals: list[BasePositional]
     _last: Optional[Parameter]
 
     def __init__(self, ctx: Context, params: CommandParameters, config: CommandConfig):
         self._last = None
         self.ctx = ctx
         self.params = params
         self.positionals = params.get_positionals_to_parse(ctx)
@@ -370,15 +377,15 @@
         s = '' if nargs.min == 1 else 's'
         raise MissingArgument(param, f'expected {nargs.min} value{s}, but only found {found}')
 
 
 parse_args_and_get_next_cmd = CommandParser.parse_args_and_get_next_cmd
 
 
-def _to_pop(positionals: Iterable[BasePositional], can_pop: List[int], available: int, req_mod: int = 0) -> int:
+def _to_pop(positionals: Iterable[BasePositional], can_pop: list[int], available: int, req_mod: int = 0) -> int:
     if not can_pop:
         return 0
 
     required, acceptable = nargs_min_and_max_sums(p.nargs for p in positionals)
     if available < required:
         return 0
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/testing.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # pylint: disable=R0913,C0103
 
 from __future__ import annotations
 
 import sys
 from contextlib import AbstractContextManager, contextmanager
 from difflib import unified_diff
-from io import StringIO, BytesIO
+from io import BytesIO, StringIO
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Any, Iterable, Type, Union, Callable, IO, ContextManager, Dict, List, Tuple
+from typing import IO, TYPE_CHECKING, Any, Callable, ContextManager, Dict, Iterable, List, Tuple, Type, Union
 from unittest import TestCase
-from unittest.mock import Mock, seal, patch
+from unittest.mock import Mock, patch, seal
 
 from .commands import Command
 from .context import Context
 from .core import get_params
 from .documentation import load_commands
 from .exceptions import UsageError
 from .parameters import help_action
@@ -231,15 +231,15 @@
             sio.write(_colored(line, 6, '\n\n'))
         else:
             sio.write(line + '\n')
 
     return sio.getvalue()
 
 
-def format_dict_diff(a: Dict[str, Any], b: Dict[str, Any]) -> str:
+def format_dict_diff(a: dict[str, Any], b: dict[str, Any]) -> str:
     formatted_a = []
     formatted_b = []
     for key in sorted(set(a) | set(b)):
         try:
             val_a = a[key]
         except KeyError:
             str_b = f'{key!r}: {b[key]!r}'
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser/utils.py` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Utilities for working with terminals, strings, and Enums.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from enum import Flag, EnumMeta
+from enum import EnumMeta, Flag
 from inspect import isawaitable
 from shutil import get_terminal_size
 from time import monotonic
-from typing import Any, Callable, TypeVar, Awaitable, List
+from typing import Any, Awaitable, Callable, TypeVar
 
 try:
     from enum import CONFORM
 except ImportError:
     CONFORM = None
 
 try:
@@ -135,15 +135,15 @@
                     break
             else:
                 if tmp._value_ != 0:
                     return tmp
 
         raise KeyError
 
-    def _decompose(self) -> List[FlagEnum]:
+    def _decompose(self) -> list[FlagEnum]:
         if self._name_ is None or '|' in self._name_:  # | check is for 3.11 where pseudo-members are assigned names
             val = self._value_
             return sorted(mem for mem in self.__class__ if mem._value_ & val == mem._value_)  # noqa
         return [self]
 
     def __lt__(self, other: FlagEnum) -> bool:
         return self._value_ < other._value_
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2024.4.21
+Version: 2024.5.18.post1
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Project-URL: Documentation, https://dskrypa.github.io/cli_command_parser
@@ -30,27 +30,27 @@
 Requires-Dist: wcwidth; extra == "wcwidth"
 Provides-Extra: conversion
 Requires-Dist: astunparse; python_version < "3.9" and extra == "conversion"
 
 CLI Command Parser
 ##################
 
-|downloads| |py_version| |coverage_badge| |build_status| |Blue|
+|downloads| |py_version| |coverage_badge| |build_status| |Ruff|
 
 .. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
 
-.. |Blue| image:: https://img.shields.io/badge/code%20style-blue-blue.svg
-    :target: https://blue.readthedocs.io/
+.. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://docs.astral.sh/ruff/
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/cli-command-parser
     :target: https://pypistats.org/packages/cli-command-parser
 
 
 CLI Command Parser is a class-based CLI argument parser that defines parameters with descriptors.  It provides the
 tools to quickly and easily get started with basic CLIs, and it scales well to support even very large and complex
```

### Comparing `cli_command_parser-2024.4.21/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2024.5.18.post1/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2024.4.21/readme.rst` & `cli_command_parser-2024.5.18.post1/readme.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 CLI Command Parser
 ##################
 
-|downloads| |py_version| |coverage_badge| |build_status| |Blue|
+|downloads| |py_version| |coverage_badge| |build_status| |Ruff|
 
 .. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
 
-.. |Blue| image:: https://img.shields.io/badge/code%20style-blue-blue.svg
-    :target: https://blue.readthedocs.io/
+.. |Ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://docs.astral.sh/ruff/
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/cli-command-parser
     :target: https://pypistats.org/packages/cli-command-parser
 
 
 CLI Command Parser is a class-based CLI argument parser that defines parameters with descriptors.  It provides the
 tools to quickly and easily get started with basic CLIs, and it scales well to support even very large and complex
```

### Comparing `cli_command_parser-2024.4.21/setup.cfg` & `cli_command_parser-2024.5.18.post1/setup.cfg`

 * *Files identical despite different names*

