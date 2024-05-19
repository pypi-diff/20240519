# Comparing `tmp/jaims_py-2.0.0b2.tar.gz` & `tmp/jaims_py-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims_py-2.0.0b2.tar", last modified: Sun May 19 16:15:00 2024, max compression
+gzip compressed data, was "jaims_py-2.0.0b3.tar", last modified: Sun May 19 16:26:32 2024, max compression
```

## Comparing `jaims_py-2.0.0b2.tar` & `jaims_py-2.0.0b3.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.554247 jaims_py-2.0.0b2/
--rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:15:00.554028 jaims_py-2.0.0b2/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     4692 2024-05-19 16:10:04.000000 jaims_py-2.0.0b2/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.549955 jaims_py-2.0.0b2/jaims/
--rw-r--r--   0 mush       (501) staff       (20)     1455 2024-05-19 15:19:54.000000 jaims_py-2.0.0b2/jaims/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.550191 jaims_py-2.0.0b2/jaims/adapters/
--rw-r--r--   0 mush       (501) staff       (20)       74 2024-05-18 20:45:15.000000 jaims_py-2.0.0b2/jaims/adapters/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.551031 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      103 2024-05-19 15:10:17.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)     8712 2024-05-19 15:27:59.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)     1973 2024-05-19 15:09:20.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/factory.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.551983 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      353 2024-05-19 14:46:29.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    23461 2024-05-19 14:46:37.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)     1999 2024-05-19 15:02:51.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/factory.py
--rw-r--r--   0 mush       (501) staff       (20)     7093 2024-05-19 15:42:10.000000 jaims_py-2.0.0b2/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b2/jaims/default_history_manager.py
--rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b2/jaims/default_tool_manager.py
--rw-r--r--   0 mush       (501) staff       (20)    14293 2024-05-19 14:44:55.000000 jaims_py-2.0.0b2/jaims/entities.py
--rw-r--r--   0 mush       (501) staff       (20)     2308 2024-05-19 15:13:30.000000 jaims_py-2.0.0b2/jaims/factories.py
--rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b2/jaims/interfaces.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.553552 jaims_py-2.0.0b2/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      710 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-19 16:15:00.554292 jaims_py-2.0.0b2/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-19 16:10:25.000000 jaims_py-2.0.0b2/setup.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.553265 jaims_py-2.0.0b2/tests/
--rw-r--r--   0 mush       (501) staff       (20)     5042 2024-05-18 19:41:11.000000 jaims_py-2.0.0b2/tests/test_adapters_exponential_backoff.py
--rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b2/tests/test_agent.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.221115 jaims_py-2.0.0b3/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:26:32.220880 jaims_py-2.0.0b3/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     4692 2024-05-19 16:10:04.000000 jaims_py-2.0.0b3/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.217547 jaims_py-2.0.0b3/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)     1455 2024-05-19 15:19:54.000000 jaims_py-2.0.0b3/jaims/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.217676 jaims_py-2.0.0b3/jaims/adapters/
+-rw-r--r--   0 mush       (501) staff       (20)       74 2024-05-18 20:45:15.000000 jaims_py-2.0.0b3/jaims/adapters/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.218093 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      103 2024-05-19 15:10:17.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     8712 2024-05-19 15:27:59.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1973 2024-05-19 15:09:20.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/factory.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.218752 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      353 2024-05-19 14:46:29.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    23461 2024-05-19 14:46:37.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1999 2024-05-19 15:02:51.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/factory.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.219277 jaims_py-2.0.0b3/jaims/adapters/shared/
+-rw-r--r--   0 mush       (501) staff       (20)       76 2024-05-19 16:22:55.000000 jaims_py-2.0.0b3/jaims/adapters/shared/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     2012 2024-05-19 15:30:07.000000 jaims_py-2.0.0b3/jaims/adapters/shared/exponential_backoff_operation.py
+-rw-r--r--   0 mush       (501) staff       (20)      709 2024-05-17 18:13:25.000000 jaims_py-2.0.0b3/jaims/adapters/shared/image_utilities.py
+-rw-r--r--   0 mush       (501) staff       (20)     7093 2024-05-19 15:42:10.000000 jaims_py-2.0.0b3/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b3/jaims/default_history_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b3/jaims/default_tool_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)    14293 2024-05-19 14:44:55.000000 jaims_py-2.0.0b3/jaims/entities.py
+-rw-r--r--   0 mush       (501) staff       (20)     2308 2024-05-19 15:13:30.000000 jaims_py-2.0.0b3/jaims/factories.py
+-rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b3/jaims/interfaces.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.220375 jaims_py-2.0.0b3/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      840 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-19 16:26:32.221155 jaims_py-2.0.0b3/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-19 16:26:28.000000 jaims_py-2.0.0b3/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.220212 jaims_py-2.0.0b3/tests/
+-rw-r--r--   0 mush       (501) staff       (20)     5042 2024-05-18 19:41:11.000000 jaims_py-2.0.0b3/tests/test_adapters_exponential_backoff.py
+-rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b3/tests/test_agent.py
```

### Comparing `jaims_py-2.0.0b2/PKG-INFO` & `jaims_py-2.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: An extensible library to create AI agents using many providers.
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow==10.3.0
```

### Comparing `jaims_py-2.0.0b2/README.md` & `jaims_py-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/__init__.py` & `jaims_py-2.0.0b3/jaims/__init__.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/adapter.py` & `jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/factory.py` & `jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/factory.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/adapters/openai_adapter/adapter.py` & `jaims_py-2.0.0b3/jaims/adapters/openai_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/adapters/openai_adapter/factory.py` & `jaims_py-2.0.0b3/jaims/adapters/openai_adapter/factory.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/agent.py` & `jaims_py-2.0.0b3/jaims/agent.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/default_history_manager.py` & `jaims_py-2.0.0b3/jaims/default_history_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/default_tool_manager.py` & `jaims_py-2.0.0b3/jaims/default_tool_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/entities.py` & `jaims_py-2.0.0b3/jaims/entities.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/factories.py` & `jaims_py-2.0.0b3/jaims/factories.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims/interfaces.py` & `jaims_py-2.0.0b3/jaims/interfaces.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/jaims_py.egg-info/PKG-INFO` & `jaims_py-2.0.0b3/jaims_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: An extensible library to create AI agents using many providers.
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow==10.3.0
```

### Comparing `jaims_py-2.0.0b2/jaims_py.egg-info/SOURCES.txt` & `jaims_py-2.0.0b3/jaims_py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 jaims/adapters/__init__.py
 jaims/adapters/google_generative_ai_adapter/__init__.py
 jaims/adapters/google_generative_ai_adapter/adapter.py
 jaims/adapters/google_generative_ai_adapter/factory.py
 jaims/adapters/openai_adapter/__init__.py
 jaims/adapters/openai_adapter/adapter.py
 jaims/adapters/openai_adapter/factory.py
+jaims/adapters/shared/__init__.py
+jaims/adapters/shared/exponential_backoff_operation.py
+jaims/adapters/shared/image_utilities.py
 jaims_py.egg-info/PKG-INFO
 jaims_py.egg-info/SOURCES.txt
 jaims_py.egg-info/dependency_links.txt
 jaims_py.egg-info/requires.txt
 jaims_py.egg-info/top_level.txt
 tests/test_adapters_exponential_backoff.py
 tests/test_agent.py
```

### Comparing `jaims_py-2.0.0b2/setup.py` & `jaims_py-2.0.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Read Google Cloud AI specific requirements
 with open("requirements-googleai.txt") as f:
     requirements_google_ai = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="2.0.0-beta.2",
+    version="2.0.0-beta.3",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

### Comparing `jaims_py-2.0.0b2/tests/test_adapters_exponential_backoff.py` & `jaims_py-2.0.0b3/tests/test_adapters_exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b2/tests/test_agent.py` & `jaims_py-2.0.0b3/tests/test_agent.py`

 * *Files identical despite different names*

