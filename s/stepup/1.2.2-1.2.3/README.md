# Comparing `tmp/stepup-1.2.2.tar.gz` & `tmp/stepup-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup-1.2.2.tar", last modified: Thu May 16 09:16:58 2024, max compression
+gzip compressed data, was "stepup-1.2.3.tar", last modified: Sun May 19 11:05:50 2024, max compression
```

## Comparing `stepup-1.2.2.tar` & `stepup-1.2.3.tar`

### file list

```diff
@@ -1,950 +1,950 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.361860 stepup-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 09:16:53.000000 stepup-1.2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.217860 stepup-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.229860 stepup-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 09:16:53.000000 stepup-1.2.2/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-16 09:16:53.000000 stepup-1.2.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-16 09:16:53.000000 stepup-1.2.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 09:16:53.000000 stepup-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-16 09:16:53.000000 stepup-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 09:16:53.000000 stepup-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 09:16:58.361860 stepup-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 09:16:53.000000 stepup-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.229860 stepup-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.233860 stepup-1.2.2/docs/advanced_topics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.233860 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/config.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_static_inputs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.233860 stepup-1.2.2/docs/advanced_topics/amending_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/amending_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.233860 stepup-1.2.2/docs/advanced_topics/blocked_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/blocked_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/blocked_steps/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/blocked_steps/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/blocked_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/blocked_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.233860 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/cyclic_dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/environment_variables/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/environment_variables/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/environment_variables/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/environment_variables/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/environment_variables.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/here_and_root/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/here_and_root/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/here_and_root/source/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/source/sub/example.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/source/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/here_and_root.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/manual_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/optional_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/plot_logmap.png
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/optional_steps.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/pools/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/pools/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/pools/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/pools/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/pools/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/pools.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.237860 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_deferred_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/static_named_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch1/unused.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch2/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch3/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch4/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/static_named_glob.md
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/stepup_root.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/variable_substitution/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/dst_foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/src_foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/variable_substitution.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.241860 stepup-1.2.2/docs/advanced_topics/volatile_outputs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/volatile_outputs/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/volatile_outputs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/volatile_outputs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/volatile_outputs/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/advanced_topics/volatile_outputs.md
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.245860 stepup-1.2.2/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/automatic_cleaning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.245860 stepup-1.2.2/docs/getting_started/copy_mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/copy_mkdir/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/copy_mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/copy_mkdir/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/copy_mkdir/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/copy_mkdir.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.245860 stepup-1.2.2/docs/getting_started/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/graph_creator.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/graph_supplier.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/dependencies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.245860 stepup-1.2.2/docs/getting_started/distributed_plans/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/part1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/stdout.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.245860 stepup-1.2.2/docs/getting_started/distributed_plans/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/sub/part2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/distributed_plans.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.249860 stepup-1.2.2/docs/getting_started/first_step/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      218 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step/stdout3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/first_step.md
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/interactive_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.249860 stepup-1.2.2/docs/getting_started/no_rules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/lower1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/lower2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/no_rules.md
--rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/processes.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.249860 stepup-1.2.2/docs/getting_started/script_multiple/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/ebbr.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/ebos.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/matplotlibrc
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/plot_ebbr.png
--rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/plot_ebos.png
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_multiple.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.249860 stepup-1.2.2/docs/getting_started/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/script_single.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/getting_started/static_files/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files/limerick.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/getting_started/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/getting_started/static_glob/src/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/src/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/src/foo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/getting_started/static_glob_conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/getting_started/static_glob_conditional/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/stdout1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional/stdout2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/getting_started/static_glob_conditional.md
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/license.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.253860 stepup-1.2.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/reference/interactive.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/reference/stepup.core.api.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/reference/stepup.core.interact.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-16 09:16:53.000000 stepup-1.2.2/docs/run_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-16 09:16:53.000000 stepup-1.2.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-16 09:16:53.000000 stepup-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:16:58.361860 stepup-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.217860 stepup-1.2.2/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.257860 stepup-1.2.2/stepup/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/deferred_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/director.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/interact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    32855 2024-05-16 09:16:53.000000 stepup-1.2.2/stepup/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.357860 stepup-1.2.2/stepup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:58.000000 stepup-1.2.2/stepup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.261860 stepup-1.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.261860 stepup-1.2.2/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.261860 stepup-1.2.2/tests/cases/amend/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_stdout_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/expected_stdout_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/inp1.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.265860 stepup-1.2.2/tests/cases/amend_delay/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_delay/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.265860 stepup-1.2.2/tests/cases/amend_env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/foo.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      845 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_env_vars/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.265860 stepup-1.2.2/tests/cases/amend_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_missing/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.269860 stepup-1.2.2/tests/cases/amend_outdir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_outdir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.269860 stepup-1.2.2/tests/cases/amend_voldir_pending/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/amend_voldir_pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.269860 stepup-1.2.2/tests/cases/deferred_glob1/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1519 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.269860 stepup-1.2.2/tests/cases/deferred_glob1/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.269860 stepup-1.2.2/tests/cases/deferred_glob1/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob1/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.273860 stepup-1.2.2/tests/cases/deferred_glob2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.273860 stepup-1.2.2/tests/cases/deferred_glob2/static/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/static/data1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/static/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.273860 stepup-1.2.2/tests/cases/deferred_glob2/static/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/static/sub/bar.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_glob2/static/sub/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.273860 stepup-1.2.2/tests/cases/deferred_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.273860 stepup-1.2.2/tests/cases/deferred_subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/sub/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/sub/unused.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/deferred_subdir/sub/used.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.277860 stepup-1.2.2/tests/cases/env_vars/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_graph_05.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_stdout_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_stdout_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_stdout_d.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_variables_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_variables_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_variables_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_variables_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/expected_variables_05.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3805 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/printvars.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/variables_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars/variables_02.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.277860 stepup-1.2.2/tests/cases/env_vars_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/demovars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1332 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_amend/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.277860 stepup-1.2.2/tests/cases/env_vars_path/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/FOO.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/FOO.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1561 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_path/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/env_vars_subs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/env_vars_subs/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_subs/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/env_vars_workdir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/env_vars_workdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/env_vars_workdir/sub/input.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/error_cyclic_late/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      744 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_cyclic_late/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.281860 stepup-1.2.2/tests/cases/error_deferred_nonexisting/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_deferred_nonexisting/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_deferred_nonexisting/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_deferred_nonexisting/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_deferred_nonexisting/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_deferred_nonexisting/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.285860 stepup-1.2.2/tests/cases/error_env_var/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_env_var/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.285860 stepup-1.2.2/tests/cases/error_main_fails/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_main_fails/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.285860 stepup-1.2.2/tests/cases/error_not_executable/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_not_executable/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_not_executable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_not_executable/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_not_executable/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_not_executable/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.285860 stepup-1.2.2/tests/cases/error_overlap_deferred/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_overlap_deferred/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.285860 stepup-1.2.2/tests/cases/error_static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/error_static_dir/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_static_dir/subdir/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/error_step/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/error_step/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/here/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/here/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/source/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/here/source/www/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/source/www/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/here/source/www/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.289860 stepup-1.2.2/tests/cases/makedirs/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/bunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/makedirs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.293860 stepup-1.2.2/tests/cases/mkdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.293860 stepup-1.2.2/tests/cases/mkdir/exists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/exists/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.293860 stepup-1.2.2/tests/cases/mkdir_error/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/mkdir_error/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.293860 stepup-1.2.2/tests/cases/nodata/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1801 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nodata/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.293860 stepup-1.2.2/tests/cases/noplan/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/noplan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/noplan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/noplan/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/noplan/main.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.297860 stepup-1.2.2/tests/cases/nostatic/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1928 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/nostatic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.297860 stepup-1.2.2/tests/cases/not_cyclic/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/not_cyclic/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.297860 stepup-1.2.2/tests/cases/optional_convert/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/expected_graph_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/expected_graph_b.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/expected_graph_c.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1846 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/raw_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/raw_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/raw_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/optional_convert/raw_04.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.301860 stepup-1.2.2/tests/cases/output_not_created/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/output_not_created/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.301860 stepup-1.2.2/tests/cases/pending/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pending/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.301860 stepup-1.2.2/tests/cases/permissions_file_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_file_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.305860 stepup-1.2.2/tests/cases/permissions_plan_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.305860 stepup-1.2.2/tests/cases/permissions_plan_rerun/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_rerun/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.305860 stepup-1.2.2/tests/cases/permissions_plan_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1446 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.305860 stepup-1.2.2/tests/cases/permissions_plan_restart/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_plan_restart/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.305860 stepup-1.2.2/tests/cases/permissions_step_rerun/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_rerun/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.309860 stepup-1.2.2/tests/cases/permissions_step_restart/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1364 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/permissions_step_restart/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.309860 stepup-1.2.2/tests/cases/pool/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      741 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/pool/r.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.313860 stepup-1.2.2/tests/cases/reqdir_missing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/reqdir_missing/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.313860 stepup-1.2.2/tests/cases/restart_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1358 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.317860 stepup-1.2.2/tests/cases/restart_changes/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/source_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/source_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_changes/source_both.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.317860 stepup-1.2.2/tests/cases/restart_deferred_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1250 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.317860 stepup-1.2.2/tests/cases/restart_deferred_glob/static/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_deferred_glob/static/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.321860 stepup-1.2.2/tests/cases/restart_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.321860 stepup-1.2.2/tests/cases/restart_orphan/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1292 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_orphan/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.321860 stepup-1.2.2/tests/cases/restart_outdated_amend/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1446 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_outdated_amend/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.325860 stepup-1.2.2/tests/cases/restart_output/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1272 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/restart_output/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.325860 stepup-1.2.2/tests/cases/script_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.329860 stepup-1.2.2/tests/cases/script_cases_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_cases_settings/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.329860 stepup-1.2.2/tests/cases/script_single/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.329860 stepup-1.2.2/tests/cases/script_single/work/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/work/config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/script_single/work/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.329860 stepup-1.2.2/tests/cases/static/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.333860 stepup-1.2.2/tests/cases/static_abs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_abs/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.333860 stepup-1.2.2/tests/cases/static_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      748 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_dir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.333860 stepup-1.2.2/tests/cases/static_glob/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1993 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_glob/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.333860 stepup-1.2.2/tests/cases/static_nglob/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.337860 stepup-1.2.2/tests/cases/static_nglob/ch-1-intro/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.337860 stepup-1.2.2/tests/cases/static_nglob/ch-2-theory/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.337860 stepup-1.2.2/tests/cases/static_nglob/ch-3-conclusions/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3638 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob/sec-2-2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.337860 stepup-1.2.2/tests/cases/static_nglob_partial/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_04.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_stdout_a.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/expected_stdout_b.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2439 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_partial/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.337860 stepup-1.2.2/tests/cases/static_nglob_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      895 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.341860 stepup-1.2.2/tests/cases/static_nglob_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/sub/inp1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/sub/inp2.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/static_nglob_subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.341860 stepup-1.2.2/tests/cases/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/example.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      789 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.341860 stepup-1.2.2/tests/cases/subdir/sub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/subdir/sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.341860 stepup-1.2.2/tests/cases/watch_blocked/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/expensive.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/initial.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/plan_blocked.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_blocked/plan_unblocked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.345860 stepup-1.2.2/tests/cases/watch_boot/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_boot/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.345860 stepup-1.2.2/tests/cases/watch_chain/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/config_01.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/config_02.json
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1222 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_chain/use_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.345860 stepup-1.2.2/tests/cases/watch_input/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/first.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_input/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.349860 stepup-1.2.2/tests/cases/watch_middle/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/original.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_middle/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.349860 stepup-1.2.2/tests/cases/watch_mixed/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/backup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/plan_full.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_mixed/plan_trimmed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.353860 stepup-1.2.2/tests/cases/watch_nochanges/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1029 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_nochanges/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.353860 stepup-1.2.2/tests/cases/watch_outdated_amend1/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend1/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.353860 stepup-1.2.2/tests/cases/watch_outdated_amend2/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1413 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_outdated_amend2/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.357860 stepup-1.2.2/tests/cases/watch_output/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/input.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1073 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_output/second.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:58.357860 stepup-1.2.2/tests/cases/watch_wanted/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/expected_graph_03.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/cases/watch_wanted/plan_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/core_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/echo_server_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/echo_server_stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_assoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_nglob.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65157 2024-05-16 09:16:53.000000 stepup-1.2.2/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-19 11:05:46.000000 stepup-1.2.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.180800 stepup-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.192800 stepup-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-19 11:05:46.000000 stepup-1.2.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-19 11:05:46.000000 stepup-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 11:05:46.000000 stepup-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-19 11:05:50.324799 stepup-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 11:05:46.000000 stepup-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.196800 stepup-1.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.196800 stepup-1.2.3/docs/advanced_topics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/config.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      149 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_static_inputs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/amending_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/amending_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/blocked_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/blocked_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/cyclic_dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/environment_variables.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.200800 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/example.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/source/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/here_and_root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/manual_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/optional_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62512 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/plot_logmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/optional_steps.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/pools/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/pools.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_deferred_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/sec1_1_introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/sec1_2_objectives.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch1/unused.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.204800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/sec2_1_mathematical_requisites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch2/sec2_2_theory.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/sec3_1_applications.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch3/sec3_2_discussion.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch4/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/ch4/sec4_1_summary.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      647 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/static_named_glob.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/stepup_root.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/variable_substitution/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/dst_foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      186 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/src_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/variable_substitution.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.208800 stepup-1.2.3/docs/advanced_topics/volatile_outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       96 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/advanced_topics/volatile_outputs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/automatic_cleaning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/copy_mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/copy_mkdir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/graph_creator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/graph_supplier.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      286 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/dependencies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/distributed_plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/part1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/stdout.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/distributed_plans/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/sub/part2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/distributed_plans.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.212800 stepup-1.2.3/docs/getting_started/first_step/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      218 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step/stdout3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/first_step.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/interactive_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/no_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/lower1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/lower2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/no_rules.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/processes.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/script_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/ebbr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/ebos.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)      199 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/matplotlibrc
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60027 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot_ebbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69904 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/plot_ebos.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_multiple.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/script_single.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.216800 stepup-1.2.3/docs/getting_started/static_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/limerick.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      154 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/src/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/src/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob_conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/getting_started/static_glob_conditional/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/dataset/bigfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      232 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      339 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/getting_started/static_glob_conditional.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/license.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1847 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.220800 stepup-1.2.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/interactive.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.interact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/reference/stepup.core.nglob.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-19 11:05:46.000000 stepup-1.2.3/docs/run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-19 11:05:46.000000 stepup-1.2.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-19 11:05:46.000000 stepup-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:05:50.324799 stepup-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.184800 stepup-1.2.3/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.224800 stepup-1.2.3/stepup/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/deferred_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12834 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/interact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28646 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32855 2024-05-19 11:05:46.000000 stepup-1.2.3/stepup/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/stepup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    33367 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:50.000000 stepup-1.2.3/stepup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.228800 stepup-1.2.3/tests/cases/amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/expected_stdout_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/inp1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      250 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      308 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      307 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_delay/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/foo.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      845 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      100 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_env_vars/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      715 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_missing/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.232800 stepup-1.2.3/tests/cases/amend_outdir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_outdir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/amend_voldir_pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/amend_voldir_pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1538 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob1/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.236800 stepup-1.2.3/tests/cases/deferred_glob2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/data1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_glob2/static/sub/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.240800 stepup-1.2.3/tests/cases/deferred_subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/unused.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/deferred_subdir/sub/used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_graph_05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_stdout_d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/expected_variables_05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/printvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/variables_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars/variables_02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/demovars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_amend/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.244799 stepup-1.2.3/tests/cases/env_vars_path/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/FOO.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/FOO.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1580 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_path/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_subs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_subs/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_subs/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_workdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      355 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/env_vars_workdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/env_vars_workdir/sub/input.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/error_cyclic_late/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      744 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_cyclic_late/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.248799 stepup-1.2.3/tests/cases/error_deferred_nonexisting/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_deferred_nonexisting/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_env_var/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_env_var/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_main_fails/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_main_fails/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_not_executable/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_not_executable/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.252800 stepup-1.2.3/tests/cases/error_overlap_deferred/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_overlap_deferred/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_static_dir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_static_dir/subdir/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/error_step/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/error_step/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/here/source/www/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/www/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/here/source/www/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.256800 stepup-1.2.3/tests/cases/makedirs/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      763 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/makedirs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir/exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/exists/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/mkdir_error/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       79 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/mkdir_error/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.260800 stepup-1.2.3/tests/cases/nodata/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1820 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nodata/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/noplan/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/noplan/main.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/nostatic/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1947 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/nostatic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.264799 stepup-1.2.3/tests/cases/not_cyclic/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1539 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/not_cyclic/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/optional_convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_graph_c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1865 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/optional_convert/raw_04.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/output_not_created/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      780 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      169 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/output_not_created/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/pending/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pending/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.268799 stepup-1.2.3/tests/cases/permissions_file_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_file_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_rerun/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_rerun/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_plan_restart/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_plan_restart/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.272799 stepup-1.2.3/tests/cases/permissions_step_rerun/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_rerun/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/permissions_step_restart/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1383 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       95 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/permissions_step_restart/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/pool/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/expected_graph.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      741 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/pool/r.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.276799 stepup-1.2.3/tests/cases/reqdir_missing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/reqdir_missing/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1377 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      301 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_changes/source_both.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_deferred_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1269 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      142 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.280799 stepup-1.2.3/tests/cases/restart_deferred_glob/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_deferred_glob/static/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_orphan/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      132 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_orphan/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.284799 stepup-1.2.3/tests/cases/restart_outdated_amend/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1465 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_outdated_amend/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/restart_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1291 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/restart_output/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/script_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      396 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.288799 stepup-1.2.3/tests/cases/script_cases_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_cases_settings/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/script_single/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      193 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/script_single/work/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/work/config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/script_single/work/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_abs/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.292799 stepup-1.2.3/tests/cases/static_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      748 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_dir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_glob/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2012 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_glob/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/sec-1-1-blabla.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-1-intro/sec-1-2-some-more.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-2-theory/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-2-theory/sec-2-1-basics.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.296799 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/sec-3-1-summary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/ch-3-conclusions/sec-3-2-outlook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18883 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob/sec-2-2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_partial/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_b.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2458 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_partial/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      895 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/inp1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/inp2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/static_nglob_subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.300799 stepup-1.2.3/tests/cases/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/example.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      789 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      170 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/subdir/sub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/subdir/sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/watch_blocked/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/expensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/initial.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      261 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/plan_blocked.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_blocked/plan_unblocked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.304799 stepup-1.2.3/tests/cases/watch_boot/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1136 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_boot/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.308799 stepup-1.2.3/tests/cases/watch_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/config_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/config_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1222 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_chain/use_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.308799 stepup-1.2.3/tests/cases/watch_input/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/first.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1093 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_input/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.312799 stepup-1.2.3/tests/cases/watch_middle/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/original.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_middle/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.312799 stepup-1.2.3/tests/cases/watch_mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/backup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      219 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/plan_full.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_mixed/plan_trimmed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.316799 stepup-1.2.3/tests/cases/watch_nochanges/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1029 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_nochanges/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.316799 stepup-1.2.3/tests/cases/watch_outdated_amend1/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      164 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      271 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend1/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.320799 stepup-1.2.3/tests/cases/watch_outdated_amend2/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1413 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      331 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_outdated_amend2/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.320799 stepup-1.2.3/tests/cases/watch_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/input.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1073 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_output/second.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:05:50.324799 stepup-1.2.3/tests/cases/watch_wanted/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_graph_03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      328 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/cases/watch_wanted/plan_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/core_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/echo_server_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/echo_server_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_assoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21270 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_nglob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65157 2024-05-19 11:05:46.000000 stepup-1.2.3/tests/test_workflow.py
```

### Comparing `stepup-1.2.2/.github/workflows/release.yaml` & `stepup-1.2.3/.github/workflows/release.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+# This workflow is adapted from:
+# https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
+# Changed made:
+# - Remove emoticons
+# - Update some actions to more recent versions
+
 name: release
 
 on: push
 
