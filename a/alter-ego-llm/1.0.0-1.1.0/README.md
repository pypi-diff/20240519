# Comparing `tmp/alter_ego_llm-1.0.0.tar.gz` & `tmp/alter_ego_llm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alter_ego_llm-1.0.0.tar", last modified: Wed Dec  6 10:34:54 2023, max compression
+gzip compressed data, was "alter_ego_llm-1.1.0.tar", last modified: Sun May 19 15:53:30 2024, max compression
```

## Comparing `alter_ego_llm-1.0.0.tar` & `alter_ego_llm-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.222722 alter_ego_llm-1.0.0/
--rw-r--r--   0 max       (1000) max       (1000)     7652 2023-12-02 11:48:58.000000 alter_ego_llm-1.0.0/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)       59 2023-12-02 11:49:30.000000 alter_ego_llm-1.0.0/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)    13792 2023-12-06 10:34:54.222722 alter_ego_llm-1.0.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)    13332 2023-12-06 10:34:36.000000 alter_ego_llm-1.0.0/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.198722 alter_ego_llm-1.0.0/alter_ego/
--rw-r--r--   0 max       (1000) max       (1000)       22 2023-12-06 09:51:07.000000 alter_ego_llm-1.0.0/alter_ego/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.202722 alter_ego_llm-1.0.0/alter_ego/agents/
--rw-r--r--   0 max       (1000) max       (1000)     2568 2023-12-03 11:04:09.000000 alter_ego_llm-1.0.0/alter_ego/agents/APIThread.py
--rw-r--r--   0 max       (1000) max       (1000)     1587 2023-12-06 09:48:25.000000 alter_ego_llm-1.0.0/alter_ego/agents/CLIThread.py
--rw-r--r--   0 max       (1000) max       (1000)     1570 2023-11-30 20:24:44.000000 alter_ego_llm-1.0.0/alter_ego/agents/ConstantThread.py
--rw-r--r--   0 max       (1000) max       (1000)      439 2023-07-18 15:26:23.000000 alter_ego_llm-1.0.0/alter_ego/agents/ExternalThread.py
--rw-r--r--   0 max       (1000) max       (1000)     3581 2023-12-06 10:03:21.000000 alter_ego_llm-1.0.0/alter_ego/agents/GPTThread.py
--rw-r--r--   0 max       (1000) max       (1000)     4341 2023-12-03 20:52:48.000000 alter_ego_llm-1.0.0/alter_ego/agents/TextSynthThread.py
--rw-r--r--   0 max       (1000) max       (1000)      326 2023-08-19 13:31:47.000000 alter_ego_llm-1.0.0/alter_ego/agents/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.206722 alter_ego_llm-1.0.0/alter_ego/experiment/
--rw-r--r--   0 max       (1000) max       (1000)     3770 2023-12-03 11:13:12.000000 alter_ego_llm-1.0.0/alter_ego/experiment/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.206722 alter_ego_llm-1.0.0/alter_ego/exports/
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 11:01:33.000000 alter_ego_llm-1.0.0/alter_ego/exports/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4683 2023-11-28 13:02:08.000000 alter_ego_llm-1.0.0/alter_ego/exports/otree.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.206722 alter_ego_llm-1.0.0/alter_ego/structure/
--rw-r--r--   0 max       (1000) max       (1000)     2473 2023-11-28 19:32:00.000000 alter_ego_llm-1.0.0/alter_ego/structure/Relay.py
--rw-r--r--   0 max       (1000) max       (1000)     7733 2023-12-06 09:47:28.000000 alter_ego_llm-1.0.0/alter_ego/structure/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.206722 alter_ego_llm-1.0.0/alter_ego/utils/
--rw-r--r--   0 max       (1000) max       (1000)     2545 2023-12-03 19:28:23.000000 alter_ego_llm-1.0.0/alter_ego/utils/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.210722 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    13792 2023-12-06 10:34:53.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      918 2023-12-06 10:34:54.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-12-06 10:34:53.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       37 2023-12-06 10:34:53.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       60 2023-12-06 10:34:53.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       30 2023-12-06 10:34:53.000000 alter_ego_llm-1.0.0/alter_ego_llm.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.214722 alter_ego_llm-1.0.0/ego/
--rw-r--r--   0 max       (1000) max       (1000)       18 2023-12-03 12:02:11.000000 alter_ego_llm-1.0.0/ego/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2415 2023-12-06 10:03:19.000000 alter_ego_llm-1.0.0/ego/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.214722 alter_ego_llm-1.0.0/games/
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 09:36:16.000000 alter_ego_llm-1.0.0/games/__init__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.214722 alter_ego_llm-1.0.0/games/pd/
--rw-r--r--   0 max       (1000) max       (1000)     3023 2023-09-27 16:03:49.000000 alter_ego_llm-1.0.0/games/pd/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      766 2023-11-28 13:03:10.000000 alter_ego_llm-1.0.0/games/pd/treatments.py
--rw-r--r--   0 max       (1000) max       (1000)       60 2023-12-02 14:02:10.000000 alter_ego_llm-1.0.0/requirements.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-12-06 10:34:54.218722 alter_ego_llm-1.0.0/scenarios/
--rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 09:36:16.000000 alter_ego_llm-1.0.0/scenarios/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3785 2023-12-04 12:45:55.000000 alter_ego_llm-1.0.0/scenarios/built.py
--rw-r--r--   0 max       (1000) max       (1000)      116 2023-11-28 19:17:05.000000 alter_ego_llm-1.0.0/scenarios/ego35.py
--rw-r--r--   0 max       (1000) max       (1000)      108 2023-11-28 19:17:05.000000 alter_ego_llm-1.0.0/scenarios/ego4.py
--rw-r--r--   0 max       (1000) max       (1000)     2447 2023-11-28 19:16:44.000000 alter_ego_llm-1.0.0/scenarios/ego_prereg.py
--rw-r--r--   0 max       (1000) max       (1000)     2649 2023-12-05 19:10:53.000000 alter_ego_llm-1.0.0/scenarios/mindgame.py
--rw-r--r--   0 max       (1000) max       (1000)       38 2023-12-06 10:34:54.222722 alter_ego_llm-1.0.0/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      838 2023-12-06 10:32:47.000000 alter_ego_llm-1.0.0/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.285815 alter_ego_llm-1.1.0/
+-rw-r--r--   0 max       (1000) max       (1000)     7652 2023-12-02 11:48:58.000000 alter_ego_llm-1.1.0/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)       59 2023-12-02 11:49:30.000000 alter_ego_llm-1.1.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)    13934 2024-05-19 15:53:30.285815 alter_ego_llm-1.1.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)    13332 2023-12-06 10:34:36.000000 alter_ego_llm-1.1.0/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.277815 alter_ego_llm-1.1.0/alter_ego/
+-rw-r--r--   0 max       (1000) max       (1000)       22 2023-12-11 21:56:57.000000 alter_ego_llm-1.1.0/alter_ego/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.277815 alter_ego_llm-1.1.0/alter_ego/agents/
+-rw-r--r--   0 max       (1000) max       (1000)     2497 2024-05-19 15:41:18.000000 alter_ego_llm-1.1.0/alter_ego/agents/APIThread.py
+-rw-r--r--   0 max       (1000) max       (1000)     1587 2023-12-06 09:48:25.000000 alter_ego_llm-1.1.0/alter_ego/agents/CLIThread.py
+-rw-r--r--   0 max       (1000) max       (1000)     1570 2023-11-30 20:24:44.000000 alter_ego_llm-1.1.0/alter_ego/agents/ConstantThread.py
+-rw-r--r--   0 max       (1000) max       (1000)      439 2023-07-18 15:26:23.000000 alter_ego_llm-1.1.0/alter_ego/agents/ExternalThread.py
+-rw-r--r--   0 max       (1000) max       (1000)     3389 2024-05-19 15:48:59.000000 alter_ego_llm-1.1.0/alter_ego/agents/GPTThread.py
+-rw-r--r--   0 max       (1000) max       (1000)     4006 2024-05-19 15:44:14.000000 alter_ego_llm-1.1.0/alter_ego/agents/TextSynthThread.py
+-rw-r--r--   0 max       (1000) max       (1000)      326 2023-08-19 13:31:47.000000 alter_ego_llm-1.1.0/alter_ego/agents/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.277815 alter_ego_llm-1.1.0/alter_ego/experiment/
+-rw-r--r--   0 max       (1000) max       (1000)     3770 2023-12-03 11:13:12.000000 alter_ego_llm-1.1.0/alter_ego/experiment/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/alter_ego/exports/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 11:01:33.000000 alter_ego_llm-1.1.0/alter_ego/exports/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     4683 2023-11-28 13:02:08.000000 alter_ego_llm-1.1.0/alter_ego/exports/otree.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/alter_ego/structure/
+-rw-r--r--   0 max       (1000) max       (1000)     2473 2023-11-28 19:32:00.000000 alter_ego_llm-1.1.0/alter_ego/structure/Relay.py
+-rw-r--r--   0 max       (1000) max       (1000)     7733 2023-12-06 09:47:28.000000 alter_ego_llm-1.1.0/alter_ego/structure/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/alter_ego/utils/
+-rw-r--r--   0 max       (1000) max       (1000)     2545 2023-12-03 19:28:23.000000 alter_ego_llm-1.1.0/alter_ego/utils/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    13934 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      918 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       37 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       67 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       30 2024-05-19 15:53:30.000000 alter_ego_llm-1.1.0/alter_ego_llm.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/ego/
+-rw-r--r--   0 max       (1000) max       (1000)       18 2023-12-03 12:02:11.000000 alter_ego_llm-1.1.0/ego/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2415 2023-12-06 10:03:19.000000 alter_ego_llm-1.1.0/ego/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/games/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 09:36:16.000000 alter_ego_llm-1.1.0/games/__init__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/games/pd/
+-rw-r--r--   0 max       (1000) max       (1000)     3023 2023-09-27 16:03:49.000000 alter_ego_llm-1.1.0/games/pd/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      766 2023-11-28 13:03:10.000000 alter_ego_llm-1.1.0/games/pd/treatments.py
+-rw-r--r--   0 max       (1000) max       (1000)       67 2024-05-19 15:46:41.000000 alter_ego_llm-1.1.0/requirements.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-19 15:53:30.281815 alter_ego_llm-1.1.0/scenarios/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-18 09:36:16.000000 alter_ego_llm-1.1.0/scenarios/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3834 2023-12-11 21:55:17.000000 alter_ego_llm-1.1.0/scenarios/built.py
+-rw-r--r--   0 max       (1000) max       (1000)      116 2023-11-28 19:17:05.000000 alter_ego_llm-1.1.0/scenarios/ego35.py
+-rw-r--r--   0 max       (1000) max       (1000)      108 2023-11-28 19:17:05.000000 alter_ego_llm-1.1.0/scenarios/ego4.py
+-rw-r--r--   0 max       (1000) max       (1000)     2447 2023-11-28 19:16:44.000000 alter_ego_llm-1.1.0/scenarios/ego_prereg.py
+-rw-r--r--   0 max       (1000) max       (1000)     2649 2023-12-05 19:10:53.000000 alter_ego_llm-1.1.0/scenarios/mindgame.py
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-19 15:53:30.285815 alter_ego_llm-1.1.0/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      838 2023-12-11 21:56:50.000000 alter_ego_llm-1.1.0/setup.py
```

### Comparing `alter_ego_llm-1.0.0/LICENSE` & `alter_ego_llm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/PKG-INFO` & `alter_ego_llm-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: alter_ego_llm
-Version: 1.0.0
-Summary: Library to run experiments with LLMs
-Home-page: https://ego.mg.sb
-Author: Max R. P. Grossmann
-Author-email: ego@mg.sb
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # alter\_ego
 
 <p align="center">
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 `alter_ego` is a library that allows you to run experiments with LLMs. `ego` is a command-line helper included with this package.
```

### Comparing `alter_ego_llm-1.0.0/README.md` & `alter_ego_llm-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: alter_ego_llm
+Version: 1.1.0
+Summary: Library to run experiments with LLMs
+Home-page: https://ego.mg.sb
+Author: Max R. P. Grossmann
+Author-email: ego@mg.sb
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click>=8.1
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: openai~=1.30.0
+Requires-Dist: requests<3
+
 # alter\_ego
 
 <p align="center">
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 `alter_ego` is a library that allows you to run experiments with LLMs. `ego` is a command-line helper included with this package.
```

### Comparing `alter_ego_llm-1.0.0/alter_ego/agents/APIThread.py` & `alter_ego_llm-1.1.0/alter_ego/agents/APIThread.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
         Initialize the APIThread.
 
         :param args: Additional arguments.
         :type args: Any
