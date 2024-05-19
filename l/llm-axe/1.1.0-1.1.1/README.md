# Comparing `tmp/llm_axe-1.1.0.tar.gz` & `tmp/llm_axe-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-1.1.0.tar", last modified: Sat May 18 16:20:25 2024, max compression
+gzip compressed data, was "llm_axe-1.1.1.tar", last modified: Sun May 19 20:29:45 2024, max compression
```

## Comparing `llm_axe-1.1.0.tar` & `llm_axe-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.194175 llm_axe-1.1.0/
--rw-rw-rw-   0        0        0     3914 2024-05-18 16:20:25.193673 llm_axe-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.178674 llm_axe-1.1.0/llm_axe/
--rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.1.0/llm_axe/__init__.py
--rw-rw-rw-   0        0        0    26131 2024-05-18 16:12:16.000000 llm_axe-1.1.0/llm_axe/agents.py
--rw-rw-rw-   0        0        0     6172 2024-05-18 05:39:43.000000 llm_axe-1.1.0/llm_axe/core.py
--rw-rw-rw-   0        0        0      640 2024-05-18 05:10:13.000000 llm_axe-1.1.0/llm_axe/models.py
--rw-rw-rw-   0        0        0     9070 2024-05-18 16:01:16.000000 llm_axe-1.1.0/llm_axe/system_prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-05-18 16:20:25.192673 llm_axe-1.1.0/llm_axe.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 16:20:25.000000 llm_axe-1.1.0/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 16:20:25.194175 llm_axe-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4619 2024-05-18 16:19:51.000000 llm_axe-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.616440 llm_axe-1.1.1/
+-rw-rw-rw-   0        0        0     3914 2024-05-19 20:29:45.615441 llm_axe-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.575940 llm_axe-1.1.1/llm_axe/
+-rw-rw-rw-   0        0        0       67 2024-04-22 04:52:11.000000 llm_axe-1.1.1/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    27219 2024-05-19 20:27:16.000000 llm_axe-1.1.1/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     6486 2024-05-19 20:27:25.000000 llm_axe-1.1.1/llm_axe/core.py
+-rw-rw-rw-   0        0        0      640 2024-05-18 05:10:13.000000 llm_axe-1.1.1/llm_axe/models.py
+-rw-rw-rw-   0        0        0     9689 2024-05-19 15:56:00.000000 llm_axe-1.1.1/llm_axe/system_prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-05-19 20:29:45.614439 llm_axe-1.1.1/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 20:29:45.000000 llm_axe-1.1.1/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 20:29:45.616440 llm_axe-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4619 2024-05-19 20:26:57.000000 llm_axe-1.1.1/setup.py
```

### Comparing `llm_axe-1.1.0/PKG-INFO` & `llm_axe-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_axe
-Version: 1.1.0
+Version: 1.1.1
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.1.0/llm_axe/agents.py` & `llm_axe-1.1.1/llm_axe/agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,37 @@
 from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf, make_prompt, llm_has_ask
 
 
 class Agent:
     """
     Basic agent that can use premade or custom system prompts.
     """
-    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None, temperature:float=0.8):
+    def __init__(self, llm:object, agent_type:AgentType=None, additional_system_instructions:str="", custom_system_prompt:str=None, format:str="", temperature:float=0.8):
         """
         Args:
             llm (object): An LLM object with an ask function.
             agent_type (AgentType, optional): The type of agent to use. Choose from AgentType enum. Defaults to None.
-            additional_system_instructions (str, optional): Additional system instructions to include in the system prompt. Defaults to "".
-            custom_system_prompt (any, optional): An optional string to override and use as the custom system prompt.
+            additional_system_instructions (str, optional): Additional system instructions to include in the premade system prompt. Defaults to "".
+            custom_system_prompt (any, optional): An optional string to totally override and use as the custom system prompt.
+            format (str, optional): The format of the response. Use "json" for json. Defaults to "".
             temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         self.llm = llm
         self.chat_history = []
         if custom_system_prompt is None:
             if agent_type is None:
                 raise ValueError("You must provide either a AgentType or a custom_system_prompt.")
             else:
                 self.system_prompt = get_yaml_prompt("system_prompts.yaml", agent_type.value)
         else:
             self.system_prompt = custom_system_prompt
         
         self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
         self.temperature = temperature
+        self.format = format
 
     def get_prompt(self, question):
         """
         Get the prompt for the given question.
         Args:
             question (str): The question to get the prompt for.
         """
@@ -52,78 +54,87 @@
             return None
         
         prompts = [self.system_prompt]
         if history is not None:
             prompts.extend(history)
 
         prompts.append(make_prompt("user", prompt))
-        response = self.llm.ask(prompts, temperature=self.temperature)
+        response = self.llm.ask(prompts, temperature=self.temperature, format=self.format)
     
         self.chat_history.append(prompts[-1])
         self.chat_history.append(make_prompt("assistant", response))
         return response
 
 
 class ObjectDetectorAgent():
     """
     An ObjectDetectorAgent agent is used to detect objects in an image.
     Requires a multimodal LLM.
     """
-    def __init__(self, llm:object, temperature:float=0.3):
+    def __init__(self, vision_llm:object, text_llm:object, vision_temperature:float=0.3, text_temperature:float=0.3):
         """
         Initializes a new ObjectDetectorAgent object.
 
         Args:
-            llm (object): A multimodal LLM object that implements the ask() method.
-            temperature (float, optional): The temperature of the LLM. Defaults to 0.3.
+            vision_llm (object): A multimodal LLM object that implements the ask() method.
+            text_llm (object): An llm that is responsible for the final output
+            vision_temperature (float, optional): The temperature of the vision LLM. Defaults to 0.3.
+            text_temperature (float, optional): The temperature of the text LLM. Defaults to 0.3.
         """
-        self.llm = llm
+        self.vision_llm = vision_llm
+        self.text_llm = text_llm
         self.__system_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ObjectDetector"))
-        self.temperature = temperature
+        self.vision_temperature = vision_temperature
+        self.text_temperature = text_temperature
 
     def detect(self, images:list, objects:list=None, detection_criteria:str=None):
         """
         Detects objects in an image.
         If given a list of objects, only the objects in the list will be detected.
-        If a prompt is given instead, it will detect according to the prompt's instructions. 
+        If a detection_criteria is given instead, it will detect according to the criteria's instructions. 
         Args:
             images (list): The images to detect objects in. List of string paths or byte data.
             objects (list, optional): An optional list of objects to detect. Defaults to None.
             detection_criteria (str, optional): An opetional detection criteria to give.
         """
-        if llm_has_ask(self.llm) is False:
+        if llm_has_ask(self.vision_llm) is False or llm_has_ask(self.text_llm) is False:
             return None
         
         prompts = make_prompt("user", "Detect all objects in this image", images=images)
-        detected_objects = self.llm.ask([self.__system_prompt, prompts], temperature=self.temperature)
+        detected_objects = self.vision_llm.ask([self.__system_prompt, prompts], temperature=self.vision_temperature)
         prompts = self.__get_prompt(images, detected_objects, objects, detection_criteria)
-        response = self.llm.ask(prompts, format="json", temperature=0.1)
+        response = self.text_llm.ask(prompts, format="json", temperature=self.text_temperature)
 
         return response
         
     def __get_prompt(self, images:list, detected_objects:list, objects:list=None, detection_criteria:str=None):
         """
         Get the prompt for the given objects and detection_prompt.
         Args:
             images (list): The images to detect objects in. List of string paths or byte data.
             detected_objects (list): The detected objects in the images.
             objects (list, optional): An optional list of objects to detect. Defaults to None.
             detection_criteria (str, optional): An opetional detection criteria to give.
         """
         prompt = ""
         sys_prompt = make_prompt("system", get_yaml_prompt("system_prompts.yaml", "ObjectFilterer"))
-        if detection_criteria is None:
-            if objects is None:
-                raise ValueError("You must provide either an object list or a detection_prompt.")
-            else:
-                prompt = "Image Objects: " + detected_objects + "\n\n My list of objects I'm interested in is: " + ", ".join(objects)
+
+        if objects is not None and detection_criteria is not None:
+            raise ValueError("You cannot provide both an object list and a detection_prompt.")
         else:
-            prompt = "Image Objects: " + detected_objects + "\n" + detection_criteria
-        prompt = make_prompt("user", prompt, images=images)
-        return [sys_prompt, prompt]
+            if detection_criteria is None:
+                if objects is None:
+                    raise ValueError("You must provide either an object list or a detection_prompt.")
+                else:
+                    prompt = "Image Description: " + detected_objects + "\n\nI'm INTERESTED in the following OBJECTS: " + ", ".join(objects)
+            else:
+                prompt = "Image Description: " + detected_objects + "\n\n I'm INTERESTED in the following: " + detection_criteria
+            prompt = prompt + "\n Only return the objects that fit my interests"
+            prompt = make_prompt("user", prompt)
+            return [sys_prompt, prompt]
 
 
 class PythonAgent():
     """
     A PytonAgent agent is used to solve problems by writing Python code.
     It will provide code to execute and the imports used in the code.
     IMPORTANT!!: Code should ALWAYS be executed in a virtual or isolated environment.
