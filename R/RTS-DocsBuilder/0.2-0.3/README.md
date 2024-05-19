# Comparing `tmp/RTS_DocsBuilder-0.2.tar.gz` & `tmp/RTS_DocsBuilder-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_DocsBuilder-0.2.tar", last modified: Sun May 19 10:20:42 2024, max compression
+gzip compressed data, was "RTS_DocsBuilder-0.3.tar", last modified: Sun May 19 11:49:55 2024, max compression
```

## Comparing `RTS_DocsBuilder-0.2.tar` & `RTS_DocsBuilder-0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.615400 RTS_DocsBuilder-0.2/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.2/LICENCE
--rw-rw-rw-   0        0        0      869 2024-05-19 10:20:42.614893 RTS_DocsBuilder-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.598597 RTS_DocsBuilder-0.2/RTS_DocsBuilder/
--rw-rw-rw-   0        0        0     5757 2024-05-19 10:20:36.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/RInitiate.py
--rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/__init__.py
--rw-rw-rw-   0        0        0    10655 2024-04-29 16:06:45.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/doclayout.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.613889 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/
--rw-rw-rw-   0        0        0      869 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:20:42.615400 RTS_DocsBuilder-0.2/setup.cfg
--rw-rw-rw-   0        0        0      938 2024-04-29 17:41:43.000000 RTS_DocsBuilder-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.115406 RTS_DocsBuilder-0.3/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.3/LICENCE
+-rw-rw-rw-   0        0        0      869 2024-05-19 11:49:55.114902 RTS_DocsBuilder-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.091094 RTS_DocsBuilder-0.3/RTS_DocsBuilder/
+-rw-rw-rw-   0        0        0     6174 2024-05-19 10:25:24.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/RInitiate.py
+-rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/__init__.py
+-rw-rw-rw-   0        0        0    10656 2024-05-19 11:18:43.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/doclayout.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.113899 RTS_DocsBuilder-0.3/RTS_DocsBuilder/srcFolder/
+-rw-rw-rw-   0        0        0        0 2024-05-19 11:49:40.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder/srcFolder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:49:55.113394 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/
+-rw-rw-rw-   0        0        0      869 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 11:49:55.000000 RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:49:55.115406 RTS_DocsBuilder-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      938 2024-05-19 11:49:51.000000 RTS_DocsBuilder-0.3/setup.py
```

### Comparing `RTS_DocsBuilder-0.2/LICENCE` & `RTS_DocsBuilder-0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_DocsBuilder-0.2/PKG-INFO` & `RTS_DocsBuilder-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS_DocsBuilder
-Version: 0.2
+Version: 0.3
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.2/RTS_DocsBuilder/RInitiate.py` & `RTS_DocsBuilder-0.3/RTS_DocsBuilder/RInitiate.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,21 @@
                 py_files = [file for file in os.listdir(topic_path) if file.endswith('.py')]
                 # Check if there is exactly one .py file
                 if len(py_files) == 1:
                     # Add the topic to the 'topics' list
                     self.topics.append((os.path.splitext(py_files[0])[0], '/' + display_topic))
                     # Store the module path and function name
                     module_path = os.path.join(topic_path, os.path.splitext(py_files[0])[0])
-                    module_path = os.path.relpath(module_path, module_root_folder).replace(os.sep, '.')
+                    try:
+                        # Versuchen Sie, den relativen Pfad zu berechnen
+                        module_path = os.path.relpath(module_path, module_root_folder).replace(os.sep, '.')
+                    except ValueError:
+                        # Wenn sich die Pfade auf unterschiedlichen Laufwerken befinden, verwenden Sie den absoluten Pfad
+                        # und ersetzen Sie die Pfadtrennzeichen durch Punkte
+                        module_path = module_path.replace(os.sep, '.')
                     if module_path.startswith('...'):
                         module_path = module_path[3:]
                     function_name = os.path.splitext(py_files[0])[0]  # Get the function name from the file name
                     self.initiator.append((module_path, function_name))
                     # Initialize the 'topic_subtopics' list
                     topic_subtopics = []
                     # Iterate over the subtopics in the topic folder
```

### Comparing `RTS_DocsBuilder-0.2/RTS_DocsBuilder/doclayout.py` & `RTS_DocsBuilder-0.3/RTS_DocsBuilder/doclayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self._currentTopic , self._currentsub = whereami
         self._currentTopic = re.sub(r'^[a-z]--', '', self._currentTopic)
         if self._currentsub:
             self._currentsub = re.sub(r'^[a-z]--', '', self._currentsub)
         print("--------------------------------------------------------------------")
         print(self._modulename + " > " + self._currentTopic + " > " + str(self._currentsub))
         
-        module_name = self._modulename + ".docs.load"
+        module_name = self._modulename + ".docs.loads"
         module = importlib.import_module(module_name)
 
         docMemory = module.docMemory
         #print("rlos",docMemory.initDocs.topics, docMemory.initDocs.subtopics)
         
 
         if not isinstance(path, str):
```

### Comparing `RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/PKG-INFO` & `RTS_DocsBuilder-0.3/RTS_DocsBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-DocsBuilder
-Version: 0.2
+Version: 0.3
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.2/setup.py` & `RTS_DocsBuilder-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS_DocsBuilder',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     description='Create local documentations for your modules. Requires RTS_WebUIBuilder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