-        :param kwargs: Additional keyword arguments, includes `api_key`, `delay`, `max_retries`, and `verbose`.
+        :param kwargs: Additional keyword arguments, includes `api_key`, `delay`, and `verbose`.
         :type kwargs: Any
         """
         self.log = []  # Initialize log
 
         self.api_key = kwargs.get("api_key", self.get_api_key())
         self.delay = kwargs.get("delay", 0)
-        self.max_retries = kwargs.get("max_retries", 3)
         self.verbose = kwargs.get("verbose", False)
 
         super().__init__(*args, **kwargs)
 
     def get_api_key(self) -> str:
         """
         Retrieve the API key from the environment variable or file.
```

### Comparing `alter_ego_llm-1.0.0/alter_ego/agents/CLIThread.py` & `alter_ego_llm-1.1.0/alter_ego/agents/CLIThread.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/agents/ConstantThread.py` & `alter_ego_llm-1.1.0/alter_ego/agents/ConstantThread.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/agents/GPTThread.py` & `alter_ego_llm-1.1.0/alter_ego/agents/GPTThread.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,35 +79,33 @@
 
         :param message: The user's message.
         :type message: str
         :param max_tokens: Maximum number of tokens for the model to generate.
         :type max_tokens: int
         :return: The model output.
         :rtype: str
