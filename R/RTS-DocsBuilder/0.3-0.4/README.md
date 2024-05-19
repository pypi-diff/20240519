# Comparing `tmp/RTS_DocsBuilder-0.3.tar.gz` & `tmp/RTS_DocsBuilder-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_DocsBuilder-0.3.tar", last modified: Sun May 19 11:49:55 2024, max compression
+gzip compressed data, was "RTS_DocsBuilder-0.4.tar", last modified: Sun May 19 11:57:45 2024, max compression
```

## Comparing `RTS_DocsBuilder-0.3.tar` & `RTS_DocsBuilder-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.115406 RTS_DocsBuilder-0.3/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.3/LICENCE
--rw-rw-rw-   0        0        0      869 2024-05-19 11:49:55.114902 RTS_DocsBuilder-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.091094 RTS_DocsBuilder-0.3/RTS_DocsBuilder/
--rw-rw-rw-   0        0        0     6174 2024-05-19 10:25:24.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/RInitiate.py
--rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/__init__.py
--rw-rw-rw-   0        0        0    10656 2024-05-19 11:18:43.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/doclayout.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.113899 RTS_DocsBuilder-0.3/RTS_DocsBuilder/srcFolder/
--rw-rw-rw-   0        0        0        0 2024-05-19 11:49:40.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/srcFolder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.113394 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/
--rw-rw-rw-   0        0        0      869 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 11:49:55.115406 RTS_DocsBuilder-0.3/setup.cfg
--rw-rw-rw-   0        0        0      938 2024-05-19 11:49:51.000000 RTS_DocsBuilder-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:57:45.055107 RTS_DocsBuilder-0.4/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.4/LICENCE
+-rw-rw-rw-   0        0        0      869 2024-05-19 11:57:45.054608 RTS_DocsBuilder-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 11:57:45.042594 RTS_DocsBuilder-0.4/RTS_DocsBuilder/
+-rw-rw-rw-   0        0        0     6022 2024-05-19 11:53:08.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder/RInitiate.py
+-rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder/__init__.py
+-rw-rw-rw-   0        0        0    10656 2024-05-19 11:18:43.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder/doclayout.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:57:45.053608 RTS_DocsBuilder-0.4/RTS_DocsBuilder/srcFolder/
+-rw-rw-rw-   0        0        0        0 2024-05-19 11:49:40.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder/srcFolder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:57:45.052611 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/
+-rw-rw-rw-   0        0        0      869 2024-05-19 11:57:45.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-19 11:57:45.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:57:45.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 11:57:45.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 11:57:45.000000 RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:57:45.055107 RTS_DocsBuilder-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      970 2024-05-19 11:57:41.000000 RTS_DocsBuilder-0.4/setup.py
```

### Comparing `RTS_DocsBuilder-0.3/LICENCE` & `RTS_DocsBuilder-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_DocsBuilder-0.3/PKG-INFO` & `RTS_DocsBuilder-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS_DocsBuilder
-Version: 0.3
+Version: 0.4
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.3/RTS_DocsBuilder/RInitiate.py` & `RTS_DocsBuilder-0.4/RTS_DocsBuilder/RInitiate.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,27 @@
         module_root_folder = os.path.dirname(module_file_path)
         
         if os.path.basename(module_root_folder) != 'docs':
             docs_folder_path = os.path.join(module_root_folder, 'docs')
         else:
             docs_folder_path = module_root_folder
         if os.path.exists(docs_folder_path):
-            self.create_topic_subtopic_structure(docs_folder_path)
+            stack = inspect.stack()
+            caller_frame = stack[1]
+            caller_module = inspect.getmodule(caller_frame[0])
+            caller_path = caller_module.__file__
+            module_root_folder = os.path.dirname(os.path.abspath(caller_path))
+            self.create_topic_subtopic_structure(docs_folder_path,module_root_folder)
         else:
             print("No 'docs' folder exists in the module root folder.")
 
-    def create_topic_subtopic_structure(self, docs_folder_path):
+    def create_topic_subtopic_structure(self, docs_folder_path, module_root_folder):
+        
+        # Durchsuchen Sie den Stack, um den Pfad des aufrufenden Skripts zu finden
         
-        # Get the root folder of the module
-        module_root_folder = os.path.dirname(os.path.abspath(__file__))
     
         # Initialize the 'subtopics' list and 'initiator' list
         self.subtopics = []
         self.initiator = []
     
         # Iterate over the topics in the 'docs' folder
         for topic in os.listdir(docs_folder_path):
@@ -57,21 +62,26 @@
                 py_files = [file for file in os.listdir(topic_path) if file.endswith('.py')]
                 # Check if there is exactly one .py file
                 if len(py_files) == 1:
                     # Add the topic to the 'topics' list
                     self.topics.append((os.path.splitext(py_files[0])[0], '/' + display_topic))
                     # Store the module path and function name
                     module_path = os.path.join(topic_path, os.path.splitext(py_files[0])[0])
+                    print("Module Path: ", module_path)
+                    print("Module Root Folder: ", module_root_folder)
                     try:
                         # Versuchen Sie, den relativen Pfad zu berechnen
                         module_path = os.path.relpath(module_path, module_root_folder).replace(os.sep, '.')
+                        print("Module Path: ", module_path)
                     except ValueError:
                         # Wenn sich die Pfade auf unterschiedlichen Laufwerken befinden, verwenden Sie den absoluten Pfad
                         # und ersetzen Sie die Pfadtrennzeichen durch Punkte
                         module_path = module_path.replace(os.sep, '.')
+                    print("Module Path: ", module_path)
+
                     if module_path.startswith('...'):
                         module_path = module_path[3:]
                     function_name = os.path.splitext(py_files[0])[0]  # Get the function name from the file name
                     self.initiator.append((module_path, function_name))
                     # Initialize the 'topic_subtopics' list
                     topic_subtopics = []
                     # Iterate over the subtopics in the topic folder
@@ -93,22 +103,7 @@
                                 subtopic_function_name = os.path.splitext(subtopic_py_files[0])[0]  # Get the function name from the file name
                                 self.initiator.append((subtopic_module_path, subtopic_function_name))
                     # Add the 'topic_subtopics' list to the 'subtopics' list
                     self.subtopics.append(topic_subtopics)
             print("Topics: ", self.topics)
             print("Subtopics: ", self.subtopics)
     
-    def execute_initiator(self):
-        for module_path, function_name in self.initiator:
-            #try:
-                # Import the module
-                module = importlib.import_module(module_path)
-                # Get the function
-                function = getattr(module, function_name)
-                # Call the function
-                function()
-            #except ImportError as e:
-            #    print(f"Failed to import module {module_path}. Error: ", e)
-            #    return
-            #except AttributeError as e:
-            #    print(f"Failed to find function {function_name} in module {module_path}. Error: ", e)
-            #    return
```

### Comparing `RTS_DocsBuilder-0.3/RTS_DocsBuilder/doclayout.py` & `RTS_DocsBuilder-0.4/RTS_DocsBuilder/doclayout.py`

 * *Files identical despite different names*

### Comparing `RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/PKG-INFO` & `RTS_DocsBuilder-0.4/RTS_DocsBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-DocsBuilder
-Version: 0.3
+Version: 0.4
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.3/setup.py` & `RTS_DocsBuilder-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS_DocsBuilder',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
+    include_package_data=True,
     description='Create local documentations for your modules. Requires RTS_WebUIBuilder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
     url='https://github.com/RandomTimeLP/RTS_Documentations',
```

