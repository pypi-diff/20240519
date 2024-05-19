# Comparing `tmp/infinity_emb-0.0.8.tar.gz` & `tmp/infinity_emb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinity_emb-0.0.8.tar", max compression
+gzip compressed data, was "infinity_emb-0.0.9.tar", max compression
```

## Comparing `infinity_emb-0.0.8.tar` & `infinity_emb-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     7838 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/README.md
--rw-r--r--   0        0        0      439 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/__init__.py
--rw-r--r--   0        0        0        0 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/fastapi_schemas/__init__.py
--rw-r--r--   0        0        0      575 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/fastapi_schemas/convert.py
--rw-r--r--   0        0        0      688 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/fastapi_schemas/docs.py
--rw-r--r--   0        0        0      883 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/fastapi_schemas/errors.py
--rw-r--r--   0        0        0     1277 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/fastapi_schemas/pymodels.py
--rw-r--r--   0        0        0      398 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/__init__.py
--rw-r--r--   0        0        0    13871 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/batch_handler.py
--rw-r--r--   0        0        0     2591 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/caching_layer.py
--rw-r--r--   0        0        0     1139 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/primitives.py
--rw-r--r--   0        0        0     3228 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/select_model.py
--rw-r--r--   0        0        0     2167 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/inference/threading_asyncio.py
--rw-r--r--   0        0        0    10564 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/infinity_server.py
--rw-r--r--   0        0        0      921 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/log_handler.py
--rw-r--r--   0        0        0       89 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/__init__.py
--rw-r--r--   0        0        0      885 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/abstract.py
--rw-r--r--   0        0        0      849 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/dummytransformer.py
--rw-r--r--   0        0        0     2382 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/fastembed.py
--rw-r--r--   0        0        0     9818 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/sentence_transformer.py
--rw-r--r--   0        0        0     2057 2023-11-25 13:33:11.971670 infinity_emb-0.0.8/infinity_emb/transformer/utils.py
--rw-r--r--   0        0        0     2482 2023-11-25 13:33:11.975670 infinity_emb-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9848 1970-01-01 00:00:00.000000 infinity_emb-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7838 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/README.md
+-rw-r--r--   0        0        0      439 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/fastapi_schemas/__init__.py
+-rw-r--r--   0        0        0      575 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/fastapi_schemas/convert.py
+-rw-r--r--   0        0        0      688 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/fastapi_schemas/docs.py
+-rw-r--r--   0        0        0      883 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/fastapi_schemas/errors.py
+-rw-r--r--   0        0        0     1277 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/fastapi_schemas/pymodels.py
+-rw-r--r--   0        0        0      466 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/__init__.py
+-rw-r--r--   0        0        0    13871 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/batch_handler.py
+-rw-r--r--   0        0        0     2591 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/caching_layer.py
+-rw-r--r--   0        0        0     1367 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/primitives.py
+-rw-r--r--   0        0        0     3358 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/select_model.py
+-rw-r--r--   0        0        0     2167 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/inference/threading_asyncio.py
+-rw-r--r--   0        0        0    11092 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/infinity_server.py
+-rw-r--r--   0        0        0      921 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/log_handler.py
+-rw-r--r--   0        0        0       89 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/__init__.py
+-rw-r--r--   0        0        0      885 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/abstract.py
+-rw-r--r--   0        0        0      849 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/dummytransformer.py
+-rw-r--r--   0        0        0     2476 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/fastembed.py
+-rw-r--r--   0        0        0     9819 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/sentence_transformer.py
+-rw-r--r--   0        0        0     2059 2023-12-05 00:13:48.393328 infinity_emb-0.0.9/infinity_emb/transformer/utils.py
+-rw-r--r--   0        0        0     2464 2023-12-05 00:13:48.397328 infinity_emb-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9832 1970-01-01 00:00:00.000000 infinity_emb-0.0.9/PKG-INFO
```

### Comparing `infinity_emb-0.0.8/README.md` & `infinity_emb-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   poetry install --extras all
   ```
 </details>
 
 
 ### Launch via Python
 ```Python
-from infinity_emb import create server
+from infinity_emb import create_server
 fastapi_app = create_server()
 ```
 or use the AsyncAPI directly.:
 
 ```python
 from infinity_emb import AsyncEmbeddingEngine, transformer
 sentences = ["Embedded this is sentence via Infinity.", "Paris is in France."]
