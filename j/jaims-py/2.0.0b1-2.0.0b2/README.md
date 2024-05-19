# Comparing `tmp/jaims_py-2.0.0b1.tar.gz` & `tmp/jaims_py-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims_py-2.0.0b1.tar", last modified: Fri May 17 18:28:34 2024, max compression
+gzip compressed data, was "jaims_py-2.0.0b2.tar", last modified: Sun May 19 16:15:00 2024, max compression
```

## Comparing `jaims_py-2.0.0b1.tar` & `jaims_py-2.0.0b2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.680957 jaims_py-2.0.0b1/
--rw-r--r--   0 mush       (501) staff       (20)     4404 2024-05-17 18:28:34.680741 jaims_py-2.0.0b1/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     3838 2023-11-28 15:46:12.000000 jaims_py-2.0.0b1/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.676830 jaims_py-2.0.0b1/jaims/
--rw-r--r--   0 mush       (501) staff       (20)      580 2024-05-17 17:45:03.000000 jaims_py-2.0.0b1/jaims/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.677076 jaims_py-2.0.0b1/jaims/adapters/
--rw-r--r--   0 mush       (501) staff       (20)       30 2024-05-09 13:53:36.000000 jaims_py-2.0.0b1/jaims/adapters/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.678005 jaims_py-2.0.0b1/jaims/adapters/google_generative_ai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      112 2024-05-17 14:52:27.000000 jaims_py-2.0.0b1/jaims/adapters/google_generative_ai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)     8620 2024-05-17 18:21:26.000000 jaims_py-2.0.0b1/jaims/adapters/google_generative_ai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)      358 2024-05-17 14:51:57.000000 jaims_py-2.0.0b1/jaims/adapters/google_generative_ai_adapter/constants.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.678604 jaims_py-2.0.0b1/jaims/adapters/openai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      205 2024-05-15 11:49:20.000000 jaims_py-2.0.0b1/jaims/adapters/openai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    29457 2024-05-17 18:02:27.000000 jaims_py-2.0.0b1/jaims/adapters/openai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)     6384 2024-05-16 15:27:47.000000 jaims_py-2.0.0b1/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b1/jaims/default_history_manager.py
--rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b1/jaims/default_tool_manager.py
--rw-r--r--   0 mush       (501) staff       (20)    10024 2024-05-17 18:00:11.000000 jaims_py-2.0.0b1/jaims/entities.py
--rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b1/jaims/interfaces.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.680091 jaims_py-2.0.0b1/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     4404 2024-05-17 18:28:34.000000 jaims_py-2.0.0b1/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      609 2024-05-17 18:28:34.000000 jaims_py-2.0.0b1/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-17 18:28:34.000000 jaims_py-2.0.0b1/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-17 18:28:34.000000 jaims_py-2.0.0b1/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-17 18:28:34.000000 jaims_py-2.0.0b1/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-17 18:28:34.681008 jaims_py-2.0.0b1/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-17 18:26:33.000000 jaims_py-2.0.0b1/setup.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-17 18:28:34.679815 jaims_py-2.0.0b1/tests/
--rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b1/tests/test_agent.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.554247 jaims_py-2.0.0b2/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:15:00.554028 jaims_py-2.0.0b2/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     4692 2024-05-19 16:10:04.000000 jaims_py-2.0.0b2/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.549955 jaims_py-2.0.0b2/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)     1455 2024-05-19 15:19:54.000000 jaims_py-2.0.0b2/jaims/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.550191 jaims_py-2.0.0b2/jaims/adapters/
+-rw-r--r--   0 mush       (501) staff       (20)       74 2024-05-18 20:45:15.000000 jaims_py-2.0.0b2/jaims/adapters/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.551031 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      103 2024-05-19 15:10:17.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     8712 2024-05-19 15:27:59.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1973 2024-05-19 15:09:20.000000 jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/factory.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.551983 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      353 2024-05-19 14:46:29.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    23461 2024-05-19 14:46:37.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1999 2024-05-19 15:02:51.000000 jaims_py-2.0.0b2/jaims/adapters/openai_adapter/factory.py
+-rw-r--r--   0 mush       (501) staff       (20)     7093 2024-05-19 15:42:10.000000 jaims_py-2.0.0b2/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b2/jaims/default_history_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b2/jaims/default_tool_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)    14293 2024-05-19 14:44:55.000000 jaims_py-2.0.0b2/jaims/entities.py
+-rw-r--r--   0 mush       (501) staff       (20)     2308 2024-05-19 15:13:30.000000 jaims_py-2.0.0b2/jaims/factories.py
+-rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b2/jaims/interfaces.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.553552 jaims_py-2.0.0b2/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      710 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-19 16:15:00.000000 jaims_py-2.0.0b2/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-19 16:15:00.554292 jaims_py-2.0.0b2/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-19 16:10:25.000000 jaims_py-2.0.0b2/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:15:00.553265 jaims_py-2.0.0b2/tests/
+-rw-r--r--   0 mush       (501) staff       (20)     5042 2024-05-18 19:41:11.000000 jaims_py-2.0.0b2/tests/test_adapters_exponential_backoff.py
+-rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b2/tests/test_agent.py
```

### Comparing `jaims_py-2.0.0b1/jaims/adapters/google_generative_ai_adapter/adapter.py` & `jaims_py-2.0.0b2/jaims/adapters/google_generative_ai_adapter/adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os
 from ...interfaces import JAImsLLMInterface, JAImsHistoryManager, JAImsToolManager
 from ...entities import (
     JAImsMessage,
     JAImsFunctionTool,
     JAImsToolCall,
     JAImsMessageRole,
-    JAImsContentType,
     JAImsImageContent,
     JAImsStreamingMessage,
+    JAImsOptions,
 )
 from ...agent import JAImsAgent
 from ..shared.image_utilities import image_to_bytes