+env:
+  # This is not critical
+  # It is used only for showing URLs in GitHub Actions web interface.
+  PYPI_NAME: stepup
+
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
@@ -18,34 +29,34 @@
     - name: Install pypa/build
       run: >-
         python -m pip install build
     - name: Build package
       run: >-
         python -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: Publish Python distribution to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
-      url: https://pypi.org/p/stepup
+      url: https://pypi.org/p/${{ env.PYPI_NAME }}
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -58,20 +69,20 @@
 
     permissions:
       contents: write
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.1
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
@@ -96,22 +107,22 @@
     if: ${{ github.ref == 'refs/heads/main' &&  github.repository_owner == 'reproducible-reporting'}}
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
-      url: https://test.pypi.org/p/stepup
+      url: https://test.pypi.org/p/${{ env.PYPI_NAME }}
 
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `stepup-1.2.2/.pre-commit-config.yaml` & `stepup-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/LICENSE` & `stepup-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/PKG-INFO` & `stepup-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.2
+Version: 1.2.3
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
```

### Comparing `stepup-1.2.2/README.md` & `stepup-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/amending_static_inputs/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/amending_static_inputs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/amending_static_inputs.md` & `stepup-1.2.3/docs/advanced_topics/amending_static_inputs.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/amending_steps/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/amending_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/amending_steps.md` & `stepup-1.2.3/docs/advanced_topics/amending_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/blocked_steps/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/blocked_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/blocked_steps.md` & `stepup-1.2.3/docs/advanced_topics/blocked_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/cyclic_dependencies/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/cyclic_dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/cyclic_dependencies.md` & `stepup-1.2.3/docs/advanced_topics/cyclic_dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/environment_variables/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/environment_variables/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/environment_variables.md` & `stepup-1.2.3/docs/advanced_topics/environment_variables.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/here_and_root/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/here_and_root/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/here_and_root.md` & `stepup-1.2.3/docs/advanced_topics/here_and_root.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/manual_cleaning.md` & `stepup-1.2.3/docs/advanced_topics/manual_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/optional_steps/plot_logmap.png` & `stepup-1.2.3/docs/advanced_topics/optional_steps/plot_logmap.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/optional_steps/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/optional_steps/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/optional_steps.md` & `stepup-1.2.3/docs/advanced_topics/optional_steps.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/pools/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/pools/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/pools.md` & `stepup-1.2.3/docs/advanced_topics/pools.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph.txt` & `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph_creator.svg` & `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_deferred_glob/graph_supplier.svg` & `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_deferred_glob/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/static_deferred_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_deferred_glob.md` & `stepup-1.2.3/docs/advanced_topics/static_deferred_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_named_glob/plan.py` & `stepup-1.2.3/docs/advanced_topics/static_named_glob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_named_glob/stdout.txt` & `stepup-1.2.3/docs/advanced_topics/static_named_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/static_named_glob.md` & `stepup-1.2.3/docs/advanced_topics/static_named_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/stepup_root.md` & `stepup-1.2.3/docs/advanced_topics/stepup_root.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/variable_substitution.md` & `stepup-1.2.3/docs/advanced_topics/variable_substitution.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/advanced_topics/volatile_outputs.md` & `stepup-1.2.3/docs/advanced_topics/volatile_outputs.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/changelog.md` & `stepup-1.2.3/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.2.3] - 2024-05-19
+
+### Changed
+
+- Completed and revised docstrings in `stepup.core.nglob`,
+  and added this module to the reference documentation.
+
+### Fixed
+
+- Improve hash computation of a symbolic links in `stepup.core.hash`.
+
+
 ## [1.2.2] - 2024-05-16
 
 ### Fixed
 
 - Make `cleanup` command work in project subdirectories when `STEPUP_ROOT` is set.
 - Avoid useless wait when running a `plan.py` script outside of `stepup`.