```

### Comparing `infinity_emb-0.0.8/infinity_emb/fastapi_schemas/convert.py` & `infinity_emb-0.0.9/infinity_emb/fastapi_schemas/convert.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/fastapi_schemas/docs.py` & `infinity_emb-0.0.9/infinity_emb/fastapi_schemas/docs.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/fastapi_schemas/errors.py` & `infinity_emb-0.0.9/infinity_emb/fastapi_schemas/errors.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/fastapi_schemas/pymodels.py` & `infinity_emb-0.0.9/infinity_emb/fastapi_schemas/pymodels.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/inference/batch_handler.py` & `infinity_emb-0.0.9/infinity_emb/inference/batch_handler.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/inference/caching_layer.py` & `infinity_emb-0.0.9/infinity_emb/inference/caching_layer.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/inference/primitives.py` & `infinity_emb-0.0.9/infinity_emb/inference/primitives.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import asyncio
+import enum
 import time
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Dict, Optional
 from uuid import uuid4
 
 import numpy as np
 
 NpEmbeddingType = np.ndarray
 
 
+class Device(enum.Enum):
+    cpu = "cpu"
+    cuda = "cuda"
+    auto = None
+
+
+_devices: Dict[str, str] = {e.name: e.name for e in Device}
+DeviceTypeHint = enum.Enum("DeviceTypeHint", _devices)  # type: ignore
+
+
 @dataclass(order=True)
 class EmbeddingResult:
     sentence: str = field(compare=False)
     future: asyncio.Future = field(compare=False)
     uuid: str = field(default_factory=lambda: str(uuid4()), compare=False)
     embedding: Optional[NpEmbeddingType] = field(default=None, compare=False)
```

### Comparing `infinity_emb-0.0.8/infinity_emb/inference/select_model.py` & `infinity_emb-0.0.9/infinity_emb/inference/select_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from time import perf_counter
 from typing import List, Optional, Tuple
 
-from infinity_emb.inference.primitives import EmbeddingResult, NpEmbeddingType
+from infinity_emb.inference.primitives import Device, EmbeddingResult, NpEmbeddingType
 from infinity_emb.log_handler import logger
 from infinity_emb.transformer.abstract import BaseTransformer
 from infinity_emb.transformer.utils import InferenceEngine
 
 
 def select_model_to_functional(
-    model_name_or_path: str, batch_size: int, engine: InferenceEngine, model_warmup=True
+    model_name_or_path: str,
+    batch_size: int,
+    engine: InferenceEngine,
+    model_warmup=True,
+    device: Device = Device.auto,
 ):
-    logger.info(f"model=`{model_name_or_path}` selected, using engine=`{engine.value}`")
-    init_engine = engine.value(model_name_or_path)
+    logger.info(
+        f"model=`{model_name_or_path}` selected, using engine=`{engine.value}`"
+        f" and device=`{device.value}`"
+    )
+    init_engine = engine.value(model_name_or_path, device=device.value)
 
     min_inference_t = 4e-3
     if model_warmup:
         # size one, warm up warm start timings.
         runtime_check_callable(init_engine, log=False)
         # size one
         runtime_check_callable(init_engine, log=True)
```

### Comparing `infinity_emb-0.0.8/infinity_emb/inference/threading_asyncio.py` & `infinity_emb-0.0.9/infinity_emb/inference/threading_asyncio.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/infinity_server.py` & `infinity_emb-0.0.9/infinity_emb/infinity_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 import time
-from typing import List
+from typing import List, Union
 
 # prometheus
 import infinity_emb
 from infinity_emb.fastapi_schemas import docs, errors
 from infinity_emb.fastapi_schemas.convert import list_embeddings_to_response
 from infinity_emb.fastapi_schemas.pymodels import (
     OpenAIEmbeddingInput,
     OpenAIEmbeddingResult,
     OpenAIModelInfo,
 )
