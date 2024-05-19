# Comparing `tmp/mlv-1.3.6.tar.gz` & `tmp/mlv-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlv-1.3.6.tar", last modified: Fri May 17 13:28:22 2024, max compression
+gzip compressed data, was "mlv-1.3.7.tar", last modified: Sun May 19 03:43:44 2024, max compression
```

## Comparing `mlv-1.3.6.tar` & `mlv-1.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 13:28:22.576980 mlv-1.3.6/
--rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.6/MANIFEST.in
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 13:28:22.576746 mlv-1.3.6/PKG-INFO
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 13:28:22.574156 mlv-1.3.6/mlv/
--rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.6/mlv/__init__.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.6/mlv/base_model.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     9318 2024-05-17 13:20:37.000000 mlv-1.3.6/mlv/drawing.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     6255 2024-03-11 02:34:04.000000 mlv-1.3.6/mlv/http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.6/mlv/mps_workaround.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.6/mlv/old_http.py
--rw-r--r--   0 xiaotan    (501) staff       (20)    16126 2024-04-03 16:19:29.000000 mlv-1.3.6/mlv/old_stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.6/mlv/ollama.py
--rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.6/mlv/rpc.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.6/mlv/segment_anything.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.6/mlv/stable_diffusion.py
--rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.6/mlv/util.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 13:28:22.576453 mlv-1.3.6/mlv.egg-info/
--rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-17 13:28:22.000000 mlv-1.3.6/mlv.egg-info/PKG-INFO
--rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-17 13:28:22.000000 mlv-1.3.6/mlv.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-17 13:28:22.000000 mlv-1.3.6/mlv.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-17 13:28:22.000000 mlv-1.3.6/mlv.egg-info/requires.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-17 13:28:22.000000 mlv-1.3.6/mlv.egg-info/top_level.txt
--rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.6/pyproject.toml
--rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-17 13:28:22.577151 mlv-1.3.6/setup.cfg
--rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-17 13:28:04.000000 mlv-1.3.6/setup.py
-drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-17 13:28:22.575709 mlv-1.3.6/tests/
--rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.6/tests/test_hello.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.545136 mlv-1.3.7/
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-01-19 07:04:28.000000 mlv-1.3.7/MANIFEST.in
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-19 03:43:44.544939 mlv-1.3.7/PKG-INFO
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.543856 mlv-1.3.7/mlv/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       40 2024-05-17 07:04:00.000000 mlv-1.3.7/mlv/__init__.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      172 2024-01-24 03:53:24.000000 mlv-1.3.7/mlv/base_model.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     9958 2024-05-19 03:27:27.000000 mlv-1.3.7/mlv/drawing.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)        0 2024-05-19 01:55:07.000000 mlv-1.3.7/mlv/http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     7392 2024-05-17 06:57:36.000000 mlv-1.3.7/mlv/mps_workaround.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     4485 2024-01-24 08:00:40.000000 mlv-1.3.7/mlv/old_http.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)    16708 2024-05-19 01:53:13.000000 mlv-1.3.7/mlv/old_stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3553 2024-01-21 09:16:52.000000 mlv-1.3.7/mlv/ollama.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)      926 2024-01-28 05:59:55.000000 mlv-1.3.7/mlv/rpc.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3050 2024-01-20 05:15:14.000000 mlv-1.3.7/mlv/segment_anything.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     3166 2024-01-22 18:45:49.000000 mlv-1.3.7/mlv/stable_diffusion.py
+-rw-r--r--   0 xiaotan    (501) staff       (20)     5304 2024-05-17 07:03:15.000000 mlv-1.3.7/mlv/util.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.544731 mlv-1.3.7/mlv.egg-info/
+-rw-r--r--   0 xiaotan    (501) staff       (20)      319 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotan    (501) staff       (20)      401 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        1 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)      128 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/requires.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)        4 2024-05-19 03:43:44.000000 mlv-1.3.7/mlv.egg-info/top_level.txt
+-rw-r--r--   0 xiaotan    (501) staff       (20)       51 2024-01-19 06:35:51.000000 mlv-1.3.7/pyproject.toml
+-rw-r--r--   0 xiaotan    (501) staff       (20)       38 2024-05-19 03:43:44.545178 mlv-1.3.7/setup.cfg
+-rw-r--r--   0 xiaotan    (501) staff       (20)      400 2024-05-19 03:42:24.000000 mlv-1.3.7/setup.py
+drwxr-xr-x   0 xiaotan    (501) staff       (20)        0 2024-05-19 03:43:44.544575 mlv-1.3.7/tests/
+-rw-r--r--   0 xiaotan    (501) staff       (20)       36 2024-01-19 05:12:11.000000 mlv-1.3.7/tests/test_hello.py
```

### Comparing `mlv-1.3.6/mlv/drawing.py` & `mlv-1.3.7/mlv/drawing.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,17 +106,28 @@
     )
 
     device = get_device()
     pipe.to(device=device)
 
     pipe.scheduler = LCMScheduler.from_config(pipe.scheduler.config)
     pipe.load_lora_weights(
-        os.path.join(cache_path, "lora", "pytorch_lora_weights.safetensors")
+        os.path.join(cache_path, "lora", "pytorch_lora_weights.safetensors"),
+        adapter_name="lcm",
     )
     pipe.fuse_lora()
