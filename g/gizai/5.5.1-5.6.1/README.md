# Comparing `tmp/gizai-5.5.1.tar.gz` & `tmp/gizai-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gizai-5.5.1.tar", last modified: Sat May 18 23:52:54 2024, max compression
+gzip compressed data, was "gizai-5.6.1.tar", last modified: Sat May 18 23:53:27 2024, max compression
```

## Comparing `gizai-5.5.1.tar` & `gizai-5.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:52:54.019126 gizai-5.5.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-23 00:28:51.000000 gizai-5.5.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      753 2024-05-18 23:52:54.018215 gizai-5.5.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      454 2024-05-18 23:45:26.000000 gizai-5.5.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:52:54.015560 gizai-5.5.1/gizai/
--rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-18 23:52:49.000000 gizai-5.5.1/gizai/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1253 2024-05-18 23:39:40.000000 gizai-5.5.1/gizai/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      273 2024-05-18 23:39:55.000000 gizai-5.5.1/gizai/build.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3155 2024-05-18 23:39:59.000000 gizai-5.5.1/gizai/digest.py
--rw-r--r--   0 kamangir   (502) staff       (20)       86 2024-05-18 23:40:07.000000 gizai-5.5.1/gizai/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-23 00:28:51.000000 gizai-5.5.1/gizai/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:52:54.017437 gizai-5.5.1/gizai.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      753 2024-05-18 23:52:54.000000 gizai-5.5.1/gizai.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-18 23:52:54.000000 gizai-5.5.1/gizai.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 23:52:54.000000 gizai-5.5.1/gizai.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 23:52:54.000000 gizai-5.5.1/gizai.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 23:52:54.019317 gizai-5.5.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      484 2024-05-18 23:52:44.000000 gizai-5.5.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:53:27.902383 gizai-5.6.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-23 00:28:51.000000 gizai-5.6.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)      744 2024-05-18 23:53:27.901707 gizai-5.6.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      454 2024-05-18 23:45:26.000000 gizai-5.6.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:53:27.897651 gizai-5.6.1/gizai/
+-rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-18 23:53:24.000000 gizai-5.6.1/gizai/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1253 2024-05-18 23:39:40.000000 gizai-5.6.1/gizai/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      273 2024-05-18 23:39:55.000000 gizai-5.6.1/gizai/build.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3155 2024-05-18 23:39:59.000000 gizai-5.6.1/gizai/digest.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       86 2024-05-18 23:40:07.000000 gizai-5.6.1/gizai/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-23 00:28:51.000000 gizai-5.6.1/gizai/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:53:27.901020 gizai-5.6.1/gizai.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      744 2024-05-18 23:53:27.000000 gizai-5.6.1/gizai.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-18 23:53:27.000000 gizai-5.6.1/gizai.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 23:53:27.000000 gizai-5.6.1/gizai.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 23:53:27.000000 gizai-5.6.1/gizai.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 23:53:27.902562 gizai-5.6.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      481 2024-05-18 23:53:21.000000 gizai-5.6.1/setup.py
```

### Comparing `gizai-5.5.1/LICENSE` & `gizai-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gizai-5.5.1/PKG-INFO` & `gizai-5.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gizai
-Version: 5.5.1
+Version: 5.6.1
 Summary: 🔻 A recipe for AI languages.
 Author: kamangir
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔻 giza (gizai)
 
-📜 read the working paper: "A Related Set of Bash Expansions of Relevance to AI" - ([tex](https://github.com/kamangir/giza/raw/current/tex/giza.tex)), ([pdf](https://kamangir-public.s3.ca-central-1.amazonaws.com/giza-v1/giza.pdf)).
+📜 read the working paper: "A Related Set of Bash Expansions of Relevance to AI" - ([tex](https://github.com/kamangir/giza/raw/main/tex/giza.tex)), ([pdf](https://kamangir-public.s3.ca-central-1.amazonaws.com/giza-v1/giza.pdf)).
 
-🚀 [awesome bash cli](https://github.com/kamangir/awesome-bash-cli) (`abcli`) is an example implementation of `giza` ([svg](https://github.com/kamangir/giza/raw/current/assets/giza.svg)).
+🚀 [awesome bash cli](https://github.com/kamangir/awesome-bash-cli) (`abcli`) is an example implementation of `giza` ([svg](https://github.com/kamangir/giza/raw/main/assets/giza.svg)).
 
-![image](https://github.com/kamangir/giza/raw/current/assets/giza.png)
+![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)
 
 > ℹ️ a push to this repo triggers a `giza build [publish]`.
```

### Comparing `gizai-5.5.1/gizai/__main__.py` & `gizai-5.6.1/gizai/__main__.py`

 * *Files identical despite different names*

### Comparing `gizai-5.5.1/gizai/digest.py` & `gizai-5.6.1/gizai/digest.py`

 * *Files identical despite different names*

### Comparing `gizai-5.5.1/gizai.egg-info/PKG-INFO` & `gizai-5.6.1/gizai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gizai
-Version: 5.5.1
+Version: 5.6.1
 Summary: 🔻 A recipe for AI languages.
 Author: kamangir
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔻 giza (gizai)
 
-📜 read the working paper: "A Related Set of Bash Expansions of Relevance to AI" - ([tex](https://github.com/kamangir/giza/raw/current/tex/giza.tex)), ([pdf](https://kamangir-public.s3.ca-central-1.amazonaws.com/giza-v1/giza.pdf)).
+📜 read the working paper: "A Related Set of Bash Expansions of Relevance to AI" - ([tex](https://github.com/kamangir/giza/raw/main/tex/giza.tex)), ([pdf](https://kamangir-public.s3.ca-central-1.amazonaws.com/giza-v1/giza.pdf)).
 
-🚀 [awesome bash cli](https://github.com/kamangir/awesome-bash-cli) (`abcli`) is an example implementation of `giza` ([svg](https://github.com/kamangir/giza/raw/current/assets/giza.svg)).
+🚀 [awesome bash cli](https://github.com/kamangir/awesome-bash-cli) (`abcli`) is an example implementation of `giza` ([svg](https://github.com/kamangir/giza/raw/main/assets/giza.svg)).
 
-![image](https://github.com/kamangir/giza/raw/current/assets/giza.png)
+![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)
 
 > ℹ️ a push to this repo triggers a `giza build [publish]`.
```

