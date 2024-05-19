# Comparing `tmp/vsdpir-4.0.0-py3-none-any.whl.zip` & `tmp/vsdpir-4.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13322 bytes, number of entries: 12
--rw-r--r--  2.0 fat    15816 b- defN 20-Feb-02 00:00 vsdpir/__init__.py
+Zip file size: 13309 bytes, number of entries: 12
+-rw-r--r--  2.0 fat    15807 b- defN 20-Feb-02 00:00 vsdpir/__init__.py
 -rw-r--r--  2.0 fat      922 b- defN 20-Feb-02 00:00 vsdpir/__main__.py
 -rw-r--r--  2.0 fat    21548 b- defN 20-Feb-02 00:00 vsdpir/basicblock.py
 -rw-r--r--  2.0 fat     2757 b- defN 20-Feb-02 00:00 vsdpir/network_unet.py
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_color.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_color.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_deblocking_gray.pth
 -rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 vsdpir/models/drunet_gray.pth
-?rw-r--r--  2.0 fat     1684 b- defN 20-Feb-02 00:00 vsdpir-4.0.0.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-4.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1084 b- defN 20-Feb-02 00:00 vsdpir-4.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      962 b- defN 20-Feb-02 00:00 vsdpir-4.0.0.dist-info/RECORD
-12 files, 44860 bytes uncompressed, 11698 bytes compressed:  73.9%
+?rw-r--r--  2.0 fat     1774 b- defN 20-Feb-02 00:00 vsdpir-4.1.0.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 vsdpir-4.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1084 b- defN 20-Feb-02 00:00 vsdpir-4.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      962 b- defN 20-Feb-02 00:00 vsdpir-4.1.0.dist-info/RECORD
+12 files, 44941 bytes uncompressed, 11685 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: vsdpir/models/drunet_deblocking_gray.pth
 Comment: 
 
 Filename: vsdpir/models/drunet_gray.pth
 Comment: 
 
-Filename: vsdpir-4.0.0.dist-info/METADATA
+Filename: vsdpir-4.1.0.dist-info/METADATA
 Comment: 
 
-Filename: vsdpir-4.0.0.dist-info/WHEEL
+Filename: vsdpir-4.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: vsdpir-4.0.0.dist-info/licenses/LICENSE
+Filename: vsdpir-4.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: vsdpir-4.0.0.dist-info/RECORD
+Filename: vsdpir-4.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vsdpir/__init__.py

```diff
@@ -5,19 +5,19 @@
 import warnings
 from dataclasses import dataclass
 from threading import Lock
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from vstools import check_variable, fallback, vs
+import vapoursynth as vs
 
 from .network_unet import UNetRes
 
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 os.environ["CUDA_MODULE_LOADING"] = "LAZY"
 
 warnings.filterwarnings("ignore", "The given NumPy array is not writable")
 
 model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
 
@@ -39,15 +39,15 @@
     num_streams: int = 1,
     task: str = "deblock",
     strength: float | vs.VideoNode | None = None,
     tile: list[int] = [0, 0],
     tile_pad: int = 8,
     trt: bool = False,
     trt_debug: bool = False,
-    trt_min_shape: list[int] = [640, 360],
+    trt_min_shape: list[int] = [128, 128],
     trt_opt_shape: list[int] = [1920, 1080],
     trt_max_shape: list[int] = [1920, 1080],
     trt_workspace_size: int = 0,
     trt_int8: bool = False,
     trt_int8_sample_step: int = 120,
     trt_int8_batch_size: int = 1,
     trt_cache_dir: str = model_dir,
@@ -78,15 +78,16 @@
     :param trt_int8_sample_step:    Interval between sampled frames.
     :param trt_int8_batch_size:     How many samples per batch to load. Calibrate with as large a single batch as
                                     possible. Batch size can affect truncation error and may impact the final result.
     :param trt_cache_dir:           Directory for TensorRT engine file. Engine will be cached when it's built for the
                                     first time. Note each engine is created for specific settings such as model
                                     path/name, precision, workspace etc, and specific GPUs and it's not portable.
     """
-    assert check_variable(clip, dpir)
+    if not isinstance(clip, vs.VideoNode):
+        raise vs.Error("dpir: this is not a clip")
 
     if clip.format.id not in [vs.RGBH, vs.RGBS, vs.GRAYH, vs.GRAYS]:
         raise vs.Error("dpir: only RGBH/RGBS/GRAYH/GRAYS formats are supported")
 
     if not torch.cuda.is_available():
         raise vs.Error("dpir: CUDA is not available")
 
@@ -95,16 +96,14 @@
 
     task = task.lower()
 
     if task not in ["deblock", "denoise"]:
         raise vs.Error("dpir: task must be 'deblock' or 'denoise'")
 
     if isinstance(strength, vs.VideoNode):
-        assert check_variable(strength, dpir)
-
         if strength.format.color_family != vs.GRAY:
             raise vs.Error("dpir: strength must be of GRAY format")
 
         if strength.width != clip.width or strength.height != clip.height or strength.num_frames != clip.num_frames:
             raise vs.Error("dpir: strength must have the same dimensions and number of frames as main clip")
 
     if not isinstance(tile, list) or len(tile) != 2:
@@ -147,22 +146,26 @@
 
     if task == "deblock":
         model_name = f"drunet_deblocking_{color_or_gray}.pth"
 
         if isinstance(strength, vs.VideoNode):
             noise = strength.std.Expr("x 100 /", format=noise_format)
         else:
-            noise = clip.std.BlankClip(format=noise_format, color=fallback(strength, 50.0) / 100, keep=True)
+            noise = clip.std.BlankClip(
+                format=noise_format, color=(50.0 if strength is None else strength) / 100, keep=True
+            )
     else:
         model_name = f"drunet_{color_or_gray}.pth"
 
         if isinstance(strength, vs.VideoNode):
             noise = strength.std.Expr("x 255 /", format=noise_format)
         else:
-            noise = clip.std.BlankClip(format=noise_format, color=fallback(strength, 5.0) / 255, keep=True)
+            noise = clip.std.BlankClip(
+                format=noise_format, color=(5.0 if strength is None else strength) / 255, keep=True
+            )
 
     module = UNetRes(in_nc=clip.format.num_planes + 1, out_nc=clip.format.num_planes)
     module.load_state_dict(torch.load(os.path.join(model_dir, model_name), map_location=device))
     module.eval().to(device)
     if fp16:
         module.half()
 
@@ -246,19 +249,17 @@
 
             module = torch_tensorrt.compile(
                 module,
                 ir="ts",
                 inputs=inputs,
                 enabled_precisions={torch.half, torch.int8} if trt_int8 else {dtype},
                 device=torch_tensorrt.Device(gpu_id=device_index),
-                num_avg_timing_iters=8,
                 workspace_size=trt_workspace_size,
                 calibrator=calibrator if trt_int8 else None,
                 truncate_long_and_double=True,
-                require_full_compilation=True,
                 min_block_size=1,
                 allow_shape_tensors=True,
             )
 
             torch.jit.save(module, trt_engine_path)
 
         module = [torch.jit.load(trt_engine_path) for _ in range(num_streams)]
```