-        :raises RuntimeError: If maximum number of retries is exceeded.
         """
         client.api_key = self.api_key
 
-        retries = 0
+        try:
+            if self.verbose:
+                print("+", end="", file=sys.stderr, flush=True)
+
+            llm_out = client.chat.completions.create(
+                model=self.model,
+                messages=self.history,
+                max_tokens=max_tokens,
+                n=1,
+                stop=None,
+                temperature=self.temperature,
+            )
+
+            if llm_out.choices[0].finish_reason != "stop":
+                raise ValueError("GPT finished early")
+
+            self.log.append(llm_out)
+
+            return llm_out
+        except Exception as e:
+            self.log.append(e)
 
-        while retries <= self.max_retries:
-            try:
-                if self.verbose:
-                    print("+", end="", file=sys.stderr, flush=True)
-
-                llm_out = client.chat.completions.create(
-                    model=self.model,
-                    messages=self.history,
-                    max_tokens=max_tokens,
-                    n=1,
-                    stop=None,
-                    temperature=self.temperature,
-                )
-                self.log.append(llm_out)
-
-                return llm_out
-            except Exception as e:
-                retries += 1
-                self.log.append(e)
-                time.sleep(1)
-
-        raise RuntimeError(f"max_retries ({self.max_retries}) exceeded for {self}.")
+            raise e  # re-raise
```

### Comparing `alter_ego_llm-1.0.0/alter_ego/agents/TextSynthThread.py` & `alter_ego_llm-1.1.0/alter_ego/agents/TextSynthThread.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,42 +102,37 @@
         :type message: str
         :param max_tokens: Maximum number of tokens for the model to generate.
         :type max_tokens: int
         :param extra_params: Additional parameters for the model.
         :type extra_params: Optional[Dict[str, Any]]
         :return: The model output.
         :rtype: Any
-        :raises RuntimeError: If the maximum number of retries is exceeded.
         """