```

### Comparing `stepup-1.2.2/docs/development.md` & `stepup-1.2.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/automatic_cleaning.md` & `stepup-1.2.3/docs/getting_started/automatic_cleaning.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/copy_mkdir/stdout.txt` & `stepup-1.2.3/docs/getting_started/copy_mkdir/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/copy_mkdir.md` & `stepup-1.2.3/docs/getting_started/copy_mkdir.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/dependencies/graph_creator.svg` & `stepup-1.2.3/docs/getting_started/dependencies/graph_creator.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/dependencies/graph_supplier.svg` & `stepup-1.2.3/docs/getting_started/dependencies/graph_supplier.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/dependencies/stdout.txt` & `stepup-1.2.3/docs/getting_started/dependencies/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/dependencies.md` & `stepup-1.2.3/docs/getting_started/dependencies.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/distributed_plans/stdout.txt` & `stepup-1.2.3/docs/getting_started/distributed_plans/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/distributed_plans.md` & `stepup-1.2.3/docs/getting_started/distributed_plans.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/first_step/stdout1.txt` & `stepup-1.2.3/docs/getting_started/first_step/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/first_step.md` & `stepup-1.2.3/docs/getting_started/first_step.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/interactive_usage.md` & `stepup-1.2.3/docs/getting_started/interactive_usage.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/introduction.md` & `stepup-1.2.3/docs/getting_started/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/no_rules/stdout.txt` & `stepup-1.2.3/docs/getting_started/no_rules/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/no_rules.md` & `stepup-1.2.3/docs/getting_started/no_rules.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/processes.svg` & `stepup-1.2.3/docs/getting_started/processes.svg`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/ebbr.csv` & `stepup-1.2.3/docs/getting_started/script_multiple/ebbr.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/ebos.csv` & `stepup-1.2.3/docs/getting_started/script_multiple/ebos.csv`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/plot.py` & `stepup-1.2.3/docs/getting_started/script_multiple/plot.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/plot_ebbr.png` & `stepup-1.2.3/docs/getting_started/script_multiple/plot_ebbr.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/plot_ebos.png` & `stepup-1.2.3/docs/getting_started/script_multiple/plot_ebos.png`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple/stdout.txt` & `stepup-1.2.3/docs/getting_started/script_multiple/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_multiple.md` & `stepup-1.2.3/docs/getting_started/script_multiple.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/script_single.md` & `stepup-1.2.3/docs/getting_started/script_single.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/static_files.md` & `stepup-1.2.3/docs/getting_started/static_files.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/static_glob/stdout.txt` & `stepup-1.2.3/docs/getting_started/static_glob/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/static_glob.md` & `stepup-1.2.3/docs/getting_started/static_glob.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/static_glob_conditional/stdout1.txt` & `stepup-1.2.3/docs/getting_started/static_glob_conditional/stdout1.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/getting_started/static_glob_conditional.md` & `stepup-1.2.3/docs/getting_started/static_glob_conditional.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/index.md` & `stepup-1.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/installation.md` & `stepup-1.2.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/license.md` & `stepup-1.2.3/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/plan.py` & `stepup-1.2.3/docs/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/reference/interactive.md` & `stepup-1.2.3/docs/reference/interactive.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/reference/stepup.core.api.md` & `stepup-1.2.3/docs/reference/stepup.core.api.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/docs/run_example.py` & `stepup-1.2.3/docs/run_example.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/mkdocs.yml` & `stepup-1.2.3/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     - advanced_topics/cyclic_dependencies.md
     - advanced_topics/amending_static_inputs.md
     - advanced_topics/manual_cleaning.md
     - advanced_topics/stepup_root.md
   - Reference:
     - reference/stepup.core.api.md
     - reference/stepup.core.interact.md
+    - reference/stepup.core.nglob.md
     - reference/interactive.md
   - changelog.md
   - development.md
   - license.md
 
 exclude_docs: |
   */*/ch*/*.md
```

### Comparing `stepup-1.2.2/pyproject.toml` & `stepup-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/__init__.py` & `stepup-1.2.3/stepup/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/api.py` & `stepup-1.2.3/stepup/core/api.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/assoc.py` & `stepup-1.2.3/stepup/core/assoc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/asyncio.py` & `stepup-1.2.3/stepup/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/cascade.py` & `stepup-1.2.3/stepup/core/cascade.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/cleanup.py` & `stepup-1.2.3/stepup/core/cleanup.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/deferred_glob.py` & `stepup-1.2.3/stepup/core/deferred_glob.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/director.py` & `stepup-1.2.3/stepup/core/director.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/exceptions.py` & `stepup-1.2.3/stepup/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/file.py` & `stepup-1.2.3/stepup/core/file.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/hash.py` & `stepup-1.2.3/stepup/core/hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,36 @@
         else:
             TypeError(f"Not supported by HashWords: {type(word)}")
 
     def digest(self):
         return self._hash.digest()
 
 
-def compute_file_digest(path) -> bytes:
+def compute_file_digest(path: str, follow_symlinks=True) -> bytes:
+    """Compute the blake2b digest of a file or a symbolic link.
+
+    Parameters
+    ----------
+    path
+        The file of which the hash must be computed.
+    follow_symlinks
+        If True (default) and the path is a symbolic link,
+        try to hash the contents of the destination file.
+        If False, the destination path itself is hashed.
+
+    Returns
+    -------
+    digest
+        A 64 bytes blake2b hash.
+    """
+    path = Path(path)
+    if path.islink() and not follow_symlinks:
+        return hashlib.blake2b(path.readlink().encode("utf-8")).digest()
+    if path.is_dir():
+        raise OSError("File digests of directories are not supported.")
     with open(path, "rb") as fh:
         return hashlib.file_digest(fh, hashlib.blake2b).digest()
 
 
 @attrs.define
 class FileHash:
     _digest: bytes = attrs.field()