+from ..shared.exponential_backoff_operation import (
+    call_with_exponential_backoff,
+    ErrorHandlingMethod,
+)
 
 from typing import Iterable, List, Generator, Optional
 from PIL import Image
 
 
 from google.generativeai import GenerativeModel
 from google.generativeai.types import content_types
@@ -22,24 +26,27 @@
 import google.ai.generativelanguage as glm
 
 
 class JAImsGoogleGenerativeAIAdapter(JAImsLLMInterface):
     def __init__(
         self,
         model: str,
-        api_key: Optional[str],
-        generation_config: Optional[generation_types.GenerationConfigType],
-        tool_config: Optional[content_types.ToolConfigType],
+        tool_config: Optional[content_types.ToolConfigType] = None,
+        generation_config: Optional[generation_types.GenerationConfigType] = None,
+        options: Optional[JAImsOptions] = None,
+        api_key: Optional[str] = None,
     ):
         self.api_key = api_key or os.getenv("GOOGLE_API_KEY")
         if not self.api_key:
             raise Exception("GOOGLE_API_KEY not provided.")
+
         self.model = model
         self.generation_config = generation_config
         self.tool_config = tool_config
+        self.options = options or JAImsOptions()
 
     def call(
         self, messages: List[JAImsMessage], tools: List[JAImsFunctionTool]
     ) -> JAImsMessage:
         response = self.__get_gemini_response(messages, tools)
         assert isinstance(response, generation_types.GenerateContentResponse)
         return self.__gemini_to_jaims_message(response)
@@ -159,85 +166,58 @@
                         tool_args=args,
                     )
                 )
 
             if txt := part.text:
                 contents.append(txt)
 
-            # TODO: Add image support
-
         return JAImsMessage(
             role=role,
             contents=contents,
             tool_calls=tool_calls,
             raw=response,
         )
 
     def __get_gemini_response(
         self,
         messages: List[JAImsMessage],
         tools: List[JAImsFunctionTool],
         stream: bool = False,
     ):
 
-        # TODO: Add error and rate limit handling
-
-        system_instruction, gemini_messages = self.__jaims_messages_to_gemini(messages)
-        gemini_tools = self.__jaims_tools_to_gemini(tools) if tools else None
-
-        multimodal_model = GenerativeModel(
-            self.model,
-            generation_config=self.generation_config,
-            tools=gemini_tools,
-            tool_config=self.tool_config,
-            system_instruction=system_instruction or None,
-        )
-
-        response = multimodal_model.generate_content(
-            contents=gemini_messages,
-            stream=stream,
-        )
+        def handle_gemini_error(error):
 
-        return response
+            # From: https://ai.google.dev/gemini-api/docs/troubleshooting
+            # 400	INVALID_ARGUMENT	The request body is malformed.	Check the API reference for request format, examples, and supported versions. Using features from a newer API version with an older endpoint can cause errors.
+            # 403	PERMISSION_DENIED	Your API key doesn't have the required permissions.	Check that your API key is set and has the right access.
+            # 404	NOT_FOUND	The requested resource wasn't found.	Check if all parameters in your request are valid for your API version.
+            # 429	RESOURCE_EXHAUSTED	You've exceeded the rate limit.	Ensure you're within the model's rate limit. Request a quota increase if needed.
+            # 500	INTERNAL	An unexpected error occurred on Google's side.	Wait a bit and retry your request. If the issue persists after retrying, please report it using the Send feedback button in Google AI Studio.
+            # 503	UNAVAILABLE	The service may be temporarily overloaded or down.	Wait a bit and retry your request. If the issue persists after retrying, please report it using the Send feedback button in Google AI Studio.
+
+            if error.code == 429 or error.code == 503 or error.code == 500:
+                return ErrorHandlingMethod.EXPONENTIAL_BACKOFF
+
+            return ErrorHandlingMethod.FAIL
+
+        def call_gemini():
+            system_instruction, gemini_messages = self.__jaims_messages_to_gemini(
+                messages
+            )
+            gemini_tools = self.__jaims_tools_to_gemini(tools) if tools else None
 
+            multimodal_model = GenerativeModel(
+                self.model,
+                generation_config=self.generation_config,
+                tools=gemini_tools,
+                tool_config=self.tool_config,
+                system_instruction=system_instruction or None,
+            )
 
-def create_jaims_gemini(
-    model: str = "gemini-1.5-pro",
-    api_key: Optional[str] = None,
-    generation_config: Optional[generation_types.GenerationConfigType] = None,
-    tool_config: Optional[content_types.ToolConfigType] = None,
-    history_manager: Optional[JAImsHistoryManager] = None,
-    tool_manager: Optional[JAImsToolManager] = None,
-    tools: Optional[List[JAImsFunctionTool]] = None,
-) -> JAImsAgent:
-    """
-    Creates a JAIms instance with a Google Cloud AI adapter.
-
-    Args:
-        project_id (str): The Google Cloud project ID.
-        location (str): The Google Cloud location.
-        model (JAImsGeminiModel): The Gemini model to use. Defaults to JAImsGeminiModel.GEMINI_1_5_PRO.
-        generation_config (Optional[GenerationConfig]): The generation configuration. Defaults to None.
-        tool_config (Optional[ToolConfig]): The tool configuration. Defaults to None.
-        history_manager (Optional[JAImsHistoryManager]): The history manager. Defaults to None.
-        tool_manager (Optional[JAImsToolManager]): The tool manager. Defaults to None.
-        tools (Optional[List[JAImsFunctionTool]]): The list of function tools. Defaults to None.
-
-    Returns:
-        JAImsAgent: The JAIms agent, initialized with the Google Cloud AI adapter.
-    """
-
-    adapter = JAImsGoogleGenerativeAIAdapter(
-        api_key=api_key,
-        model=model,
-        generation_config=generation_config,
-        tool_config=tool_config,
-    )
-
-    agent = JAImsAgent(
-        llm_interface=adapter,
-        history_manager=history_manager,
-        tool_manager=tool_manager,
-        tools=tools,
-    )
+            return multimodal_model.generate_content(
+                contents=gemini_messages,
+                stream=stream,
+            )
 