-        retries = 0
 
-        while retries <= self.max_retries:
-            try:
-                if self.verbose:
-                    print("+", end="", file=sys.stderr, flush=True)
-
-                headers = {
-                    "Content-Type": "application/json",
-                    "Authorization": f"Bearer {self.api_key}",
-                }
-
-                params = {
-                    "max_tokens": max_tokens,
-                    "temperature": self.temperature,
-                } | (extra_params if extra_params is not None else {})
-
-                rq = requests.post(
-                    self.endpoint,
-                    headers=headers,
-                    data=json.dumps(self.ts_data() | params),
-                )
-
-                llm_out = rq.json()
-                self.log.append(llm_out)
-
-                return llm_out
-            except Exception as e:
-                retries += 1
-                self.log.append(e)
-                time.sleep(1)
+        try:
+            if self.verbose:
+                print("+", end="", file=sys.stderr, flush=True)
+
+            headers = {
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.api_key}",
+            }
+
+            params = {
+                "max_tokens": max_tokens,
+                "temperature": self.temperature,
+            } | (extra_params if extra_params is not None else {})
+
+            rq = requests.post(
+                self.endpoint,
+                headers=headers,
+                data=json.dumps(self.ts_data() | params),
+            )
+
+            llm_out = rq.json()
+            self.log.append(llm_out)
+
+            return llm_out
+        except Exception as e:
+            self.log.append(e)
 
