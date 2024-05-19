# Comparing `tmp/llm_parametrizer-0.1.1.tar.gz` & `tmp/llm_parametrizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_parametrizer-0.1.1.tar", last modified: Sun May 19 06:04:59 2024, max compression
+gzip compressed data, was "llm_parametrizer-0.1.2.tar", last modified: Sun May 19 06:50:00 2024, max compression
```

## Comparing `llm_parametrizer-0.1.1.tar` & `llm_parametrizer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:04:59.930487 llm_parametrizer-0.1.1/
--rw-r--r--   0 i5         (501) staff       (20)     5391 2024-05-19 06:04:59.929883 llm_parametrizer-0.1.1/PKG-INFO
--rw-r--r--   0 i5         (501) staff       (20)     5109 2024-05-18 20:13:03.000000 llm_parametrizer-0.1.1/README.md
-drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:04:59.922742 llm_parametrizer-0.1.1/llm_parametrizer/
--rw-r--r--   0 i5         (501) staff       (20)       84 2024-05-18 20:16:02.000000 llm_parametrizer-0.1.1/llm_parametrizer/__init__.py
--rw-r--r--   0 i5         (501) staff       (20)     6673 2024-05-18 20:21:19.000000 llm_parametrizer-0.1.1/llm_parametrizer/llm_parametrizer.py
--rw-r--r--   0 i5         (501) staff       (20)     2307 2024-05-18 12:25:36.000000 llm_parametrizer-0.1.1/llm_parametrizer/open_AI_models.py
-drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:04:59.928220 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/
--rw-r--r--   0 i5         (501) staff       (20)     5391 2024-05-19 06:04:59.000000 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/PKG-INFO
--rw-r--r--   0 i5         (501) staff       (20)      318 2024-05-19 06:04:59.000000 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/SOURCES.txt
--rw-r--r--   0 i5         (501) staff       (20)        1 2024-05-19 06:04:59.000000 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/dependency_links.txt
--rw-r--r--   0 i5         (501) staff       (20)       21 2024-05-19 06:04:59.000000 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/requires.txt
--rw-r--r--   0 i5         (501) staff       (20)       17 2024-05-19 06:04:59.000000 llm_parametrizer-0.1.1/llm_parametrizer.egg-info/top_level.txt
--rw-r--r--   0 i5         (501) staff       (20)       38 2024-05-19 06:04:59.930726 llm_parametrizer-0.1.1/setup.cfg
--rw-r--r--   0 i5         (501) staff       (20)      548 2024-05-19 06:04:26.000000 llm_parametrizer-0.1.1/setup.py
+drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:50:00.571076 llm_parametrizer-0.1.2/
+-rw-r--r--   0 i5         (501) staff       (20)     5443 2024-05-19 06:50:00.570643 llm_parametrizer-0.1.2/PKG-INFO
+-rw-r--r--   0 i5         (501) staff       (20)     5161 2024-05-19 06:47:04.000000 llm_parametrizer-0.1.2/README.md
+drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:50:00.563929 llm_parametrizer-0.1.2/llm_parametrizer/
+-rw-r--r--   0 i5         (501) staff       (20)       84 2024-05-18 20:16:02.000000 llm_parametrizer-0.1.2/llm_parametrizer/__init__.py
+-rw-r--r--   0 i5         (501) staff       (20)     6677 2024-05-19 06:43:28.000000 llm_parametrizer-0.1.2/llm_parametrizer/llm_parametrizer.py
+-rw-r--r--   0 i5         (501) staff       (20)     2307 2024-05-18 12:25:36.000000 llm_parametrizer-0.1.2/llm_parametrizer/open_AI_models.py
+drwxr-xr-x   0 i5         (501) staff       (20)        0 2024-05-19 06:50:00.569753 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/
+-rw-r--r--   0 i5         (501) staff       (20)     5443 2024-05-19 06:50:00.000000 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/PKG-INFO
+-rw-r--r--   0 i5         (501) staff       (20)      318 2024-05-19 06:50:00.000000 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/SOURCES.txt
+-rw-r--r--   0 i5         (501) staff       (20)        1 2024-05-19 06:50:00.000000 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/dependency_links.txt
+-rw-r--r--   0 i5         (501) staff       (20)       21 2024-05-19 06:50:00.000000 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/requires.txt
+-rw-r--r--   0 i5         (501) staff       (20)       17 2024-05-19 06:50:00.000000 llm_parametrizer-0.1.2/llm_parametrizer.egg-info/top_level.txt
+-rw-r--r--   0 i5         (501) staff       (20)       38 2024-05-19 06:50:00.571309 llm_parametrizer-0.1.2/setup.cfg
+-rw-r--r--   0 i5         (501) staff       (20)      548 2024-05-19 06:49:20.000000 llm_parametrizer-0.1.2/setup.py
```

### Comparing `llm_parametrizer-0.1.1/PKG-INFO` & `llm_parametrizer-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_parametrizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to parametrize multiple API calls for LLMs
 Home-page: https://github.com/arjuna-dev/llm_parametrizer
 Author: Alejandro Camus
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -27,24 +27,20 @@
 
 * openai
 * python-dotenv
 
 
 ## Features
 