```

### Comparing `stepup-1.2.2/stepup/core/interact.py` & `stepup-1.2.3/stepup/core/interact.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/job.py` & `stepup-1.2.3/stepup/core/job.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/nglob.py` & `stepup-1.2.3/stepup/core/nglob.py`

 * *Files 23% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     - `feedback_001.md` with `report_001.pdf`
     - `feedback_123.md` with `report_123.pdf`
 
     The following won't be in the results, despite the fact that the files exist:
 
     - `feedback_001.md` with `report_123.pdf`
 
-- Conventional glob wildcards are also allowed and are called "anonymous wildcards"
+- Conventional (recursive) glob wildcards are also allowed and are called "anonymous wildcards"
   to clarify the distinction from named wildcards.
 """
 
 import copy
 import glob
 import re
 from collections.abc import Collection, Iterable, Iterator
@@ -99,32 +99,57 @@
     "convert_nglob_to_glob",
     "has_wildcards",
 )
 
 
 @attrs.define
 class NGlobMatch:
+    """A set of matches corresponding sharing consistent values for named wildcards.
+
+    The matching files can be accessed by integer indexing or through the `files` attribute:
+
+    ```python
+    assert match[0] == match.files[0]
+    ```
+
+    The substring matching the named wildcards can be accessed as attributes.
+    For example, the substring matching a named wildcard `foo` is accessed as follows:
+
+    ```python
+    print(match.foo)
+    ```
+    """
+
     _mapping: dict[str, str]
     _files: list[Path | list[Path]]
 
     def __getitem__(self, idx) -> Path | list[Path]:
         return self._files[idx]
 
     def __getattr__(self, name) -> str:
         try:
             return self._mapping[name]
         except KeyError as exc:
-            raise AttributeError(f"'NGlobMatch' object has not attribute '{name}'") from exc
+            raise AttributeError(f"'NGlobMatch' object has no attribute '{name}'") from exc
 
     @property
     def mapping(self) -> dict[str, str]:
+        """Dictionary with `(wildcard_name, substring)` items."""
         return self._mapping
 
     @property
-    def files(self) -> list[Path]:
+    def files(self) -> list[Path | list[Path]]:
+        """Matching files, all having consistent substrings matching the named wildcards.
+
+        Each item corresponds to a pattern in `NGlobMulti.patterns`.
+        If a pattern has anonymous wildcards,
+        the item itself is a list of all files matching the pattern,
+        If the pattern contains no anonymous wildcards,
+        the corresponding item in the returned list is a single path.
+        """
         return self._files
 
 
 @attrs.define
 class NGlobSingle:
     """Named glob with a single pattern."""
 
@@ -133,20 +158,22 @@
     _results: dict[tuple[str, ...], set[Path]] = attrs.field(factory=dict)
     _used_names: tuple[str, ...] = attrs.field(init=False)
     _glob_pattern: str = attrs.field(init=False)
     _regex: re.Pattern = attrs.field(init=False)
 
     @classmethod
     def structure(cls, state, strings: list[str]):
+        """Create an instance from the result of the `unstructure` method."""
         results = {
             tuple(values): {Path(strings[path]) for path in paths} for values, paths in state["r"]
         }
         return cls(strings[state["p"]], state["s"], results)
 
     def unstructure(self, lookup: dict[str, int]) -> dict[str, Any]:
+        """Return a serializable representation of the instance."""
         results = [
             (key, [lookup[path] for path in sorted(paths)]) for key, paths in self._results.items()
         ]
         return {"p": lookup[self.pattern], "s": self.subs, "r": results}
 
     @_used_names.default
     def _default_used_names(self) -> tuple[str, ...]:
@@ -158,68 +185,113 @@
 
     @_regex.default
     def _default_regex(self) -> re.Pattern:
         return re.compile(convert_nglob_to_regex(self._pattern, self._subs))
 
     @property
     def pattern(self) -> str:
+        """The Named Glob pattern used to match filenames."""
         return self._pattern
 
     @property
     def subs(self) -> dict[str, str]:
+        """User-defined glob patterns for the named wildcards.
+
+        When a name is not present, `*` is used.
+        """
         return self._subs
 
     @property
     def results(self) -> dict[tuple[str, ...], set[Path]]:
+        """All matching files, grouped by substrings matching the named wildcards.
+
+        The keys of the `results` dictionary are tuples with the substrings,
+        matching the respective named wildcards in the `used_names` tuple.
+        The values are sets with matching paths.
+        """
         return self._results
 
     @property
     def used_names(self) -> tuple[str, ...]:
+        """A tuple of named wildcards present in the pattern."""
         return self._used_names
 
     @property
     def glob_pattern(self) -> str:
+        """The conversion of the named glob to a (more general) conventional glob pattern."""
         return self._glob_pattern
 
     @property
     def regex(self) -> re.Pattern:
+        """The conversion of the named glob to a regular expression."""
         return self._regex
 
     def _loop_matches(
         self, paths: Iterable[str]
     ) -> Iterator[tuple[tuple[str, ...], set[Path], Path]]:
+        """Low-level iterator used by the `extend` and `reduce` methods.
+
+        The paths are tested one by one against the regular expression.
+        In case of a hit, it yields a tuple with the following three items:
+
+        - `values`: the substrings matching the named wildcards.
+        - `path_set`: the current set of paths associated with the combination of substrings.
+        - `path`: a `Path` instance of the matching path.
+        """
         for path in paths:
             match_ = self._regex.fullmatch(path)
             if match_ is not None:
                 mapping = match_.groupdict()
                 values = tuple(mapping[name] for name in self._used_names)
                 paths = self._results.get(values)
                 if paths is None:
                     paths = set()
                     self._results[values] = paths
                 yield values, paths, Path(path)
                 if len(paths) == 0:
                     del self._results[values]
 
     def extend(self, paths: Iterable[str]) -> Iterator[tuple[str, ...]]:
-        """Add matching paths from the given list paths. Yield new values for named wildcards."""
+        """Add matching paths from the given list paths.
+
+        Yields
+        ------
+        values
+            A tuple with substring matching the named wildcards,
+            only this combination of names was not present yet.
+        """
         for values, path_set, path in self._loop_matches(paths):
             if len(path_set) == 0:
                 yield values
             path_set.add(path)
 
     def reduce(self, paths: Iterable[str]) -> Iterator[tuple[str, ...]]:
-        """Remove matching paths from given list paths. Yield deleted values of named wildcards."""
+        """Remove matching paths from given list paths.
+
+        Yields
+        ------
+        values
+            A tuple with deleted substring matching the named wildcards,
+            only if the last matching paths were removed.
+        """
         for values, path_set, path in self._loop_matches(paths):
             if len(path_set) > 0:
                 path_set.discard(path)
                 if len(path_set) == 0:
                     yield values
 
     def glob(self) -> Iterator[tuple[str, ...]]:
+        """Extend the results with paths obtained through the built-in glob module.
+
+        Yields
+        ------
+        values
+            A tuple with substring matching the named wildcards,
+            only this combination of names was not present yet.
+        """
         yield from self.extend(glob.glob(self._glob_pattern, recursive=True))
 
 
 def has_wildcards(pattern: str) -> bool:
     """Test if a glob pattern has anonymous or named wildcards."""
     return RE_NAMED_WILD.search(pattern) is not None
 
@@ -229,21 +301,24 @@
     for ipart, part in enumerate(RE_NAMED_WILD.split(pattern)):
         if ipart % 2 == 1 and not part.startswith("${*"):
             return True
     return False
 
 
 def iter_wildcard_names(pattern: str) -> Iterator[str]:
+    """Iterate over the names of the named wildcards in a Named Glob pattern."""
     for ipart, part in enumerate(RE_NAMED_WILD.split(pattern)):
         if ipart % 2 == 1 and part.startswith("${*"):
             yield part[3:-1]
 
 
 @attrs.define
 class NGlobMulti:
+    """A sequence of Named Glob patterns for which consistent matches are collected."""
+
     _nglob_singles: tuple[NGlobSingle, ...] = attrs.field()
     _subs: dict[str, str] = attrs.field(init=False)
     _used_names: tuple[str, ...] = attrs.field(init=False)
     _has_wildcards: bool = attrs.field(init=False)
     _results: dict[tuple[str, ...], list[set[Path]]] = attrs.field(init=False, factory=dict)
 
     @_subs.default
@@ -276,36 +351,50 @@
                 return True
             if has_anonymous_wildcards(pattern):
                 return True
         return False
 
     @classmethod
     def structure(cls, state: list, strings: list[str]) -> Self:
+        """Create an instance from the result of the `unstructure` method."""
         subs = state[1].copy()
         for ngs_data in state[0]:
             ngs_data["s"] = subs
         ngss = tuple(NGlobSingle.structure(ngs_data, strings) for ngs_data in state[0])
         result = cls(ngss)
         for i, ngs in enumerate(ngss):
             for values in ngs.results:
                 result._extend_consistent(i, values)
         return result
 
     def unstructure(self, lookup: dict[str, int]) -> list:
+        """Return a serializable representation of the instance."""
         data = [
             [ngs.unstructure(lookup) for ngs in self._nglob_singles],
             self._subs.copy(),
         ]
         # A little hacky way to make the result more compact.
         for ngs_data in data[0]:
             del ngs_data["s"]
         return data
 
     @classmethod
     def from_patterns(cls, patterns: Iterable[str], subs: dict[str, str] | None = None) -> Self:
+        """Create a new instance for given patterns without any results.
+
+        Parameters
+        ----------
+        patterns
+            Named Glob patterns.
+            Results will be constrained to have consistently matching substrings
+            for the named wildcards appearing in all the patterns.
+        subs
+            Optional anonymous glob patterns for the named patterns.
+            When a name is not present, the wildcard `*` is used for this name.
+        """
         if isinstance(patterns, str):
             raise TypeError("The patterns argument cannot be a string")
         if not all(isinstance(pattern, str) for pattern in patterns):
             raise TypeError(f"The patterns must be a list of strings, got {patterns}")
         if subs is None:
             subs = {}
         else:
@@ -313,86 +402,153 @@
                 raise TypeError(f"The subs keys must be a list of strings, got {patterns}")
             if not all(isinstance(value, str) for value in subs.values()):
                 raise TypeError(f"The subs values must be a list of strings, got {patterns}")
         return cls(tuple(NGlobSingle(str(pattern), subs) for pattern in patterns))
 
     @property
     def nglob_singles(self) -> tuple[NGlobSingle, ...]:
+        """The list of NGlobSingle instances, one for each pattern.
+
+        These instances collect (partial) matches before any consistency is imposed between
+        the substrings matching the same name in different patterns.
+        """
         return self._nglob_singles
 
     @property
     def patterns(self):
+        """The list of Named Glob patterns."""
         return [ngs.pattern for ngs in self._nglob_singles]
 
     @property
     def subs(self) -> dict[str, str]:
+        """User-defined glob patterns for the named wildcards.
+
+        When a name is not present, `*` is used.
+        """
         return self._subs
 
     @property
     def used_names(self) -> tuple[str, ...]:
+        """The names used across all the named glob patterns."""
         return self._used_names
 
     @property
     def has_wildcards(self) -> bool:
+        """True if any named or anonymous wildcards are present in the patterns."""
         return self._has_wildcards
 
     @property
     def results(self) -> dict[tuple[str, ...], list[set[Path]]]:
+        """A dictionary with all matches collected so far.
+
+        A key in this dictionary is a tuple of substrings named wildcards,
+        using the same order as the `used_names` attribute.
+
+        A value is a list of sets of paths.
+        Each item in the list is a set of matching filenames for the corresponding
+        pattern from the `patterns` attribute, whose named wildcards match the substrings
+        of the key.
+
+        The results can be extended with the `extend` and `glob` methods.
+        Conversely, results can be removed with the `reduce` method.
+        """
         return self._results
 
-    def _iter_consistent(self, criteria: dict[str, str], full_paths: list | int):
+    def _iter_consistent(
+        self, criteria: dict[str, str], full_paths: list | int
+    ) -> Iterator[tuple[str, ...], list[list[Path]]]:
+        """Iterate over (partial) matching substrings and corresponding paths.
+
+        Parameters
+        ----------
+        criteria
+            A dictionary mapping named wildcards to matching substrings.
+        full_paths
+            If this is a list, it contains lists of paths matching the patterns
+            in of the `patterns` attribute with substrings consistent with those in
+            the criteria argument.
+            Note that this is a recursive iterator, so full_paths may contain fewer
+            items than there are patterns when the recursion has not reached it full
+            depth yet.
+            If this is an integer, it is in index referring to the item in the `patterns`
+            to identify the current pattern being processed.
+        """
         start = full_paths if isinstance(full_paths, int) else len(full_paths)
         if start == len(self._nglob_singles):
+            # We're in the deepest recursion: yield a result.
             yield tuple(criteria[name] for name in self._used_names), full_paths
         else:
+            # Recursion in progress...
             ngs = self._nglob_singles[start]
             for new_values, paths in ngs.results.items():
                 next_criteria = criteria.copy()
+                # Check if named wildcards are consistent with the matching paths so far.
                 for name, new_value in zip(ngs.used_names, new_values, strict=False):
                     value = next_criteria.get(name)
                     if value is None:
                         next_criteria[name] = new_value
                     elif value != new_value:
+                        # Inconsistent matches for named wildcards in different patterns.
+                        # This cannot produce a useful result.
                         next_criteria = None
                         break
                 if next_criteria is not None:
+                    # Consistency can still be imposed, so enter the next recursion...
                     next_full_paths = (
                         start + 1 if isinstance(full_paths, int) else [*full_paths, paths]
                     )
                     yield from self._iter_consistent(next_criteria, next_full_paths)
 
     def _extend_consistent(self, i: int, values: tuple[str, ...]):
+        """Extend the results of this instance, given an added combination of matching substrings.
+
+        Parameters
+        ----------
+        i
+            The integer index of the pattern in the `patterns` attribute being processed.
+        values
+            A new set of substrings matching the named wildcards.
+        """
         criteria = dict(zip(self._nglob_singles[i].used_names, values, strict=False))
         new_items = list(self._iter_consistent(criteria, []))
         for full_values, full_paths in new_items:
             self._results[full_values] = full_paths
 
     def _reduce_consistent(self, i: int, values: tuple[str, ...]):
+        """Return the results of this instance, given a removed combination of matching substrings.
+        Parameters
+        ----------
+        i
+            The integer index of the pattern in the `patterns` attribute being processed.
+        values
+            A new set of substrings matching the named wildcards.
+        """
         criteria = dict(zip(self._nglob_singles[i].used_names, values, strict=False))
         old_items = list(self._iter_consistent(criteria, 0))
         for full_values, _ in old_items:
             del self._results[full_values]
 
     def extend(self, paths: Iterable[str]):
-        """Find matches from a list of paths. Return new full matches (and track partial matches)"""
+        """Try to extend the results by searching for matches in the given list of paths."""
         if isinstance(paths, str):
             raise TypeError("The paths argument cannot be a string.")
         for i, ngs in enumerate(self._nglob_singles):
             for values in ngs.extend(paths):
                 self._extend_consistent(i, values)
 
     def reduce(self, paths: Iterable[str]):
-        """Drop matches based on deleted paths. Return old full matches (and track partial)."""
+        """Drop results by eliminating the provided paths."""
         if isinstance(paths, str):
             raise TypeError("The paths argument cannot be a string.")
         for i, ngs in enumerate(self._nglob_singles):
             for values in ngs.reduce(paths):
                 self._reduce_consistent(i, values)
 
     def glob(self):
+        """Extend the results with paths found by the built-in glob function."""
         for i, ngs in enumerate(self._nglob_singles):
             for values in ngs.glob():
                 self._extend_consistent(i, values)
 
     def deepcopy(self):
         """Return an independent copy."""
         return copy.deepcopy(self)
@@ -400,15 +556,24 @@
     def equals(self, other: "NGlobMulti") -> bool:
         """Compare the results."""
         return self._results == other._results
 
     # Convenience methods
 
     def matches(self) -> Iterator[NGlobMatch]:
-        """Iterate over combinations of files that consistently match of all patterns."""
+        """Iterate over combinations of files that consistently match all patterns.
+
+        This offers a more convenient interface of the `results` attribute.
+
+        Yields
+        ------
+        nglob_match
+            An instance of NGlobMatch, which contains the substrings matching the named wildcards
+            and the corresponding lists of paths.
+        """
         for values, path_sets in sorted(self._results.items()):
             mapping = dict(zip(self._used_names, values, strict=False))
             files = [
                 (sorted(paths) if has_anonymous_wildcards(ngs.pattern) else next(iter(paths)))
                 for ngs, paths in zip(self._nglob_singles, path_sets, strict=False)
             ]
             yield NGlobMatch(mapping, files)
@@ -422,63 +587,64 @@
         result = set()
         for ngs in self._nglob_singles:
             for path_set in ngs.results.values():
                 result.update(path_set)
         return tuple(sorted(result))
 
     def __bool__(self):
-        """True when there were some matches."""
+        """True when there are some items in the `results` attribute."""
         return len(self.results) > 0
 
     def __iter__(self) -> Iterator[str | NGlobMatch]:
+        """Iterates over `self.matches` if there are named wildcards, else over `self.files`."""
         if len(self._used_names) > 0:
             return self.matches()
         else:
             return iter(self.files())
 
     def may_match(self, path):
         """Return True if the path matches one of the NGlobSingle instances.
 
         This means that it may be path contributing to a consistent match of NGlobMulti.
-        When added, it will show up in the result of the `files` method and it may affect the
-        outcome of the `matches` method.
+        When added, it will show up in the result of the `files` method,
+        and it may affect the outcome of the `matches` method.
         """
         return any(ngs.regex.fullmatch(path) for ngs in self._nglob_singles)
 
-    def may_change(self, deleted: set[str], added: set[str]) -> bool:
+    def may_change(self, deleted: set[str], updated: set[str]) -> bool:
         """Determine whether the results may change (later) after deleting or adding files.
 
         Parameters
         ----------
         deleted
             Set of files to be deleted.
-        added
-            Set of files to be added.
+        updated
+            Set of files to be updated.
 
         Returns
         -------
         may_change
             True if the NGlobMulti results may change.
             (It may require additional additions and deletions to get any effect,
-            but cannot be excluded that that is possible.)
+            but cannot be excluded that the provided deletions and updates play a role in it.)
         """
-        added_new = added.copy()
+        updated_new = updated.copy()
         for ngs in self._nglob_singles:
             for paths in ngs.results.values():
                 if not deleted.isdisjoint(paths):
                     return True
-                added_new.difference_update(paths)
+                updated_new.difference_update(paths)
         for ngs in self._nglob_singles:
-            for path in added_new:
+            for path in updated_new:
                 if ngs.regex.fullmatch(path):
                     return True
         return False
 
     def will_change(self, deleted: Collection[str], updated: Collection[str]) -> bool:
-        """Determine whether the results may change after deleting or adding files.
+        """Determine whether the results will change after deleting or adding files.
 
         Parameters
         ----------
         deleted
             Set of files to be deleted.
         updated
             Set of files to be added or changed.
@@ -501,24 +667,25 @@
 
     Parameters
     ----------
     pattern
         A string with named wildcards.
     subs
         A dictionary mapping names to glob patterns.
-        If a name is not present, "*" is used as default.
+        If a name is not present, `*` is used as default.
     allow_names
-        When set to False, named wildcards are not allowed.
+        When set to `False`, named wildcards are not allowed.
 
     Returns
     -------
     regex
-        A regex string to test if a string matches the pattern.
+        A regular expression string to test if a string matches the pattern.
         It also contains symbolic groups to extract values
-        corresponding to named wildcards.
+        corresponding to named wildcards
+        and to impose consistency when the same name appears multiple times.
     """
     if subs is None:
         subs = {}
     parts = []
     encountered = set()
     for i, part in enumerate(RE_NAMED_WILD.split(pattern)):
         if i % 2 == 0:
@@ -547,28 +714,29 @@
             else:
                 raise ValueError(f"Cannot convert wildcard to regex: {part}")
             parts.append(regex)
     return "".join(parts)
 
 
 def convert_nglob_to_glob(pattern: str, subs: dict[str, str] | None = None) -> str:
-    """Convert nglob wildcards to ordinary ones, compatible with builtin glob and fnmatch.
+    """Convert nglob wildcards to ordinary ones, compatible with builtin glob and fnmatch modules.
 
     Parameters
     ----------
     pattern
         A string with named wildcards.
     subs
         A dictionary mapping names to glob patterns.
-        If a name is not present, "*" is used as default.
+        If a name is not present, `*` is used as default.
 
     Returns
     -------
+    pattern
         A conventional wildcard string, without the constraint that named wildcards must correspond.
-        Where possible, neighbouring wildcards are merged into one.
+        Where possible, neighboring wildcards are merged into one.
     """
     if subs is None:
         subs = {}
     # Split in text, wildcard and named wildcard fragments.
     parts = []
     # The odd-numbered indices match a (named) wildcard.
     for i, part in enumerate(RE_NAMED_WILD.split(pattern)):
```