## Comparing `vsdpir-4.0.0.dist-info/METADATA` & `vsdpir-4.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.3
 Name: vsdpir
-Version: 4.0.0
+Version: 4.1.0
 Summary: DPIR function for VapourSynth
 Project-URL: Homepage, https://github.com/HolyWu/vs-dpir
 Project-URL: Issues, https://github.com/HolyWu/vs-dpir/issues
 Author-email: HolyWu <holywu@gmail.com>
 License-File: LICENSE
 Keywords: DPIR,PyTorch,TensorRT,VapourSynth
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Video
 Requires-Python: >=3.10
 Requires-Dist: numpy
 Requires-Dist: requests
-Requires-Dist: torch>=2.3.0
+Requires-Dist: torch>=2.4.0.dev
 Requires-Dist: tqdm
 Requires-Dist: vapoursynth>=66
-Requires-Dist: vstools
 Description-Content-Type: text/markdown
 
 # DPIR
 Plug-and-Play Image Restoration with Deep Denoiser Prior, based on https://github.com/cszn/DPIR.
 
 
 ## Dependencies
-- [PyTorch](https://pytorch.org/get-started/) 2.3 or later
+- [PyTorch](https://pytorch.org/get-started/) 2.4.0.dev or later
 - [VapourSynth](http://www.vapoursynth.com/) R66 or later
 
 `trt` requires additional Python packages:
 - [TensorRT](https://developer.nvidia.com/tensorrt/) 10.0.1
-- [Torch-TensorRT](https://pytorch.org/TensorRT/)
+- [Torch-TensorRT](https://pytorch.org/TensorRT/) 2.4.0.dev
 
-To install TensorRT, simply run `pip install tensorrt==10.0.1`
+To install TensorRT, run `pip install tensorrt==10.0.1 tensorrt-cu12_bindings==10.0.1 tensorrt-cu12_libs==10.0.1 --extra-index-url https://pypi.nvidia.com`
 
 To install Torch-TensorRT, Windows users can pip install the whl file on [Releases](https://github.com/HolyWu/vs-dpir/releases). Linux users can run `pip install --pre torch-tensorrt --index-url https://download.pytorch.org/whl/nightly/cu121` (requires PyTorch nightly build).
 
 
 ## Installation
 ```
 pip install -U vsdpir
```

## Comparing `vsdpir-4.0.0.dist-info/licenses/LICENSE` & `vsdpir-4.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `vsdpir-4.0.0.dist-info/RECORD` & `vsdpir-4.1.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-vsdpir/__init__.py,sha256=Ctds68kOmgnccXswuKoLe9VwPOIheBF0Y49ZDy51Ljw,15816
+vsdpir/__init__.py,sha256=DPOCl72P6e-rFCiKlqixihLKZsNLZ6QG9vEbtdUG4cg,15807
 vsdpir/__main__.py,sha256=YC0lk6_VwvF8PwUCOwEXF_c0zQ1Zh_x03EFjXr8vUOU,922
 vsdpir/basicblock.py,sha256=JgSHEeEWi4t2x1ZlDzjbQA2PH5gSECaN83ql0cN3Ptw,21548
 vsdpir/network_unet.py,sha256=4WzY7UAmfMlhYazd-tfeOOIz_mktNcU_OL4ZrgTJoY8,2757
 vsdpir/models/drunet_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_deblocking_color.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_deblocking_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vsdpir/models/drunet_gray.pth,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-vsdpir-4.0.0.dist-info/METADATA,sha256=PvmwPOpRkStW6fN32N1bNfRSDumIRysEuuQTYdtROCY,1684
-vsdpir-4.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-vsdpir-4.0.0.dist-info/licenses/LICENSE,sha256=TOnHjjjk72COaBl3aWUvIQWIiDASReAL7xEEGPSGN3E,1084
-vsdpir-4.0.0.dist-info/RECORD,,
+vsdpir-4.1.0.dist-info/METADATA,sha256=Bik9ROo8A1UYalzEHetaiysOOYJKmDuwhr_c7q4kFRg,1774
+vsdpir-4.1.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+vsdpir-4.1.0.dist-info/licenses/LICENSE,sha256=TOnHjjjk72COaBl3aWUvIQWIiDASReAL7xEEGPSGN3E,1084
+vsdpir-4.1.0.dist-info/RECORD,,
```