-Test an API call with various parametrized values:
-
-* Prompts
-* Roles
-* Models
-* Temperatures
-
-  \
-
-
+* Test an API call with various parametrized values:
+  * Prompts
+  * Roles
+  * Models
+  * Temperatures
+* Save as CSV to view en google sheets or similar
 
 
 Parameters not yet implemented include:
 
 * Seeds
 * Frequency penalties
 * Presence penalties
```

### Comparing `llm_parametrizer-0.1.1/README.md` & `llm_parametrizer-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,20 @@
 
 * openai
 * python-dotenv
 
 
 ## Features
 
-Test an API call with various parametrized values:
-
-* Prompts
-* Roles
-* Models
-* Temperatures
-
-  \
-
-
+* Test an API call with various parametrized values:
+  * Prompts
+  * Roles
+  * Models
+  * Temperatures
+* Save as CSV to view en google sheets or similar
 
 
 Parameters not yet implemented include:
 
 * Seeds
 * Frequency penalties
 * Presence penalties
```

### Comparing `llm_parametrizer-0.1.1/llm_parametrizer/llm_parametrizer.py` & `llm_parametrizer-0.1.2/llm_parametrizer/llm_parametrizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,17 @@
 
                 except Exception as e:
                     if return_raw:
                         results[str(parameters)] = f"Error: {str(e)}"
                     else:
                         results += f"Error: {str(e)}\n"
             if output_csv:
-                with open(f"results_{date}", mode='w', newline='') as file:
+                with open(f"results_{date}.csv", mode='w', newline='') as file:
                     writer = csv.writer(file)
-                    writer.writerow(["Prompt User", "Prompt System", "Temperature", "Model", "Time", "Response"])
+                    writer.writerow(["Prompt User", "Prompt System", "Temperature", "Model", "Date", "Response"])
                     writer.writerows(csv_data)
 
             return results
 
     def parametrize(self):
         combinations = product(self.messages, self.models, self.temperatures)
         self.all_parameters = [{'messages':messages, 'model': model, "temperature": temperature} for messages, model, temperature in combinations]
```

### Comparing `llm_parametrizer-0.1.1/llm_parametrizer/open_AI_models.py` & `llm_parametrizer-0.1.2/llm_parametrizer/open_AI_models.py`

 * *Files identical despite different names*

### Comparing `llm_parametrizer-0.1.1/llm_parametrizer.egg-info/PKG-INFO` & `llm_parametrizer-0.1.2/llm_parametrizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-parametrizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to parametrize multiple API calls for LLMs
 Home-page: https://github.com/arjuna-dev/llm_parametrizer
 Author: Alejandro Camus
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -27,24 +27,20 @@
 
 * openai
 * python-dotenv
 
 
 ## Features
 
-Test an API call with various parametrized values:
-
-* Prompts
-* Roles
-* Models
-* Temperatures
-
-  \
-
-
+* Test an API call with various parametrized values:
+  * Prompts
+  * Roles
+  * Models
+  * Temperatures
+* Save as CSV to view en google sheets or similar
 
 
 Parameters not yet implemented include:
 
 * Seeds
 * Frequency penalties
 * Presence penalties
```

### Comparing `llm_parametrizer-0.1.1/setup.py` & `llm_parametrizer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='llm_parametrizer',
-    version='0.1.1',
+    version='0.1.2',
     author ="Alejandro Camus",
     description="A library to parametrize multiple API calls for LLMs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['llm_parametrizer'],
     url="https://github.com/arjuna-dev/llm_parametrizer",
     install_requires=[
```