### Comparing `stepup-1.2.2/stepup/core/pytest.py` & `stepup-1.2.3/stepup/core/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/reporter.py` & `stepup-1.2.3/stepup/core/reporter.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/rpc.py` & `stepup-1.2.3/stepup/core/rpc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/runner.py` & `stepup-1.2.3/stepup/core/runner.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/scheduler.py` & `stepup-1.2.3/stepup/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/script.py` & `stepup-1.2.3/stepup/core/script.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/step.py` & `stepup-1.2.3/stepup/core/step.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/tui.py` & `stepup-1.2.3/stepup/core/tui.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/utils.py` & `stepup-1.2.3/stepup/core/utils.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/watcher.py` & `stepup-1.2.3/stepup/core/watcher.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/worker.py` & `stepup-1.2.3/stepup/core/worker.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup/core/workflow.py` & `stepup-1.2.3/stepup/core/workflow.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/stepup.egg-info/PKG-INFO` & `stepup-1.2.3/stepup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup
-Version: 1.2.2
+Version: 1.2.3
 Summary: StepUp Core provides the basic framework for the StepUp build tool
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-core/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-core/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-core/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-core/changelog/
 Classifier: Environment :: Console
```

### Comparing `stepup-1.2.2/stepup.egg-info/SOURCES.txt` & `stepup-1.2.3/stepup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 docs/getting_started/static_glob_conditional/plan.py
 docs/getting_started/static_glob_conditional/stdout1.txt
 docs/getting_started/static_glob_conditional/stdout2.txt
 docs/getting_started/static_glob_conditional/dataset/bigfile.txt
 docs/reference/interactive.md
 docs/reference/stepup.core.api.md
 docs/reference/stepup.core.interact.md