-    return agent
+        return call_with_exponential_backoff(
+            call_gemini, handle_gemini_error, self.options
+        )
```

### Comparing `jaims_py-2.0.0b1/jaims/adapters/openai_adapter/adapter.py` & `jaims_py-2.0.0b2/jaims/adapters/openai_adapter/adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,57 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from io import BytesIO
 import json
-from enum import Enum
 from math import ceil
-import time
 from typing import Generator, Union
 import openai
 from openai import OpenAI
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import ChoiceDelta, ChoiceDeltaToolCall
 from openai import Stream
 import tiktoken
-import logging
-import random
 from typing import List, Optional, Dict
 from PIL import Image
 
 from ...interfaces import (
     JAImsLLMInterface,
     JAImsHistoryOptimizer,
-    JAImsHistoryManager,
-    JAImsToolManager,
 )
 from ...entities import (
     JAImsImageContent,
     JAImsContentType,
     JAImsMessage,
     JAImsStreamingMessage,
     JAImsToolCall,
     JAImsFunctionTool,
     JAImsMessageRole,
+    JAImsOptions,
 )
-from ...agent import JAImsAgent
 from ..shared.image_utilities import image_to_b64
+from ..shared.exponential_backoff_operation import (
+    call_with_exponential_backoff,
+    ErrorHandlingMethod,
+)
 
 import os
+from copy import deepcopy
 
 # ---------------------
 # openai / LLM modeling
 # ---------------------
 
 
