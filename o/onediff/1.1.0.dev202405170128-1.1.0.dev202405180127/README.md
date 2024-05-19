# Comparing `tmp/onediff-1.1.0.dev202405170128.tar.gz` & `tmp/onediff-1.1.0.dev202405180127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.1.0.dev202405170128.tar", last modified: Fri May 17 01:28:13 2024, max compression
+gzip compressed data, was "onediff-1.1.0.dev202405180127.tar", last modified: Sat May 18 01:27:27 2024, max compression
```

## Comparing `onediff-1.1.0.dev202405170128.tar` & `onediff-1.1.0.dev202405180127.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-17 01:28:03.000000 onediff-1.1.0.dev202405170128/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-17 01:28:03.000000 onediff-1.1.0.dev202405170128/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.698478 onediff-1.1.0.dev202405170128/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.698478 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77140 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/nexfort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.702478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/core/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/core/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/core/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.706478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.706478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/nexfort/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/nexfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/nexfort/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.706478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.706478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-17 01:28:13.000000 onediff-1.1.0.dev202405170128/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-17 01:28:13.000000 onediff-1.1.0.dev202405170128/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:28:13.000000 onediff-1.1.0.dev202405170128/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 01:28:13.000000 onediff-1.1.0.dev202405170128/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 01:28:13.000000 onediff-1.1.0.dev202405170128/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:28:13.710478 onediff-1.1.0.dev202405170128/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-17 01:28:04.000000 onediff-1.1.0.dev202405170128/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.224080 onediff-1.1.0.dev202405180127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77140 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.228080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/nexfort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.232080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/core/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/core/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.232080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.232080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/nexfort/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/nexfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/nexfort/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.232080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.232080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-18 01:27:27.000000 onediff-1.1.0.dev202405180127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-18 01:27:27.000000 onediff-1.1.0.dev202405180127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:27:27.000000 onediff-1.1.0.dev202405180127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-18 01:27:27.000000 onediff-1.1.0.dev202405180127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 01:27:27.000000 onediff-1.1.0.dev202405180127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:27:27.236080 onediff-1.1.0.dev202405180127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-18 01:27:21.000000 onediff-1.1.0.dev202405180127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.1.0.dev202405170128/LICENSE` & `onediff-1.1.0.dev202405180127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/PKG-INFO` & `onediff-1.1.0.dev202405180127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405170128
+Version: 1.1.0.dev202405180127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405170128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405180127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405170128/README.md` & `onediff-1.1.0.dev202405180127/README.md`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/setup.py` & `onediff-1.1.0.dev202405180127/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.1.0.dev202405180127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/nexfort.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/nexfort.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/core/with_onediff_compile.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/core/with_onediff_compile.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/nexfort/deployable_module.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/nexfort/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
 @torch2oflow.register
 def _(mod: type):
     if not is_need_mock(mod):
         return mod
     return proxy_class(mod)
 
 
-def default_converter(obj, verbose=False, *, proxy_cls=None):
-    if not is_need_mock(type(obj)):
+def default_converter(obj, verbose=False, *, proxy_cls=None, bypass_check=False):
+    if not bypass_check and not is_need_mock(type(obj)):
         return obj
     try:
         new_obj_cls = proxy_class(type(obj)) if proxy_cls is None else proxy_cls
 
         def init(self):
             for k, _ in obj.__dict__.items():
                 attr = getattr(obj, k)
@@ -443,15 +443,15 @@
                 logger.warning(
                     f"warning when get {mod.__name__} in torch.nn.functional: {e}"
                 )
                 mod_name = mod.__module__.replace("torch", "oneflow")
         if mod_name is not None:
             m = importlib.import_module(mod_name)
             return getattr(m, mod.__name__)
-
+    
     return default_converter(mod, verbose)
 
 
 @torch2oflow.register
 def _(mod: torch.device, verbose=False):
     index = mod.index if mod.index is not None else 0
     return flow.device(mod.type, index)
```

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,17 @@
             self.logger.info(
                 f"{mock_full_cls_name} not in _oflow_to_torch_cls_map, import it directly."
             )
             mod = importlib.import_module(cls.__module__)
             return getattr(mod, cls.__qualname__)
 
     def transform_func(self, func: types.FunctionType):