+docs/reference/stepup.core.nglob.md
 stepup.egg-info/PKG-INFO
 stepup.egg-info/SOURCES.txt
 stepup.egg-info/dependency_links.txt
 stepup.egg-info/entry_points.txt
 stepup.egg-info/requires.txt
 stepup.egg-info/top_level.txt
 stepup/core/__init__.py
@@ -541,15 +542,14 @@
 tests/cases/permissions_step_restart/expected_stdout_02.txt
 tests/cases/permissions_step_restart/main.sh
 tests/cases/permissions_step_restart/plan.py
 tests/cases/permissions_step_restart/step.py
 tests/cases/pool/.gitignore
 tests/cases/pool/README.md
 tests/cases/pool/expected_graph.txt
-tests/cases/pool/expected_stdout.txt
 tests/cases/pool/main.sh
 tests/cases/pool/plan.py
 tests/cases/pool/r.txt
 tests/cases/reqdir_missing/.gitignore
 tests/cases/reqdir_missing/README.md
 tests/cases/reqdir_missing/expected_graph.txt
 tests/cases/reqdir_missing/expected_stdout.txt
```

### Comparing `stepup-1.2.2/tests/cases/README.md` & `stepup-1.2.3/tests/cases/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/amend/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_graph_04.txt` & `stepup-1.2.3/tests/cases/amend/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/amend/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/expected_stdout_03.txt` & `stepup-1.2.3/tests/cases/amend/expected_stdout_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend/main.sh` & `stepup-1.2.3/tests/cases/amend/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 grep word1 out1.txt
 grep word2 out2.txt
 
 # Wait for background processes, if any.
 wait
 
 # Restart StepUp without changes
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -73,14 +74,15 @@
 grep word2 out2.txt
 
 # Wait for background processes, if any.
 wait
 
 # Restart StepUp with changes
 echo "word2 and other" > inp2.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_03.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/amend_delay/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/amend_delay/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_delay/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/amend_delay/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_delay/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/amend_delay/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_delay/expected_stdout.txt` & `stepup-1.2.3/tests/cases/amend_delay/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_delay/main.sh` & `stepup-1.2.3/tests/cases/amend_delay/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_env_vars/expected_graph.txt` & `stepup-1.2.3/tests/cases/amend_env_vars/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_env_vars/main.sh` & `stepup-1.2.3/tests/cases/amend_env_vars/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_missing/expected_graph.txt` & `stepup-1.2.3/tests/cases/amend_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_missing/expected_stdout.txt` & `stepup-1.2.3/tests/cases/amend_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_missing/main.sh` & `stepup-1.2.3/tests/cases/amend_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_outdir_pending/expected_graph.txt` & `stepup-1.2.3/tests/cases/amend_outdir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_outdir_pending/expected_stdout.txt` & `stepup-1.2.3/tests/cases/amend_outdir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_outdir_pending/main.sh` & `stepup-1.2.3/tests/cases/amend_outdir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_voldir_pending/expected_graph.txt` & `stepup-1.2.3/tests/cases/amend_voldir_pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_voldir_pending/expected_stdout.txt` & `stepup-1.2.3/tests/cases/amend_voldir_pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/amend_voldir_pending/main.sh` & `stepup-1.2.3/tests/cases/amend_voldir_pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob1/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob1/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/deferred_glob1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob1/main.sh` & `stepup-1.2.3/tests/cases/deferred_glob1/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 grep foo copy.txt
 
 # Wait for background processes, if any.
 wait
 
 # Restart the example with a different input
 export ENV_VAR_TEST_STEPUP_INP="static/sub/bar.txt"
+rm -r .stepup/logs
 stepup -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/deferred_glob2/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob2/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/deferred_glob2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob2/expected_stdout.txt` & `stepup-1.2.3/tests/cases/deferred_glob2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_glob2/main.sh` & `stepup-1.2.3/tests/cases/deferred_glob2/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_subdir/expected_graph.txt` & `stepup-1.2.3/tests/cases/deferred_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/deferred_subdir/main.sh` & `stepup-1.2.3/tests/cases/deferred_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_graph_04.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_graph_05.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_graph_05.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_stdout_a.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_stdout_b.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_stdout_c.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_stdout_c.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/expected_stdout_d.txt` & `stepup-1.2.3/tests/cases/env_vars/expected_stdout_d.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars/main.sh` & `stepup-1.2.3/tests/cases/env_vars/main.sh`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 [[ -f plan.py ]] || exit -1
 grep AAAA current_variables.txt
 grep BBBB current_variables.txt
 cp current_variables.txt current_variables_03.txt
 
 # Change a variable and restart
 export ENV_VAR_TEST_STEPUP_DFTHYH="CCCC"
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -89,14 +90,15 @@
 [[ -f plan.py ]] || exit -1
 grep AAAA current_variables.txt
 grep CCCC current_variables.txt
 cp current_variables.txt current_variables_04.txt
 
 # unset a variable and restart
 unset ENV_VAR_TEST_STEPUP_AWDFTD
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_c.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -115,14 +117,15 @@
 cp current_variables.txt current_variables_05.txt
 
 # Wait for background processes, if any.
 wait
 
 # Set a variable again and restart
 export ENV_VAR_TEST_STEPUP_AWDFTD="DDDD"
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_d.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/env_vars_amend/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_amend/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/env_vars_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_amend/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/env_vars_amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_amend/main.sh` & `stepup-1.2.3/tests/cases/env_vars_amend/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 grep AAAA output.txt
 
 # Wait for background processes, if any.
 wait
 
 # Rerstart with changed variable
 export ENV_VAR_TEST_STEPUP_SDASFD="BBBB"
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/env_vars_path/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/env_vars_path/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_path/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/env_vars_path/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_path/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_path/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/env_vars_path/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_path/main.sh` & `stepup-1.2.3/tests/cases/permissions_plan_restart/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the example
-export ENV_VAR_TEST_STEPUP_PREFIX="README"
+# Run the plan with non-executable step.py.
+chmod -x sub/plan.py
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Get the graph after completion of the pending steps.
+# Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_01")
 join()
 EOD
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ -f README-stdout.txt ]] || exit -1
-[[ -f README-stderr.txt ]] || exit -1
-
 # Wait for background processes, if any.
 wait
 
-# Restart the example with a different variable
-export ENV_VAR_TEST_STEPUP_PREFIX="FOO"
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ ! -f sub/done.txt ]] || exit -1
+
+# Restart the plan with executable step.py.
+chmod +x sub/plan.py
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Get the graph after completion of the pending steps.
+# Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_02")
 join()
 EOD
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ ! -f README-stdout.txt ]] || exit -1
-[[ ! -f README-stderr.txt ]] || exit -1
-[[ -f FOO-stdout.txt ]] || exit -1
-[[ -f FOO-stderr.txt ]] || exit -1
-
 # Wait for background processes, if any.
 wait
+
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ -f sub/plan.py ]] || exit -1
+[[ -f sub/done.txt ]] || exit -1
```

### Comparing `stepup-1.2.2/tests/cases/env_vars_subs/expected_graph.txt` & `stepup-1.2.3/tests/cases/env_vars_subs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_subs/expected_stdout.txt` & `stepup-1.2.3/tests/cases/env_vars_subs/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_subs/main.sh` & `stepup-1.2.3/tests/cases/env_vars_subs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_workdir/expected_graph.txt` & `stepup-1.2.3/tests/cases/env_vars_workdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/env_vars_workdir/main.sh` & `stepup-1.2.3/tests/cases/env_vars_workdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_cyclic_late/expected_graph.txt` & `stepup-1.2.3/tests/cases/error_cyclic_late/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_cyclic_late/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_cyclic_late/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_cyclic_late/main.sh` & `stepup-1.2.3/tests/cases/error_cyclic_late/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_deferred_nonexisting/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_deferred_nonexisting/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_deferred_nonexisting/main.sh` & `stepup-1.2.3/tests/cases/error_deferred_nonexisting/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_env_var/expected_graph.txt` & `stepup-1.2.3/tests/cases/error_env_var/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_env_var/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_env_var/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_env_var/main.sh` & `stepup-1.2.3/tests/cases/error_env_var/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_main_fails/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/error_main_fails/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_main_fails/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/error_main_fails/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_main_fails/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/error_main_fails/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_main_fails/main.sh` & `stepup-1.2.3/tests/cases/error_main_fails/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f output.txt ]] || exit -1
 
 # Run the example, version 2
 cp plan_02.py plan.py
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/error_not_executable/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_not_executable/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_overlap_deferred/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_overlap_deferred/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_overlap_deferred/main.sh` & `stepup-1.2.3/tests/cases/error_overlap_deferred/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_static_dir/expected_graph.txt` & `stepup-1.2.3/tests/cases/error_static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_static_dir/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_static_dir/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_static_dir/main.sh` & `stepup-1.2.3/tests/cases/error_static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_step/expected_graph.txt` & `stepup-1.2.3/tests/cases/error_step/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_step/expected_stdout.txt` & `stepup-1.2.3/tests/cases/error_step/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/error_step/main.sh` & `stepup-1.2.3/tests/cases/error_step/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/here/expected_graph.txt` & `stepup-1.2.3/tests/cases/here/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/here/expected_stdout.txt` & `stepup-1.2.3/tests/cases/here/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/here/main.sh` & `stepup-1.2.3/tests/cases/here/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/makedirs/expected_graph.txt` & `stepup-1.2.3/tests/cases/makedirs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/makedirs/main.sh` & `stepup-1.2.3/tests/cases/makedirs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/mkdir/expected_graph.txt` & `stepup-1.2.3/tests/cases/mkdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/mkdir/main.sh` & `stepup-1.2.3/tests/cases/mkdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/mkdir_error/expected_graph.txt` & `stepup-1.2.3/tests/cases/mkdir_error/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/mkdir_error/expected_stdout.txt` & `stepup-1.2.3/tests/cases/mkdir_error/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/mkdir_error/main.sh` & `stepup-1.2.3/tests/cases/mkdir_error/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/nodata/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/nodata/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/nodata/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/expected_stdout_a.txt` & `stepup-1.2.3/tests/cases/nodata/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/expected_stdout_b.txt` & `stepup-1.2.3/tests/cases/nodata/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nodata/main.sh` & `stepup-1.2.3/tests/cases/nodata/main.sh`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 [[ -f analyzed.txt ]] || exit -1
 
 # Wait for background processes, if any.
 wait
 
 # Create file again and restart
 cp original.txt data.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/noplan/expected_stdout.txt` & `stepup-1.2.3/tests/cases/noplan/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nostatic/expected_graph.txt` & `stepup-1.2.3/tests/cases/nostatic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nostatic/expected_stdout.txt` & `stepup-1.2.3/tests/cases/nostatic/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/nostatic/main.sh` & `stepup-1.2.3/tests/cases/nostatic/main.sh`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f first.txt ]] || exit -1
 [[ -f second.txt ]] || exit -1
 
 # Start stepup without checking expected output because watchdog file
 # order is not reproducible.
