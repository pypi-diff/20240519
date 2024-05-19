# Comparing `tmp/python_mqtt_framework-0.0.2.tar.gz` & `tmp/python_mqtt_framework-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_mqtt_framework-0.0.2.tar", last modified: Sat May 18 20:00:26 2024, max compression
+gzip compressed data, was "python_mqtt_framework-0.0.3.tar", last modified: Sat May 18 21:24:35 2024, max compression
```

## Comparing `python_mqtt_framework-0.0.2.tar` & `python_mqtt_framework-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.217307 python_mqtt_framework-0.0.2/mqtt_framework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/_topic_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/mqtt_framework/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 20:00:26.000000 python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:00:26.221308 python_mqtt_framework-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-18 20:00:15.000000 python_mqtt_framework-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/mqtt_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/_topic_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/mqtt_framework/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 21:24:35.000000 python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:24:35.496065 python_mqtt_framework-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-18 21:24:08.000000 python_mqtt_framework-0.0.3/setup.py
```

### Comparing `python_mqtt_framework-0.0.2/PKG-INFO` & `python_mqtt_framework-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -50,56 +50,37 @@
 
 * Python 3.8+
 
 We **highly recommend** and only officially support the latest patch release of each Python series.
 
 # Installation
 
-Install using `pip` (soon)...
+Install using `pip`.
 
     pip install python-mqtt-framework
 
+# Defining topic handlers
 
-# Django Integration
-
-Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'mqtt_framework',
-]
-```
-
-## Running the MQTT listener
-
-To run the MQTT listener, you can use the `runmqtt` management command:
-
-    python manage.py runmqtt
-
-## Defining topic handlers
-
-Within `your_app/topic_handlers.py` module, you'll write the topic handlers:
+This is how you write the topic handlers:
 
 ```python
 from mqtt_framework import TopicHandler
 from rest_framework import serializers
-from django.core.cache import cache
 from pydantic import BaseModel
 
 
 class SimpleTestModel(BaseModel):
     testing: str
 
 
 class SimpleTestSerializer(serializers.Serializer):
     testing = serializers.CharField()
 
     def create(self, validated_data):
-        cache.set('test_message', validated_data)
+        print('test_message', validated_data)
         return validated_data
 
 
 class SerializerTopicHandler(TopicHandler):
     topic = 'test/topic'
     serializer_class = SimpleTestSerializer
     qos = 1
@@ -113,14 +94,33 @@
     qos = 0
 
     def handle(self):
         pydantic_instance = self.get_validated_payload()
         # Do something with the pydantic_instance
 ```
 
+There's no need to register the topic handlers, the framework will automatically discover them as long as they are imported.
+
+# Django Integration
+
+Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'mqtt_framework',
+]
+```
+
+## Running the MQTT listener
+
+To run the MQTT listener, you can use the `runmqtt` management command:
+
+    python manage.py runmqtt
+
 ## Settings
 
 ```python
 MQTT_FRAMEWORK = {
     'BROKER_URL': 'mqtt://<user>:<password>@<host>:<port>',
     'TOPIC_HANDLERS': 'your_app.topic_handlers',
     'KEEPALIVE': 60,
```

### Comparing `python_mqtt_framework-0.0.2/README.md` & `python_mqtt_framework-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,56 +16,37 @@
 
 * Python 3.8+
 
 We **highly recommend** and only officially support the latest patch release of each Python series.
 
 # Installation
 
-Install using `pip` (soon)...
+Install using `pip`.
 
     pip install python-mqtt-framework
 
+# Defining topic handlers
 
-# Django Integration
-
-Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'mqtt_framework',
-]
-```
-
-## Running the MQTT listener
-
-To run the MQTT listener, you can use the `runmqtt` management command:
-
-    python manage.py runmqtt
-
-## Defining topic handlers
-
-Within `your_app/topic_handlers.py` module, you'll write the topic handlers:
+This is how you write the topic handlers:
 
 ```python
 from mqtt_framework import TopicHandler
 from rest_framework import serializers
-from django.core.cache import cache
 from pydantic import BaseModel
 
 
 class SimpleTestModel(BaseModel):
     testing: str
 
 
 class SimpleTestSerializer(serializers.Serializer):
     testing = serializers.CharField()
 
     def create(self, validated_data):