-        # TODO: support transform function cache
+        mock_full_cls_name = self.get_transformed_entity_name(func)
+        if mock_full_cls_name in self._torch_to_oflow_cls_map:
+            return self._torch_to_oflow_cls_map[mock_full_cls_name]
         return self._transform_entity(func)
 
     def transform_package(self, package_name):
         return self._transform_entity(package_name)
 
 
 debug_mode = os.getenv("ONEDIFF_DEBUG", "0") == "1"
```

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/__init__.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,25 +50,20 @@
         )
 
         if is_first_load:
             graph_file = generate_graph_file_name(
                 graph_file, self, args=args, kwargs=kwargs
             )
             setattr(self, "_load_graph_first_run", False)
-
-        def apply_patch_after_loading_state_dict(state_dict):
-            nonlocal self, args, kwargs
-            graph = self.get_graph()
+            # Avoid graph file conflicts
             if importlib.util.find_spec("register_comfy"):
                 from register_comfy import CrossAttntionStateDictPatch as state_patch
-
-                state_dict = state_patch.apply_patch_after_loading_state_dict(
-                    state_dict, input_kwargs=kwargs, graph=graph
-                )
-            return state_dict
+                attn2_patch_sum = state_patch.attn2_patch_sum(input_kwargs=kwargs)
+                if attn2_patch_sum > 0:
+                    graph_file = graph_file.replace(".graph", f"_attn2_{attn2_patch_sum}.graph")
 
         def process_state_dict_before_saving(state_dict: Dict):
             nonlocal self, args, kwargs, graph_file
             graph = self.get_graph()
             if importlib.util.find_spec("register_comfy"):
                 from register_comfy import CrossAttntionStateDictPatch as state_patch
 
@@ -88,26 +83,29 @@
                 )
             else:
                 graph_device = compile_options.graph_file_device
                 state_dict = flow.load(graph_file)
                 self.load_graph(
                     graph_file, torch2oflow(graph_device), state_dict=state_dict
                 )
-                apply_patch_after_loading_state_dict(state_dict)
                 logger.info(f"Loaded graph file: {graph_file}")
                 is_first_load = False
 
         def handle_graph_saving():
             nonlocal graph_file, compile_options, is_first_load
             if not is_first_load:
                 return
             try:
                 parent_dir = os.path.dirname(graph_file)
                 if parent_dir != "":
                     os.makedirs(parent_dir, exist_ok=True)
+                
+                # Avoid graph file conflicts
+                if os.path.exists(graph_file):
+                    raise FileExistsError(f"File {graph_file} exists!")
 
                 self.save_graph(
                     graph_file, process_state_dict=process_state_dict_before_saving
                 )
                 logger.info(f"Saved graph file: {graph_file}")
 
             except Exception as e:
```

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/options.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.1.0.dev202405180127/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/optimization/attention_processor.py` & `onediff-1.1.0.dev202405180127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/optimization/quant_optimizer.py` & `onediff-1.1.0.dev202405180127/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.1.0.dev202405180127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/quantization/load_quantized_model.py` & `onediff-1.1.0.dev202405180127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.1.0.dev202405180127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.1.0.dev202405180127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff/quantization/quantize_utils.py` & `onediff-1.1.0.dev202405180127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/src/onediff.egg-info/PKG-INFO` & `onediff-1.1.0.dev202405180127/src/onediff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.1.0.dev202405170128
+Version: 1.1.0.dev202405180127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: contact@siliconflow.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405170128 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.1.0.dev202405180127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 contact@siliconflow.com License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
```

### Comparing `onediff-1.1.0.dev202405170128/src/onediff.egg-info/SOURCES.txt` & `onediff-1.1.0.dev202405180127/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/tests/test_dual_module_list.py` & `onediff-1.1.0.dev202405180127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.1.0.dev202405180127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/tests/test_quantitative_quality.py` & `onediff-1.1.0.dev202405180127/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.1.0.dev202405170128/tests/test_quantize_custom_model.py` & `onediff-1.1.0.dev202405180127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