-        raise RuntimeError(f"max_retries ({self.max_retries}) exceeded for {self}.")
+            raise e  # re-raise
```

### Comparing `alter_ego_llm-1.0.0/alter_ego/experiment/__init__.py` & `alter_ego_llm-1.1.0/alter_ego/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/exports/otree.py` & `alter_ego_llm-1.1.0/alter_ego/exports/otree.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/structure/Relay.py` & `alter_ego_llm-1.1.0/alter_ego/structure/Relay.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/structure/__init__.py` & `alter_ego_llm-1.1.0/alter_ego/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego/utils/__init__.py` & `alter_ego_llm-1.1.0/alter_ego/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/alter_ego_llm.egg-info/PKG-INFO` & `alter_ego_llm-1.1.0/alter_ego_llm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
-Name: alter-ego-llm
-Version: 1.0.0
+Name: alter_ego_llm
+Version: 1.1.0
 Summary: Library to run experiments with LLMs
 Home-page: https://ego.mg.sb
 Author: Max R. P. Grossmann
 Author-email: ego@mg.sb
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click>=8.1
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: openai~=1.30.0
+Requires-Dist: requests<3
 
 # alter\_ego
 
 <p align="center">
     <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
```

### Comparing `alter_ego_llm-1.0.0/alter_ego_llm.egg-info/SOURCES.txt` & `alter_ego_llm-1.1.0/alter_ego_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/ego/cli.py` & `alter_ego_llm-1.1.0/ego/cli.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/games/pd/__init__.py` & `alter_ego_llm-1.1.0/games/pd/__init__.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/games/pd/treatments.py` & `alter_ego_llm-1.1.0/games/pd/treatments.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/scenarios/built.py` & `alter_ego_llm-1.1.0/scenarios/built.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
             thread.i = i_
 
         convo = alter_ego.structure.Conversation(*threads)
 
         e.link(convo)  # randomly assign treatment
 
+        convo.all.rounds = definition["rounds"]
+
         convo.all.system(
             alter_ego.utils.homogenize(definition["prompts"]["system"]),
             **convo.treatment.variables,
         )
 
         try:
             for round_ in range(1, definition["rounds"] + 1):
```

### Comparing `alter_ego_llm-1.0.0/scenarios/ego_prereg.py` & `alter_ego_llm-1.1.0/scenarios/ego_prereg.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/scenarios/mindgame.py` & `alter_ego_llm-1.1.0/scenarios/mindgame.py`

 * *Files identical despite different names*

### Comparing `alter_ego_llm-1.0.0/setup.py` & `alter_ego_llm-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alter_ego_llm",
-    version="1.0.0",
+    version="1.1.0",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "ego=ego:cli.main",  # Adjust if necessary
         ],
     },
```

