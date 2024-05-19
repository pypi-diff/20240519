# Comparing `tmp/beangrep-0.4.0.tar.gz` & `tmp/beangrep-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beangrep-0.4.0.tar", last modified: Sat May 18 07:19:02 2024, max compression
+gzip compressed data, was "beangrep-0.5.0.tar", last modified: Sun May 19 15:01:06 2024, max compression
```

## Comparing `beangrep-0.4.0.tar` & `beangrep-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.558627 beangrep-0.4.0/
--rw-r--r--   0 zack      (1000) zack      (1000)       56 2024-05-17 15:18:49.000000 beangrep-0.4.0/.coveragerc
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/.github/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/.github/workflows/
--rw-r--r--   0 zack      (1000) zack      (1000)     1377 2024-05-13 07:53:11.000000 beangrep-0.4.0/.github/workflows/python-package.yml
--rw-r--r--   0 zack      (1000) zack      (1000)      111 2024-05-17 16:21:49.000000 beangrep-0.4.0/.gitignore
--rw-r--r--   0 zack      (1000) zack      (1000)      651 2024-05-14 13:14:24.000000 beangrep-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.4.0/LICENSE-GPL-2.0-or-later
--rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:16:41.000000 beangrep-0.4.0/Makefile
--rw-r--r--   0 zack      (1000) zack      (1000)     8860 2024-05-18 07:19:02.558627 beangrep-0.4.0/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)     7787 2024-05-18 07:17:44.000000 beangrep-0.4.0/README.md
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/bin/
--rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.4.0/bin/bean-grep
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/data/
--rw-r--r--   0 zack      (1000) zack      (1000)      397 2024-05-17 16:21:49.000000 beangrep-0.4.0/data/man-extras.h2m
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/dev/
--rwxr-xr-x   0 zack      (1000) zack      (1000)       63 2024-05-17 15:23:37.000000 beangrep-0.4.0/dev/coverage
--rwxr-xr-x   0 zack      (1000) zack      (1000)      562 2024-05-17 15:23:37.000000 beangrep-0.4.0/dev/update-readme
--rw-r--r--   0 zack      (1000) zack      (1000)     1243 2024-05-17 16:21:49.000000 beangrep-0.4.0/pyproject.toml
--rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-18 07:19:02.558627 beangrep-0.4.0/setup.cfg
--rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.4.0/setup.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/beangrep/
--rw-r--r--   0 zack      (1000) zack      (1000)      263 2024-05-12 10:30:41.000000 beangrep-0.4.0/src/beangrep/__init__.py
--rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.4.0/src/beangrep/__main__.py
--rw-r--r--   0 zack      (1000) zack      (1000)    33230 2024-05-18 07:03:01.000000 beangrep-0.4.0/src/beangrep/beangrep.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/beangrep/data/
--rw-r--r--   0 zack      (1000) zack      (1000)        0 2024-05-17 16:21:49.000000 beangrep-0.4.0/src/beangrep/data/.gitkeep
--rw-r--r--   0 zack      (1000) zack      (1000)     4894 2024-05-18 07:19:01.000000 beangrep-0.4.0/src/beangrep/data/bean-grep.1
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.558627 beangrep-0.4.0/src/beangrep.egg-info/
--rw-r--r--   0 zack      (1000) zack      (1000)     8860 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)      681 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/SOURCES.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/dependency_links.txt
--rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/entry_points.txt
--rw-r--r--   0 zack      (1000) zack      (1000)      102 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/requires.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/top_level.txt
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/data/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/data/documents/
--rw-r--r--   0 zack      (1000) zack      (1000)       40 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/data/documents/statements.txt
--rw-r--r--   0 zack      (1000) zack      (1000)   347380 2024-05-14 09:41:00.000000 beangrep-0.4.0/tests/data/example.beancount
--rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/data/small.beancount
--rw-r--r--   0 zack      (1000) zack      (1000)    18680 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/test_beangrep.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/
+-rw-r--r--   0 zack      (1000) zack      (1000)       56 2024-05-17 15:18:49.000000 beangrep-0.5.0/.coveragerc
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/.github/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/.github/workflows/
+-rw-r--r--   0 zack      (1000) zack      (1000)     1375 2024-05-19 11:47:38.000000 beangrep-0.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zack      (1000) zack      (1000)      111 2024-05-17 16:21:49.000000 beangrep-0.5.0/.gitignore
+-rw-r--r--   0 zack      (1000) zack      (1000)      651 2024-05-14 13:14:24.000000 beangrep-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.5.0/LICENSE-GPL-2.0-or-later
+-rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:16:41.000000 beangrep-0.5.0/Makefile
+-rw-r--r--   0 zack      (1000) zack      (1000)     9887 2024-05-19 15:01:06.593736 beangrep-0.5.0/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)     8814 2024-05-19 14:57:30.000000 beangrep-0.5.0/README.md
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/bin/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.5.0/bin/bean-grep
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/data/
+-rw-r--r--   0 zack      (1000) zack      (1000)      397 2024-05-17 16:21:49.000000 beangrep-0.5.0/data/man-extras.h2m
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/dev/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)       63 2024-05-17 15:23:37.000000 beangrep-0.5.0/dev/coverage
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      465 2024-05-19 14:57:57.000000 beangrep-0.5.0/dev/tag-release
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      562 2024-05-17 15:23:37.000000 beangrep-0.5.0/dev/update-readme
+-rw-r--r--   0 zack      (1000) zack      (1000)     1243 2024-05-17 16:21:49.000000 beangrep-0.5.0/pyproject.toml
+-rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-19 15:01:06.593736 beangrep-0.5.0/setup.cfg
+-rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.5.0/setup.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/src/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/src/beangrep/
+-rw-r--r--   0 zack      (1000) zack      (1000)      297 2024-05-18 14:01:02.000000 beangrep-0.5.0/src/beangrep/__init__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.5.0/src/beangrep/__main__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)    27002 2024-05-19 14:57:29.000000 beangrep-0.5.0/src/beangrep/beangrep.py
+-rw-r--r--   0 zack      (1000) zack      (1000)    10740 2024-05-19 14:54:28.000000 beangrep-0.5.0/src/beangrep/cli.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/src/beangrep/data/
+-rw-r--r--   0 zack      (1000) zack      (1000)        0 2024-05-17 16:21:49.000000 beangrep-0.5.0/src/beangrep/data/.gitkeep
+-rw-r--r--   0 zack      (1000) zack      (1000)     5751 2024-05-19 15:01:02.000000 beangrep-0.5.0/src/beangrep/data/bean-grep.1
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/src/beangrep.egg-info/
+-rw-r--r--   0 zack      (1000) zack      (1000)     9887 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)      735 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/SOURCES.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/dependency_links.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/entry_points.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)      102 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/requires.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-19 15:01:06.000000 beangrep-0.5.0/src/beangrep.egg-info/top_level.txt
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/tests/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/tests/data/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-19 15:01:06.593736 beangrep-0.5.0/tests/data/documents/
+-rw-r--r--   0 zack      (1000) zack      (1000)       40 2024-05-18 07:03:01.000000 beangrep-0.5.0/tests/data/documents/statements.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)   347380 2024-05-14 09:41:00.000000 beangrep-0.5.0/tests/data/example.beancount
+-rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:03:01.000000 beangrep-0.5.0/tests/data/small.beancount
+-rw-r--r--   0 zack      (1000) zack      (1000)    12388 2024-05-18 18:05:14.000000 beangrep-0.5.0/tests/test_beangrep.py
+-rw-r--r--   0 zack      (1000) zack      (1000)     9296 2024-05-19 11:47:38.000000 beangrep-0.5.0/tests/test_cli.py
```

### Comparing `beangrep-0.4.0/.github/workflows/python-package.yml` & `beangrep-0.5.0/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: build
 
 on:
   push:
-    branches: [ "main" ]
+    branches: [ "**" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
```

### Comparing `beangrep-0.4.0/.pre-commit-config.yaml` & `beangrep-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/LICENSE-GPL-2.0-or-later` & `beangrep-0.5.0/LICENSE-GPL-2.0-or-later`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/Makefile` & `beangrep-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/PKG-INFO` & `beangrep-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.4.0
+Version: 0.5.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -81,23 +81,20 @@
 ```
 Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
   Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
-  explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
-  date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
-  account (start with an account type, e.g., "Assets", "Income", etc.),
-  metadata pair ("key:value"), or string to be matched anywhere (see
-  -s/--somewhere below), in this order. If PATTERN is not given, search
-  criteria are defined by explicit options.
+  explicit "smart" PATTERN. If given, PATTERN is interpreted as described
+  below under "Patterns". If not given, search criteria are defined by
+  explicit options.
 
-  Multiple options and/or PATTERN are logically joined (AND-ed) together. In
-  case of overlap, explicit options override PATTERN.
+  Multiple options, options given mutiple times, and PATTERN(s) are logically
+  joined (AND-ed) together.
 
   The granularity of matching (and results) is that of individual entries,
   e.g., full transactions, balances, notes, etc. By default only transactions
   are returned; use the --type/-T option to override.
 
   To read from standard input, pass "-" as FILENAME, but beware that it
   implies on-disk buffering of stdin.
@@ -105,75 +102,108 @@
 Options:
   -a, --account REGEX             Only return entries referencing accounts
                                   with names matching given regex.
   -A, --amount "[OP]AMOUNT [REGEX]"
                                   Only return entries with amounts matching
                                   the given amount predicate. An amount
                                   predicate start with an optional comparison
-                                  operator (one of '<', '<=', '=', '>=', '>',
-                                  with '=' being the default), followed by a
-                                  decimal number (using '.' as decimal
+                                  operator (one of "<", "<=", "=", ">=", ">",
+                                  with "=" being the default), followed by a
+                                  decimal number (using "." as decimal
                                   separator), followed by an optional currency
                                   regex. Multiple amount predicates can be
                                   given to express complex amount ranges.
   -d, --date [OP]DATE             Only return entries with dates matching the
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
-                                  '<', '<=', '=', '>=', '>', with '=' being
+                                  "<", "<=", "=", ">=", ">", with "=" being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
   -l, --link REGEX                Only return entries with at least one link
                                   matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
-                                  separated by ':', the former matching on
+                                  separated by ":", the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
-                                  '.*'.
+                                  ".*".
   -n, --narration REGEX           Only return entries whose narrations match
                                   given regex.
   -p, --payee REGEX               Only return entries whose payees match given
                                   regex.
   -s, --somewhere, --anywhere REGEX
                                   Only return entries with a value in them,
                                   anywhere, matching given regex.
   -t, --tag REGEX                 Only return entries with at least one tag
                                   matching given regex. The tag can be located
                                   anywhere.
-  -T, --type TYPE(S)              Only return entries of certain types. Types
-                                  are specified as a ','-separated list of
+  -T, --type TYPE(S)              Only return entries of certain types.  Types
+                                  are specified as a ","-separated list of
                                   type names; type names are: open, close,
                                   commodity, pad, balance, transaction, note,
                                   event, query, price, document, custom. The
-                                  special value 'all' means: all directive
+                                  special value "all" means: all directive
                                   types. [default: transaction]
-  -i, --ignore-case / --no-ignore-case
-                                  Ignore case distinctions in string matches.
-                                  [default: no-ignore-case]
+  --case-sensitive                Search case sensitively. Overrides:
+                                  -i/--ignore-case and -S/--smart-case.
+  -i, --ignore-case               Search case insensitively. Overrides
+                                  -S/--smart-case; overridden by --case-
+                                  sensitive.
+  -S, --smart-case                Search case insensitively if all criteria
+                                  are lowercase, sensitively otherwise.
+                                  Overridden by: --case-sensitive and
+                                  -i/--ignore-case.  [default: True]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
                                   output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
+  -v, --invert-match              Invert the sense of matching: return entries
+                                  that do *not* match given criteria. This
+                                  clears the default "--type transaction"
+                                  criteria, to avoid only returning non-
+                                  transaction entries by default.
   --verbose                       Increase logging verbosity. Default
                                   verbosity is at WARNING level; passing this
                                   option once will increase it to INFO, twice
                                   or more to DEBUG.
   -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
+  Patterns:
+
+  When given the "smart" PATTERN is interpreted according to the following
+  heuristics, tried in order, first match wins:
+
+  - if it is in the form "YYYY-MM-DD" -> then it is interpreted as --date
+
+  - "#tag" -> --tag
+
+  - "^link" -> --link
+
+  - "@payee" -> --payee
+
+  - if it starts with one of the five account types ("Assets", "Equity",
+  "Expenses",   "Income", "Liabilities") -> --account
+
+  - "key:value" -> --metadata
+
+  - otherwise -> --somewhere
+
+  Exit status:
+
   Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.4.0/README.md` & `beangrep-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,23 +55,20 @@
 ```
 Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
   Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
-  explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
-  date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
-  account (start with an account type, e.g., "Assets", "Income", etc.),
-  metadata pair ("key:value"), or string to be matched anywhere (see
-  -s/--somewhere below), in this order. If PATTERN is not given, search
-  criteria are defined by explicit options.
+  explicit "smart" PATTERN. If given, PATTERN is interpreted as described
+  below under "Patterns". If not given, search criteria are defined by
+  explicit options.
 
-  Multiple options and/or PATTERN are logically joined (AND-ed) together. In
-  case of overlap, explicit options override PATTERN.
+  Multiple options, options given mutiple times, and PATTERN(s) are logically
+  joined (AND-ed) together.
 
   The granularity of matching (and results) is that of individual entries,
   e.g., full transactions, balances, notes, etc. By default only transactions
   are returned; use the --type/-T option to override.
 
   To read from standard input, pass "-" as FILENAME, but beware that it
   implies on-disk buffering of stdin.
@@ -79,75 +76,108 @@
 Options:
   -a, --account REGEX             Only return entries referencing accounts
                                   with names matching given regex.
   -A, --amount "[OP]AMOUNT [REGEX]"
                                   Only return entries with amounts matching
                                   the given amount predicate. An amount
                                   predicate start with an optional comparison
-                                  operator (one of '<', '<=', '=', '>=', '>',
-                                  with '=' being the default), followed by a
-                                  decimal number (using '.' as decimal
+                                  operator (one of "<", "<=", "=", ">=", ">",
+                                  with "=" being the default), followed by a
+                                  decimal number (using "." as decimal
                                   separator), followed by an optional currency
                                   regex. Multiple amount predicates can be
                                   given to express complex amount ranges.
   -d, --date [OP]DATE             Only return entries with dates matching the
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
-                                  '<', '<=', '=', '>=', '>', with '=' being
+                                  "<", "<=", "=", ">=", ">", with "=" being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
   -l, --link REGEX                Only return entries with at least one link
                                   matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
-                                  separated by ':', the former matching on
+                                  separated by ":", the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
-                                  '.*'.
+                                  ".*".
   -n, --narration REGEX           Only return entries whose narrations match
                                   given regex.
   -p, --payee REGEX               Only return entries whose payees match given
                                   regex.
   -s, --somewhere, --anywhere REGEX
                                   Only return entries with a value in them,
                                   anywhere, matching given regex.
   -t, --tag REGEX                 Only return entries with at least one tag
                                   matching given regex. The tag can be located
                                   anywhere.
-  -T, --type TYPE(S)              Only return entries of certain types. Types
-                                  are specified as a ','-separated list of
+  -T, --type TYPE(S)              Only return entries of certain types.  Types
+                                  are specified as a ","-separated list of
                                   type names; type names are: open, close,
                                   commodity, pad, balance, transaction, note,
                                   event, query, price, document, custom. The
-                                  special value 'all' means: all directive
+                                  special value "all" means: all directive
                                   types. [default: transaction]
-  -i, --ignore-case / --no-ignore-case
-                                  Ignore case distinctions in string matches.
-                                  [default: no-ignore-case]
+  --case-sensitive                Search case sensitively. Overrides:
+                                  -i/--ignore-case and -S/--smart-case.
+  -i, --ignore-case               Search case insensitively. Overrides
+                                  -S/--smart-case; overridden by --case-
+                                  sensitive.
+  -S, --smart-case                Search case insensitively if all criteria
+                                  are lowercase, sensitively otherwise.
+                                  Overridden by: --case-sensitive and
+                                  -i/--ignore-case.  [default: True]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
                                   output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
+  -v, --invert-match              Invert the sense of matching: return entries
+                                  that do *not* match given criteria. This
+                                  clears the default "--type transaction"
+                                  criteria, to avoid only returning non-
+                                  transaction entries by default.
   --verbose                       Increase logging verbosity. Default
                                   verbosity is at WARNING level; passing this
                                   option once will increase it to INFO, twice
                                   or more to DEBUG.
   -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
+  Patterns:
+
+  When given the "smart" PATTERN is interpreted according to the following
+  heuristics, tried in order, first match wins:
+
+  - if it is in the form "YYYY-MM-DD" -> then it is interpreted as --date
+
+  - "#tag" -> --tag
+
+  - "^link" -> --link
+
+  - "@payee" -> --payee
+
+  - if it starts with one of the five account types ("Assets", "Equity",
+  "Expenses",   "Income", "Liabilities") -> --account
+
+  - "key:value" -> --metadata
+
+  - otherwise -> --somewhere
+
+  Exit status:
+
   Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.4.0/dev/update-readme` & `beangrep-0.5.0/dev/update-readme`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/pyproject.toml` & `beangrep-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/src/beangrep/beangrep.py` & `beangrep-0.5.0/src/beangrep/beangrep.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,39 +2,70 @@
 # SPDX-License-Identifier: GPL-2.0-or-later
 __copyright__ = "Copyright (C) 2024  Stefano Zacchiroli <zack@upsilon.cc>"
 __license__ = "GPL-2.0-or-later"
 
 import calendar
 import logging
 import re
-import shutil
-import sys
 from collections.abc import Iterable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import date, timedelta
 from decimal import Decimal
 from enum import Enum
-from tempfile import NamedTemporaryFile
 from typing import Optional, Self, cast
 
-import beancount.loader  # type: ignore
-import click
 from beancount.core import data  # type: ignore
 from beancount.core.amount import Amount  # type: ignore
-from beancount.parser import printer  # type: ignore
 
-KEY_VAL_SEP = ":"
 INTERNALS_META = set(["filename", "lineno"])
+KEY_VAL_SEP = ":"
 META_VAL_RE = ".*"
 POSTING_TAGS_META = "tags"
 POSTING_TAGS_SEP = ","
 SKIP_INTERNALS = True
+TYPES_DEFAULT = frozenset([data.Transaction])
 TYPE_SEP = ","
 
 
+class Caseness(Enum):
+    """Case-matching policy."""
+
+    MATCH = 1
+    IGNORE = 2
+    SMART = 3
+
+    @classmethod
+    def from_cli(
+        cls, case_sensitive: bool, ignore_case: bool, smart_case: bool
+    ) -> Self:
+        """Create a CaseMatching enum from CLI arguments, applying overrides."""
+        if case_sensitive:
+            result = cls.MATCH
+        elif ignore_case:
+            result = cls.IGNORE
+        else:
+            result = cls.SMART
+        return cast(Self, result)
+
+    def ignore_case(self, s: str) -> bool:
+        """Check if caseness should be ignored for a given string."""
+        result = False
+        match self:
+            case self.MATCH:
+                result = False
+            case self.IGNORE:
+                result = True
+            case self.SMART:
+                if any(c.isupper() for c in s):
+                    result = False
+                else:
+                    result = True
+        return result
+
+
 class RelOp(Enum):
     """Relational comparison operator."""
 
     EQ = 1  # =
     LT = 2  # <
     GT = 3  # >
     LEQ = 4  # <=
@@ -225,117 +256,148 @@
         return cls(**matches)  # type: ignore  # too dynamic to type properly
 
 
 @dataclass
 class Criteria:
     """Criteria to select matching Beancount entries."""
 
-    account: Optional[re.Pattern] = None
-    amount: Optional[list[AmountPredicate]] = None
-    date: Optional[list[DatePredicate]] = None
-    link: Optional[re.Pattern] = None
-    metadata: Optional[tuple[re.Pattern, re.Pattern]] = None
-    narration: Optional[re.Pattern] = None
-    payee: Optional[re.Pattern] = None
-    somewhere: Optional[re.Pattern] = None
-    tag: Optional[re.Pattern] = None
-    types: Optional[frozenset[type]] = frozenset([data.Transaction])
+    accounts: list[re.Pattern] = field(default_factory=list)
+    amounts: list[AmountPredicate] = field(default_factory=list)
+    dates: list[DatePredicate] = field(default_factory=list)
+    links: list[re.Pattern] = field(default_factory=list)
+    metadatas: list[tuple[re.Pattern, re.Pattern]] = field(default_factory=list)
+    narrations: list[re.Pattern] = field(default_factory=list)
+    payees: list[re.Pattern] = field(default_factory=list)
+    somewheres: list[re.Pattern] = field(default_factory=list)
+    tags: list[re.Pattern] = field(default_factory=list)
+    types: frozenset[type] = TYPES_DEFAULT
 
     @staticmethod
     def _re_compile(ignore_case: bool, s: str) -> re.Pattern:
         """Compile a regex, ignoring case or not."""
         re_flags = 0
         if ignore_case:
             re_flags = re.IGNORECASE
 
         return re.compile(s, flags=re_flags)
 
     @classmethod
     def guess(
-        cls, pattern: str, ignore_case: bool = False, base: Optional[Self] = None
+        cls,
+        pattern: str,
+        caseness: Caseness = Caseness.SMART,
+        base: Optional[Self] = None,
     ) -> Self:
         """Guess criteria from a single textual pattern, using heuristics.
 
         Heuristics (ordered by priority):
 
         - "YYYY-MM-DD" -> date criteria
         - "#tag" -> tag criteria
         - "^link" -> link criteria
+        - "@payee" -> payee criteria
         - starting with an account type (Assets, Liabilities, etc.) -> account criteria
         - "key:value" -> metadata criteria
         - default -> somewhere criteria
 
         """
         criteria = base if base is not None else cls()
+        ignore_case = caseness.ignore_case(pattern)
 
         if re.search(r"^\d{4}-\d{2}-\d{2}$", pattern):
-            criteria.date = [DatePredicate.parse(f"={pattern}")]
+            criteria.dates.append(DatePredicate.parse(f"={pattern}"))
         elif re.search(r"^#[-\w]+$", pattern):
-            criteria.tag = cls._re_compile(ignore_case, pattern[1:])
+            criteria.tags.append(cls._re_compile(ignore_case, pattern[1:]))
+        elif re.search(r"^@.+$", pattern):
+            criteria.payees.append(cls._re_compile(ignore_case, pattern[1:]))
         elif re.search(r"^\^[-\w]+$", pattern):
-            criteria.link = cls._re_compile(ignore_case, pattern[1:])
+            criteria.links.append(cls._re_compile(ignore_case, pattern[1:]))
         elif re.search(r"^(Assets|Liabilities|Equity|Income|Expenses)", pattern):
-            criteria.account = cls._re_compile(ignore_case, pattern)
+            criteria.accounts.append(cls._re_compile(ignore_case, pattern))
         elif m := re.search(r"(?P<key>\w+):(?P<val>\w+)$", pattern):
             matches = m.groupdict()
-            criteria.metadata = (
-                cls._re_compile(ignore_case, matches["key"]),
-                cls._re_compile(ignore_case, matches["val"]),
+            criteria.metadatas.append(
+                (
+                    cls._re_compile(ignore_case, matches["key"]),
+                    cls._re_compile(ignore_case, matches["val"]),
+                )
             )
         else:
-            criteria.somewhere = cls._re_compile(ignore_case, pattern)
+            criteria.somewheres.append(cls._re_compile(ignore_case, pattern))
 
         return criteria
 
     @classmethod
-    def build(
+    def from_cli(
         cls,
-        account_re,
-        amount_preds,
-        date_preds,
-        link_re,
-        metadata_pat,
-        narration_re,
-        payee_re,
-        somewhere_re,
-        tag_re,
-        type_pat,
-        ignore_case,
+        accounts,
+        amounts,
+        dates,
+        links,
+        metadatas,
+        narrations,
+        payees,
+        somewheres,
+        tags,
+        types,
+        caseness,
+        invert_match,
         base: Optional[Self] = None,
     ) -> Self:
         """Build criteria from command line arguments."""
         criteria = base if base is not None else cls()
-
-        if account_re is not None:
-            criteria.account = cls._re_compile(ignore_case, account_re)
-        if amount_preds is not None:
-            criteria.amount = list(map(AmountPredicate.parse, amount_preds))
-        if date_preds is not None:
-            criteria.date = list(map(DatePredicate.parse, date_preds))
-        if link_re is not None:
-            criteria.link = cls._re_compile(ignore_case, link_re)
-        if metadata_pat is not None:
-            if KEY_VAL_SEP in metadata_pat:
-                (key_re, val_re) = metadata_pat.split(KEY_VAL_SEP, maxsplit=1)
-            else:
-                (key_re, val_re) = (metadata_pat, META_VAL_RE)
-            criteria.metadata = (
-                cls._re_compile(ignore_case, key_re),
-                cls._re_compile(ignore_case, val_re),
-            )
-        if narration_re is not None:
-            criteria.narration = cls._re_compile(ignore_case, narration_re)
-        if payee_re is not None:
-            criteria.payee = cls._re_compile(ignore_case, payee_re)
-        if somewhere_re is not None:
-            criteria.somewhere = cls._re_compile(ignore_case, somewhere_re)
-        if tag_re is not None:
-            criteria.tag = cls._re_compile(ignore_case, tag_re)
-        if type_pat is not None:
-            criteria.types = parse_types(type_pat)
+        if invert_match and criteria.types == TYPES_DEFAULT:
+            # clear "--type transaction" default if "--invert-match"
+            criteria.types = frozenset()
+
+        if accounts is not None:
+            criteria.accounts.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in accounts
+            )
+        if amounts is not None:
+            criteria.amounts.extend(AmountPredicate.parse(s) for s in amounts)
+        if dates is not None:
+            criteria.dates.extend(DatePredicate.parse(s) for s in dates)
+        if links is not None:
+            criteria.links.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in links
+            )
+        if metadatas is not None:
+            for s in metadatas:
+                ignore_case = caseness.ignore_case(s)
+                if KEY_VAL_SEP in s:
+                    (key_re, val_re) = s.split(KEY_VAL_SEP, maxsplit=1)
+                else:
+                    (key_re, val_re) = (s, META_VAL_RE)
+                criteria.metadatas.append(
+                    (
+                        cls._re_compile(ignore_case, key_re),
+                        cls._re_compile(ignore_case, val_re),
+                    )
+                )
+        if narrations is not None:
+            criteria.narrations.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in narrations
+            )
+        if payees is not None:
+            criteria.payees.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in payees
+            )
+        if somewheres is not None:
+            criteria.somewheres.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in somewheres
+            )
+        if tags is not None:
+            criteria.tags.extend(
+                cls._re_compile(caseness.ignore_case(s), s) for s in tags
+            )
+        if types is not None:
+            # Note: we *override* here, rather than merging, because types are not meant
+            # to be incrementally specified.
+            criteria.types = frozenset(parse_types(types))
 
         return criteria
 
 
 def get_accounts(entry: data.Directive) -> set[str]:
     """Extract account names referenced from a Beancount entry.
 
@@ -504,17 +566,17 @@
         case data.Custom:
             strings.add(entry.type)
             strings = strings.union(set(str(v) for v in entry.values))
 
     return strings
 
 
-def account_matches(entry: data.Directive, criteria: re.Pattern) -> bool:
+def account_matches(entry: data.Directive, criteria: Iterable[re.Pattern]) -> bool:
     """Check if a Beancount entry matches account criteria."""
-    return any(criteria.search(a) for a in get_accounts(entry))
+    return all(any(pat.search(a) for a in get_accounts(entry)) for pat in criteria)
 
 
 def amount_matches(entry: data.Directive, criteria: Iterable[AmountPredicate]) -> bool:
     """Check if a Beancount entry matches amount criteria."""
     # Matching semantics: there exists at least one amount that matches all amount
     # predicates. Note: should return False for transactions with no amount.
     return bool(  # there is at least one amount...
@@ -531,63 +593,79 @@
     return bool(  # there is at least one date...
         dates := get_dates(entry)
     ) and any(  # ... that matches all amount predicates
         all(date_pred.match(a) for date_pred in criteria) for a in dates
     )
 
 
-def link_matches(entry: data.Directive, criteria: re.Pattern) -> bool:
+def link_matches(entry: data.Directive, criteria: Iterable[re.Pattern]) -> bool:
     """Check if a Beancount entry matches links criteria."""
-    return any(criteria.search(link) for link in get_links(entry))
+    return all(any(pat.search(link) for link in get_links(entry)) for pat in criteria)
 
 
 def metadata_matches(
     entry: data.Directive,
-    criteria: tuple[re.Pattern, re.Pattern],
+    criteria: Iterable[tuple[re.Pattern, re.Pattern]],
     skip_internals: bool = SKIP_INTERNALS,
 ) -> bool:
     """Check if a Beancount entry matches metadata criteria."""
-    (key_re, val_re) = criteria
-    return any(
-        key_re.search(k) and val_re.search(str(v))
-        for (k, v) in get_metadata(entry, skip_internals=skip_internals)
+    return all(
+        any(
+            key_pat.search(k) and val_pat.search(str(v))
+            for (k, v) in get_metadata(entry, skip_internals=skip_internals)
+        )
+        for (key_pat, val_pat) in criteria
     )
 
 
-def narration_matches(entry: data.Directive, criteria: re.Pattern) -> bool:
+def narration_matches(entry: data.Directive, criteria: Iterable[re.Pattern]) -> bool:
     """Check if a Beancount entry matches narration criteria."""
-    return (s := get_narration(entry)) is not None and bool(criteria.search(s))
+    return (s := get_narration(entry)) is not None and all(
+        bool(pat.search(s)) for pat in criteria
+    )
 
 
-def payee_matches(entry: data.Directive, criteria: re.Pattern) -> bool:
+def payee_matches(entry: data.Directive, criteria: Iterable[re.Pattern]) -> bool:
     """Check if a Beancount entry matches payee criteria."""
-    return (s := get_payee(entry)) is not None and bool(criteria.search(s))
+    return (s := get_payee(entry)) is not None and all(
+        bool(pat.search(s)) for pat in criteria
+    )
 
 
 def somewhere_matches(
     entry: data.Directive,
-    criteria: re.Pattern,
+    criteria: Iterable[re.Pattern],
     posting_tags_meta: str = POSTING_TAGS_META,
     skip_internals: bool = SKIP_INTERNALS,
 ) -> bool:
     """Check if a Beancount entry matches somewhere criteria."""
-    return any(
-        criteria.search(s)
-        for s in get_strings(
-            entry, posting_tags_meta=posting_tags_meta, skip_internals=skip_internals
+    return all(
+        any(
+            pat.search(s)
+            for s in get_strings(
+                entry,
+                posting_tags_meta=posting_tags_meta,
+                skip_internals=skip_internals,
+            )
         )
+        for pat in criteria
     )
     # return bool(criteria.search(printer.format_entry(entry)))
 
 
 def tag_matches(
-    entry: data.Directive, criteria: re.Pattern, posting_tags_meta=POSTING_TAGS_META
+    entry: data.Directive,
+    criteria: Iterable[re.Pattern],
+    posting_tags_meta=POSTING_TAGS_META,
 ) -> bool:
     """Check if a Beancount entry matches tag criteria."""
-    return any(criteria.search(t) for t in get_tags(entry, posting_tags_meta))
+    return all(
+        any(pat.search(t) for t in get_tags(entry, posting_tags_meta))
+        for pat in criteria
+    )
 
 
 def type_matches(entry: data.Directive, types: Iterable[type]) -> bool:
     """Check if a Beancount entry matches type criteria."""
     return type(entry) in types
 
 
@@ -596,44 +674,42 @@
     criteria: Criteria,
     posting_tags_meta=POSTING_TAGS_META,
     skip_internals=SKIP_INTERNALS,
 ) -> bool:
     """Check if a Beancount entry matches stated criteria."""
 
     predicates = []
-    # ignoring types below because mypy fails to understand criteria fields are not None
-    # inside lambdas, in spite of the explicit `is not None` guard
-    if criteria.account is not None:
-        predicates.append(lambda e: account_matches(e, criteria.account))  # type: ignore  # noqa:E501
-    if criteria.amount is not None:
-        predicates.append(lambda e: amount_matches(e, criteria.amount))  # type: ignore
-    if criteria.date is not None:
-        predicates.append(lambda e: date_matches(e, criteria.date))  # type: ignore
-    if criteria.link is not None:
-        predicates.append(lambda e: link_matches(e, criteria.link))  # type: ignore
-    if criteria.metadata is not None:
+    if criteria.accounts:
+        predicates.append(lambda e: account_matches(e, criteria.accounts))
+    if criteria.amounts:
+        predicates.append(lambda e: amount_matches(e, criteria.amounts))
+    if criteria.dates:
+        predicates.append(lambda e: date_matches(e, criteria.dates))
+    if criteria.links:
+        predicates.append(lambda e: link_matches(e, criteria.links))
+    if criteria.metadatas:
         predicates.append(
             lambda e: metadata_matches(
-                e, criteria.metadata, skip_internals=skip_internals  # type: ignore
+                e, criteria.metadatas, skip_internals=skip_internals
             )
         )
-    if criteria.narration is not None:
-        predicates.append(lambda e: narration_matches(e, criteria.narration))  # type: ignore  # noqa:E501
-    if criteria.payee is not None:
-        predicates.append(lambda e: payee_matches(e, criteria.payee))  # type: ignore
-    if criteria.somewhere is not None:
+    if criteria.narrations:
+        predicates.append(lambda e: narration_matches(e, criteria.narrations))
+    if criteria.payees:
+        predicates.append(lambda e: payee_matches(e, criteria.payees))
+    if criteria.somewheres:
         predicates.append(
             lambda e: somewhere_matches(
-                e, criteria.somewhere, posting_tags_meta, skip_internals  # type: ignore
+                e, criteria.somewheres, posting_tags_meta, skip_internals
             )
         )
-    if criteria.tag is not None:
-        predicates.append(lambda e: tag_matches(e, criteria.tag, posting_tags_meta))  # type: ignore  # noqa:E501
-    if criteria.types is not None:
-        predicates.append(lambda e: type_matches(entry, criteria.types))  # type: ignore
+    if criteria.tags:
+        predicates.append(lambda e: tag_matches(e, criteria.tags, posting_tags_meta))
+    if criteria.types:
+        predicates.append(lambda e: type_matches(entry, criteria.types))
 
     is_match = all(p(entry) for p in predicates)
     return is_match
 
 
 STR_TO_TYPE: dict[str, type] = {
     "balance": data.Balance,
@@ -674,286 +750,37 @@
 
     return frozenset(types)
 
 
 def filter_entries(
     entries,
     criteria,
+    invert_match: bool = False,
     posting_tags_meta=POSTING_TAGS_META,
     skip_internals=SKIP_INTERNALS,
 ):
     """Filter entries to only return those that match criteria."""
     for entry in entries:
-        if entry_matches(
+        is_match = entry_matches(
             entry,
             criteria,
             posting_tags_meta=posting_tags_meta,
             skip_internals=skip_internals,
-        ):
-            logging.debug("Entry %s matches criteria, keeping it", entry)
-            yield entry
-        else:
-            logging.debug("Entry %s does not match criteria, skipping it", entry)
-
-
-@click.command(
-    help="Search for entries matching given criteria in Beancount journals. "
-    "Pretty print matching entries to standard output."
-    "\n\n"
-    "Search criteria can be specified with the options below and/or providing an "
-    'explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a date '
-    '(if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"), account '
-    '(start with an account type, e.g., "Assets", "Income", etc.), metadata pair '
-    '("key:value"), or string to be matched anywhere (see -s/--somewhere below), '
-    "in this order. "
-    "If PATTERN is not given, search criteria are defined by explicit options. "
-    "\n\n"
-    "Multiple options and/or PATTERN are logically joined (AND-ed) together. "
-    "In case of overlap, explicit options override PATTERN. "
-    "\n\n"
-    "The granularity of matching (and results) is that of individual entries, e.g., "
-    "full transactions, balances, notes, etc. By default only transactions are returned"
-    "; use the --type/-T option to override."
-    "\n\n"
-    'To read from standard input, pass "-" as FILENAME, but beware that it implies '
-    "on-disk buffering of stdin.",
-    epilog="Exit status is 0 (success) if a match is found, "
-    "1 if no match is found, 2 if an error occurred.",
-)
-@click.argument(
-    "args",
-    required=True,
-    nargs=-1,
-    metavar="[PATTERN] FILENAME...",  # override metavar to show what is required
-)
-@click.option(
-    "--account",
-    "-a",
-    "account_re",
-    metavar="REGEX",
-    help="Only return entries referencing accounts with names matching given regex.",
-)
-@click.option(
-    "--amount",
-    "-A",
-    "amount_preds",
-    metavar='"[OP]AMOUNT [REGEX]"',
-    multiple=True,
-    help="Only return entries with amounts matching the given amount predicate. "
-    "An amount predicate start with an optional comparison operator "
-    "(one of '<', '<=', '=', '>=', '>', with '=' being the default), "
-    "followed by a decimal number (using '.' as decimal separator), "
-    "followed by an optional currency regex. "
-    "Multiple amount predicates can be given to express complex amount ranges.",
-)
-@click.option(
-    "--date",
-    "-d",
-    "date_preds",
-    metavar="[OP]DATE",
-    multiple=True,
-    help="Only return entries with dates matching the given date predicate. "
-    "A date predicate start with an optional comparison operator "
-    "(one of '<', '<=', '=', '>=', '>', with '=' being the default), "
-    "and is followed by a date in the form YYYY-[MM[-DD]]. "
-    "Multiple date predicates can be given to express complex date ranges.",
-)
-@click.option(
-    "--link",
-    "-l",
-    "link_re",
-    metavar="REGEX",
-    help="Only return entries with at least one link matching given regex.",
-)
-@click.option(
-    "--meta",
-    "--metadata",
-    "-m",
-    "metadata_pat",
-    metavar="REGEX[:REGEX]",
-    help="Only return entries with at least one metadata key/value pair matching "
-    "given pattern. A pattern is a pair of regexs separated by ':', "
-    "the former matching on metadata key, the latter on metadata value. "
-    f"The second regex is optional and defaults to '{META_VAL_RE}'.",
-)
-@click.option(
-    "--narration",
-    "-n",
-    "narration_re",
-    metavar="REGEX",
-    help="Only return entries whose narrations match given regex.",
-)
-@click.option(
-    "--payee",
-    "-p",
-    "payee_re",
-    metavar="REGEX",
-    help="Only return entries whose payees match given regex.",
-)
-@click.option(
-    "--somewhere",
-    "--anywhere",
-    "-s",
-    "somewhere_re",
-    metavar="REGEX",
-    help="Only return entries with a value in them, anywhere, matching given regex.",
-)
-@click.option(
-    "--tag",
-    "-t",
-    "tag_re",
-    metavar="REGEX",
-    help="Only return entries with at least one tag matching given regex. "
-    "The tag can be located anywhere.",
-)
-@click.option(
-    "--type",
-    "-T",
-    "type_pat",
-    metavar="TYPE(S)",
-    help="Only return entries of certain types. "
-    f"Types are specified as a '{TYPE_SEP}'-separated list of type names; "
-    "type names are: open, close, commodity, pad, balance, transaction, "
-    "note, event, query, price, document, custom. "
-    "The special value 'all' means: all directive types. "
-    "[default: transaction]",
-)
-@click.option(
-    "--ignore-case/--no-ignore-case",
-    "-i",
-    "ignore_case",
-    default=False,
-    show_default=True,
-    help="Ignore case distinctions in string matches.",
-)
-@click.option(
-    "--posting-tags-meta",
-    default=POSTING_TAGS_META,
-    show_default=True,
-    help="Metadata key used to attach tags to transaction postings.",
-)
-@click.option(
-    "--quiet/--no-quiet",
-    "-q",
-    "quiet",
-    default=False,
-    show_default=True,
-    help="Quiet, do not write anything to standard output. "
-    "Exit successfully immediately if any match is found.",
-)
-@click.option(
-    "--skip-internals/--no-skip-internals",
-    "skip_internals",
-    default=True,
-    show_default=True,
-    help="When matching, ignore internal information not visible in the ledger. "
-    f"This includes the automatic metadata: {sorted(INTERNALS_META)}",
-)
-@click.option(
-    "--verbose",
-    count=True,
-    help="Increase logging verbosity. "
-    "Default verbosity is at WARNING level; "
-    "passing this option once will increase it to INFO, twice or more to DEBUG.",
-)
-@click.version_option(None, "--version", "-V")
-@click.pass_context
-def cli(
-    ctx,
-    args,
-    account_re,
-    amount_preds,
-    date_preds,
-    link_re,
-    metadata_pat,
-    narration_re,
-    payee_re,
-    somewhere_re,
-    tag_re,
-    type_pat,
-    ignore_case,
-    posting_tags_meta,
-    quiet,
-    skip_internals,
-    verbose,
-):
-    match verbose:
-        case 0:
-            log_level = logging.WARNING
-        case 1:
-            log_level = logging.INFO
-        case _:  # >= 2
-            log_level = logging.DEBUG
-    logging.basicConfig(level=log_level)
-
-    (pattern, filenames) = (None, [])
-    if len(args) == 1:  # len(args) == 0 should not happen due to required=True
-        filenames = list(args)
-    elif len(args) >= 2:
-        (pattern, filenames) = (args[0], list(args[1:]))
-    if len(list(filter(lambda fname: fname == "-", filenames))) > 1:
-        raise click.BadArgumentUsage(
-            'Standard input ("-") cannot be specified multipled times'
-        )
-
-    try:
-        criteria = Criteria()  # start from default criteria
-        if pattern is not None:  # override with smart pattern, if given as argument
-            criteria = Criteria.guess(pattern, ignore_case, base=criteria)
-        criteria = Criteria.build(  # override with explicit options, if any
-            account_re=account_re,
-            amount_preds=(amount_preds or None),
-            date_preds=(date_preds or None),
-            link_re=link_re,
-            metadata_pat=metadata_pat,
-            narration_re=narration_re,
-            payee_re=payee_re,
-            somewhere_re=somewhere_re,
-            tag_re=tag_re,
-            type_pat=type_pat,
-            ignore_case=ignore_case,
-            base=criteria,
         )
-    except ValueError as e:
-        raise click.UsageError(e.args[0]) from e
-    logging.info("Using search criteria: %s", criteria)
-
-    match_found = False
-    for filename in filenames:
-        if filename == "-":
-            # Beancount does not support streaming reading, so to mimic Unix filter
-            # semantics we read stdin to the end and store it to a temporary file.
-            with NamedTemporaryFile(prefix="beangrep.", suffix=".beancount") as tmpfile:
-                logging.info("Buffering stdin to temporary file %s...", tmpfile.name)
-                shutil.copyfileobj(sys.stdin.buffer, tmpfile.file)
-                tmpfile.flush()
-                logging.info("Loading ledger from %s...", tmpfile.name)
-                ledger = beancount.loader.load_file(tmpfile.name)
-        else:
-            logging.info("Loading ledger from %s...", filename)
-            ledger = beancount.loader.load_file(filename)
-
-        if ledger[1]:  # Beancount encountered loading error(s), fail with diagnostic
-            raise click.BadArgumentUsage(
-                f'\nBeancount encountered error(s) when loading "{filename}":\n'
-                + "\n".join(str(err) for err in ledger[1]),
-            )
-        logging.debug("Input ledger contains %d entries", len(ledger[0]))
-
-        for entry in filter_entries(
-            ledger[0],
-            criteria,
-            posting_tags_meta=posting_tags_meta,
-            skip_internals=skip_internals,
-        ):
-            match_found = True
-            if quiet:
-                break
-            else:
-                printer.print_entry(entry)
-
-    exit_status = 0 if match_found else 1
-    ctx.exit(exit_status)
-
-
-if __name__ == "__main__":
-    cli()
+        match (is_match, invert_match):
+            case (True, False):
+                logging.debug("Entry %s matches criteria, returning it", entry)
+                yield entry
+            case (False, False):
+                logging.debug("Entry %s does not match criteria, skipping it", entry)
+            case (True, True):
+                logging.debug(
+                    "Entry %s matches criteria, but invert match is on, skipping it",
+                    entry,
+                )
+            case (False, True):
+                logging.debug(
+                    "Entry %s does not match criteria, but invert match is on, "
+                    "returning it",
+                    entry,
+                )
+                yield entry
```

### Comparing `beangrep-0.4.0/src/beangrep/data/bean-grep.1` & `beangrep-0.5.0/src/beangrep/data/bean-grep.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man 1.49.3.
-.TH BEAN-GREP, "1" "May 2024" "bean-grep, version 0.4.0" "User Commands"
+.TH BEAN-GREP, "1" "May 2024" "bean-grep, version 0.5.0" "User Commands"
 .SH NAME
 bean-grep, \- grep-like filter for Beancount
 .SH SYNOPSIS
 .B bean-grep
 [\fI\,OPTIONS\/\fR] [\fI\,PATTERN\/\fR] \fI\,FILENAME\/\fR...
 .SH DESCRIPTION
 .IP
 Search for entries matching given criteria in Beancount journals. Pretty
 print matching entries to standard output.
 .IP
 Search criteria can be specified with the options below and/or providing an
-explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
-date (if it is in the "YYYY\-MM\-DD" format), tag ("#tag"), link ("^link"),
-account (start with an account type, e.g., "Assets", "Income", etc.),
-metadata pair ("key:value"), or string to be matched anywhere (see
-\fB\-s\fR/\-\-somewhere below), in this order. If PATTERN is not given, search
-criteria are defined by explicit options.
+explicit "smart" PATTERN. If given, PATTERN is interpreted as described
+below under "Patterns". If not given, search criteria are defined by
+explicit options.
 .IP
-Multiple options and/or PATTERN are logically joined (AND\-ed) together. In
-case of overlap, explicit options override PATTERN.
+Multiple options, options given mutiple times, and PATTERN(s) are logically
+joined (AND\-ed) together.
 .IP
 The granularity of matching (and results) is that of individual entries,
 e.g., full transactions, balances, notes, etc. By default only transactions
 are returned; use the \fB\-\-type\fR/\-T option to override.
 .IP
 To read from standard input, pass "\-" as FILENAME, but beware that it
 implies on\-disk buffering of stdin.
@@ -33,43 +30,43 @@
 Only return entries referencing accounts
 with names matching given regex.
 .TP
 \fB\-A\fR, \fB\-\-amount\fR "[OP]AMOUNT [REGEX]"
 Only return entries with amounts matching
 the given amount predicate. An amount
 predicate start with an optional comparison
-operator (one of '<', '<=', '=', '>=', '>',
-with '=' being the default), followed by a
-decimal number (using '.' as decimal
+operator (one of "<", "<=", "=", ">=", ">",
+with "=" being the default), followed by a
+decimal number (using "." as decimal
 separator), followed by an optional currency
 regex. Multiple amount predicates can be
 given to express complex amount ranges.
 .TP
 \fB\-d\fR, \fB\-\-date\fR [OP]DATE
 Only return entries with dates matching the
 given date predicate. A date predicate start
 with an optional comparison operator (one of
-\&'<', '<=', '=', '>=', '>', with '=' being
+"<", "<=", "=", ">=", ">", with "=" being
 the default), and is followed by a date in
 the form YYYY\-[MM[\-DD]]. Multiple date
 predicates can be given to express complex
 date ranges.
 .TP
 \fB\-l\fR, \fB\-\-link\fR REGEX
 Only return entries with at least one link
 matching given regex.
 .TP
 \fB\-m\fR, \fB\-\-meta\fR, \fB\-\-metadata\fR REGEX[:REGEX]
 Only return entries with at least one
 metadata key/value pair matching given
 pattern. A pattern is a pair of regexs
-separated by ':', the former matching on
+separated by ":", the former matching on
 metadata key, the latter on metadata value.
 The second regex is optional and defaults to
-\&'.*'.
+".*".
 .TP
 \fB\-n\fR, \fB\-\-narration\fR REGEX
 Only return entries whose narrations match
 given regex.
 .TP
 \fB\-p\fR, \fB\-\-payee\fR REGEX
 Only return entries whose payees match given
@@ -81,25 +78,35 @@
 .TP
 \fB\-t\fR, \fB\-\-tag\fR REGEX
 Only return entries with at least one tag
 matching given regex. The tag can be located
 anywhere.
 .TP
 \fB\-T\fR, \fB\-\-type\fR TYPE(S)
-Only return entries of certain types. Types
-are specified as a ','\-separated list of
+Only return entries of certain types.  Types
+are specified as a ","\-separated list of
 type names; type names are: open, close,
 commodity, pad, balance, transaction, note,
 event, query, price, document, custom. The
-special value 'all' means: all directive
+special value "all" means: all directive
 types. [default: transaction]
 .TP
-\fB\-i\fR, \fB\-\-ignore\-case\fR / \fB\-\-no\-ignore\-case\fR
-Ignore case distinctions in string matches.
-[default: no\-ignore\-case]
+\fB\-\-case\-sensitive\fR
+Search case sensitively. Overrides:
+\fB\-i\fR/\-\-ignore\-case and \fB\-S\fR/\-\-smart\-case.
+.TP
+\fB\-i\fR, \fB\-\-ignore\-case\fR
+Search case insensitively. Overrides
+\fB\-S\fR/\-\-smart\-case; overridden by \fB\-\-casesensitive\fR.
+.TP
+\fB\-S\fR, \fB\-\-smart\-case\fR
+Search case insensitively if all criteria
+are lowercase, sensitively otherwise.
+Overridden by: \fB\-\-case\-sensitive\fR and
+\fB\-i\fR/\-\-ignore\-case.  [default: True]
 .TP
 \fB\-\-posting\-tags\-meta\fR TEXT
 Metadata key used to attach tags to
 transaction postings.  [default: tags]
 .TP
 \fB\-q\fR, \fB\-\-quiet\fR / \fB\-\-no\-quiet\fR
 Quiet, do not write anything to standard
@@ -108,26 +115,54 @@
 .TP
 \fB\-\-skip\-internals\fR / \fB\-\-no\-skip\-internals\fR
 When matching, ignore internal information
 not visible in the ledger. This includes the
 automatic metadata: ['filename', 'lineno']
 [default: skip\-internals]
 .TP
+\fB\-v\fR, \fB\-\-invert\-match\fR
+Invert the sense of matching: return entries
+that do *not* match given criteria. This
+clears the default "\-\-type transaction"
+criteria, to avoid only returning nontransaction entries by default.
+.TP
 \fB\-\-verbose\fR
 Increase logging verbosity. Default
 verbosity is at WARNING level; passing this
 option once will increase it to INFO, twice
 or more to DEBUG.
 .TP
 \fB\-V\fR, \fB\-\-version\fR
 Show the version and exit.
 .TP
 \fB\-\-help\fR
 Show this message and exit.
 .IP
+Patterns:
+.IP
+When given the "smart" PATTERN is interpreted according to the following
+heuristics, tried in order, first match wins:
+.IP
+\- if it is in the form "YYYY\-MM\-DD" \-> then it is interpreted as \fB\-\-date\fR
+.IP
+\- "#tag" \-> \fB\-\-tag\fR
+.IP
+\- "^link" \-> \fB\-\-link\fR
+.IP
+\- "@payee" \-> \fB\-\-payee\fR
+.IP
+\- if it starts with one of the five account types ("Assets", "Equity",
+"Expenses",   "Income", "Liabilities") \-> \fB\-\-account\fR
+.IP
+\- "key:value" \-> \fB\-\-metadata\fR
+.IP
+\- otherwise \-> \fB\-\-somewhere\fR
+.IP
+Exit status:
+.IP
 Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
 an error occurred.
 .SH AUTHOR
 Stefano Zacchiroli <zack@upsilon.cc>
 .SH "REPORTING BUGS"
 https://github.com/zacchiro/beangrep/issues
 .SH COPYRIGHT
```

### Comparing `beangrep-0.4.0/src/beangrep.egg-info/PKG-INFO` & `beangrep-0.5.0/src/beangrep.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.4.0
+Version: 0.5.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -81,23 +81,20 @@
 ```
 Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
   Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
-  explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
-  date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
-  account (start with an account type, e.g., "Assets", "Income", etc.),
-  metadata pair ("key:value"), or string to be matched anywhere (see
-  -s/--somewhere below), in this order. If PATTERN is not given, search
-  criteria are defined by explicit options.
+  explicit "smart" PATTERN. If given, PATTERN is interpreted as described
+  below under "Patterns". If not given, search criteria are defined by
+  explicit options.
 
-  Multiple options and/or PATTERN are logically joined (AND-ed) together. In
-  case of overlap, explicit options override PATTERN.
+  Multiple options, options given mutiple times, and PATTERN(s) are logically
+  joined (AND-ed) together.
 
   The granularity of matching (and results) is that of individual entries,
   e.g., full transactions, balances, notes, etc. By default only transactions
   are returned; use the --type/-T option to override.
 
   To read from standard input, pass "-" as FILENAME, but beware that it
   implies on-disk buffering of stdin.
@@ -105,75 +102,108 @@
 Options:
   -a, --account REGEX             Only return entries referencing accounts
                                   with names matching given regex.
   -A, --amount "[OP]AMOUNT [REGEX]"
                                   Only return entries with amounts matching
                                   the given amount predicate. An amount
                                   predicate start with an optional comparison
-                                  operator (one of '<', '<=', '=', '>=', '>',
-                                  with '=' being the default), followed by a
-                                  decimal number (using '.' as decimal
+                                  operator (one of "<", "<=", "=", ">=", ">",
+                                  with "=" being the default), followed by a
+                                  decimal number (using "." as decimal
                                   separator), followed by an optional currency
                                   regex. Multiple amount predicates can be
                                   given to express complex amount ranges.
   -d, --date [OP]DATE             Only return entries with dates matching the
                                   given date predicate. A date predicate start
                                   with an optional comparison operator (one of
-                                  '<', '<=', '=', '>=', '>', with '=' being
+                                  "<", "<=", "=", ">=", ">", with "=" being
                                   the default), and is followed by a date in
                                   the form YYYY-[MM[-DD]]. Multiple date
                                   predicates can be given to express complex
                                   date ranges.
   -l, --link REGEX                Only return entries with at least one link
                                   matching given regex.
   -m, --meta, --metadata REGEX[:REGEX]
                                   Only return entries with at least one
                                   metadata key/value pair matching given
                                   pattern. A pattern is a pair of regexs
-                                  separated by ':', the former matching on
+                                  separated by ":", the former matching on
                                   metadata key, the latter on metadata value.
                                   The second regex is optional and defaults to
-                                  '.*'.
+                                  ".*".
   -n, --narration REGEX           Only return entries whose narrations match
                                   given regex.
   -p, --payee REGEX               Only return entries whose payees match given
                                   regex.
   -s, --somewhere, --anywhere REGEX
                                   Only return entries with a value in them,
                                   anywhere, matching given regex.
   -t, --tag REGEX                 Only return entries with at least one tag
                                   matching given regex. The tag can be located
                                   anywhere.
-  -T, --type TYPE(S)              Only return entries of certain types. Types
-                                  are specified as a ','-separated list of
+  -T, --type TYPE(S)              Only return entries of certain types.  Types
+                                  are specified as a ","-separated list of
                                   type names; type names are: open, close,
                                   commodity, pad, balance, transaction, note,
                                   event, query, price, document, custom. The
-                                  special value 'all' means: all directive
+                                  special value "all" means: all directive
                                   types. [default: transaction]
-  -i, --ignore-case / --no-ignore-case
-                                  Ignore case distinctions in string matches.
-                                  [default: no-ignore-case]
+  --case-sensitive                Search case sensitively. Overrides:
+                                  -i/--ignore-case and -S/--smart-case.
+  -i, --ignore-case               Search case insensitively. Overrides
+                                  -S/--smart-case; overridden by --case-
+                                  sensitive.
+  -S, --smart-case                Search case insensitively if all criteria
+                                  are lowercase, sensitively otherwise.
+                                  Overridden by: --case-sensitive and
+                                  -i/--ignore-case.  [default: True]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
                                   output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
+  -v, --invert-match              Invert the sense of matching: return entries
+                                  that do *not* match given criteria. This
+                                  clears the default "--type transaction"
+                                  criteria, to avoid only returning non-
+                                  transaction entries by default.
   --verbose                       Increase logging verbosity. Default
                                   verbosity is at WARNING level; passing this
                                   option once will increase it to INFO, twice
                                   or more to DEBUG.
   -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
+  Patterns:
+
+  When given the "smart" PATTERN is interpreted according to the following
+  heuristics, tried in order, first match wins:
+
+  - if it is in the form "YYYY-MM-DD" -> then it is interpreted as --date
+
+  - "#tag" -> --tag
+
+  - "^link" -> --link
+
+  - "@payee" -> --payee
+
+  - if it starts with one of the five account types ("Assets", "Equity",
+  "Expenses",   "Income", "Liabilities") -> --account
+
+  - "key:value" -> --metadata
+
+  - otherwise -> --somewhere
+
+  Exit status:
+
   Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.4.0/src/beangrep.egg-info/SOURCES.txt` & `beangrep-0.5.0/src/beangrep.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 README.md
 pyproject.toml
 setup.py
 .github/workflows/python-package.yml
 bin/bean-grep
 data/man-extras.h2m
 dev/coverage
+dev/tag-release
 dev/update-readme
 src/beangrep/__init__.py
 src/beangrep/__main__.py
 src/beangrep/beangrep.py
+src/beangrep/cli.py
 src/beangrep.egg-info/PKG-INFO
 src/beangrep.egg-info/SOURCES.txt
 src/beangrep.egg-info/dependency_links.txt
 src/beangrep.egg-info/entry_points.txt
 src/beangrep.egg-info/requires.txt
 src/beangrep.egg-info/top_level.txt
 src/beangrep/data/.gitkeep
 src/beangrep/data/bean-grep.1
 tests/test_beangrep.py
+tests/test_cli.py
 tests/data/example.beancount
 tests/data/small.beancount
 tests/data/documents/statements.txt
```

### Comparing `beangrep-0.4.0/tests/data/example.beancount` & `beangrep-0.5.0/tests/data/example.beancount`

 * *Files identical despite different names*

### Comparing `beangrep-0.4.0/tests/data/small.beancount` & `beangrep-0.5.0/tests/data/small.beancount`

 * *Files identical despite different names*