+rm -r .stepup/logs
 stepup -w 1 plan.py &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/not_cyclic/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/not_cyclic/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/not_cyclic/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/not_cyclic/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/not_cyclic/expected_stdout.txt` & `stepup-1.2.3/tests/cases/not_cyclic/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/not_cyclic/main.sh` & `stepup-1.2.3/tests/cases/not_cyclic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/optional_convert/expected_graph_a.txt` & `stepup-1.2.3/tests/cases/optional_convert/expected_graph_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/optional_convert/expected_graph_b.txt` & `stepup-1.2.3/tests/cases/optional_convert/expected_graph_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/optional_convert/expected_graph_c.txt` & `stepup-1.2.3/tests/cases/optional_convert/expected_graph_c.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/optional_convert/expected_stdout_a.txt` & `stepup-1.2.3/tests/cases/optional_convert/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/optional_convert/main.sh` & `stepup-1.2.3/tests/cases/optional_convert/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 grep raw_03 used.txt
 [[ ! -f converted_01.txt ]] || exit -1
 [[ ! -f converted_02.txt ]] || exit -1
 [[ ! -f converted_04.txt ]] || exit -1
 
 # Restart with a different environment variables
 export ENV_VAR_TEST_STEPUP_IDX="1"
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/output_not_created/expected_graph.txt` & `stepup-1.2.3/tests/cases/output_not_created/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/output_not_created/expected_stdout.txt` & `stepup-1.2.3/tests/cases/output_not_created/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/output_not_created/main.sh` & `stepup-1.2.3/tests/cases/output_not_created/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/pending/expected_graph.txt` & `stepup-1.2.3/tests/cases/pending/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/pending/expected_stdout.txt` & `stepup-1.2.3/tests/cases/pending/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/pending/main.sh` & `stepup-1.2.3/tests/cases/pending/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_file_rerun/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_file_rerun/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_file_rerun/expected_stdout.txt` & `stepup-1.2.3/tests/cases/permissions_file_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_file_rerun/main.sh` & `stepup-1.2.3/tests/cases/permissions_file_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_rerun/expected_stdout.txt` & `stepup-1.2.3/tests/cases/permissions_plan_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_rerun/main.sh` & `stepup-1.2.3/tests/cases/permissions_plan_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_restart/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_restart/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_restart/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_restart/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/permissions_plan_restart/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_plan_restart/main.sh` & `stepup-1.2.3/tests/cases/restart_blocked/main.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the plan with non-executable step.py.
-chmod -x sub/plan.py
-stepup -e -w 1 plan.py & # > current_stdout_01.txt &
+# Run the initial plan.
+cp plan_blocked.py plan.py
+stepup -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Wait and get graph.
+# First graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_01")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait
 
-# Check files that are expected to be present and/or missing.
-[[ -f plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ ! -f sub/done.txt ]] || exit -1
-
-# Restart the plan with executable step.py.
-chmod +x sub/plan.py
-stepup -e -w 1 plan.py & # > current_stdout_02.txt &
+[[ -f initial.txt ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ ! -f output.txt ]] || exit -1
+[[ ! -f final.txt ]] || exit -1
+
+# Modify a few things and restart
+cp plan_unblocked.py plan.py
+rm -r .stepup/logs
+stepup -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Wait and get graph.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ -f sub/plan.py ]] || exit -1
-[[ -f sub/done.txt ]] || exit -1
+[[ -f initial.txt ]] || exit -1
+[[ -f input.txt ]] || exit -1
+[[ -f output.txt ]] || exit -1
+[[ -f final.txt ]] || exit -1
```

### Comparing `stepup-1.2.2/tests/cases/permissions_step_rerun/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_rerun/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_rerun/expected_stdout.txt` & `stepup-1.2.3/tests/cases/permissions_step_rerun/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_rerun/main.sh` & `stepup-1.2.3/tests/cases/permissions_step_rerun/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_restart/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_restart/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/permissions_step_restart/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_restart/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_restart/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/permissions_step_restart/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/permissions_step_restart/main.sh` & `stepup-1.2.3/tests/cases/env_vars_path/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the plan with non-executable step.py.
-chmod -x step.py
+# Run the example
+export ENV_VAR_TEST_STEPUP_PREFIX="README"
 stepup -e -w 1 plan.py & # > current_stdout_01.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Wait and get graph.
+# Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_01")
 join()
 EOD
 
-# Wait for background processes, if any.
-wait
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f step.py ]] || exit -1
-[[ ! -f message.txt ]] || exit -1
+[[ -f README-stdout.txt ]] || exit -1
+[[ -f README-stderr.txt ]] || exit -1
+
+# Wait for background processes, if any.
+wait
 
-# Restart the plan with executable step.py.
-chmod +x step.py
+# Restart the example with a different variable
+export ENV_VAR_TEST_STEPUP_PREFIX="FOO"
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# Wait and get graph.
+# Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_02")
 join()
 EOD
 
-# Wait for background processes, if any.
-wait
-
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f step.py ]] || exit -1
-[[ -f message.txt ]] || exit -1
+[[ ! -f README-stdout.txt ]] || exit -1
+[[ ! -f README-stderr.txt ]] || exit -1
+[[ -f FOO-stdout.txt ]] || exit -1
+[[ -f FOO-stderr.txt ]] || exit -1
+
+# Wait for background processes, if any.
+wait
```

### Comparing `stepup-1.2.2/tests/cases/pool/expected_graph.txt` & `stepup-1.2.3/tests/cases/pool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/pool/main.sh` & `stepup-1.2.3/tests/cases/pool/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/reqdir_missing/expected_graph.txt` & `stepup-1.2.3/tests/cases/reqdir_missing/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/reqdir_missing/expected_stdout.txt` & `stepup-1.2.3/tests/cases/reqdir_missing/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/reqdir_missing/main.sh` & `stepup-1.2.3/tests/cases/reqdir_missing/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_blocked/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_blocked/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_blocked/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_blocked/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_blocked/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_blocked/main.sh` & `stepup-1.2.3/tests/cases/watch_boot/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the initial plan.
-cp plan_blocked.py plan.py
-stepup -w 1 plan.py & # > current_stdout_01.txt &
+cp -a plan_01.py plan.py
+stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-# First graph
+# Initial graph
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_01")
-join()
 EOD
 
-# Wait for background processes, if any.
-wait
-
-[[ -f initial.txt ]] || exit -1
-[[ -f input.txt ]] || exit -1
-[[ ! -f output.txt ]] || exit -1
-[[ ! -f final.txt ]] || exit -1
-
-# Modify a few things and restart
-cp plan_unblocked.py plan.py
-stepup -w 1 plan.py & # > current_stdout_02.txt &
-
-# Wait for the director and get its socket.
-export STEPUP_DIRECTOR_SOCKET=$(
-  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
-)
+# Check files that are expected to be present and/or missing.
+[[ -f plan.py ]] || exit -1
+[[ -f first.txt ]] || exit -1
+[[ -f final.txt ]] || exit -1
 
+# Modify the plan.py script and rerun with the modified plan.py.
+cp -a plan_02.py plan.py
 python3 - << EOD
 from stepup.core.interact import *
+watch_update("plan.py")
+run()
 wait()
 graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f initial.txt ]] || exit -1
-[[ -f input.txt ]] || exit -1
-[[ -f output.txt ]] || exit -1
+[[ ! -f first.txt ]] || exit -1
+[[ -f second.txt ]] || exit -1
 [[ -f final.txt ]] || exit -1
```

### Comparing `stepup-1.2.2/tests/cases/restart_changes/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_changes/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_changes/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_changes/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_changes/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_changes/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_changes/main.sh` & `stepup-1.2.3/tests/cases/restart_changes/main.sh`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 [[ -f copy_01.txt ]] || exit -1
 [[ -f copy_both1.txt ]] || exit -1
 [[ -f source_both.txt ]] || exit -1
 [[ -f source_01.txt ]] || exit -1
 
 # second with a different plan.
 echo
+rm -r .stepup/logs
 stepup -e -w 1 plan_02.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/restart_deferred_glob/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_deferred_glob/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_deferred_glob/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_deferred_glob/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_deferred_glob/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_deferred_glob/main.sh` & `stepup-1.2.3/tests/cases/restart_orphan/main.sh`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f static/foo.txt ]] || exit -1