-class JAImsGPTModel(Enum):
-    """
-    The OPENAI Chat GPT models available.
-    """
-
-    GPT_3_5_TURBO = ("gpt-3.5-turbo", 4096)
-    GPT_3_5_TURBO_16K = ("gpt-3.5-turbo-16k", 16384)
-    GPT_3_5_TURBO_0613 = ("gpt-3.5-turbo-0613", 4096)
-    GPT_3_5_TURBO_16K_0613 = ("gpt-3.5-turbo-16k-0613", 16384)
-    GPT_3_5_TURBO_1106 = ("gpt-3.5-turbo-1106", 16385)
-    GPT_4 = ("gpt-4", 8192)
-    GPT_4_32K = ("gpt-4-32k", 32768)
-    GPT_4_0613 = ("gpt-4-0613", 8192)
-    GPT_4_32K_0613 = ("gpt-4-32k-0613", 32768)
-    GPT_4_1106_PREVIEW = ("gpt-4-1106-preview", 128000)
-    GPT_4_VISION_PREVIEW = ("gpt-4-vision-preview", 128000)
-
-    def __init__(self, string, max_tokens):
-        self.string = string
-        self.max_tokens = max_tokens
-
-    def __str__(self):
-        return self.string
-
-
 class JAImsOpenaiKWArgs:
     """
     Represents the keyword arguments for the JAIms OpenAI wrapper.
     This class entirely mirrors the openai API parameters, so refer to it for documentation.
     (https://platform.openai.com/docs/api-reference/chat/create).
 
     Args:
-        model (JAImsGPTModel, optional): The OpenAI model to use. Defaults to JAImsGPTModel.GPT_3_5_TURBO.
+        model (str, optional): The OpenAI model to use. Defaults to gpt-3.5-turbo.
         messages (List[dict], optional): The list of messages for the chat completion. Defaults to an empty list, it is automatically populated by the run method so it is not necessary to pass them. If passed, they will always be appended to the messages passed in the run method.
         max_tokens (int, optional): The maximum number of tokens in the generated response. Defaults to 500.
         stream (bool, optional): Whether to use streaming for the API call. Defaults to False.
         temperature (float, optional): The temperature for generating creative text. Defaults to 0.0.
         top_p (Optional[int], optional): The top-p value for nucleus sampling. Defaults to None.
         n (int, optional): The number of responses to generate. Defaults to 1.
         seed (Optional[int], optional): The seed to be passed to openai to have more consistent outputs. Defaults to None.
@@ -89,15 +62,15 @@
         stop (Union[Optional[str], Optional[List[str]]], optional): The stop condition for the generated response. Defaults to None.
         tool_choice (Union[str, Dict], optional): The choice of tool to use. Defaults to "auto".
         tools (Optional[List[JAImsFunctionToolWrapper]], optional): The list of function tool wrappers to use. Defaults to None.
     """
 
     def __init__(
         self,
-        model: JAImsGPTModel = JAImsGPTModel.GPT_3_5_TURBO,
+        model: str = "gpt-3.5-turbo",
         messages: List[dict] = [],
         max_tokens: int = 1024,
         stream: bool = False,
         temperature: float = 0.0,
         top_p: Optional[int] = None,
         n: int = 1,
         seed: Optional[int] = None,
@@ -123,15 +96,15 @@
         self.response_format = response_format
         self.stop = stop
         self.tool_choice = tool_choice
         self.tools = tools
 
     def to_dict(self):
         kwargs = {
-            "model": self.model.string,
+            "model": self.model,
             "temperature": self.temperature,
             "n": self.n,
             "stream": self.stream,
             "messages": self.messages,
             "top_p": self.top_p,
             "max_tokens": self.max_tokens,
             "seed": self.seed,
@@ -148,17 +121,37 @@
 
         if self.tools:
             kwargs["tools"] = self.tools
             kwargs["tool_choice"] = self.tool_choice
 
         return kwargs
 
+    @staticmethod
+    def from_dict(kwargs: dict) -> JAImsOpenaiKWArgs:
+        return JAImsOpenaiKWArgs(
+            model=kwargs.get("model", "gpt-3.5-turbo"),
+            messages=kwargs.get("messages", []),
+            max_tokens=kwargs.get("max_tokens", 1024),
+            stream=kwargs.get("stream", False),
+            temperature=kwargs.get("temperature", 0.0),
+            top_p=kwargs.get("top_p", None),
+            n=kwargs.get("n", 1),
+            seed=kwargs.get("seed", None),
+            frequency_penalty=kwargs.get("frequency_penalty", 0.0),
+            presence_penalty=kwargs.get("presence_penalty", 0.0),
+            logit_bias=kwargs.get("logit_bias", None),
+            response_format=kwargs.get("response_format", None),
+            stop=kwargs.get("stop", None),
+            tool_choice=kwargs.get("tool_choice", "auto"),
+            tools=kwargs.get("tools", None),
+        )
+
     def copy_with_overrides(
         self,
-        model: Optional[JAImsGPTModel] = None,
+        model: Optional[str] = None,
         messages: Optional[List[dict]] = None,
         max_tokens: Optional[int] = None,
         stream: Optional[bool] = None,
         temperature: Optional[float] = None,
         top_p: Optional[int] = None,
         n: Optional[int] = None,
         seed: Optional[int] = None,
@@ -194,96 +187,22 @@
             ),
             stop=stop if stop else self.stop,
             tool_choice=tool_choice if tool_choice else self.tool_choice,
             tools=tools if tools else self.tools,
         )
 
 
-class JAImsOptions:
-    """
-    Represents the options for Openai Adapter.
-
-    Args:
-        max_retries (int): The maximum number of retries after a failing openai call.
-        retry_delay (int): The delay between each retry.
-        exponential_base (int): The base for exponential backoff calculation.
-        exponential_delay (int): The initial delay for exponential backoff.
-        exponential_cap (Optional[int]): The maximum delay for exponential backoff.
-        jitter (bool): Whether to add jitter to the delay (to avoid concurrent firing).
-        debug_stream_function_call (bool): Prints the arguments streamed by OpenAI during function call when streaming enabled.
-    """
-
-    def __init__(
-        self,
-        max_retries=15,
-        retry_delay=10,
-        exponential_base: int = 2,
-        exponential_delay: int = 1,
-        exponential_cap: Optional[int] = None,
-        jitter: bool = True,
-        debug_stream_function_call=False,
-    ):
-        self.max_retries = max_retries
-        self.retry_delay = retry_delay
-        self.exponential_base = exponential_base
-        self.exponential_delay = exponential_delay
-        self.exponential_cap = exponential_cap
-        self.jitter = jitter
-        self.debug_stream_function_call = debug_stream_function_call
-
-    def copy_with_overrides(
-        self,
-        max_retries: Optional[int] = None,
-        retry_delay: Optional[int] = None,
-        exponential_base: Optional[int] = None,
-        exponential_delay: Optional[int] = None,
-        exponential_cap: Optional[int] = None,
-        jitter: Optional[bool] = None,
-        debug_stream_function_call: Optional[bool] = None,
-    ) -> JAImsOptions:
-        """
-        Returns a new JAImsOptions instance with the passed kwargs overridden.
-        """
-        return JAImsOptions(
-            max_retries=max_retries if max_retries else self.max_retries,
-            retry_delay=retry_delay if retry_delay else self.retry_delay,
-            exponential_base=(
-                exponential_base if exponential_base else self.exponential_base
-            ),
-            exponential_delay=(
-                exponential_delay if exponential_delay else self.exponential_delay
-            ),
-            exponential_cap=(
-                exponential_cap if exponential_cap else self.exponential_cap
-            ),
-            jitter=jitter if jitter else self.jitter,
-            debug_stream_function_call=(
-                debug_stream_function_call
-                if debug_stream_function_call
-                else self.debug_stream_function_call
-            ),
-        )
-
-
-class ErrorHandlingMethod(Enum):
-    FAIL = "fail"
-    RETRY = "retry"
-    EXPONENTIAL_BACKOFF = "exponential_backoff"
-
-
 class JAImsTokenHistoryOptimizer(JAImsHistoryOptimizer):
     def __init__(
         self,
         options: JAImsOptions,
-        openai_kwargs: JAImsOpenaiKWArgs,
         history_max_tokens: int,
-        model: JAImsGPTModel,
+        model: str,
     ):
         self.options = options
-        self.openai_kwargs = openai_kwargs
         self.history_max_tokens = history_max_tokens
         self.model = model
 
     def optimize_history(self, messages: List[JAImsMessage]) -> List:
 
         # Copying the whole history to avoid altering the original one
         buffer = messages.copy()
@@ -299,18 +218,18 @@
             # Popping the first (oldest) message from the chat history between the user and agent
             buffer.pop(0)
             # Recalculating the tokens for the compound history
             messages_tokens = self.__tokens_from_messages(buffer, self.model)
 
         return buffer
 
-    def __estimate_token_count(self, string: str, model: JAImsGPTModel) -> int:
+    def __estimate_token_count(self, string: str, model: str) -> int:
         """Returns the number of tokens in a text string."""
 
-        encoding = tiktoken.encoding_for_model(model.string)
+        encoding = tiktoken.encoding_for_model(model)
         num_tokens = len(encoding.encode(string))
         return num_tokens
 
     def __estimate_image_tokens_count(self, width: int, height: int):
         h = ceil(height / 512)
         w = ceil(width / 512)
         n = w * h
@@ -363,70 +282,78 @@
     The JAIms OpenAI adapter.
     """
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         options: Optional[JAImsOptions] = None,
-        kwargs: Optional[JAImsOpenaiKWArgs] = None,
+        kwargs: Optional[Union[JAImsOpenaiKWArgs, Dict]] = None,
         transaction_storage: Optional[OpenAITransactionStorageInterface] = None,
     ):
         self.api_key = api_key or os.getenv("OPENAI_API_KEY")
         if not self.api_key:
             raise Exception("OpenAI API key not provided.")
 
         self.options = options or JAImsOptions()
         self.kwargs = kwargs or JAImsOpenaiKWArgs()
         self.transaction_storage = transaction_storage
 
+    def __get_args(
+        self,
+        messages: List[JAImsMessage],
+        tools: List[JAImsFunctionTool],
+        stream: bool = False,
+    ):
+        openai_messages = self.__jaims_messages_to_openai(messages)
+        openai_tools = self.__jaims_tools_to_openai(tools)
+
+        if isinstance(self.kwargs, JAImsOpenaiKWArgs):
+            args = self.kwargs.to_dict()
+        else:
+            args = deepcopy(self.kwargs)
+
+        args["messages"] = openai_messages
+        args["tools"] = openai_tools
+        args["stream"] = stream
+
+        return args
+
     def call(
         self, messages: List[JAImsMessage], tools: List[JAImsFunctionTool]
     ) -> JAImsMessage:
-        openai_messages = self.__jaims_messages_to_openai(messages)
-        openai_tools = self.__jaims_tools_to_openai(tools)
-        openai_kw_args = self.kwargs.copy_with_overrides(
-            messages=openai_messages,
-            tools=openai_tools,
-            stream=False,
-        )
-        response = self.___get_openai_response(openai_kw_args, self.options)
+        args = self.__get_args(messages, tools)
+        response = self.___get_openai_response(args, self.options)
         assert isinstance(response, ChatCompletion)
         if self.transaction_storage:
             self.transaction_storage.store_transaction(
-                request=openai_kw_args.to_dict(),
+                request=args,
                 response=response.model_dump(exclude_none=True),
             )
 
         return self.__openai_chat_completion_to_jaims_message(response)
 
     def call_streaming(
         self, messages: List[JAImsMessage], tools: List[JAImsFunctionTool]
     ) -> Generator[JAImsStreamingMessage, None, None]:
-        openai_messages = self.__jaims_messages_to_openai(messages)
-        openai_tools = self.__jaims_tools_to_openai(tools)
-        openai_kw_args = self.kwargs.copy_with_overrides(
-            messages=openai_messages,
-            tools=openai_tools,
-            stream=True,
-        )
-        response = self.___get_openai_response(openai_kw_args, self.options)
+        args = self.__get_args(messages, tools, stream=True)
+        response = self.___get_openai_response(args, self.options)
         assert isinstance(response, Stream)
 
         accumulated_delta = None
         for completion_chunk in response:
             accumulated_delta = self.__accumulate_choice_delta(
                 accumulated_delta, completion_chunk.choices[0].delta
             )
             yield self.__openai_chat_completion_choice_delta_to_jaims_message(
                 accumulated_delta, completion_chunk
             )
 
         if self.transaction_storage and accumulated_delta:
             self.transaction_storage.store_transaction(
-                request=openai_kw_args.to_dict(),
+                request=args,
                 response=accumulated_delta.model_dump(exclude_none=True),
             )
 
     def __jaims_messages_to_openai(self, messages: List[JAImsMessage]) -> List[dict]:
 
         def format_contents(contents: List[JAImsContentType]):
             if len(contents) == 1 and isinstance(contents[0], str):
@@ -583,80 +510,49 @@
                 contents=contents,
                 tool_calls=function_tool_calls,
                 raw=accumulated_choice_delta,
             ),
             textDelta=textDelta,
         )
 
-    def __handle_openai_error(self, error: openai.OpenAIError) -> ErrorHandlingMethod:
-        # errors are handled according to the guidelines here: https://platform.openai.com/docs/guides/error-codes/api-errors (dated 03/10/2023)
-        # this map indexes all the error that require a retry or an exponential backoff, every other error is a fail
-        error_handling_map = {
-            openai.RateLimitError: ErrorHandlingMethod.EXPONENTIAL_BACKOFF,
-            openai.InternalServerError: ErrorHandlingMethod.RETRY,
-            openai.APITimeoutError: ErrorHandlingMethod.RETRY,
-        }
-
-        for error_type, error_handling_method in error_handling_map.items():
-            if isinstance(error, error_type):
-                return error_handling_method
-
-        return ErrorHandlingMethod.FAIL
-
     def ___get_openai_response(
         self,
-        openai_kw_args: JAImsOpenaiKWArgs,
+        openai_kw_args: dict,
         call_options: JAImsOptions,
     ) -> Union[ChatCompletion, Stream[ChatCompletionChunk]]:
-        retries = 0
-        logger = logging.getLogger(__name__)
-        # keeps how long to sleep between retries
-        sleep_time = call_options.retry_delay
-        # keeps track of the exponential backoff
-        backoff_time = call_options.exponential_delay
-
-        while retries < call_options.max_retries:
-            try:
-                client = OpenAI(api_key=self.api_key)
-                kwargs = openai_kw_args.to_dict()
-                response = client.chat.completions.create(
-                    **kwargs,
-                )
 
-                return response
-            except openai.OpenAIError as error:
-                logger.error(f"OpenAI API error:\n{error}\n")
-                error_handling_method = self.__handle_openai_error(error)
-
-                if error_handling_method == ErrorHandlingMethod.FAIL:
-                    raise Exception(f"OpenAI API error: {error}")
-
-                if error_handling_method == ErrorHandlingMethod.RETRY:
-                    sleep_time = call_options.retry_delay
-
-                elif error_handling_method == ErrorHandlingMethod.EXPONENTIAL_BACKOFF:
-                    logger.info(f"Performing exponential backoff")
-                    jitter = 1 + call_options.jitter * random.random()
-                    backoff_time = backoff_time * call_options.exponential_base * jitter
-
-                    if (
-                        call_options.exponential_cap is not None
-                        and backoff_time > call_options.exponential_cap
-                    ):
-                        backoff_time = call_options.exponential_cap * jitter
-
-                    sleep_time = backoff_time
-
-                logger.warning(f"Retrying in {sleep_time} seconds")
-                time.sleep(sleep_time)
-                retries += 1
-
-        max_retries_error = f"Max retries exceeded! OpenAI API call failed {call_options.max_retries} times."
-        logger.error(max_retries_error)
-        raise Exception(max_retries_error)
+        def handle_openai_error(error) -> ErrorHandlingMethod:
+            # errors are handled according to the guidelines here: https://platform.openai.com/docs/guides/error-codes/api-errors (dated 03/10/2023)
+            # this map indexes all the error that require a retry or an exponential backoff, every other error is a fail
+            error_handling_map = {
+                openai.RateLimitError: ErrorHandlingMethod.EXPONENTIAL_BACKOFF,
+                openai.InternalServerError: ErrorHandlingMethod.RETRY,
+                openai.APITimeoutError: ErrorHandlingMethod.RETRY,
+            }
+
+            for error_type, error_handling_method in error_handling_map.items():
+                if isinstance(error, error_type):
+                    return error_handling_method
+
+            return ErrorHandlingMethod.FAIL
+
+        def openai_api_call():
+            client = OpenAI(api_key=self.api_key)
+            kwargs = openai_kw_args
+            response = client.chat.completions.create(
+                **kwargs,
+            )
+
+            return response
+
+        return call_with_exponential_backoff(
+            openai_api_call,
+            handle_openai_error,
+            call_options,
+        )
 
     def __merge_tool_calls(
         self,
         existing_tool_calls: Optional[List[ChoiceDeltaToolCall]],
         new_tool_calls_delta: List[ChoiceDeltaToolCall],
     ):
         if not existing_tool_calls:
@@ -720,48 +616,7 @@
             accumulator.role = new_delta.role
         if new_delta.tool_calls:
             accumulator.tool_calls = self.__merge_tool_calls(
                 accumulator.tool_calls, new_delta.tool_calls
             )
 
         return accumulator
-
-
-def create_jaims_openai(
-    api_key: Optional[str] = None,
-    options: Optional[JAImsOptions] = None,
-    kwargs: Optional[JAImsOpenaiKWArgs] = None,
-    transaction_storage: Optional[OpenAITransactionStorageInterface] = None,
-    history_manager: Optional[JAImsHistoryManager] = None,
-    tool_manager: Optional[JAImsToolManager] = None,
-    tools: Optional[List[JAImsFunctionTool]] = None,
-) -> JAImsAgent:
-    """
-    Creates a JAIms instance with an OpenAI adapter.
-
-    Args:
-        api_key (Optional[str], optional): The OpenAI API key. Defaults to None.
-        options (Optional[JAImsOptions], optional): The options for the adapter. Defaults to None.
-        kwargs (Optional[JAImsOpenaiKWArgs], optional): The keyword arguments for the adapter. Defaults to None.
-        transaction_storage (Optional[JAImsTransactionStorageInterface], optional): The transaction storage interface. Defaults to None.
-        history_manager (Optional[JAImsHistoryManager], optional): The history manager. Defaults to None.
-        tool_manager (Optional[JAImsToolManager], optional): The tool manager. Defaults to None.
-        tools (Optional[List[JAImsFunctionTool]], optional): The list of function tools. Defaults to None.
-
-    Returns:
-        JAImsAgent: The JAIms agent, initialized with the OpenAI adapter.
-    """
-    adapter = JAImsOpenaiAdapter(
-        api_key=api_key,
-        options=options,
-        kwargs=kwargs,
-        transaction_storage=transaction_storage,
-    )
-
-    agent = JAImsAgent(
-        llm_interface=adapter,
-        history_manager=history_manager,
-        tool_manager=tool_manager,
-        tools=tools,
-    )
-
-    return agent
```

### Comparing `jaims_py-2.0.0b1/jaims/agent.py` & `jaims_py-2.0.0b2/jaims/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 if TYPE_CHECKING:
     from .interfaces import JAImsLLMInterface, JAImsHistoryManager, JAImsToolManager
 
+from .factories import openai_factory, google_factory
+
 from typing import Generator, List, Optional
 
 
 from jaims.default_tool_manager import JAImsDefaultToolManager
 
 
 from jaims.entities import (
     JAImsMaxConsecutiveFunctionCallsExceeded,
     JAImsMessage,
     JAImsFunctionTool,
+    JAImsLLMConfig,
+    JAImsOptions,
 )
 
-# TODO: Refactor all docstrings
-# TODO: Refactor logging entirely
-# TODO: Adjust imports in __init__.py files making them more explicit
-# TODO: Adjust transaction storage for openai streaming response
-# TODO: Add original response to jaims message and return it instead of strings
-# TODO: Decide return type of runs, might not be ideal to return a string
+
+# TODOS:
+# High Priority
+# TODO: Refactor all docstrings and docs, check imports and remove unused imports
+
+# Mid Priority
 # TODO: Implement a method to pass a function directly instead of the jaims descriptors
-# TODO: Add images support
+# TODO: Implement Tests
 
-# TODO: Test Stuff:
-# - Agent:
-#  - with and without history
-#  - with and without tools
-#  - use mocks for the interfaces
-# - History Managers []
-# - Tool Manager []
-#
+# Low Priority
+# TODO: Add support for multiple completion responses
+# TODO: Adjust transaction storage for openai streaming response
+# TODO: Refactor logging entirely
 
 
 class JAImsAgent:
     """
     Base  JAIms Agent class, interacts with the JAImsLLMInterface to run messages and tools.
 
     Args:
@@ -60,33 +60,54 @@
         self.llm_interface = llm_interface
         self.tool_manager = tool_manager or JAImsDefaultToolManager()
         self.tools = tools or []
         self.history_manager = history_manager
         self.__session_iteration = -1
         self.__session_messages = []
 
-    def __get_messages_for_run(
-        self, messages: Optional[List[JAImsMessage]]
-    ) -> List[JAImsMessage]:
-        """
-        Processes a list of messages for the agent run and, if necessary, adds them to history.
-
-        Args:
-            messages (Optional[List[JAImsMessage]]): The list of messages. Defaults to None.
-
-        Returns:
-            List[JAImsMessage]: The session messages.
-        """
-        session_messages = messages or []
-
-        if self.history_manager:
-            self.history_manager.add_messages(session_messages)
-            session_messages = self.history_manager.get_messages()
+    @staticmethod
+    def build(
+        model: str,
+        provider: Literal["openai", "google"],
+        api_key: Optional[str] = None,
+        options: Optional[JAImsOptions] = None,
+        config: Optional[JAImsLLMConfig] = None,
+        history_manager: Optional[JAImsHistoryManager] = None,
+        tool_manager: Optional[JAImsToolManager] = None,
+        tools: Optional[List[JAImsFunctionTool]] = None,
+    ) -> JAImsAgent:
 
-        return session_messages
+        # assert provider in ["openai", "google"], "Provider must be either 'openai' or 'google'"
+        assert provider in [
+            "openai",
+            "google",
+        ], f"curretnly supported providers are: [openai, google] . If you're targeting an unsupported provider you should supply your own adapter instead."
+
+        if provider == "openai":
+            return openai_factory(
+                model=model,
+                api_key=api_key,
+                options=options,
+                config=config,
+                history_manager=history_manager,
+                tool_manager=tool_manager,
+                tools=tools,
+            )
+        elif provider == "google":
+            return google_factory(
+                model=model,
+                api_key=api_key,
+                options=options,
+                config=config,
+                history_manager=history_manager,
+                tool_manager=tool_manager,
+                tools=tools,
+            )
+        else:
+            raise ValueError("Provider is not supported.")
 
     def __update_session(
         self, session_messages: List[JAImsMessage], max_iterations: int
     ):
         self.__session_iteration += 1
         if self.__session_iteration > max_iterations:
             raise JAImsMaxConsecutiveFunctionCallsExceeded(self.__session_iteration)
```

### Comparing `jaims_py-2.0.0b1/jaims/default_history_manager.py` & `jaims_py-2.0.0b2/jaims/default_history_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b1/jaims/default_tool_manager.py` & `jaims_py-2.0.0b2/jaims/default_tool_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b1/jaims/entities.py` & `jaims_py-2.0.0b2/jaims/entities.py`

 * *Files 17% similar despite different names*

```diff
@@ -305,14 +305,113 @@
             params : dict
                 the parameters passed to the wrapped function
         """
 
         return self.function(**params) if params and self.function else None
 
 
+class JAImsModelCode:
+    """
+    Constants for the LLM names.
+    """
+
+    GEMINI_1_PRO = "gemini-1.0-pro"
+    GEMINI_1_PRO_LATEST = "gemini-1.0-pro-latest"
+    GEMINI_1_PRO_001 = "gemini-1.0-pro-001"
+    GEMINI_1_PRO_VISION = "gemini-1.0-pro-vision"
+    GEMINI_1_PRO_VISION_LATEST = "gemini-1.0-pro-vision-latest"
+    GEMINI_1_5_FLASH_LATEST = "gemini-1.5-flash-latest"
+    GEMINI_1_5_PRO = "gemini-1.5-pro"
+    GEMINI_1_5_PRO_LATEST = "gemini-1.5-pro-latest"
+    GPT_3_5_TURBO = "gpt-3.5-turbo"
+    GPT_4 = "gpt-4"
+    GPT_4_32K = "gpt-4-32k"
+    GPT_4_0613 = "gpt-4-0613"
+    GPT_4_32K_0613 = "gpt-4-32k-0613"
+    GPT_4_TURBO = "gpt-4-turbo"
+    GPT_4_TURBO_2024_04_09 = "gpt-4-turbo-2024-04-09"
+    GPT_4_TURBO_PREVIEW = "gpt-4-turbo-preview"
+    GPT_4_0125_PREVIEW = "gpt-4-0125-preview"
+    GPT_4_1106_PREVIEW = "gpt-4-1106-preview"
+    GPT_4_VISION_PREVIEW = "gpt-4-vision-preview"
+    GPT_4_1106_VISION_PREVIEW = "gpt-4-1106-vision-preview"
+    GPT_4o = "gpt-4o"
+    GPT_4o_2024_05_13 = "gpt-4o-2024-05-13"
+
+
+class JAImsLLMConfig:
+    def __init__(
+        self,
+        temperature: float = 0.5,
+        max_tokens: int = 1024,
+        response_format: Optional[Dict[str, Any]] = None,
+    ):
+        self.temperature = temperature
+        self.max_tokens = max_tokens
+        self.response_format = response_format
+
+
+class JAImsOptions:
+    """
+    Config options for the JAImsAgent when calling the remote LLM.
+    Exponential backoff is calculated using the formula: min(delay * exponential_base, exponential_cap) * (1 + jitter * random())
+
+    Args:
+        max_retries (int): The maximum number of retries after a failing a call.
+        retry_delay (int): The delay between each retry in case of failure without exponential backoff.
+        exponential_base (int): The base for exponential backoff calculation.
+        exponential_delay (int): The initial delay, in seconds, to multiply by the base for exponential backoff.
+        exponential_cap (Optional[int]): The maximum value, in seconds, for exponential backoff delay. Leave None to let it grow indefinitely.
+        jitter (bool): Whether to add a small jitter to the delay (to avoid concurrent firing), in case of exponential backoff, in the worst case, it will be 2x the delay.
+    """
+
+    def __init__(
+        self,
+        max_retries=15,
+        retry_delay=10,
+        exponential_base: int = 2,
+        exponential_delay: int = 1,
+        exponential_cap: Optional[int] = None,
+        jitter: bool = True,
+    ):
+        self.max_retries = max_retries
+        self.retry_delay = retry_delay
+        self.exponential_base = exponential_base
+        self.exponential_delay = exponential_delay
+        self.exponential_cap = exponential_cap
+        self.jitter = jitter
+
+    def copy_with_overrides(
+        self,
+        max_retries: Optional[int] = None,
+        retry_delay: Optional[int] = None,
+        exponential_base: Optional[int] = None,
+        exponential_delay: Optional[int] = None,
+        exponential_cap: Optional[int] = None,
+        jitter: Optional[bool] = None,
+    ) -> JAImsOptions:
+        """
+        Returns a new JAImsOptions instance with the passed parameters overridden.
+        """
+        return JAImsOptions(
+            max_retries=max_retries if max_retries else self.max_retries,
+            retry_delay=retry_delay if retry_delay else self.retry_delay,
+            exponential_base=(
+                exponential_base if exponential_base else self.exponential_base
+            ),
+            exponential_delay=(
+                exponential_delay if exponential_delay else self.exponential_delay
+            ),
+            exponential_cap=(
+                exponential_cap if exponential_cap else self.exponential_cap
+            ),
+            jitter=jitter if jitter else self.jitter,
+        )
+
+
 # ----------
 # exceptions
 # ----------
 
 
 class JAImsMaxConsecutiveFunctionCallsExceeded(Exception):
     """
@@ -334,7 +433,22 @@
     Attributes:
         func_name -- name of the unexpected function
     """
 
     def __init__(self, func_name):
         message = f"Unexpected function call: {func_name}"
         super().__init__(message)
+
+
+class JAImsMaxRetriesExceeded(Exception):
+    """
+    Exception raised when the maximum number of retries is performed by an adapter client.
+
+    Attributes:
+        max_consecutive_calls -- maximum number of consecutive calls allowed
+    """
+
+    def __init__(self, max_retries, last_exception=None):
+        message = (
+            f"Max retries exceeded: {max_retries}, last exception: {last_exception}"
+        )
+        super().__init__(message)
```

### Comparing `jaims_py-2.0.0b1/jaims/interfaces.py` & `jaims_py-2.0.0b2/jaims/interfaces.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b1/jaims_py.egg-info/SOURCES.txt` & `jaims_py-2.0.0b2/jaims_py.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 README.md
 setup.py
 jaims/__init__.py
 jaims/agent.py
 jaims/default_history_manager.py
 jaims/default_tool_manager.py
 jaims/entities.py
+jaims/factories.py
 jaims/interfaces.py
 jaims/adapters/__init__.py
 jaims/adapters/google_generative_ai_adapter/__init__.py
 jaims/adapters/google_generative_ai_adapter/adapter.py
-jaims/adapters/google_generative_ai_adapter/constants.py
+jaims/adapters/google_generative_ai_adapter/factory.py
 jaims/adapters/openai_adapter/__init__.py
 jaims/adapters/openai_adapter/adapter.py
+jaims/adapters/openai_adapter/factory.py
 jaims_py.egg-info/PKG-INFO
 jaims_py.egg-info/SOURCES.txt
 jaims_py.egg-info/dependency_links.txt
 jaims_py.egg-info/requires.txt
 jaims_py.egg-info/top_level.txt
+tests/test_adapters_exponential_backoff.py
 tests/test_agent.py
```

### Comparing `jaims_py-2.0.0b1/setup.py` & `jaims_py-2.0.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Read Google Cloud AI specific requirements
 with open("requirements-googleai.txt") as f:
     requirements_google_ai = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="2.0.0-beta.1",
+    version="2.0.0-beta.2",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

### Comparing `jaims_py-2.0.0b1/tests/test_agent.py` & `jaims_py-2.0.0b2/tests/test_agent.py`

 * *Files identical despite different names*

