# Comparing `tmp/pytest_parameterize_from_files-0.12.tar.gz` & `tmp/pytest_parameterize_from_files-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_parameterize_from_files-0.12.tar", last modified: Sun May 19 04:41:28 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytest_parameterize_from_files-0.12.tar` & `pytest_parameterize_from_files-0.9.5.tar`

### file list

```diff
@@ -1,11 +1,41 @@
-drwxr-xr-x   0 plsuh      (502) staff       (20)        0 2024-05-19 04:41:28.563256 pytest_parameterize_from_files-0.12/
--rw-r--r--   0 plsuh      (502) staff       (20)      472 2024-05-19 04:41:28.563070 pytest_parameterize_from_files-0.12/PKG-INFO
--rw-r--r--   0 plsuh      (502) staff       (20)      205 2024-05-19 04:39:19.000000 pytest_parameterize_from_files-0.12/README.md
-drwxr-xr-x   0 plsuh      (502) staff       (20)        0 2024-05-19 04:41:28.562894 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/
--rw-r--r--   0 plsuh      (502) staff       (20)      472 2024-05-19 04:41:28.000000 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/PKG-INFO
--rw-r--r--   0 plsuh      (502) staff       (20)      287 2024-05-19 04:41:28.000000 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/SOURCES.txt
--rw-r--r--   0 plsuh      (502) staff       (20)        1 2024-05-19 04:41:28.000000 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/dependency_links.txt
--rw-r--r--   0 plsuh      (502) staff       (20)       22 2024-05-19 04:41:28.000000 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/requires.txt
--rw-r--r--   0 plsuh      (502) staff       (20)        1 2024-05-19 04:41:28.000000 pytest_parameterize_from_files-0.12/pytest_parameterize_from_files.egg-info/top_level.txt
--rw-r--r--   0 plsuh      (502) staff       (20)       38 2024-05-19 04:41:28.563295 pytest_parameterize_from_files-0.12/setup.cfg
--rw-r--r--   0 plsuh      (502) staff       (20)      598 2024-05-19 04:39:19.000000 pytest_parameterize_from_files-0.12/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/src/pytest_parameterize_from_files/__init__.py
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/src/pytest_parameterize_from_files/plugin.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/conftest.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_help_message.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_ignore_multi_files.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_by_reference.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_file_extended_name.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_multi_files.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_multi_values.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_one_file.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_separate_subdirs.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_load_subdirs.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/test_merge_multi_fixtures.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_by_reference_tester.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_multi_files_tester_1.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_multi_files_tester_2.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_multi_files_tester_3.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_multi_values_tester.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_one_file_tester.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_one_tester_1.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_one_tester_1.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_subdirs_tester_1.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_load_subdirs_tester_2.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_merge_multi_fixtures_tester_1.yaml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_merge_multi_fixtures_tester_2.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/data_merge_multi_fixtures_tester_3.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_ignore_multi_files_tester.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_by_reference_tester.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_multi_files_tester.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_multi_values_tester.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_one_file_tester.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_one_tester.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_load_subdirs_tester.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/tests/pytester_example_files/example_test_merge_multi_fixtures_tester.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/LICENSE
+-rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/README.md
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 pytest_parameterize_from_files-0.9.5/PKG-INFO
```