+[[ -f foo.txt ]] || exit -1
+[[ -f bar.txt ]] || exit -1
 
 # Run the plan.
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -44,8 +46,9 @@
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f static/foo.txt ]] || exit -1
+[[ -f foo.txt ]] || exit -1
+[[ -f bar.txt ]] || exit -1
```

### Comparing `stepup-1.2.2/tests/cases/restart_nochanges/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_nochanges/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_nochanges/expected_stdout_01.txt` & `stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_nochanges/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_nochanges/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_nochanges/main.sh` & `stepup-1.2.3/tests/cases/restart_nochanges/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f single.txt ]] || exit -1
 [[ -f double.txt ]] || exit -1
 [[ -f quadruple.txt ]] || exit -1
 
 # Run the plan.
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/restart_orphan/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_orphan/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_orphan/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_orphan/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_orphan/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_orphan/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_orphan/main.sh` & `stepup-1.2.3/tests/cases/restart_deferred_glob/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f foo.txt ]] || exit -1
-[[ -f bar.txt ]] || exit -1
+[[ -f static/foo.txt ]] || exit -1
 
 # Run the plan.
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
@@ -45,9 +45,8 @@
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f foo.txt ]] || exit -1
-[[ -f bar.txt ]] || exit -1
+[[ -f static/foo.txt ]] || exit -1
```

### Comparing `stepup-1.2.2/tests/cases/restart_outdated_amend/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_outdated_amend/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_outdated_amend/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_outdated_amend/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_outdated_amend/main.sh` & `stepup-1.2.3/tests/cases/restart_outdated_amend/main.sh`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 [[ -f copy.txt ]] || exit -1
 grep inp1 copy.txt
 
 # Change subs.txt and rerstart.
 rm inp1.txt
 echo inp2 > inp2.txt
 echo inp2.txt > subs.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/restart_output/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/restart_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_output/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/restart_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_output/expected_stdout_02.txt` & `stepup-1.2.3/tests/cases/restart_output/expected_stdout_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/restart_output/main.sh` & `stepup-1.2.3/tests/cases/restart_output/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f original.txt ]] || exit -1
 [[ -f copy.txt ]] || exit -1
 
 # Restart StepUp after removing the output.
 rm copy.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_02.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/script_cases/expected_graph.txt` & `stepup-1.2.3/tests/cases/script_cases/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_cases/main.sh` & `stepup-1.2.3/tests/cases/script_cases/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_cases_settings/README.md` & `stepup-1.2.3/tests/cases/script_cases_settings/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_cases_settings/expected_graph.txt` & `stepup-1.2.3/tests/cases/script_cases_settings/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_cases_settings/main.sh` & `stepup-1.2.3/tests/cases/script_cases_settings/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_single/expected_graph.txt` & `stepup-1.2.3/tests/cases/script_single/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_single/expected_stdout.txt` & `stepup-1.2.3/tests/cases/script_single/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_single/main.sh` & `stepup-1.2.3/tests/cases/script_single/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/script_single/work/generate.py` & `stepup-1.2.3/tests/cases/script_single/work/generate.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static/expected_graph.txt` & `stepup-1.2.3/tests/cases/static/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static/main.sh` & `stepup-1.2.3/tests/cases/static/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_abs/expected_graph.txt` & `stepup-1.2.3/tests/cases/static_abs/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_abs/main.sh` & `stepup-1.2.3/tests/cases/static_abs/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_dir/expected_graph.txt` & `stepup-1.2.3/tests/cases/static_dir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_dir/main.sh` & `stepup-1.2.3/tests/cases/static_dir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/static_glob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/static_glob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/static_glob/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/expected_stdout_a.txt` & `stepup-1.2.3/tests/cases/static_glob/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/expected_stdout_b.txt` & `stepup-1.2.3/tests/cases/static_glob/expected_stdout_b.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_glob/main.sh` & `stepup-1.2.3/tests/cases/static_glob/main.sh`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 # Wait for background processes, if any.
 wait
 
 # Modify nglob results and restart
 echo "Fourth input" > inp4.txt
 rm inp2.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/static_nglob/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/static_nglob/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/static_nglob/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob/expected_stdout.txt` & `stepup-1.2.3/tests/cases/static_nglob/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob/main.sh` & `stepup-1.2.3/tests/cases/static_nglob/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 [[ -f ch-3-conclusions/sec-3-1-summary.md ]] || exit -1
 [[ -f ch-3-conclusions/sec-3-2-outlook.md ]] || exit -1
 [[ -f ch-3-conclusions/ch-3-compiled.md ]] || exit -1
 [[ -f book.md ]] || exit -1
 
 # Start stepup without checking expected output because watchdog file
 # order is not reproducible.
+rm -r .stepup/logs
 stepup -w 1 plan.py &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
```

### Comparing `stepup-1.2.2/tests/cases/static_nglob/plan.py` & `stepup-1.2.3/tests/cases/static_nglob/plan.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_graph_04.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_graph_04.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_stdout_a.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_a.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/expected_stdout_b.txt` & `stepup-1.2.3/tests/cases/static_nglob_partial/expected_stdout_b.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 Same out hash        paste_x.txt
 ────────────────────────────────────────────────────────────────────────────────
      START │ paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
    SUCCESS │ paste -d ' ' head_y.txt tail_y.txt > paste_y.txt
      START │ paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
    SUCCESS │ paste -d ' ' head_z.txt tail_z.txt > paste_z.txt
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-   UPDATED │ tail_y.txt
-   UPDATED │ tail_z.txt
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup-1.2.2/tests/cases/static_nglob_partial/main.sh` & `stepup-1.2.3/tests/cases/static_nglob_partial/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -69,32 +69,33 @@
 [[ ! -f paste_y.txt ]] || exit -1
 [[ ! -f paste_z.txt ]] || exit -1
 
 # Wait for background processes, if any.
 wait
 
 # Modify nglob results and restart
+echo "ty" > tail_y.txt
+echo "tz" > tail_z.txt
+rm -r .stepup/logs
 stepup -e -w 1 plan.py & # > current_stdout_b.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
-echo "ty" > tail_y.txt
-echo "tz" > tail_z.txt
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_04")
 join()
 EOD
 
+# Wait for background processes, if any.
+wait
+
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ ! -f paste_ignored.txt ]] || exit -1
 grep 'hx tx' paste_x.txt
 grep 'hy ty' paste_y.txt
 grep 'hz tz' paste_z.txt
-
-# Wait for background processes, if any.
-wait
```

### Comparing `stepup-1.2.2/tests/cases/static_nglob_subdir/expected_graph.txt` & `stepup-1.2.3/tests/cases/static_nglob_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/static_nglob_subdir/main.sh` & `stepup-1.2.3/tests/cases/static_nglob_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/subdir/expected_graph.txt` & `stepup-1.2.3/tests/cases/subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/subdir/expected_stdout.txt` & `stepup-1.2.3/tests/cases/subdir/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/subdir/main.sh` & `stepup-1.2.3/tests/cases/subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_blocked/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_blocked/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_blocked/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_blocked/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_blocked/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_blocked/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_blocked/main.sh` & `stepup-1.2.3/tests/cases/watch_blocked/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_boot/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_boot/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_boot/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_boot/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_boot/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_boot/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_boot/main.sh` & `stepup-1.2.3/tests/cases/watch_outdated_amend2/main.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
-# Run the initial plan.
-cp -a plan_01.py plan.py
-stepup -w 1 plan.py & # > current_stdout.txt &
+# Run with the initial subs.txt.
+echo inp1 > inp1.txt
+echo conv1.txt > subs1.txt
+stepup -e -w 1 plan.py & # > current_stdout.txt &
 
 # Wait for the director and get its socket.
 export STEPUP_DIRECTOR_SOCKET=$(
   python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
 )
 
 # Initial graph
@@ -18,29 +19,40 @@
 from stepup.core.interact import *
 wait()
 graph("current_graph_01")
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f first.txt ]] || exit -1
-[[ -f final.txt ]] || exit -1
-
-# Modify the plan.py script and rerun with the modified plan.py.
-cp -a plan_02.py plan.py
+[[ -f inp1.txt ]] || exit -1
+[[ -f subs1.txt ]] || exit -1
+[[ -f subs2.txt ]] || exit -1
+grep conv1.txt subs2.txt
+[[ -f subs3.txt ]] || exit -1
+grep conv1.txt subs3.txt
+
+# Change subs.txt and rerun.
+rm inp1.txt
+echo inp2 > inp2.txt
+echo conv2.txt > subs1.txt
 python3 - << EOD
 from stepup.core.interact import *
-watch_update("plan.py")
+watch_update("subs1.txt")
+watch_delete("inp1.txt")
 run()
 wait()
 graph("current_graph_02")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ ! -f first.txt ]] || exit -1
-[[ -f second.txt ]] || exit -1
-[[ -f final.txt ]] || exit -1
+[[ ! -f inp1.txt ]] || exit -1
+[[ -f inp2.txt ]] || exit -1
+[[ -f subs1.txt ]] || exit -1
+[[ -f subs2.txt ]] || exit -1
+grep conv2.txt subs2.txt
+[[ -f subs3.txt ]] || exit -1
+grep conv2.txt subs3.txt
```

### Comparing `stepup-1.2.2/tests/cases/watch_chain/README.md` & `stepup-1.2.3/tests/cases/watch_chain/README.md`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_chain/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_chain/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_chain/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_chain/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_chain/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_chain/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_chain/main.sh` & `stepup-1.2.3/tests/cases/watch_chain/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_chain/use_config.py` & `stepup-1.2.3/tests/cases/watch_chain/use_config.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_input/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_input/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_input/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_input/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_input/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/watch_input/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_input/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_input/main.sh` & `stepup-1.2.3/tests/cases/watch_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_middle/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_middle/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_middle/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_middle/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_middle/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/watch_middle/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_middle/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_middle/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_middle/main.sh` & `stepup-1.2.3/tests/cases/watch_middle/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_mixed/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_mixed/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_mixed/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_mixed/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_mixed/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_mixed/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_mixed/main.sh` & `stepup-1.2.3/tests/cases/watch_mixed/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_nochanges/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_nochanges/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_nochanges/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_nochanges/main.sh` & `stepup-1.2.3/tests/cases/watch_nochanges/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend1/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend1/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend1/main.sh` & `stepup-1.2.3/tests/cases/watch_outdated_amend1/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_outdated_amend2/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_outdated_amend2/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_output/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_output/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_output/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_output/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_output/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_output/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_output/main.sh` & `stepup-1.2.3/tests/cases/watch_output/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_wanted/expected_graph_01.txt` & `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_wanted/expected_graph_02.txt` & `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_wanted/expected_graph_03.txt` & `stepup-1.2.3/tests/cases/watch_wanted/expected_graph_03.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_wanted/expected_stdout.txt` & `stepup-1.2.3/tests/cases/watch_wanted/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/cases/watch_wanted/main.sh` & `stepup-1.2.3/tests/cases/watch_wanted/main.sh`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/conftest.py` & `stepup-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/core_common.py` & `stepup-1.2.3/tests/core_common.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/echo_server_socket.py` & `stepup-1.2.3/tests/echo_server_socket.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/echo_server_stdio.py` & `stepup-1.2.3/tests/echo_server_stdio.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_assoc.py` & `stepup-1.2.3/tests/test_assoc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_basics.py` & `stepup-1.2.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_cascade.py` & `stepup-1.2.3/tests/test_cascade.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_cases.py` & `stepup-1.2.3/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_nglob.py` & `stepup-1.2.3/tests/test_nglob.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_rpc.py` & `stepup-1.2.3/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_scheduler.py` & `stepup-1.2.3/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_utils.py` & `stepup-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stepup-1.2.2/tests/test_workflow.py` & `stepup-1.2.3/tests/test_workflow.py`

 * *Files identical despite different names*