+    if len(lora_weights):
+        for i in range(len(lora_weights)):
+            pipe.load_lora_weights(
+                os.path.join(cache_path, "lora", lora_weights[i]),
+                adapter_name="lora2",
+            )
+            pipe.fuse_lora()
+            print("load lora", lora_weights[i])
+    pipe.set_adapters(["lcm", "lora2"], adapter_weights=[1.0, 1.0])
+    pipe.fuse_lora()
 
     generator = torch.Generator()
 
     def infer(
         prompt,
         image,
         num_inference_steps=3,
@@ -187,23 +198,28 @@
         original_config_file=os.path.join(cache_path, "v1-inference.yaml"),
     )
 
     device = get_device()
     txt2img_pipe.to(device=device)
     txt2img_pipe.scheduler = LCMScheduler.from_config(txt2img_pipe.scheduler.config)
     txt2img_pipe.load_lora_weights(
-        os.path.join(cache_path, "lora", "pytorch_lora_weights.safetensors")
+        os.path.join(cache_path, "lora", "pytorch_lora_weights.safetensors"),
+        adapter_name="lcm",
     )
     txt2img_pipe.fuse_lora()
     if len(lora_weights):
         for i in range(len(lora_weights)):
             txt2img_pipe.load_lora_weights(
-                os.path.join(cache_path, "lora", lora_weights[i])
+                os.path.join(cache_path, "lora", lora_weights[i]),
+                adapter_name="lora2",
             )
             txt2img_pipe.fuse_lora()
+            print("load lora", lora_weights[i])
+    txt2img_pipe.set_adapters(["lcm", "lora2"], adapter_weights=[1.0, 1.0])
+    txt2img_pipe.fuse_lora()
     generator = torch.Generator()
 
     img2img_pipe = StableDiffusionImg2ImgPipeline(**txt2img_pipe.components)
 
     def infer(
         prompt,
         image,
```

### Comparing `mlv-1.3.6/mlv/mps_workaround.py` & `mlv-1.3.7/mlv/mps_workaround.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/old_http.py` & `mlv-1.3.7/mlv/old_http.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/old_stable_diffusion.py` & `mlv-1.3.7/mlv/old_stable_diffusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,33 @@
 import os
 import random
 from os import path
 from contextlib import nullcontext
 from sys import platform
 import torch
 from PIL import Image, ImageOps
-from .util import timer
-from .setting import cache_path
+import time
+
+
+class timer:
+    def __init__(self, method_name="timed process"):
+        self.method = method_name
+
+    def __enter__(self):
+        self.start = time.time()
+        print(f"{self.method} starts")
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        end = time.time()
+        print(f"{self.method} took {str(round(end - self.start, 2))}s")
+
+
+# from .setting import cache_path
+
+cache_path = os.getenv("APP_MODEL_PATH", "")
 
 
 is_mac = platform == "darwin"
 
 
 def get_device():
     return (
@@ -475,18 +492,25 @@
                     else:
                         raise ValueError("mode not support")
 
     return infer
 
 
 def load_models_backend(
-    model_id="dreamshaper_8",
+    model_id="DreamShaper8",
     technique="safetensors",
     safety_checker=True,
-    lora_weights=[],
+    lora_weights=["HashimotoKanna"],
 ):
     if technique == "sd1.5_adapter":
         return load_sd_adapter(model_id, safety_checker, lora_weights)
     elif technique == "ssd_1b_t2i":
         return load_ssd1b(safety_checker)
     elif technique == "safetensors":
         return load_single_file(model_id, safety_checker, lora_weights)
+
+
+infer = load_models_backend()
+infer(
+    "<lora:HashimotoKanna.safetensors:0.9> HashimotoKanna, 1girl,portrait,closed mouth,otonokizaka school uniform realistic",
+    "test",
+)
```

### Comparing `mlv-1.3.6/mlv/ollama.py` & `mlv-1.3.7/mlv/ollama.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/rpc.py` & `mlv-1.3.7/mlv/rpc.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/segment_anything.py` & `mlv-1.3.7/mlv/segment_anything.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/stable_diffusion.py` & `mlv-1.3.7/mlv/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `mlv-1.3.6/mlv/util.py` & `mlv-1.3.7/mlv/util.py`

 * *Files identical despite different names*

