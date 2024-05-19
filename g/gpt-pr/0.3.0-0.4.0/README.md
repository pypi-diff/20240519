# Comparing `tmp/gpt-pr-0.3.0.tar.gz` & `tmp/gpt-pr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/gpt-pr/gpt-pr/dist/.tmp-ldna0n0d/gpt-pr-0.3.0.tar", last modified: Sun May 19 01:58:31 2024, max compression
+gzip compressed data, was "/home/runner/work/gpt-pr/gpt-pr/dist/.tmp-fdcy7kl6/gpt-pr-0.4.0.tar", last modified: Sun May 19 03:06:56 2024, max compression
```

## Comparing `gpt-pr-0.3.0.tar` & `gpt-pr-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:58:30.000000 gpt-pr-0.3.0/gpt_pr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gpt_pr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gptpr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/consolecolor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/gitutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/prdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/gptpr/test_prdata.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/gptpr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 01:58:29.000000 gpt-pr-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 01:58:31.000000 gpt-pr-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-19 01:57:48.000000 gpt-pr-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:06:55.000000 gpt-pr-0.4.0/gpt_pr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gpt_pr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/gptpr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/checkversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/consolecolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/gitutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/prdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/test_checkversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/gptpr/test_prdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 03:06:55.000000 gpt-pr-0.4.0/gptpr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 03:06:53.000000 gpt-pr-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 03:06:56.000000 gpt-pr-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-19 03:06:18.000000 gpt-pr-0.4.0/setup.py
```

### Comparing `gpt-pr-0.3.0/README.md` & `gpt-pr-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gpt_pr.egg-info/requires.txt` & `gpt-pr-0.4.0/gpt_pr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/config.py` & `gpt-pr-0.4.0/gptpr/config.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/consolecolor.py` & `gpt-pr-0.4.0/gptpr/consolecolor.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/gh.py` & `gpt-pr-0.4.0/gptpr/gh.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/gitutil.py` & `gpt-pr-0.4.0/gptpr/gitutil.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/main.py` & `gpt-pr-0.4.0/gptpr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from gptpr.gitutil import get_branch_info
 from gptpr.gh import create_pr
 from gptpr.prdata import get_pr_data
 from gptpr.version import __version__
 from gptpr.config import config, config_command_example, CONFIG_README_SECTION
 from gptpr import consolecolor as cc
+from gptpr.checkversion import check_for_updates
 
 
 def run(base_branch='main', yield_confirmation=False, version=False):
     '''
     Create Pull Requests from current branch with base branch (default 'main' branch)
     '''
 
@@ -77,18 +78,22 @@
             print('')
             current_section = section
 
         print(f'[{cc.bold(section)}]', option, '=', cc.yellow(value))
 
 
 def main():
+    check_for_updates()
+
     fire.Fire(run)
 
 
 def run_config():
+    check_for_updates()
+
     fire.Fire({
         'set': set_config,
         'get': get_config,
         'print': print_config,
         'reset': reset_config
     })
```

### Comparing `gpt-pr-0.3.0/gptpr/prdata.py` & `gpt-pr-0.4.0/gptpr/prdata.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/gptpr/test_config.py` & `gpt-pr-0.4.0/gptpr/test_config.py`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/requirements.txt` & `gpt-pr-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `gpt-pr-0.3.0/setup.py` & `gpt-pr-0.4.0/setup.py`

 * *Files identical despite different names*