-        cache.set('test_message', validated_data)
+        print('test_message', validated_data)
         return validated_data
 
 
 class SerializerTopicHandler(TopicHandler):
     topic = 'test/topic'
     serializer_class = SimpleTestSerializer
     qos = 1
@@ -79,14 +60,33 @@
     qos = 0
 
     def handle(self):
         pydantic_instance = self.get_validated_payload()
         # Do something with the pydantic_instance
 ```
 
+There's no need to register the topic handlers, the framework will automatically discover them as long as they are imported.
+
+# Django Integration
+
+Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'mqtt_framework',
+]
+```
+
+## Running the MQTT listener
+
+To run the MQTT listener, you can use the `runmqtt` management command:
+
+    python manage.py runmqtt
+
 ## Settings
 
 ```python
 MQTT_FRAMEWORK = {
     'BROKER_URL': 'mqtt://<user>:<password>@<host>:<port>',
     'TOPIC_HANDLERS': 'your_app.topic_handlers',
     'KEEPALIVE': 60,
```

### Comparing `python_mqtt_framework-0.0.2/mqtt_framework/_topic_handler.py` & `python_mqtt_framework-0.0.3/mqtt_framework/_topic_handler.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.2/mqtt_framework/client.py` & `python_mqtt_framework-0.0.3/mqtt_framework/client.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.2/mqtt_framework/settings.py` & `python_mqtt_framework-0.0.3/mqtt_framework/settings.py`

 * *Files identical despite different names*

### Comparing `python_mqtt_framework-0.0.2/python_mqtt_framework.egg-info/PKG-INFO` & `python_mqtt_framework-0.0.3/python_mqtt_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-mqtt-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: An opinionated framework to handle MQTT communication in Python.
 Home-page: https://github.com/jourdanrodrigues/python-mqtt-framework
 Author: Jourdan Rodrigues
 Author-email: thiagojourdan@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -50,56 +50,37 @@
 
 * Python 3.8+
 
 We **highly recommend** and only officially support the latest patch release of each Python series.
 
 # Installation
 
-Install using `pip` (soon)...
+Install using `pip`.
 
     pip install python-mqtt-framework
 
+# Defining topic handlers
 
-# Django Integration
-
-Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'mqtt_framework',
-]
-```
-
-## Running the MQTT listener
-
-To run the MQTT listener, you can use the `runmqtt` management command:
-
-    python manage.py runmqtt
-
-## Defining topic handlers
-
-Within `your_app/topic_handlers.py` module, you'll write the topic handlers:
+This is how you write the topic handlers:
 
 ```python
 from mqtt_framework import TopicHandler
 from rest_framework import serializers
-from django.core.cache import cache
 from pydantic import BaseModel
 
 
 class SimpleTestModel(BaseModel):
     testing: str
 
 
 class SimpleTestSerializer(serializers.Serializer):
     testing = serializers.CharField()
 
     def create(self, validated_data):
-        cache.set('test_message', validated_data)
+        print('test_message', validated_data)
         return validated_data
 
 
 class SerializerTopicHandler(TopicHandler):
     topic = 'test/topic'
     serializer_class = SimpleTestSerializer
     qos = 1
@@ -113,14 +94,33 @@
     qos = 0
 
     def handle(self):
         pydantic_instance = self.get_validated_payload()
         # Do something with the pydantic_instance
 ```
 
+There's no need to register the topic handlers, the framework will automatically discover them as long as they are imported.
+
+# Django Integration
+
+Add `'mqtt_framework'` to your `INSTALLED_APPS` setting.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'mqtt_framework',
+]
+```
+
+## Running the MQTT listener
+
+To run the MQTT listener, you can use the `runmqtt` management command:
+
+    python manage.py runmqtt
+
 ## Settings
 
 ```python
 MQTT_FRAMEWORK = {
     'BROKER_URL': 'mqtt://<user>:<password>@<host>:<port>',
     'TOPIC_HANDLERS': 'your_app.topic_handlers',
     'KEEPALIVE': 60,
```

### Comparing `python_mqtt_framework-0.0.2/setup.py` & `python_mqtt_framework-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     dev_dependencies = requirements_file.read().strip().split("\n")
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="python-mqtt-framework",
-    version="0.0.2",
+    version="0.0.3",
     description="An opinionated framework to handle MQTT communication in Python.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Jourdan Rodrigues",
     author_email="thiagojourdan@gmail.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