@@ -193,14 +204,16 @@
             llm (object): An object that implements the ask() method.
             reply_as_json (bool, optional): If True, the response will be in the format of a JSON object. Defaults to False.
             additional_system_instructions (str, optional): Additional instructions to include in the system prompt. Defaults to "".
             temperature (float, optional): The temperature of the LLM. Defaults to 0.8.
         """
         yaml_prompt = "DataExtractorJson" if reply_as_json else "DataExtractor"
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", yaml_prompt)
+        if reply_as_json:
+            self.system_prompt = self.system_prompt + "\n Respond in JSON format"
         self.system_prompt = make_prompt("system", self.system_prompt.format(additional_instructions=additional_system_instructions))
         self.llm = llm
         self.chat_history = []
         self.temperature = temperature
 
     def get_prompt(self, info:str, data_points:list=[]):
         """
```

### Comparing `llm_axe-1.1.0/llm_axe/core.py` & `llm_axe-1.1.1/llm_axe/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,23 @@
     if not hasattr(llm, "ask"):
             warnings.warn("llm object must have an ask function! See OllamaChat class in models.py for an example.")
             return False
     return True
 
 
 def make_prompt(role:str, content:str, images:list=None):
+    """
+    Creates a prompt in OpenAI format
+    Args:
+        role (str): The role of the prompt
+        content (str): The content of the prompt
+        images (list, optional): A list of images to include in the prompt. Defaults to None.
+    Returns:
+        dict: The prompt in OpenAI format
+    """
     args={
         "role": role,
         "content": content
     }
     if images is not None:
         args["images"] = images
```

### Comparing `llm_axe-1.1.0/llm_axe/models.py` & `llm_axe-1.1.1/llm_axe/models.py`

 * *Files identical despite different names*

### Comparing `llm_axe-1.1.0/llm_axe/system_prompts.yaml` & `llm_axe-1.1.1/llm_axe/system_prompts.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -223,27 +223,45 @@
         {
             "libraries": ["library1", "library2", "library3"]
         }
 
 ObjectDetector:
     prompt: |
         You are a professional object detector. 
-        Make a list of ALL objects found in images and give your reasoning as to where it is.
+        Make a list of ALL objects found in the image and give a brief description of each object which includes its location and features.
         If you are uncertain about the object, then do not include it in the list.
 
-        Example Response:
+        Example Response Format:
             I found these objects in the image:
-            obj1: Its next to the table
-            obj2: Its on the ground
+            Radio: Its next to the table, it is orange and seems damaged.
+            Toy: Its on the ground. Its brown and seems to be made of wood.
+
+        Your response must match that format.
 
 ObjectFilterer:
     prompt: |
-        You are a professional object filterer. 
-        The user will give you objects they are interested in, and you will return ONLY those objects that are also found in the image.
+        You must filter out any objects that do not match the user's interests.
 
         Simplify the object names to one or two words MAX.
+        Your response format is JSON.
+
+        Example Response Format:
+        {
+            "objects": [
+                {
+                "label": "Radio",
+                "location": "Its next to the table",
+                "description": "Its orange"
+                },
+                {
+                "label": "Toy",
+                "location": "Its on the ground",
+                "description": "No information"
+                }
+            ]
+        }
 
-        Example Information:
-        I found these objects:obj1: Its next to the table obj2: Its on the ground. There was no cat though.
+        Response MUST have label, location, and description.
+        Get the description from the user's image information.
 
-        Example Response:
-        {objects: ["obj1", "obj2"]}
+        ONLY KEEP THE SPECIFIC OBJECTS THAT MATCH THE USER'S INTERESTS.
+        If there are no matching objects, then RETURN an EMPTY list.
```

### Comparing `llm_axe-1.1.0/llm_axe.egg-info/PKG-INFO` & `llm_axe-1.1.1/llm_axe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-axe
-Version: 1.1.0
+Version: 1.1.1
 Summary: A toolkit for quickly implementing llm powered functionalities.
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm,ollama
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `llm_axe-1.1.0/setup.py` & `llm_axe-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0' 
+VERSION = '1.1.1' 
 DESCRIPTION = 'A toolkit for quickly implementing llm powered functionalities.'
 LONG_DESCRIPTION = '''
 # llm-axe 🪓
 
 <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/llm-axe"> <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/llm-axe">
 <img alt="Static Badge" src="https://img.shields.io/badge/clones-63/month-purple"> <img alt="GitHub forks" src="https://img.shields.io/github/forks/emirsahin1/llm-axe?style=flat">
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Femirsahin1%2Fllm-axe&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://github.com/emirsahin1/llm-axe)
```