-from infinity_emb.inference import BatchHandler, select_model_to_functional
+from infinity_emb.inference import (
+    BatchHandler,
+    Device,
+    DeviceTypeHint,
+    select_model_to_functional,
+)
 from infinity_emb.inference.caching_layer import INFINITY_CACHE_VECTORS
 from infinity_emb.log_handler import UVICORN_LOG_LEVELS, logger
 from infinity_emb.transformer.utils import InferenceEngine, InferenceEngineTypeHint
 
 
 class AsyncEmbeddingEngine:
     def __init__(
         self,
         model_name_or_path: str = "BAAI/bge-small-en-v1.5",
         batch_size: int = 64,
         engine: InferenceEngine = InferenceEngine.torch,
         model_warmup=True,
         vector_disk_cache_path: str = "",
+        device: Union[Device, str] = Device.auto,
     ) -> None:
         """Creating a Async EmbeddingEngine object.
 
         Args:
             model_name_or_path, str:  Defaults to "BAAI/bge-small-en-v1.5".
             batch_size, int: Defaults to 64.
             engine, InferenceEngine: backend for inference.
                 Defaults to InferenceEngine.torch.
             model_warmup, bool: decide if warmup with max batch size . Defaults to True.
             vector_disk_cache_path, str: file path to folder of cache.
                 Defaults to "" - default no caching.
+            device, Device: device to use for inference. Defaults to Device.auto
 
         Example:
             ```python
             from infinity_emb import AsyncEmbeddingEngine, transformer
             sentences = ["Embedded this via Infinity.", "Paris is in France."]
             engine = AsyncEmbeddingEngine(engine=transformer.InferenceEngine.torch)
             async with engine: # engine starts with engine.astart()
                 embeddings = np.array(await engine.embed(sentences))
             # engine stops with engine.astop().
             # For frequent restarts, handle start/stop yourself.
             ```
         """
         self.batch_size = batch_size
         self.running = False
-        self._vector_disk_cache_path=vector_disk_cache_path,
+        self._vector_disk_cache_path = vector_disk_cache_path
         self._model, self._min_inference_t = select_model_to_functional(
             model_name_or_path=model_name_or_path,
             batch_size=batch_size,
             engine=engine,
-            model_warmup=model_warmup
+            model_warmup=model_warmup,
+            device=Device[device] if isinstance(device, str) else device,
         )
 
     async def astart(self):
         """startup engine"""
         if self.running:
             raise ValueError(
                 "DoubleSpawn: already started `AsyncEmbeddingEngine`. "
@@ -125,14 +133,15 @@
     model_name_or_path: str = "BAAI/bge-small-en-v1.5",
     url_prefix: str = "/v1",
     batch_size: int = 64,
     engine: InferenceEngine = InferenceEngine.torch,
     verbose: bool = False,
     model_warmup=True,
     vector_disk_cache=INFINITY_CACHE_VECTORS,
+    device: Device = Device.auto,
     doc_extra: dict = {},
 ):
     """
     creates the FastAPI App
     """
     from fastapi import FastAPI, responses, status
     from prometheus_fastapi_instrumentator import Instrumentator
@@ -160,14 +169,15 @@
         instrumentator.expose(app)
 
         model, min_inference_t = select_model_to_functional(
             model_name_or_path=model_name_or_path,
             batch_size=batch_size,
             engine=engine,
             model_warmup=model_warmup,
+            device=device,
         )
 
         app.batch_handler = BatchHandler(
             max_batch_size=batch_size,
             model=model,
             verbose=verbose,
             batch_delay=min_inference_t / 2,
@@ -254,24 +264,25 @@
                 f"internal server error {ex}",
                 code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             )
 
     return app
 
 
