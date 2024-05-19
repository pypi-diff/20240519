# Comparing `tmp/python_mqtt_framework-0.0.3.tar.gz` & `tmp/python_mqtt_framework-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mqtt_framework-0.0.3.tar", last modified: Sat May 18 21:24:35 2024, max compression
+gzip compressed data, was "python_mqtt_framework-0.0.4.tar", last modified: Sun May 19 20:22:29 2024, max compression
```

## Comparing `python_mqtt_framework-0.0.3.tar` & `python_mqtt_framework-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/mqtt_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/_topic_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:22:29.144811 python_mqtt_framework-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-19 20:22:29.144811 python_mqtt_framework-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:22:29.140811 python_mqtt_framework-0.0.4/mqtt_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/mqtt_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/mqtt_framework/_topic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/mqtt_framework/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/mqtt_framework/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:22:29.144811 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-19 20:22:29.000000 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 20:22:29.000000 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:22:29.000000 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 20:22:29.000000 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 20:22:29.000000 python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:22:29.144811 python_mqtt_framework-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-19 20:22:16.000000 python_mqtt_framework-0.0.4/setup.py
```

### Comparing `python_mqtt_framework-0.0.3/PKG-INFO` & `python_mqtt_framework-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python_mqtt_framework-0.0.3/README.md` & `python_mqtt_framework-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.3/mqtt_framework/_topic_handler.py` & `python_mqtt_framework-0.0.4/mqtt_framework/_topic_handler.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.3/mqtt_framework/client.py` & `python_mqtt_framework-0.0.4/mqtt_framework/client.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.3/mqtt_framework/settings.py` & `python_mqtt_framework-0.0.4/mqtt_framework/settings.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/PKG-INFO` & `python_mqtt_framework-0.0.4/python_mqtt_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python_mqtt_framework-0.0.3/setup.py` & `python_mqtt_framework-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     dev_dependencies = requirements_file.read().strip().split("\n")
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="python-mqtt-framework",
-    version="0.0.3",
+    version="0.0.4",
     description="An opinionated framework to handle MQTT communication in Python.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Jourdan Rodrigues",
     author_email="thiagojourdan@gmail.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