-def start_uvicorn(
+def _start_uvicorn(
     model_name_or_path: str = "BAAI/bge-small-en-v1.5",
     batch_size: int = 64,
     url_prefix: str = "/v1",
     host: str = "0.0.0.0",
     port: int = 7997,
     log_level: UVICORN_LOG_LEVELS = UVICORN_LOG_LEVELS.info.name,  # type: ignore
     engine: InferenceEngineTypeHint = InferenceEngineTypeHint.torch.name,  # type: ignore # noqa
     model_warmup: bool = True,
     vector_disk_cache: bool = INFINITY_CACHE_VECTORS,
+    device: DeviceTypeHint = DeviceTypeHint.auto.name,
 ):
     """Infinity Embedding API ♾️  cli to start a uvicorn-server instance;
     MIT License; Copyright (c) 2023 Michael Feil
 
     Args:
         model_name_or_path, str: Huggingface model, e.g.
             "BAAI/bge-small-en-v1.5".
@@ -282,37 +293,40 @@
         log_level: logging level.
             For high performance, use "info" or higher levels. Defaults to "info".
         engine, str: framework that should perform inference.
         model_warmup, bool: perform model warmup before starting the server.
             Defaults to True.
         vector_disk_cache, bool: cache past embeddings in SQL.
             Defaults to False or env-INFINITY_CACHE_VECTORS if set
+        device, Device: device to use for inference. Defaults to Device.auto or "auto"
     """
     import uvicorn
 
     engine_load: InferenceEngine = InferenceEngine[engine.name]
+    device: Device = Device[device.name]
     logger.setLevel(log_level.to_int())
 
     app = create_server(
         model_name_or_path=model_name_or_path,
         url_prefix=url_prefix,
         batch_size=batch_size,
         engine=engine_load,
         verbose=log_level.to_int() <= 10,
         doc_extra=dict(host=host, port=port),
         model_warmup=model_warmup,
         vector_disk_cache=vector_disk_cache,
+        device=device,
     )
     uvicorn.run(app, host=host, port=port, log_level=log_level.name)
 
 
 def cli():
     """fires the command line using Python `typer.run()`"""
     import typer
 
-    typer.run(start_uvicorn)
+    typer.run(_start_uvicorn)
 
 
 # app = create_server()
 if __name__ == "__main__":
     # for debugging
     cli()
```

### Comparing `infinity_emb-0.0.8/infinity_emb/log_handler.py` & `infinity_emb-0.0.9/infinity_emb/log_handler.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/transformer/abstract.py` & `infinity_emb-0.0.9/infinity_emb/transformer/abstract.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/transformer/dummytransformer.py` & `infinity_emb-0.0.9/infinity_emb/transformer/dummytransformer.py`

 * *Files identical despite different names*

### Comparing `infinity_emb-0.0.8/infinity_emb/transformer/fastembed.py` & `infinity_emb-0.0.9/infinity_emb/transformer/fastembed.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 
 class Fastembed(DefaultEmbedding, BaseTransformer):
     def __init__(self, *args, **kwargs):
         if not FASTEMBED_AVAILABLE:
             raise ImportError(
                 "fastembed is not installed." "`pip install infinity-emb[fastembed]`"
             )
+        providers = ["CPUExecutionProvider"]
+
         if not kwargs.get("cache_dir"):
             from infinity_emb.transformer.utils import infinity_cache_dir
 
             kwargs["cache_dir"] = infinity_cache_dir()
+        if kwargs.pop("device", None) != "cpu":
+            providers = ["CUDAExecutionProvider"] + providers
         super(DefaultEmbedding, self).__init__(*args, **kwargs)
         self._infinity_tokenizer = copy.deepcopy(self.model.tokenizer)
-        self.model.model.set_providers(
-            ["CUDAExecutionProvider", "CPUExecutionProvider"]
-        )
+        self.model.model.set_providers(providers)
 
     def encode_pre(self, sentences: List[str]) -> Dict[str, np.ndarray[int]]:
         encoded = self.model.tokenizer.encode_batch(sentences)
         input_ids = np.array([e.ids for e in encoded])
         attention_mask = np.array([e.attention_mask for e in encoded])
 
         onnx_input = {
```

### Comparing `infinity_emb-0.0.8/infinity_emb/transformer/sentence_transformer.py` & `infinity_emb-0.0.9/infinity_emb/transformer/sentence_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         device = self._target_device
         self.to(device)
         # make a copy of the tokenizer,
         # to be able to could the tokens in another thread
         # without corrupting the original.
         fm = self._first_module()
         self._infinity_tokenizer = copy.deepcopy(fm.tokenizer)
+        self.eval()
+
         if OPTIMUM_AVAILABLE and not os.environ.get("INFINITY_DISABLE_OPTIMUM", False):
             logger.info(
                 "Adding optimizations via Huggingface optimum. "
                 "Disable by setting the env var `INFINITY_DISABLE_OPTIMUM`"
             )
             try:
                 fm.auto_model = BetterTransformer.transform(fm.auto_model)
@@ -74,15 +76,14 @@
             )
         else:
             logger.info(
                 "No optimizations via Huggingface optimum, "
                 "install `pip install infinity-emb[optimum]`"
             )
 
-        self.eval()
         if self._target_device.type == "cuda" and os.environ.get(
             "INFINITY_TORCH_ENABLE_HALF", False
         ):
             logger.info(
                 "Switching to half() precision (fp16)."
                 "Enabled by the setting the env var `INFINITY_TORCH_ENABLE_HALF`"
             )
```

### Comparing `infinity_emb-0.0.8/infinity_emb/transformer/utils.py` & `infinity_emb-0.0.9/infinity_emb/transformer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 class InferenceEngine(Enum):
     torch = SentenceTransformerPatched
     ctranslate2 = CT2SentenceTransformer
     fastembed = Fastembed
     debugengine = DummyTransformer
 
 
-types: Dict[str, str] = {e.name: e.name for e in InferenceEngine}
-InferenceEngineTypeHint = Enum("InferenceEngineTypeHint", types)  # type: ignore
+_types: Dict[str, str] = {e.name: e.name for e in InferenceEngine}
+InferenceEngineTypeHint = Enum("InferenceEngineTypeHint", _types)  # type: ignore
 
 
 def length_tokenizer(
     _sentences: List[str],
 ) -> List[int]:
     return [len(i) for i in _sentences]
```

### Comparing `infinity_emb-0.0.8/pyproject.toml` & `infinity_emb-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "infinity_emb"
-version = "0.0.8"
+version = "0.0.9"
 description = "Infinity is a high-throughput, low-latency REST API for serving vector embeddings, supporting a wide range of sentence-transformer models and frameworks."
 authors = ["michaelfeil <me@michaelfeil.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "infinity_emb"}]
 
 [tool.poetry.dependencies]
@@ -17,15 +17,15 @@
 # webserver-only
 fastapi = {version = "^0.103.2", optional=true}
 orjson = {version = ">=3.9.8,<4", optional=true} 
 prometheus-fastapi-instrumentator = {version = "^6.1.0", optional=true}
 uvicorn = {extras = ["standard"], version = "^0.23.2", optional=true}
 typer = {extras = ["all"], version = "^0.9.0", optional=true}
 # backend
-torch = {version = ">=2.0.0, !=2.0.1, !=2.1.0", optional=true} 
+torch = {version = ">=2.0.0", optional=true} 
 sentence-transformers = {version = "2.2.2", optional=true} 
 ctranslate2 = {version = "^3.21.0", optional=true}
 optimum = {version = "^1.13.2", optional=true}
 fastembed = {version = "0.1.1", optional=true} 
 onnxruntime-gpu = {version = "*", optional=true}
 # cache
 diskcache = {version = "*", optional=true}
```

### Comparing `infinity_emb-0.0.8/PKG-INFO` & `infinity_emb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinity_emb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Infinity is a high-throughput, low-latency REST API for serving vector embeddings, supporting a wide range of sentence-transformer models and frameworks.
 License: MIT
 Author: michaelfeil
 Author-email: me@michaelfeil.eu
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 Requires-Dist: onnxruntime-gpu ; extra == "onnxruntime-gpu"
 Requires-Dist: optimum (>=1.13.2,<2.0.0) ; extra == "optimum" or extra == "all"
 Requires-Dist: orjson (>=3.9.8,<4) ; extra == "server" or extra == "all"
 Requires-Dist: prometheus-fastapi-instrumentator (>=6.1.0,<7.0.0) ; extra == "server" or extra == "all"
 Requires-Dist: pydantic (>=2.4.0,<3) ; extra == "server" or extra == "all"
 Requires-Dist: rich (>=13,<14) ; extra == "logging" or extra == "server" or extra == "all"
 Requires-Dist: sentence-transformers (==2.2.2) ; extra == "ct2" or extra == "torch" or extra == "all"
-Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0) ; extra == "ct2" or extra == "torch" or extra == "all"
+Requires-Dist: torch (>=2.0.0) ; extra == "ct2" or extra == "torch" or extra == "all"
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0) ; extra == "server" or extra == "all"
 Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0) ; extra == "server" or extra == "all"
 Description-Content-Type: text/markdown
 
 
 <!-- PROJECT SHIELDS -->
 <!--
@@ -91,15 +91,15 @@
   poetry install --extras all
   ```
 </details>
 
 
 ### Launch via Python
 ```Python
-from infinity_emb import create server
+from infinity_emb import create_server
 fastapi_app = create_server()
 ```
 or use the AsyncAPI directly.:
 
 ```python
 from infinity_emb import AsyncEmbeddingEngine, transformer
 sentences = ["Embedded this is sentence via Infinity.", "Paris is in France."]
```

