# Comparing `tmp/TensorFlowASR-2.0.0.tar.gz` & `tmp/TensorFlowASR-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlowASR-2.0.0.tar", last modified: Sat May  4 17:02:01 2024, max compression
+gzip compressed data, was "TensorFlowASR-2.0.1.tar", last modified: Sun May 19 17:34:57 2024, max compression
```

## Comparing `TensorFlowASR-2.0.0.tar` & `TensorFlowASR-2.0.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     8995 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 17:02:01.000000 TensorFlowASR-2.0.0/TensorFlowASR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      234 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/base_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/gaussnoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/specaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/configs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20538 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/features/gammatone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/ctc_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/losses/rnnt_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.391423 TensorFlowASR-2.0.0/tensorflow_asr/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/metrics/error_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/activations/glu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28243 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/base_ctc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/deepspeech2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/jasper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/decoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.395423 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/contextnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/deepspeech2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/jasper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/rnnt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/multihead_attention.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6990 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/sequence_wise_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/layers/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49153 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/base_transducer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/contextnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/rnnt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.399423 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/regularizers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4495 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/optimizers/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16765 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:02:01.403423 TensorFlowASR-2.0.0/tensorflow_asr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/app_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/data_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/feature_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/layer_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/math_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/metric_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/plot_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/shape_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-04 17:01:44.000000 TensorFlowASR-2.0.0/tensorflow_asr/utils/tf_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8362 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-19 17:34:57.000000 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-19 17:34:57.000000 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:34:57.000000 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-19 17:34:57.000000 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 17:34:57.000000 TensorFlowASR-2.0.1/TensorFlowASR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      234 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/base_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/gaussnoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/specaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/configs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20749 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/features/gammatone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/losses/ctc_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/losses/rnnt_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/metrics/error_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.427383 TensorFlowASR-2.0.1/tensorflow_asr/models/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/activations/glu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28870 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.431383 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/base_ctc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/deepspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/jasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.431383 TensorFlowASR-2.0.1/tensorflow_asr/models/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/decoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.431383 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24566 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/contextnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/deepspeech2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/jasper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/rnnt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.431383 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19802 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/multihead_attention.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6990 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/sequence_wise_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/layers/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49243 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/base_transducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/contextnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/rnnt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/tensorflow_asr/optimizers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/optimizers/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/optimizers/regularizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4495 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/optimizers/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17184 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:57.435383 TensorFlowASR-2.0.1/tensorflow_asr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/app_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/data_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/feature_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/layer_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/math_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/metric_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/plot_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/shape_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-19 17:34:50.000000 TensorFlowASR-2.0.1/tensorflow_asr/utils/tf_util.py
```

### Comparing `TensorFlowASR-2.0.0/LICENSE` & `TensorFlowASR-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/PKG-INFO` & `TensorFlowASR-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TensorFlowASR
-Version: 2.0.0
+Version: 2.0.1
 Summary: Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2
 Home-page: https://github.com/TensorSpeech/TensorFlowASR
 Author: Huy Le Nguyen
 Author-email: nlhuy.cs.16@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -23,28 +23,28 @@
 Provides-Extra: tf2-14
 Provides-Extra: tf2-14-gpu
 Provides-Extra: tf2-15
 Provides-Extra: tf2-15-gpu
 License-File: LICENSE
 
 <h1 align="center">
-<p>TensorFlowASR :zap:</p>
+TensorFlowASR :zap:
+</h1>
 <p align="center">
 <a href="https://github.com/TensorSpeech/TensorFlowASR/blob/main/LICENSE">
   <img alt="GitHub" src="https://img.shields.io/github/license/TensorSpeech/TensorFlowASR?logo=apache&logoColor=green">
 </a>
-<img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.6-blue?logo=python">
+<img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.8-blue?logo=python">
 <img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.12.0-orange?logo=tensorflow">
 <a href="https://pypi.org/project/TensorFlowASR/">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/TensorFlowASR?color=%234285F4&label=release&logo=pypi&logoColor=%234285F4">
 </a>
 </p>
-</h1>
 <h2 align="center">
-<p>Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2</p>
+Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2
 </h2>
 
 <p align="center">
 TensorFlowASR implements some automatic speech recognition architectures such as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These models can be converted to TFLite to reduce memory and computation for deployment :smile:
 </p>
 
 ## What's New?
@@ -84,23 +84,23 @@
 
 - **Transducer Models** (End2end models using RNNT Loss for training, currently supported Conformer, ContextNet, Streaming Transducer)
 - **CTCModel** (End2end models using CTC Loss for training, currently supported DeepSpeech2, Jasper)
 
 ### Publications
 
 - **Conformer Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100))
-  See [examples/conformer](./examples/conformer)
+  See [examples/models/transducer/conformer](./examples/models/transducer/conformer)
 - **ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
-  See [examples/contextnet](./examples/contextnet)
+  See [examples/models/transducer/contextnet](./examples/models/transducer/contextnet)
 - **RNN Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
-  See [examples/rnn_transducer](./examples/rnn_transducer)
+  See [examples/models/transducer/rnnt](./examples/models/transducer/rnnt)
 - **Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595))
-  See [examples/deepspeech2](./examples/deepspeech2)
+  See [examples/models/ctc/deepspeech2](./examples/models/ctc/deepspeech2)
 - **Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288))
-  See [examples/jasper](./examples/jasper)
+  See [examples/models/ctc/jasper](./examples/models/ctc/jasper)
 
 ## Installation
 
 For training and testing, you should use `git clone` for installing necessary packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.)
 
 ### Installing from source (recommended)
 
@@ -139,35 +139,43 @@
 pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine
 ```
 
 ### Install for Apple Sillicon
 
 Due to tensorflow-text is not built for Apple Sillicon, we need to install it with the prebuilt wheel file from [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon](https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon)
 
+```bash
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+pip3 install -e "." # or pip3 install -e ".[dev] for development # or pip3 install "TensorFlowASR[dev]" from PyPi
+pip3 install tensorflow~=2.14.0 # change minor version if you want
+```
+
 Do this after installing TensorFlowASR with tensorflow above
 
 ```bash
 TF_VERSION="$(python3 -c 'import tensorflow; print(tensorflow.__version__)')" && \
 TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -d'.' -f1,2)" && \
+PY_VERSION="$(python3 -c 'import platform; major, minor, patch = platform.python_version_tuple(); print(f"{major}{minor}");')" && \
 URL="https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon" && \
-pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp310-cp310-macosx_11_0_arm64.whl"
+pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp${PY_VERSION}-cp${PY_VERSION}-macosx_11_0_arm64.whl"
 ```
 
 ### Running in a container
 
 ```bash
 docker-compose up -d
 ```
 
 
 
 ## Training & Testing Tutorial
 
-- For training, please read [tutorial_training](./docs/1_tutorial_training.md)
-- For testing, please read [tutorial_testing](./docs/2_tutorial_testing.md)
+- For training, please read [tutorial_training](./docs/tutorials/training.md)
+- For testing, please read [tutorial_testing](./docs/tutorials/testing.md)
 
 **FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
 
 See [examples](./examples/) for some predefined ASR models and results
 
 ## Features Extraction
 
@@ -175,42 +183,17 @@
 
 ## Augmentations
 
 See [augmentations](./tensorflow_asr/augmentations/README.md)
 
 ## TFLite Convertion
 
-After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **unicode code points**, then we can convert unicode points to string.
-
-1. Install `tf-nightly` using `pip install tf-nightly`
-2. Build a model with the same architecture as the trained model _(if model has tflite argument, you must set it to True)_, then load the weights from trained model to the built model
-3. Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function `add_featurizers`
-4. Convert model's function to tflite as follows:
-
-```python
-func = model.make_tflite_function(**options) # options are the arguments of the function
-concrete_func = func.get_concrete_function()
-converter = tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
-converter.experimental_new_converter = True
-converter.optimizations = [tf.lite.Optimize.DEFAULT]
-converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS,
-                                       tf.lite.OpsSet.SELECT_TF_OPS]
-tflite_model = converter.convert()
-```
-
-5. Save the converted tflite model as follows:
-
-```python
-if not os.path.exists(os.path.dirname(tflite_path)):
-    os.makedirs(os.path.dirname(tflite_path))
-with open(tflite_path, "wb") as tflite_out:
-    tflite_out.write(tflite_model)
-```
+After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **text and tokens**
 
-5. Then the `.tflite` model is ready to be deployed
+See [tflite_convertion](./docs/tutorials/tflite.md)
 
 ## Pretrained Models
 
 Go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
 
 ## Corpus Sources
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: TensorFlowASR Version: 2.0.0 Summary: Almost State-
+Metadata-Version: 2.1 Name: TensorFlowASR Version: 2.0.1 Summary: Almost State-
 of-the-art Automatic Speech Recognition using Tensorflow 2 Home-page: https://
 github.com/TensorSpeech/TensorFlowASR Author: Huy Le Nguyen Author-email:
 nlhuy.cs.16@gmail.com Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: tf2-12 Provides-Extra: tf2-12-gpu Provides-
 Extra: tf2-13 Provides-Extra: tf2-13-gpu Provides-Extra: tf2-14 Provides-Extra:
 tf2-14-gpu Provides-Extra: tf2-15 Provides-Extra: tf2-15-gpu License-File:
 LICENSE
-      ************ TTeennssoorrFFlloowwAASSRR ::zzaapp::_[[_GG_ii_tt_HH_uu_bb_]][[ppyytthhoonn]][[tteennssoorrffllooww]]_[[_PP_yy_PP_II_]] ************
+                       ************ TTeennssoorrFFlloowwAASSRR ::zzaapp:: ************
+                      _[_G_i_t_H_u_b_][python][tensorflow]_[_P_y_P_I_]
   ********** AAllmmoosstt SSttaattee--ooff--tthhee--aarrtt AAuuttoommaattiicc SSppeeeecchh RReeccooggnniittiioonn iinn TTeennssoorrffllooww 22
                                      **********
  TensorFlowASR implements some automatic speech recognition architectures such
    as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These
     models can be converted to TFLite to reduce memory and computation for
                               deployment :smile:
 ## What's New? ## Table of Contents - [What's New?](#whats-new) - [Table of
@@ -33,23 +34,25 @@
 [Vietnamese](#vietnamese) - [How to contribute](#how-to-contribute) -
 [References \& Credits](#references--credits) - [Contact](#contact) ## :yum:
 Supported Models ### Baselines - **Transducer Models** (End2end models using
 RNNT Loss for training, currently supported Conformer, ContextNet, Streaming
 Transducer) - **CTCModel** (End2end models using CTC Loss for training,
 currently supported DeepSpeech2, Jasper) ### Publications - **Conformer
 Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/
-abs/2005.08100)) See [examples/conformer](./examples/conformer) -
-**ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/
-abs/2005.03191)) See [examples/contextnet](./examples/contextnet) - **RNN
-Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/
-abs/1811.06621)) See [examples/rnn_transducer](./examples/rnn_transducer) -
-**Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://
-arxiv.org/abs/1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) -
-**Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/
-abs/1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
+abs/2005.08100)) See [examples/models/transducer/conformer](./examples/models/
+transducer/conformer) - **ContextNet** (Reference: [http://arxiv.org/abs/
+2005.03191](http://arxiv.org/abs/2005.03191)) See [examples/models/transducer/
+contextnet](./examples/models/transducer/contextnet) - **RNN Transducer**
+(Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/
+1811.06621)) See [examples/models/transducer/rnnt](./examples/models/
+transducer/rnnt) - **Deep Speech 2** (Reference: [https://arxiv.org/abs/
+1512.02595](https://arxiv.org/abs/1512.02595)) See [examples/models/ctc/
+deepspeech2](./examples/models/ctc/deepspeech2) - **Jasper** (Reference:
+[https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288)) See
+[examples/models/ctc/jasper](./examples/models/ctc/jasper) ## Installation For
 training and testing, you should use `git clone` for installing necessary
 packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.) ### Installing
 from source (recommended) ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR # Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3
 install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda create
 -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes
 sure conda install all dependencies for tensorflow conda activate tfasr pip
@@ -61,47 +64,37 @@
 Installing for development ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR pip3 install -e ".[dev]" pip3 install -e ".
 [tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine ``` ###
 Install for Apple Sillicon Due to tensorflow-text is not built for Apple
 Sillicon, we need to install it with the prebuilt wheel file from
 [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon]
 (https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-
-Apple-Silicon) Do this after installing TensorFlowASR with tensorflow above
-```bash TF_VERSION="$(python3 -c 'import tensorflow; print
-(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -
-d'.' -f1,2)" && \ URL="https://github.com/sun1638650145/Libraries-and-
+Apple-Silicon) ```bash git clone https://github.com/TensorSpeech/
+TensorFlowASR.git cd TensorFlowASR pip3 install -e "." # or pip3 install -e ".
+[dev] for development # or pip3 install "TensorFlowASR[dev]" from PyPi pip3
+install tensorflow~=2.14.0 # change minor version if you want ``` Do this after
+installing TensorFlowASR with tensorflow above ```bash TF_VERSION="$(python3 -
+c 'import tensorflow; print(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$
+(echo $TF_VERSION | cut -d'.' -f1,2)" && \ PY_VERSION="$(python3 -c 'import
+platform; major, minor, patch = platform.python_version_tuple(); print(f"
+{major}{minor}");')" && \ URL="https://github.com/sun1638650145/Libraries-and-
 Extensions-for-TensorFlow-for-Apple-Silicon" && \ pip3 install "${URL}/
 releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-
-cp310-cp310-macosx_11_0_arm64.whl" ``` ### Running in a container ```bash
-docker-compose up -d ``` ## Training & Testing Tutorial - For training, please
-read [tutorial_training](./docs/1_tutorial_training.md) - For testing, please
-read [tutorial_testing](./docs/2_tutorial_testing.md) **FYI**: Keras builtin
-training uses **infinite dataset**, which avoids the potential last partial
-batch. See [examples](./examples/) for some predefined ASR models and results
-## Features Extraction See [features_extraction](./tensorflow_asr/featurizers/
-README.md) ## Augmentations See [augmentations](./tensorflow_asr/augmentations/
-README.md) ## TFLite Convertion After converting to tflite, the tflite model is
-like a function that transforms directly from an **audio signal** to **unicode
-code points**, then we can convert unicode points to string. 1. Install `tf-
-nightly` using `pip install tf-nightly` 2. Build a model with the same
-architecture as the trained model _(if model has tflite argument, you must set
-it to True)_, then load the weights from trained model to the built model 3.
-Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function
-`add_featurizers` 4. Convert model's function to tflite as follows: ```python
-func = model.make_tflite_function(**options) # options are the arguments of the
-function concrete_func = func.get_concrete_function() converter =
-tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
-converter.experimental_new_converter = True converter.optimizations =
-[tf.lite.Optimize.DEFAULT] converter.target_spec.supported_ops =
-[tf.lite.OpsSet.TFLITE_BUILTINS, tf.lite.OpsSet.SELECT_TF_OPS] tflite_model =
-converter.convert() ``` 5. Save the converted tflite model as follows:
-```python if not os.path.exists(os.path.dirname(tflite_path)): os.makedirs
-(os.path.dirname(tflite_path)) with open(tflite_path, "wb") as tflite_out:
-tflite_out.write(tflite_model) ``` 5. Then the `.tflite` model is ready to be
-deployed ## Pretrained Models Go to [drive](https://drive.google.com/drive/
+cp${PY_VERSION}-cp${PY_VERSION}-macosx_11_0_arm64.whl" ``` ### Running in a
+container ```bash docker-compose up -d ``` ## Training & Testing Tutorial - For
+training, please read [tutorial_training](./docs/tutorials/training.md) - For
+testing, please read [tutorial_testing](./docs/tutorials/testing.md) **FYI**:
+Keras builtin training uses **infinite dataset**, which avoids the potential
+last partial batch. See [examples](./examples/) for some predefined ASR models
+and results ## Features Extraction See [features_extraction](./tensorflow_asr/
+featurizers/README.md) ## Augmentations See [augmentations](./tensorflow_asr/
+augmentations/README.md) ## TFLite Convertion After converting to tflite, the
+tflite model is like a function that transforms directly from an **audio
+signal** to **text and tokens** See [tflite_convertion](./docs/tutorials/
+tflite.md) ## Pretrained Models Go to [drive](https://drive.google.com/drive/
 folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing) ## Corpus Sources ###
 English | **Name** | **Source** | **Hours** | | :----------- | :---------------
 -------------------------------------------------- | :-------- | | LibriSpeech
 | [LibriSpeech](http://www.openslr.org/12) | 970h | | Common Voice | [https://
 commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h | ###
 Vietnamese | **Name** | **Source** | **Hours** | | :---------------------------
 ---------- | :-----------------------------------------------------------------
```

### Comparing `TensorFlowASR-2.0.0/README.md` & `TensorFlowASR-2.0.1/TensorFlowASR.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,50 @@
+Metadata-Version: 2.1
+Name: TensorFlowASR
+Version: 2.0.1
+Summary: Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2
+Home-page: https://github.com/TensorSpeech/TensorFlowASR
+Author: Huy Le Nguyen
+Author-email: nlhuy.cs.16@gmail.com
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tf2-12
+Provides-Extra: tf2-12-gpu
+Provides-Extra: tf2-13
+Provides-Extra: tf2-13-gpu
+Provides-Extra: tf2-14
+Provides-Extra: tf2-14-gpu
+Provides-Extra: tf2-15
+Provides-Extra: tf2-15-gpu
+License-File: LICENSE
+
 <h1 align="center">
-<p>TensorFlowASR :zap:</p>
+TensorFlowASR :zap:
+</h1>
 <p align="center">
 <a href="https://github.com/TensorSpeech/TensorFlowASR/blob/main/LICENSE">
   <img alt="GitHub" src="https://img.shields.io/github/license/TensorSpeech/TensorFlowASR?logo=apache&logoColor=green">
 </a>
-<img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.6-blue?logo=python">
+<img alt="python" src="https://img.shields.io/badge/python-%3E%3D3.8-blue?logo=python">
 <img alt="tensorflow" src="https://img.shields.io/badge/tensorflow-%3E%3D2.12.0-orange?logo=tensorflow">
 <a href="https://pypi.org/project/TensorFlowASR/">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/TensorFlowASR?color=%234285F4&label=release&logo=pypi&logoColor=%234285F4">
 </a>
 </p>
-</h1>
 <h2 align="center">
-<p>Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2</p>
+Almost State-of-the-art Automatic Speech Recognition in Tensorflow 2
 </h2>
 
 <p align="center">
 TensorFlowASR implements some automatic speech recognition architectures such as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These models can be converted to TFLite to reduce memory and computation for deployment :smile:
 </p>
 
 ## What's New?
@@ -56,23 +84,23 @@
 
 - **Transducer Models** (End2end models using RNNT Loss for training, currently supported Conformer, ContextNet, Streaming Transducer)
 - **CTCModel** (End2end models using CTC Loss for training, currently supported DeepSpeech2, Jasper)
 
 ### Publications
 
 - **Conformer Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/abs/2005.08100))
-  See [examples/conformer](./examples/conformer)
+  See [examples/models/transducer/conformer](./examples/models/transducer/conformer)
 - **ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/abs/2005.03191))
-  See [examples/contextnet](./examples/contextnet)
+  See [examples/models/transducer/contextnet](./examples/models/transducer/contextnet)
 - **RNN Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/1811.06621))
-  See [examples/rnn_transducer](./examples/rnn_transducer)
+  See [examples/models/transducer/rnnt](./examples/models/transducer/rnnt)
 - **Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://arxiv.org/abs/1512.02595))
-  See [examples/deepspeech2](./examples/deepspeech2)
+  See [examples/models/ctc/deepspeech2](./examples/models/ctc/deepspeech2)
 - **Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288))
-  See [examples/jasper](./examples/jasper)
+  See [examples/models/ctc/jasper](./examples/models/ctc/jasper)
 
 ## Installation
 
 For training and testing, you should use `git clone` for installing necessary packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.)
 
 ### Installing from source (recommended)
 
@@ -111,35 +139,43 @@
 pip3 install -e ".[tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine
 ```
 
 ### Install for Apple Sillicon
 
 Due to tensorflow-text is not built for Apple Sillicon, we need to install it with the prebuilt wheel file from [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon](https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon)
 
+```bash
+git clone https://github.com/TensorSpeech/TensorFlowASR.git
+cd TensorFlowASR
+pip3 install -e "." # or pip3 install -e ".[dev] for development # or pip3 install "TensorFlowASR[dev]" from PyPi
+pip3 install tensorflow~=2.14.0 # change minor version if you want
+```
+
 Do this after installing TensorFlowASR with tensorflow above
 
 ```bash
 TF_VERSION="$(python3 -c 'import tensorflow; print(tensorflow.__version__)')" && \
 TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -d'.' -f1,2)" && \
+PY_VERSION="$(python3 -c 'import platform; major, minor, patch = platform.python_version_tuple(); print(f"{major}{minor}");')" && \
 URL="https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon" && \
-pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp310-cp310-macosx_11_0_arm64.whl"
+pip3 install "${URL}/releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-cp${PY_VERSION}-cp${PY_VERSION}-macosx_11_0_arm64.whl"
 ```
 
 ### Running in a container
 
 ```bash
 docker-compose up -d
 ```
 
 
 
 ## Training & Testing Tutorial
 
-- For training, please read [tutorial_training](./docs/1_tutorial_training.md)
-- For testing, please read [tutorial_testing](./docs/2_tutorial_testing.md)
+- For training, please read [tutorial_training](./docs/tutorials/training.md)
+- For testing, please read [tutorial_testing](./docs/tutorials/testing.md)
 
 **FYI**: Keras builtin training uses **infinite dataset**, which avoids the potential last partial batch.
 
 See [examples](./examples/) for some predefined ASR models and results
 
 ## Features Extraction
 
@@ -147,42 +183,17 @@
 
 ## Augmentations
 
 See [augmentations](./tensorflow_asr/augmentations/README.md)
 
 ## TFLite Convertion
 
-After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **unicode code points**, then we can convert unicode points to string.
-
-1. Install `tf-nightly` using `pip install tf-nightly`
-2. Build a model with the same architecture as the trained model _(if model has tflite argument, you must set it to True)_, then load the weights from trained model to the built model
-3. Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function `add_featurizers`
-4. Convert model's function to tflite as follows:
-
-```python
-func = model.make_tflite_function(**options) # options are the arguments of the function
-concrete_func = func.get_concrete_function()
-converter = tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
-converter.experimental_new_converter = True
-converter.optimizations = [tf.lite.Optimize.DEFAULT]
-converter.target_spec.supported_ops = [tf.lite.OpsSet.TFLITE_BUILTINS,
-                                       tf.lite.OpsSet.SELECT_TF_OPS]
-tflite_model = converter.convert()
-```
-
-5. Save the converted tflite model as follows:
-
-```python
-if not os.path.exists(os.path.dirname(tflite_path)):
-    os.makedirs(os.path.dirname(tflite_path))
-with open(tflite_path, "wb") as tflite_out:
-    tflite_out.write(tflite_model)
-```
+After converting to tflite, the tflite model is like a function that transforms directly from an **audio signal** to **text and tokens**
 
-5. Then the `.tflite` model is ready to be deployed
+See [tflite_convertion](./docs/tutorials/tflite.md)
 
 ## Pretrained Models
 
 Go to [drive](https://drive.google.com/drive/folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing)
 
 ## Corpus Sources
```

#### html2text {}

```diff
@@ -1,8 +1,23 @@
-      ************ TTeennssoorrFFlloowwAASSRR ::zzaapp::_[[_GG_ii_tt_HH_uu_bb_]][[ppyytthhoonn]][[tteennssoorrffllooww]]_[[_PP_yy_PP_II_]] ************
+Metadata-Version: 2.1 Name: TensorFlowASR Version: 2.0.1 Summary: Almost State-
+of-the-art Automatic Speech Recognition using Tensorflow 2 Home-page: https://
+github.com/TensorSpeech/TensorFlowASR Author: Huy Le Nguyen Author-email:
+nlhuy.cs.16@gmail.com Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Intended Audience :: Science/Research Classifier: Operating System
+:: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: tf2-12 Provides-Extra: tf2-12-gpu Provides-
+Extra: tf2-13 Provides-Extra: tf2-13-gpu Provides-Extra: tf2-14 Provides-Extra:
+tf2-14-gpu Provides-Extra: tf2-15 Provides-Extra: tf2-15-gpu License-File:
+LICENSE
+                       ************ TTeennssoorrFFlloowwAASSRR ::zzaapp:: ************
+                      _[_G_i_t_H_u_b_][python][tensorflow]_[_P_y_P_I_]
   ********** AAllmmoosstt SSttaattee--ooff--tthhee--aarrtt AAuuttoommaattiicc SSppeeeecchh RReeccooggnniittiioonn iinn TTeennssoorrffllooww 22
                                      **********
  TensorFlowASR implements some automatic speech recognition architectures such
    as DeepSpeech2, Jasper, RNN Transducer, ContextNet, Conformer, etc. These
     models can be converted to TFLite to reduce memory and computation for
                               deployment :smile:
 ## What's New? ## Table of Contents - [What's New?](#whats-new) - [Table of
@@ -19,23 +34,25 @@
 [Vietnamese](#vietnamese) - [How to contribute](#how-to-contribute) -
 [References \& Credits](#references--credits) - [Contact](#contact) ## :yum:
 Supported Models ### Baselines - **Transducer Models** (End2end models using
 RNNT Loss for training, currently supported Conformer, ContextNet, Streaming
 Transducer) - **CTCModel** (End2end models using CTC Loss for training,
 currently supported DeepSpeech2, Jasper) ### Publications - **Conformer
 Transducer** (Reference: [https://arxiv.org/abs/2005.08100](https://arxiv.org/
-abs/2005.08100)) See [examples/conformer](./examples/conformer) -
-**ContextNet** (Reference: [http://arxiv.org/abs/2005.03191](http://arxiv.org/
-abs/2005.03191)) See [examples/contextnet](./examples/contextnet) - **RNN
-Transducer** (Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/
-abs/1811.06621)) See [examples/rnn_transducer](./examples/rnn_transducer) -
-**Deep Speech 2** (Reference: [https://arxiv.org/abs/1512.02595](https://
-arxiv.org/abs/1512.02595)) See [examples/deepspeech2](./examples/deepspeech2) -
-**Jasper** (Reference: [https://arxiv.org/abs/1904.03288](https://arxiv.org/
-abs/1904.03288)) See [examples/jasper](./examples/jasper) ## Installation For
+abs/2005.08100)) See [examples/models/transducer/conformer](./examples/models/
+transducer/conformer) - **ContextNet** (Reference: [http://arxiv.org/abs/
+2005.03191](http://arxiv.org/abs/2005.03191)) See [examples/models/transducer/
+contextnet](./examples/models/transducer/contextnet) - **RNN Transducer**
+(Reference: [https://arxiv.org/abs/1811.06621](https://arxiv.org/abs/
+1811.06621)) See [examples/models/transducer/rnnt](./examples/models/
+transducer/rnnt) - **Deep Speech 2** (Reference: [https://arxiv.org/abs/
+1512.02595](https://arxiv.org/abs/1512.02595)) See [examples/models/ctc/
+deepspeech2](./examples/models/ctc/deepspeech2) - **Jasper** (Reference:
+[https://arxiv.org/abs/1904.03288](https://arxiv.org/abs/1904.03288)) See
+[examples/models/ctc/jasper](./examples/models/ctc/jasper) ## Installation For
 training and testing, you should use `git clone` for installing necessary
 packages from other authors (`ctc_decoders`, `rnnt_loss`, etc.) ### Installing
 from source (recommended) ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR # Tensorflow 2.x (with 2.x.x >= 2.5.1) pip3
 install ".[tf2.x]" # or ".[tf2.x-gpu]" ``` For anaconda3: ```bash conda create
 -y -n tfasr tensorflow-gpu python=3.8 # tensorflow if using CPU, this makes
 sure conda install all dependencies for tensorflow conda activate tfasr pip
@@ -47,47 +64,37 @@
 Installing for development ```bash git clone https://github.com/TensorSpeech/
 TensorFlowASR.git cd TensorFlowASR pip3 install -e ".[dev]" pip3 install -e ".
 [tf2.x]" # or ".[tf2.x-gpu]" or ".[tf2.x-apple]" for apple m1 machine ``` ###
 Install for Apple Sillicon Due to tensorflow-text is not built for Apple
 Sillicon, we need to install it with the prebuilt wheel file from
 [sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon]
 (https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-
-Apple-Silicon) Do this after installing TensorFlowASR with tensorflow above
-```bash TF_VERSION="$(python3 -c 'import tensorflow; print
-(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$(echo $TF_VERSION | cut -
-d'.' -f1,2)" && \ URL="https://github.com/sun1638650145/Libraries-and-
+Apple-Silicon) ```bash git clone https://github.com/TensorSpeech/
+TensorFlowASR.git cd TensorFlowASR pip3 install -e "." # or pip3 install -e ".
+[dev] for development # or pip3 install "TensorFlowASR[dev]" from PyPi pip3
+install tensorflow~=2.14.0 # change minor version if you want ``` Do this after
+installing TensorFlowASR with tensorflow above ```bash TF_VERSION="$(python3 -
+c 'import tensorflow; print(tensorflow.__version__)')" && \ TF_VERSION_MAJOR="$
+(echo $TF_VERSION | cut -d'.' -f1,2)" && \ PY_VERSION="$(python3 -c 'import
+platform; major, minor, patch = platform.python_version_tuple(); print(f"
+{major}{minor}");')" && \ URL="https://github.com/sun1638650145/Libraries-and-
 Extensions-for-TensorFlow-for-Apple-Silicon" && \ pip3 install "${URL}/
 releases/download/v${TF_VERSION_MAJOR}/tensorflow_text-${TF_VERSION_MAJOR}.0-
-cp310-cp310-macosx_11_0_arm64.whl" ``` ### Running in a container ```bash
-docker-compose up -d ``` ## Training & Testing Tutorial - For training, please
-read [tutorial_training](./docs/1_tutorial_training.md) - For testing, please
-read [tutorial_testing](./docs/2_tutorial_testing.md) **FYI**: Keras builtin
-training uses **infinite dataset**, which avoids the potential last partial
-batch. See [examples](./examples/) for some predefined ASR models and results
-## Features Extraction See [features_extraction](./tensorflow_asr/featurizers/
-README.md) ## Augmentations See [augmentations](./tensorflow_asr/augmentations/
-README.md) ## TFLite Convertion After converting to tflite, the tflite model is
-like a function that transforms directly from an **audio signal** to **unicode
-code points**, then we can convert unicode points to string. 1. Install `tf-
-nightly` using `pip install tf-nightly` 2. Build a model with the same
-architecture as the trained model _(if model has tflite argument, you must set
-it to True)_, then load the weights from trained model to the built model 3.
-Load `TFSpeechFeaturizer` and `TextFeaturizer` to model using function
-`add_featurizers` 4. Convert model's function to tflite as follows: ```python
-func = model.make_tflite_function(**options) # options are the arguments of the
-function concrete_func = func.get_concrete_function() converter =
-tf.lite.TFLiteConverter.from_concrete_functions([concrete_func])
-converter.experimental_new_converter = True converter.optimizations =
-[tf.lite.Optimize.DEFAULT] converter.target_spec.supported_ops =
-[tf.lite.OpsSet.TFLITE_BUILTINS, tf.lite.OpsSet.SELECT_TF_OPS] tflite_model =
-converter.convert() ``` 5. Save the converted tflite model as follows:
-```python if not os.path.exists(os.path.dirname(tflite_path)): os.makedirs
-(os.path.dirname(tflite_path)) with open(tflite_path, "wb") as tflite_out:
-tflite_out.write(tflite_model) ``` 5. Then the `.tflite` model is ready to be
-deployed ## Pretrained Models Go to [drive](https://drive.google.com/drive/
+cp${PY_VERSION}-cp${PY_VERSION}-macosx_11_0_arm64.whl" ``` ### Running in a
+container ```bash docker-compose up -d ``` ## Training & Testing Tutorial - For
+training, please read [tutorial_training](./docs/tutorials/training.md) - For
+testing, please read [tutorial_testing](./docs/tutorials/testing.md) **FYI**:
+Keras builtin training uses **infinite dataset**, which avoids the potential
+last partial batch. See [examples](./examples/) for some predefined ASR models
+and results ## Features Extraction See [features_extraction](./tensorflow_asr/
+featurizers/README.md) ## Augmentations See [augmentations](./tensorflow_asr/
+augmentations/README.md) ## TFLite Convertion After converting to tflite, the
+tflite model is like a function that transforms directly from an **audio
+signal** to **text and tokens** See [tflite_convertion](./docs/tutorials/
+tflite.md) ## Pretrained Models Go to [drive](https://drive.google.com/drive/
 folders/1BD0AK30n8hc-yR28C5FW3LqzZxtLOQfl?usp=sharing) ## Corpus Sources ###
 English | **Name** | **Source** | **Hours** | | :----------- | :---------------
 -------------------------------------------------- | :-------- | | LibriSpeech
 | [LibriSpeech](http://www.openslr.org/12) | 970h | | Common Voice | [https://
 commonvoice.mozilla.org](https://commonvoice.mozilla.org) | 1932h | ###
 Vietnamese | **Name** | **Source** | **Hours** | | :---------------------------
 ---------- | :-----------------------------------------------------------------
```

### Comparing `TensorFlowASR-2.0.0/TensorFlowASR.egg-info/SOURCES.txt` & `TensorFlowASR-2.0.1/TensorFlowASR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/TensorFlowASR.egg-info/requires.txt` & `TensorFlowASR-2.0.1/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,49 +4,48 @@
 tqdm~=4.66.3
 librosa~=0.10.1
 PyYAML~=6.0.1
 sounddevice~=0.4.6
 jinja2~=3.1.3
 fire~=0.5.0
 jiwer~=3.0.3
-chardet~=5.1.0
-charset-normalizer~=2.1.1
 
-[dev]
+# extra=dev
 pytest~=7.4.1
 black~=24.3.0
-pylint~=3.1.0
+pylint~=3.2.1
 matplotlib~=3.7.2
 pydot~=1.4.2
 graphviz~=0.20.1
+pre-commit~=3.7.0
 
-[tf2-12]
+# extra=tf2-12
 tensorflow~=2.12.0
 tensorflow-text~=2.12.0
 
-[tf2-12-gpu]
+# extra=tf2-12-gpu
 tensorflow[and-cuda]~=2.12.0
 tensorflow-text~=2.12.0
 
-[tf2-13]
+# extra=tf2-13
 tensorflow~=2.13.0
 tensorflow-text~=2.13.0rc0
 
-[tf2-13-gpu]
+# extra=tf2-13-gpu
 tensorflow[and-cuda]~=2.13.0
 tensorflow-text~=2.13.0rc0
 
-[tf2-14]
+# extra=tf2-14
 tensorflow~=2.14.0
 tensorflow-text~=2.14.0
 
-[tf2-14-gpu]
+# extra=tf2-14-gpu
 tensorflow[and-cuda]~=2.14.0
 tensorflow-text~=2.14.0
 
-[tf2-15]
+# extra=tf2-15
 tensorflow~=2.15.0
 tensorflow-text~=2.15.0
 
-[tf2-15-gpu]
+# extra=tf2-15-gpu
 tensorflow[and-cuda]~=2.15.0
-tensorflow-text~=2.15.0
+tensorflow-text~=2.15.0
```

### Comparing `TensorFlowASR-2.0.0/setup.py` & `TensorFlowASR-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="TensorFlowASR",
-    version="2.0.0",
+    version="2.0.1",
     author="Huy Le Nguyen",
     author_email="nlhuy.cs.16@gmail.com",
     description="Almost State-of-the-art Automatic Speech Recognition using Tensorflow 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TensorSpeech/TensorFlowASR",
     packages=find_packages(include=("tensorflow_asr", "tensorflow_asr.*")),
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/__init__.py` & `TensorFlowASR-2.0.1/tensorflow_asr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import warnings
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = os.environ.get("TF_CPP_MIN_LOG_LEVEL", "2")
 os.environ["TF_FORCE_GPU_ALLOW_GROWTH"] = os.environ.get("TF_FORCE_GPU_ALLOW_GROWTH", "true")
 
 import tensorflow as tf
+import keras
 from tensorflow.python.util import deprecation  # pylint: disable = no-name-in-module
 
 # might cause performance penalty if ops fallback to cpu, see https://cloud.google.com/tpu/docs/tensorflow-ops
 tf.config.set_soft_device_placement(False)
 deprecation._PRINT_DEPRECATION_WARNINGS = False  # comment this line to print deprecation warnings
 
 logger = tf.get_logger()
@@ -42,15 +43,15 @@
 
 
 def match_dtype_and_rank(y_t, y_p, sw):
     return y_t, y_p, sw
 
 
 # monkey patch
-tf.keras.layers.Layer.output_shape = output_shape
-tf.keras.layers.Layer.build = build
-tf.keras.layers.Layer.compute_output_shape = compute_output_shape
+keras.layers.Layer.output_shape = output_shape
+keras.layers.Layer.build = build
+keras.layers.Layer.compute_output_shape = compute_output_shape
 compile_utils.match_dtype_and_rank = match_dtype_and_rank
 
 import tensorflow_asr.callbacks
 from tensorflow_asr.models import *
 from tensorflow_asr.optimizers import *
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/augmentations/augmentation.py` & `TensorFlowASR-2.0.1/tensorflow_asr/augmentations/augmentation.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/base_method.py` & `TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/base_method.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/gaussnoise.py` & `TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/gaussnoise.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/augmentations/methods/specaugment.py` & `TensorFlowASR-2.0.1/tensorflow_asr/augmentations/methods/specaugment.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/callbacks.py` & `TensorFlowASR-2.0.1/tensorflow_asr/callbacks.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/configs.py` & `TensorFlowASR-2.0.1/tensorflow_asr/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             config = {}
         self.name: str = config.pop("name", "")
         self.enabled: bool = config.pop("enabled", True)
         self.stage: str = config.pop("stage", None)
         self.data_paths = config.pop("data_paths", None)
         self.tfrecords_dir: str = config.pop("tfrecords_dir", None)
         self.tfrecords_shards: int = config.pop("tfrecords_shards", 16)
+        self.tfrecords_buffer_size: int = config.pop("tfrecords_buffer_size", 32 * 1024 * 1024)
         self.shuffle: bool = config.pop("shuffle", False)
         self.cache: bool = config.pop("cache", False)
         self.drop_remainder: bool = config.pop("drop_remainder", True)
         self.buffer_size: int = config.pop("buffer_size", 1000)
         self.metadata: str = config.pop("metadata", None)
         self.sample_rate: int = config.pop("sample_rate", 16000)
         for k, v in config.items():
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/datasets.py` & `TensorFlowASR-2.0.1/tensorflow_asr/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 # _Note_: To create transcripts for **librispeech**, see [create_librispeech_trans.py](../../scripts/create_librispeech_trans.py)
 
 # ## ASR Datasets
 
 # An ASR dataset is some `.tsv` files in format: `PATH\tDURATION\tTRANSCRIPT`. You must create those files by your own with your own data and methods.
 
-# **Note**: Each `.tsv` file must include a header `PATH\tDURATION\tTRANSCRIPT` because it will remove these headers when loading dataset, otherwise you will lose 1 data file :sob:
+# **Note**: Each `.tsv` file must include a header `PATH\tDURATION\tTRANSCRIPT`
+# because it will remove these headers when loading dataset, otherwise you will lose 1 data file :sob:
 
-# **For transcript**, if you want to include characters such as dots, commas, double quote, etc.. you must create your own `.txt` vocabulary file. Default is [English](../featurizers/english.txt)
+# **For transcript**, if you want to include characters such as dots, commas, double quote, etc.. you must create your own `.txt` vocabulary file.
+# Default is [English](../featurizers/english.txt)
 
 # **Inputs**
 
 # ```python
 # class ASRTFRecordDataset(ASRDataset):
 #     """ Dataset for ASR using TFRecords """
 
@@ -137,16 +139,17 @@
         prediction_shape=prediction_shape,
         label_shape=label_shape,
         padded_shapes=padded_shapes,
     )
 
 
 BUFFER_SIZE = 100
+TFRECORD_BUFFER_SIZE = 32 * 1024 * 1024
 TFRECORD_SHARDS = 16
-AUTOTUNE = int(os.environ.get("AUTOTUNE") or tf.data.experimental.AUTOTUNE)
+AUTOTUNE = int(os.environ.get("AUTOTUNE") or tf.data.AUTOTUNE)
 
 
 class BaseDataset:
     """Based dataset for all models"""
 
     def __init__(
         self,
@@ -412,14 +415,15 @@
         cache: bool = False,
         shuffle: bool = False,
         enabled: bool = True,
         metadata: str = None,
         indefinite: bool = True,
         drop_remainder: bool = True,
         buffer_size: int = BUFFER_SIZE,
+        tfrecords_buffer_size: int = TFRECORD_BUFFER_SIZE,
         compression_type: str = "GZIP",
         sample_rate: int = 16000,
         name: str = "",
         **kwargs,
     ):
         super().__init__(
             stage=stage,
@@ -438,14 +442,15 @@
         )
         if not self.stage:
             raise ValueError("stage must be defined, either 'train', 'eval' or 'test'")
         self.tfrecords_dir = tfrecords_dir
         if tfrecords_shards <= 0:
             raise ValueError("tfrecords_shards must be positive")
         self.tfrecords_shards = tfrecords_shards
+        self.tfrecords_buffer_size = tfrecords_buffer_size
         self.compression_type = compression_type
 
     def write_tfrecord_file(self, splitted_entries: tuple):
         shard_path, entries = splitted_entries
         logger.info(f"Processing {shard_path} ...")
         with tf.io.TFRecordWriter(shard_path, options=tf.io.TFRecordOptions(compression_type=self.compression_type)) as writer:
             for path, _, transcript in entries:
@@ -502,15 +507,17 @@
             return None
 
         pattern = os.path.join(self.tfrecords_dir, f"{self.stage}*.tfrecord")
         files_ds = tf.data.Dataset.list_files(pattern, shuffle=self.shuffle)
         ignore_order = tf.data.Options()
         ignore_order.deterministic = False
         files_ds = files_ds.with_options(ignore_order)
-        dataset = tf.data.TFRecordDataset(files_ds, compression_type=self.compression_type, num_parallel_reads=AUTOTUNE)
+        dataset = tf.data.TFRecordDataset(
+            files_ds, compression_type=self.compression_type, buffer_size=self.tfrecords_buffer_size, num_parallel_reads=AUTOTUNE
+        )
 
         return self.process(dataset, batch_size, padded_shapes=padded_shapes)
 
 
 class ASRSliceDataset(ASRDataset):
     """Dataset for ASR using Slice"""
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/features/gammatone.py` & `TensorFlowASR-2.0.1/tensorflow_asr/features/gammatone.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/losses/ctc_loss.py` & `TensorFlowASR-2.0.1/tensorflow_asr/losses/ctc_loss.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/losses/rnnt_loss.py` & `TensorFlowASR-2.0.1/tensorflow_asr/losses/rnnt_loss.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/metrics/error_rates.py` & `TensorFlowASR-2.0.1/tensorflow_asr/metrics/error_rates.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/activations/glu.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/activations/glu.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/base_layer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/base_layer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/base_model.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         """
         assert batch_size is not None and batch_size > 0
         signals = tf.keras.Input(shape=input_shape, batch_size=batch_size, dtype=tf.float32)
         signals_length = tf.keras.Input(shape=[], batch_size=batch_size, dtype=tf.int32)
         predictions = tf.keras.Input(shape=prediction_shape, batch_size=batch_size, dtype=tf.int32)
         predictions_length = tf.keras.Input(shape=[], batch_size=batch_size, dtype=tf.int32)
         self._per_replica_batch_size = int(batch_size / self.distribute_strategy.num_replicas_in_sync)
+        self._batch_size = batch_size
         outputs = self(
             schemas.TrainInput(
                 inputs=signals,
                 inputs_length=signals_length,
                 predictions=predictions,
                 predictions_length=predictions_length,
                 caching=caching,
@@ -273,15 +274,21 @@
                 self._test_step(per_ga_step_data)
         metrics = self.get_metrics_result()
         metrics = tf.nest.map_structure(lambda x: x / self.distribute_strategy.num_replicas_in_sync, metrics)
         return metrics
 
     def predict_step(self, data):
         x, y_true = data
-        inputs = schemas.PredictInput(x["inputs"], x["inputs_length"])
+        inputs = schemas.PredictInput(
+            inputs=x["inputs"],
+            inputs_length=x["inputs_length"],
+            previous_tokens=self.get_initial_tokens(),
+            previous_encoder_states=self.get_initial_encoder_states(),
+            previous_decoder_states=self.get_initial_decoder_states(),
+        )
         _tokens = self.recognize(inputs=inputs).tokens
         _beam_tokens = self.recognize_beam(inputs=inputs).tokens
         return {
             "_tokens": _tokens,
             "_beam_tokens": _beam_tokens,
             "_labels": y_true["labels"],
         }
@@ -615,45 +622,56 @@
             if getattr(self, "_eval_data_handler", None) is not None:
                 del self._eval_data_handler
             callbacks.on_train_end(logs=training_logs)
             return self.history
 
     # -------------------------------- INFERENCE FUNCTIONS -------------------------------------
 
+    def get_initial_tokens(self, batch_size=1):
+        return tf.ones([batch_size, 1], dtype=tf.int32) * self.blank
+
+    def get_initial_encoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
+
+    def get_initial_decoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
+
     def recognize(self, inputs: schemas.PredictInput, **kwargs) -> schemas.PredictOutput:
         """Greedy decoding function that used in self.predict_step"""
         raise NotImplementedError()
 
-    def recognize_beam(self, inputs: schemas.PredictInput, **kwargs) -> schemas.PredictOutput:
+    def recognize_beam(self, inputs: schemas.PredictInput, beam_width: int = 10, **kwargs) -> schemas.PredictOutput:
         """Beam search decoding function that used in self.predict_step"""
         raise NotImplementedError()
 
     # ---------------------------------- TFLITE ---------------------------------- #
 
-    def make_tflite_function(self, batch_size=1):
-        @tf.function(
-            input_signature=[
-                tf.TensorSpec([batch_size, None], dtype=tf.float32),
-                tf.TensorSpec([batch_size], dtype=tf.int32),
-                tf.TensorSpec([batch_size, 1], dtype=tf.int32),
-                tf.TensorSpec(self.encoder.get_initial_state(batch_size), dtype=tf.float32) if hasattr(self.encoder, "get_initial_state") else None,
-                tf.TensorSpec(self.predict_net.get_initial_state(batch_size).get_shape(), dtype=tf.float32),
-            ],
-        )
-        def tflite_func(inputs, inputs_length, previous_tokens, previous_encoder_states, previous_decoder_states):
-            outputs = self.recognize(
-                schemas.PredictInput(
-                    inputs=inputs,
-                    inputs_length=inputs_length,
-                    previous_tokens=previous_tokens,
-                    previous_encoder_states=previous_encoder_states,
-                    previous_decoder_states=previous_decoder_states,
-                )
-            )
-            return schemas.PredictOutput(
-                tokens=self.tokenizer.detokenize_unicode_points(outputs.tokens),
-                scores=outputs.scores,
-                encoder_states=outputs.encoder_states,
-                decoder_states=outputs.decoder_states,
+    def make_tflite_function(self, batch_size: int = 1, beam_width: int = 0):
+
+        def tflite_func(inputs: schemas.PredictInput):
+            if beam_width > 0:
+                outputs = self.recognize_beam(inputs, beam_width=beam_width)
+            else:
+                outputs = self.recognize(inputs)
+            return schemas.PredictOutputWithTranscript(
+                transcript=self.tokenizer.detokenize(outputs.tokens),
+                tokens=outputs.tokens,
+                next_tokens=outputs.next_tokens,
+                next_encoder_states=outputs.next_encoder_states,
+                next_decoder_states=outputs.next_decoder_states,
             )
 
-        return tflite_func
+        input_signature = schemas.PredictInput(
+            inputs=tf.TensorSpec([batch_size, None], dtype=tf.float32),
+            inputs_length=tf.TensorSpec([batch_size], dtype=tf.int32),
+            previous_tokens=tf.TensorSpec.from_tensor(self.get_initial_tokens(batch_size)),
+            previous_encoder_states=tf.TensorSpec.from_tensor(self.get_initial_encoder_states(batch_size)),
+            previous_decoder_states=tf.TensorSpec.from_tensor(self.get_initial_decoder_states(batch_size)),
+        )
+
+        return tf.function(
+            tflite_func,
+            input_signature=[input_signature],
+            jit_compile=True,
+            reduce_retracing=True,
+            autograph=True,
+        )
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/base_ctc.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/base_ctc.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,23 @@
         previous_encoder_states=None,
         previous_decoder_states=None,
     ):
         outputs, outputs_length, next_encoder_states = self.encoder.call_next(features, features_length, previous_encoder_states)
         outputs, outputs_length, next_decoder_states = self.decoder.call_next(outputs, outputs_length, previous_decoder_states)
         return outputs, outputs_length, next_encoder_states, next_decoder_states
 
+    def get_initial_tokens(self, batch_size=1):
+        return super().get_initial_tokens(batch_size)
+
+    def get_initial_encoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
+
+    def get_initial_decoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
+
     # -------------------------------- GREEDY -------------------------------------
 
     def recognize(self, inputs: schemas.PredictInput, **kwargs):
         with tf.name_scope(f"{self.name}_recognize"):
             features, features_length = self.feature_extraction((inputs.inputs, inputs.inputs_length), training=False)
             (
                 outputs,
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/conformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/conformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/deepspeech2.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/deepspeech2.py`

 * *Files 18% similar despite different names*

```diff
@@ -127,7 +127,13 @@
                 initializer=initializer,
                 name="decoder",
             ),
             name=name,
             **kwargs,
         )
         self.time_reduction_factor = self.encoder.time_reduction_factor
+
+    def get_initial_encoder_states(self, batch_size=1):
+        return self.encoder.get_initial_state(batch_size)
+
+    def get_initial_decoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/jasper.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/jasper.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/ctc/transformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/ctc/transformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/conformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/conformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/contextnet.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/contextnet.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/deepspeech2.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/subsampling.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,481 +10,317 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import tensorflow as tf
 
-from tensorflow_asr.models.base_layer import Identity, Layer, Reshape
-from tensorflow_asr.models.layers.convolution import DepthwiseConv1D
-from tensorflow_asr.utils import layer_util, math_util
+from tensorflow_asr.models.base_layer import Layer
+from tensorflow_asr.models.layers.convolution import Conv1D, Conv2D
+from tensorflow_asr.utils import math_util, shape_util
 
-# ----------------------------------- CONV ----------------------------------- #
 
+class TimeReduction(Layer):
+    def __init__(self, factor: int, name: str = "TimeReduction", **kwargs):
+        super().__init__(name=name, **kwargs)
+        self.time_reduction_factor = factor
 
-class RowConv1D(Layer):
-    def __init__(
-        self,
-        future_width=2,
-        activation="relu",
-        regularizer=None,
-        initializer=None,
-        **kwargs,
-    ):
-        assert future_width >= 0, "Future context must be positive"
-        super().__init__(**kwargs)
-        self.conv = DepthwiseConv1D(
-            kernel_size=future_width * 2 + 1,
-            strides=1,
-            padding="causal",
-            use_bias=False,
-            depthwise_regularizer=regularizer,
-            depthwise_initializer=initializer,
-            bias_regularizer=regularizer,
-            bias_initializer=initializer,
-            name="conv",
-            dtype=self.dtype,
-        )
-        self.bn = tf.keras.layers.BatchNormalization(
-            name="bn",
-            gamma_regularizer=regularizer,
-            beta_regularizer=regularizer,
-            dtype=self.dtype,
-        )
-        self.activation = tf.keras.activations.get(activation)
+    def padding(self, time):
+        new_time = tf.math.ceil(time / self.time_reduction_factor) * self.time_reduction_factor
+        return tf.cast(new_time, dtype=tf.int32) - time
 
-    def call(self, inputs, training=False):
-        outputs = self.conv(inputs, training=training)
-        outputs = self.bn(outputs, training=training)
-        outputs = self.activation(outputs)
-        return outputs
+    def call(self, inputs):
+        outputs, outputs_length = inputs
+        shape = shape_util.shape_list(outputs)
+        outputs = tf.pad(outputs, [[0, 0], [0, self.padding(shape[1])], [0, 0]])
+        outputs = tf.reshape(outputs, [shape[0], -1, shape[-1] * self.time_reduction_factor])
+        outputs_length = math_util.get_reduced_length(outputs_length, reduction_factor=self.time_reduction_factor)
+        return outputs, outputs_length
+
+    def compute_mask(self, inputs, mask=None):
+        outputs, outputs_length = inputs
+        maxlen = tf.shape(outputs)[1]
+        maxlen, outputs_length = (math_util.get_reduced_length(length, self.time_reduction_factor) for length in (maxlen, outputs_length))
+        mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
+        return mask, None
 
     def compute_output_shape(self, input_shape):
-        output_shape = self.conv.compute_output_shape(input_shape)
-        output_shape = self.bn.compute_output_shape(output_shape)
-        return output_shape
+        output_shape, output_length_shape = input_shape
+        reduced_time = math_util.legacy_get_reduced_length(output_shape[1], self.time_reduction_factor)
+        output_shape = output_shape[:1] + (reduced_time,) + output_shape[2:]
+        return output_shape, output_length_shape
 
 
-class ConvBlock(Layer):
+class VggSubsampling(Layer):
     def __init__(
         self,
-        conv_type: str = "conv2d",
-        kernels: list = [11, 41],
-        strides: list = [2, 2],
-        filters: int = 32,
-        padding: str = "causal",
+        filters: tuple or list = (32, 64),
+        kernel_size: int or list or tuple = 3,
+        pool_size: int or list or tuple = 2,
+        strides: int or list or tuple = 2,
+        padding: str = "same",
         activation: str = "relu",
-        dropout: float = 0.1,
         kernel_regularizer=None,
         bias_regularizer=None,
-        initializer=None,
+        name="VggSubsampling",
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.conv = layer_util.get_conv(conv_type)(
-            filters=filters,
-            kernel_size=kernels,
-            strides=strides,
+        super().__init__(name=name, **kwargs)
+        self.conv1 = Conv2D(
+            filters=filters[0],
+            kernel_size=kernel_size,
+            strides=1,
+            padding=padding,
+            name="conv_1",
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            activation=activation,
+            dtype=self.dtype,
+        )
+        self.conv2 = Conv2D(
+            filters=filters[0],
+            kernel_size=kernel_size,
+            strides=1,
             padding=padding,
-            name=conv_type,
+            name="conv_2",
             kernel_regularizer=kernel_regularizer,
-            kernel_initializer=initializer,
             bias_regularizer=bias_regularizer,
-            bias_initializer=initializer,
+            activation=activation,
             dtype=self.dtype,
         )
-        self.bn = tf.keras.layers.BatchNormalization(
-            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
+        self.maxpool1 = tf.keras.layers.MaxPool2D(pool_size=pool_size, strides=strides, padding=padding, dtype=self.dtype, name="maxpool_1")
+        self.conv3 = Conv2D(
+            filters=filters[1],
+            kernel_size=kernel_size,
+            strides=1,
+            padding=padding,
+            name="conv_3",
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            activation=activation,
+            dtype=self.dtype,
+        )
+        self.conv4 = Conv2D(
+            filters=filters[1],
+            kernel_size=kernel_size,
+            strides=1,
+            padding=padding,
+            name="conv_4",
+            kernel_regularizer=kernel_regularizer,
+            bias_regularizer=bias_regularizer,
+            activation=activation,
+            dtype=self.dtype,
         )
-        self.act = tf.keras.layers.Activation(activation=activation, dtype=self.dtype)
-        self.do = tf.keras.layers.Dropout(dropout, name="dropout", dtype=self.dtype)
-        self.time_reduction_factor = self.conv.strides[0]
+        self.maxpool2 = tf.keras.layers.MaxPool2D(pool_size=pool_size, strides=strides, padding=padding, dtype=self.dtype, name="maxpool_2")
+        self.time_reduction_factor = self.maxpool1.pool_size[0] * self.maxpool2.pool_size[0]
 
     def call(self, inputs, training=False):
         outputs, outputs_length = inputs
-        outputs = self.conv(outputs, training=training)
-        outputs = self.bn(outputs, training=training)
-        outputs = self.act(outputs, training=training)
-        outputs = self.do(outputs, training=training)
-        outputs_length = math_util.conv_output_length(
-            outputs_length, filter_size=self.conv.kernel_size[0], padding=self.conv.padding, stride=self.conv.strides[0]
-        )
+
+        outputs = self.conv1(outputs, training=training)
+        outputs = self.conv2(outputs, training=training)
+        outputs = self.maxpool1(outputs, training=training)
+
+        outputs = self.conv3(outputs, training=training)
+        outputs = self.conv4(outputs, training=training)
+        outputs = self.maxpool2(outputs, training=training)
+
+        outputs = math_util.merge_two_last_dims(outputs)
         return outputs, outputs_length
 
     def compute_mask(self, inputs, mask=None):
         outputs, outputs_length = inputs
         maxlen = tf.shape(outputs)[1]
-        maxlen, outputs_length = (
-            math_util.conv_output_length(length, filter_size=self.conv.kernel_size[0], padding=self.conv.padding, stride=self.conv.strides[0])
-            for length in (maxlen, outputs_length)
-        )
+        for pool in (self.maxpool1, self.maxpool2):
+            maxlen, outputs_length = (
+                math_util.conv_output_length(length, pool.pool_size[0], padding=pool.padding, stride=pool.strides[0])
+                for length in (maxlen, outputs_length)
+            )
         mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
         return mask, None
 
     def compute_output_shape(self, input_shape):
         output_shape, output_length_shape = input_shape
-        output_shape = self.conv.compute_output_shape(output_shape)
-        output_shape = self.bn.compute_output_shape(output_shape)
-        output_shape = self.act.compute_output_shape(output_shape)
-        output_shape = self.do.compute_output_shape(output_shape)
-        return output_shape, output_length_shape
+        outputs_shape = self.conv1.compute_output_shape(output_shape)
+        outputs_shape = self.conv2.compute_output_shape(outputs_shape)
+        outputs_shape = self.maxpool1.compute_output_shape(outputs_shape)
+        outputs_shape = self.conv3.compute_output_shape(outputs_shape)
+        outputs_shape = self.conv4.compute_output_shape(outputs_shape)
+        outputs_shape = self.maxpool2.compute_output_shape(outputs_shape)
+        outputs_shape = outputs_shape[:2] + (outputs_shape[2] * outputs_shape[3],)
+        return outputs_shape, output_length_shape
 
 
-class ConvModule(Layer):
+class Conv2dSubsampling(Layer):
     def __init__(
         self,
-        conv_type: str = "conv2d",
-        kernels: list = [[11, 41], [11, 21], [11, 21]],
-        strides: list = [[2, 2], [1, 2], [1, 2]],
-        filters: list = [32, 32, 96],
-        padding: str = "causal",
-        activation: str = "relu",
-        dropout: float = 0.1,
+        filters: list,
+        strides: list = [[2, 1], [2, 1]],
+        kernels: list = [[3, 3], [3, 3]],
+        paddings: list = ["causal", "causal"],
+        norms: list = ["none", "none"],
+        activations: list = ["relu", "relu"],
         kernel_regularizer=None,
         bias_regularizer=None,
-        initializer=None,
+        name="conv2d_subsampling",
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        assert conv_type in ("conv1d", "conv2d")
-        assert len(kernels) == len(strides) == len(filters)
-        assert dropout >= 0.0
-
-        self.pre = Reshape(name="preprocess", dtype=self.dtype) if conv_type == "conv1d" else Identity(name="iden", dtype=self.dtype)
-
+        super().__init__(name=name, **kwargs)
+        assert len(filters) == len(strides) == len(kernels) == len(paddings) == len(norms) == len(activations)
         self.convs = []
         self.time_reduction_factor = 1
         for i in range(len(filters)):
-            conv_block = ConvBlock(
-                conv_type=conv_type,
-                kernels=kernels[i],
-                strides=strides[i],
-                filters=filters[i],
-                dropout=dropout,
-                padding=padding,
-                activation=activation,
-                name=f"block_{i}",
-                kernel_regularizer=kernel_regularizer,
-                bias_regularizer=bias_regularizer,
-                initializer=initializer,
-                dtype=self.dtype,
+            subblock = tf.keras.Sequential(name=f"block_{i}")
+            subblock.add(
+                Conv2D(
+                    filters=filters[i],
+                    kernel_size=kernels[i],
+                    strides=strides[i],
+                    padding=paddings[i],
+                    name=f"conv_{i}",
+                    kernel_regularizer=kernel_regularizer,
+                    bias_regularizer=bias_regularizer,
+                    dtype=self.dtype,
+                )
             )
-            self.convs.append(conv_block)
-            self.time_reduction_factor *= conv_block.time_reduction_factor
-
-        self.post = Reshape(name="postprocess", dtype=self.dtype) if conv_type == "conv2d" else Identity(name="iden", dtype=self.dtype)
+            if norms[i] == "batch":
+                subblock.add(
+                    tf.keras.layers.BatchNormalization(
+                        name=f"bn_{i}",
+                        gamma_regularizer=kernel_regularizer,
+                        beta_regularizer=bias_regularizer,
+                        dtype=self.dtype,
+                    )
+                )
+            elif norms[i] == "layer":
+                subblock.add(
+                    tf.keras.layers.LayerNormalization(
+                        name=f"ln_{i}",
+                        gamma_regularizer=kernel_regularizer,
+                        beta_regularizer=bias_regularizer,
+                        dtype=self.dtype,
+                    )
+                )
+            subblock.add(tf.keras.layers.Activation(activations[i], name=f"{activations[i]}_{i}", dtype=self.dtype))
+            self.convs.append(subblock)
+            self.time_reduction_factor *= subblock.layers[0].strides[0]
 
     def call(self, inputs, training=False):
-        outputs = self.pre(inputs, training=training)
-        for conv in self.convs:
-            outputs = conv(outputs, training=training)
-        outputs = self.post(outputs, training=training)
-        return outputs
+        outputs, outputs_length = inputs
+        for block in self.convs:
+            outputs = block(outputs, training=training)
+            outputs_length = math_util.conv_output_length(
+                outputs_length,
+                filter_size=block.layers[0].kernel_size[0],
+                padding=block.layers[0].padding,
+                stride=block.layers[0].strides[0],
+            )
+        outputs = math_util.merge_two_last_dims(outputs)
+        return outputs, outputs_length
 
     def compute_mask(self, inputs, mask=None):
         outputs, outputs_length = inputs
         maxlen = tf.shape(outputs)[1]
-        for conv in self.convs:
+        for block in self.convs:
             maxlen, outputs_length = (
-                math_util.conv_output_length(length, filter_size=conv.conv.kernel_size[0], padding=conv.conv.padding, stride=conv.conv.strides[0])
+                math_util.conv_output_length(
+                    length, filter_size=block.layers[0].kernel_size[0], padding=block.layers[0].padding, stride=block.layers[0].strides[0]
+                )
                 for length in (maxlen, outputs_length)
             )
         mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
         return mask, None
 
     def compute_output_shape(self, input_shape):
-        output_shape = input_shape
-        output_shape = self.pre.compute_output_shape(output_shape)
-        for conv in self.convs:
-            output_shape = conv.compute_output_shape(output_shape)
-        output_shape = self.post.compute_output_shape(output_shape)
-        return output_shape
-
-
-# ------------------------------------ RNN ----------------------------------- #
-
-
-class RnnBlock(Layer):
-    def __init__(
-        self,
-        rnn_type: str = "lstm",
-        units: int = 1024,
-        bidirectional: bool = True,
-        unroll: bool = False,
-        rowconv: int = 0,
-        rowconv_activation: str = "relu",
-        dropout: float = 0.1,
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        initializer=None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.rnn = layer_util.get_rnn(rnn_type)(
-            units,
-            dropout=dropout,
-            unroll=unroll,
-            return_sequences=True,
-            use_bias=True,
-            name=rnn_type,
-            zero_output_for_mask=True,
-            kernel_regularizer=kernel_regularizer,
-            kernel_initializer=initializer,
-            bias_regularizer=bias_regularizer,
-            bias_initializer=initializer,
-            dtype=self.dtype,
-        )
-        if bidirectional:
-            self.rnn = tf.keras.layers.Bidirectional(self.rnn, name=f"b{rnn_type}", dtype=self.dtype)
-        self.bn = tf.keras.layers.BatchNormalization(
-            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
-        )
-        self.rowconv = None
-        if not bidirectional and rowconv > 0:
-            self.rowconv = RowConv1D(
-                future_width=rowconv,
-                name="rowconv",
-                regularizer=kernel_regularizer,
-                initializer=initializer,
-                activation=rowconv_activation,
-                dtype=self.dtype,
-            )
-
-    def call(self, inputs, training=False):
-        outputs, outputs_length = inputs
-        outputs = self.rnn(outputs, training=training)  # mask auto populate
-        outputs = self.bn(outputs, training=training)
-        if self.rowconv is not None:
-            outputs = self.rowconv(outputs, training=training)
-        return outputs, outputs_length
-
-    def compute_output_shape(self, input_shape):
         output_shape, output_length_shape = input_shape
-        output_shape = self.rnn.compute_output_shape(output_shape)
-        output_shape = self.bn.compute_output_shape(output_shape)
-        if self.rowconv is not None:
-            output_shape = self.rowconv.compute_output_shape(output_shape)
+        for block in self.convs:
+            output_shape = block.layers[0].compute_output_shape(output_shape)
+        output_shape = output_shape[:2] + (output_shape[2] * output_shape[3],)
         return output_shape, output_length_shape
 
 
-class RnnModule(Layer):
+class Conv1dSubsampling(Layer):
     def __init__(
         self,
-        nlayers: int = 5,
-        rnn_type: str = "lstm",
-        units: int = 1024,
-        bidirectional: bool = True,
-        unroll: bool = False,
-        rowconv: int = 0,
-        rowconv_activation: str = "relu",
-        dropout: float = 0.1,
+        filters: list,
+        strides: list = [2, 2],
+        kernels: list = [3, 3],
+        paddings: list = ["causal", "causal"],
+        norms: list = ["none", "none"],
+        activations: list = ["relu", "relu"],
         kernel_regularizer=None,
         bias_regularizer=None,
-        initializer=None,
+        name="conv1d_subsampling",
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.blocks = [
-            RnnBlock(
-                rnn_type=rnn_type,
-                units=units,
-                bidirectional=bidirectional,
-                unroll=unroll,
-                rowconv=rowconv,
-                rowconv_activation=rowconv_activation,
-                dropout=dropout,
-                kernel_regularizer=kernel_regularizer,
-                bias_regularizer=bias_regularizer,
-                initializer=initializer,
-                name=f"block_{i}",
-                dtype=self.dtype,
+        super().__init__(name=name, **kwargs)
+        assert len(filters) == len(strides) == len(kernels) == len(paddings) == len(norms) == len(activations)
+        self.convs = []
+        self.time_reduction_factor = 1
+        for i in range(len(filters)):
+            subblock = tf.keras.Sequential(name=f"block_{i}")
+            subblock.add(
+                Conv1D(
+                    filters=filters[i],
+                    kernel_size=kernels[i],
+                    strides=strides[i],
+                    padding=paddings[i],
+                    name=f"conv_{i}",
+                    kernel_regularizer=kernel_regularizer,
+                    bias_regularizer=bias_regularizer,
+                    dtype=self.dtype,
+                )
             )
-            for i in range(nlayers)
-        ]
+            if norms[i] == "batch":
+                subblock.add(
+                    tf.keras.layers.BatchNormalization(
+                        name=f"bn_{i}",
+                        gamma_regularizer=kernel_regularizer,
+                        beta_regularizer=bias_regularizer,
+                        dtype=self.dtype,
+                    )
+                )
+            elif norms[i] == "layer":
+                subblock.add(
+                    tf.keras.layers.LayerNormalization(
+                        name=f"ln_{i}",
+                        gamma_regularizer=kernel_regularizer,
+                        beta_regularizer=bias_regularizer,
+                        dtype=self.dtype,
+                    )
+                )
+            subblock.add(tf.keras.layers.Activation(activations[i], name=f"{activations[i]}_{i}", dtype=self.dtype))
+            self.convs.append(subblock)
+            self.time_reduction_factor *= subblock.layers[0].strides[0]
 
     def call(self, inputs, training=False):
-        outputs = inputs
-        for block in self.blocks:
+        outputs, outputs_length = inputs
+        outputs = math_util.merge_two_last_dims(outputs)
+        for block in self.convs:
             outputs = block(outputs, training=training)
-        return outputs
-
-    def compute_output_shape(self, input_shape):
-        output_shape = input_shape
-        for block in self.blocks:
-            output_shape = block.compute_output_shape(output_shape)
-        return output_shape
-
-
-# ------------------------------ FULLY CONNECTED ----------------------------- #
-
-
-class FcBlock(Layer):
-    def __init__(
-        self,
-        units: int = 1024,
-        activation: str = "relu",
-        dropout: float = 0.1,
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        initializer=None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.fc = tf.keras.layers.Dense(
-            units,
-            kernel_regularizer=kernel_regularizer,
-            kernel_initializer=initializer,
-            bias_regularizer=bias_regularizer,
-            bias_initializer=initializer,
-            name="fc",
-            dtype=self.dtype,
-        )
-        self.bn = tf.keras.layers.BatchNormalization(
-            name="bn", gamma_regularizer=kernel_regularizer, beta_regularizer=bias_regularizer, dtype=self.dtype
-        )
-        self.act = tf.keras.layers.Activation(activation=activation, dtype=self.dtype)
-        self.do = tf.keras.layers.Dropout(dropout, name="dropout", dtype=self.dtype)
+            outputs_length = math_util.conv_output_length(
+                outputs_length,
+                filter_size=block.layers[0].kernel_size[0],
+                padding=block.layers[0].padding,
+                stride=block.layers[0].strides[0],
+            )
+        return outputs, outputs_length
 
-    def call(self, inputs, training=False):
+    def compute_mask(self, inputs, mask=None):
         outputs, outputs_length = inputs
-        outputs = self.fc(outputs, training=training)
-        outputs = self.bn(outputs, training=training)
-        outputs = self.act(outputs, training=training)
-        outputs = self.do(outputs, training=training)
-        return outputs, outputs_length
+        maxlen = tf.shape(outputs)[1]
+        for block in self.convs:
+            maxlen, outputs_length = (
+                math_util.conv_output_length(
+                    length, filter_size=block.layers[0].kernel_size[0], padding=block.layers[0].padding, stride=block.layers[0].strides[0]
+                )
+                for length in (maxlen, outputs_length)
+            )
+        mask = tf.sequence_mask(outputs_length, maxlen=maxlen, dtype=tf.bool)
+        return mask, None
 
     def compute_output_shape(self, input_shape):
         output_shape, output_length_shape = input_shape
-        output_shape = self.fc.compute_output_shape(output_shape)
+        output_shape = output_shape[:2] + (output_shape[2] * output_shape[3],)
+        for block in self.convs:
+            output_shape = block.layers[0].compute_output_shape(output_shape)
         return output_shape, output_length_shape
-
-
-class FcModule(Layer):
-    def __init__(
-        self,
-        nlayers: int = 0,
-        units: int = 1024,
-        activation: str = "relu",
-        dropout: float = 0.1,
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        initializer=None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.blocks = [
-            FcBlock(
-                units=units,
-                activation=activation,
-                dropout=dropout,
-                kernel_regularizer=kernel_regularizer,
-                bias_regularizer=bias_regularizer,
-                initializer=initializer,
-                name=f"block_{i}",
-                dtype=self.dtype,
-            )
-            for i in range(nlayers)
-        ]
-
-    def call(self, inputs, training=False):
-        outputs = inputs
-        for block in self.blocks:
-            outputs = block(outputs, training=training)
-        return outputs
-
-    def compute_output_shape(self, input_shape):
-        output_shape = input_shape
-        for block in self.blocks:
-            output_shape = block.compute_output_shape(output_shape)
-        return output_shape
-
-
-class DeepSpeech2Encoder(Layer):
-    def __init__(
-        self,
-        conv_type: str = "conv2d",
-        conv_kernels: list = [[11, 41], [11, 21], [11, 21]],
-        conv_strides: list = [[2, 2], [1, 2], [1, 2]],
-        conv_filters: list = [32, 32, 96],
-        conv_padding: str = "same",
-        conv_activation: str = "relu",
-        conv_dropout: float = 0.1,
-        conv_initializer: str = None,
-        rnn_nlayers: int = 5,
-        rnn_type: str = "lstm",
-        rnn_units: int = 1024,
-        rnn_bidirectional: bool = True,
-        rnn_unroll: bool = False,
-        rnn_rowconv: int = 0,
-        rnn_rowconv_activation: str = "relu",
-        rnn_dropout: float = 0.1,
-        rnn_initializer: str = None,
-        fc_nlayers: int = 0,
-        fc_units: int = 1024,
-        fc_activation: str = "relu",
-        fc_dropout: float = 0.1,
-        fc_initializer: str = None,
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        initializer=None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.conv_module = ConvModule(
-            conv_type=conv_type,
-            kernels=conv_kernels,
-            strides=conv_strides,
-            filters=conv_filters,
-            padding=conv_padding,
-            activation=conv_activation,
-            dropout=conv_dropout,
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-            initializer=conv_initializer or initializer,
-            name="conv_module",
-            dtype=self.dtype,
-        )
-        self.rnn_module = RnnModule(
-            nlayers=rnn_nlayers,
-            rnn_type=rnn_type,
-            units=rnn_units,
-            bidirectional=rnn_bidirectional,
-            unroll=rnn_unroll,
-            rowconv=rnn_rowconv,
-            rowconv_activation=rnn_rowconv_activation,
-            dropout=rnn_dropout,
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-            initializer=rnn_initializer or initializer,
-            name="rnn_module",
-            dtype=self.dtype,
-        )
-        self.fc_module = FcModule(
-            nlayers=fc_nlayers,
-            units=fc_units,
-            activation=fc_activation,
-            dropout=fc_dropout,
-            kernel_regularizer=kernel_regularizer,
-            bias_regularizer=bias_regularizer,
-            initializer=fc_initializer or initializer,
-            name="fc_module",
-            dtype=self.dtype,
-        )
-        self.time_reduction_factor = self.conv_module.time_reduction_factor
-
-    def call(self, inputs, training=False):
-        *outputs, caching = inputs
-        outputs = self.conv_module(outputs, training=training)
-        outputs = self.rnn_module(outputs, training=training)
-        outputs = self.fc_module(outputs, training=training)
-        return *outputs, caching
-
-    def compute_mask(self, inputs, mask=None):
-        *outputs, caching = inputs
-        return *self.conv_module.compute_mask(outputs, mask=mask), getattr(caching, "_keras_mask", None)
-
-    def compute_output_shape(self, input_shape):
-        *output_shape, caching_shape = input_shape
-        output_shape = self.conv_module.compute_output_shape(output_shape)
-        output_shape = self.rnn_module.compute_output_shape(output_shape)
-        output_shape = self.fc_module.compute_output_shape(output_shape)
-        return *output_shape, caching_shape
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/jasper.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/jasper.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/rnnt.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/rnnt.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/encoders/transformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/encoders/transformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/blurpool.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/blurpool.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/convolution.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/embedding.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/feature_extraction.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/memory.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/memory.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/multihead_attention.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/positional_encoding.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/residual.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/residual.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/layers/sequence_wise_bn.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/layers/sequence_wise_bn.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/base_transducer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/base_transducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,23 @@
         """
         with tf.name_scope(f"{self.name}_call_next"):
             y, new_states = self.predict_net.call_next(previous_tokens, previous_decoder_states)
             ytu = self.joint_net([current_frames, y], training=False)
             ytu = tf.nn.log_softmax(ytu)
             return ytu, new_states
 
+    def get_initial_tokens(self, batch_size=1):
+        return super().get_initial_tokens(batch_size)
+
+    def get_initial_encoder_states(self, batch_size=1):
+        return tf.zeros([], dtype=self.dtype)
+
+    def get_initial_decoder_states(self, batch_size=1):
+        return self.predict_net.get_initial_state(batch_size)
+
     # -------------------------------- GREEDY -------------------------------------
 
     def recognize(self, inputs: schemas.PredictInput, max_tokens_per_frame: int = 3, **kwargs):
         """
         Recognize greedy from input signals
 
         Parameters
@@ -460,19 +469,17 @@
             (
                 tokens, will be feed to text_featurizer.detokenize or text_featurizer.detokenize_unicode_points,
                 next_encoder_states, if encoder does not have states, returns None, will be used to predict next chunk of audio,
                 next_tokens, will be used to predict next chunk of audio,
                 next_decoder_states, next states of predict_net, will be used to predict next chunk of audio,
             )
         """
-        return tf.cond(
-            tf.equal(tf.shape(inputs.inputs_length)[0], 1),
-            lambda: self.recognize_single(inputs, max_tokens_per_frame=max_tokens_per_frame, **kwargs),
-            lambda: self.recognize_batch(inputs, **kwargs),
-        )
+        if self._batch_size == 1:
+            return self.recognize_single(inputs, max_tokens_per_frame=max_tokens_per_frame, **kwargs)
+        return self.recognize_batch(inputs, **kwargs)
 
     def recognize_batch(self, inputs: schemas.PredictInput, **kwargs):
         """
         Ref: https://arxiv.org/pdf/1801.00841.pdf
         This is a greedy decoding algorithm that greedily select the best token at each time step
         Only apply for batch size > 1
         """
@@ -481,17 +488,17 @@
             encoded, encoded_length, next_encoder_states = self.encoder.call_next(features, features_length, inputs.previous_encoder_states)
 
             nframes = tf.expand_dims(encoded_length, axis=-1)  # [B, 1]
             batch_size, max_frames, _ = shape_util.shape_list(encoded)
             # The current indices of the output of encoder, shape [B, 1]
             frame_indices = tf.zeros([batch_size, 1], dtype=tf.int32, name="frame_indices")
             # Previous predicted tokens, initially are blanks, shape [B, 1]
-            previous_tokens = inputs.previous_tokens or tf.ones([batch_size, 1], dtype=tf.int32, name="previous_tokens") * self.blank
+            previous_tokens = inputs.previous_tokens
             # Previous states of the prediction network, initially are zeros, shape [B, num_rnns, nstates, rnn_units]
-            previous_decoder_states = inputs.previous_decoder_states or self.predict_net.get_initial_state(batch_size)
+            previous_decoder_states = inputs.previous_decoder_states
             # Assumption that number of tokens can not exceed (2 * the size of output of encoder + 1), this is for static runs like TPU or TFLite
             max_tokens = max_frames * 2 + 1
             # All of the tokens that are getting recognized, initially are blanks, shape [B, nframes * 2 + 1]
             tokens = tf.ones([batch_size, max_tokens], dtype=tf.int32, name="tokens") * self.blank
             # The current indices of the token that are currently being recognized, shape [B, 1], the tokens indices are started with 1 so that any
             # blank token recognized got updated to index 0 to avoid affecting results
             tokens_indices = tf.ones([batch_size, 1], dtype=tf.int32, name="tokens_indices")
@@ -560,15 +567,15 @@
         with tf.name_scope(f"{self.name}_decode_greedy"):
             features, features_length = self.feature_extraction((inputs.inputs, inputs.inputs_length), training=False)
             encoded, encoded_length, next_encoder_states = self.encoder.call_next(features, features_length, inputs.previous_encoder_states)
 
             frame = tf.zeros([1, 1], dtype=tf.int32)
             nframes = encoded_length
 
-            previous_tokens = inputs.previous_tokens or tf.ones([1, 1], dtype=tf.int32) * self.blank
+            previous_tokens = inputs.previous_tokens
             token_index = tf.ones([], dtype=tf.int32) * -1
             tokens = tf.TensorArray(
                 dtype=tf.int32,
                 size=tf.reshape(nframes, shape=[]) * max_tokens_per_frame,
                 dynamic_size=False,
                 clear_after_read=False,
                 element_shape=tf.TensorShape([]),
@@ -577,15 +584,15 @@
                 dtype=tf.int32,
                 size=tf.reshape(nframes, shape=[]),
                 dynamic_size=False,
                 clear_after_read=False,
                 element_shape=tf.TensorShape([]),
             )
 
-            previous_decoder_states = inputs.previous_decoder_states or self.predict_net.get_initial_state(1)
+            previous_decoder_states = inputs.previous_decoder_states
 
             def condition(
                 _frame,
                 _nframes,
                 _previous_tokens,
                 _token_index,
                 _tokens,
@@ -811,16 +818,16 @@
     #             index=hypothesis.index,
     #             prediction=hypothesis.prediction.stack(),
     #             states=hypothesis.states,
     #         )
 
     # -------------------------------- BEAM SEARCH -------------------------------------
 
-    def recognize_beam(self, inputs: schemas.PredictInput, **kwargs):
-        return self.recognize(inputs=inputs, **kwargs)
+    def recognize_beam(self, inputs: schemas.PredictInput, beam_width: int = 10, **kwargs):
+        return self.recognize(inputs=inputs, **kwargs)  # TODO: Implement beam search
 
     # def _perform_beam_search_batch(
     #     self,
     #     encoded: tf.Tensor,
     #     encoded_length: tf.Tensor,
     #     lm: bool = False,
     #     parallel_iterations: int = 10,
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/conformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/conformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/contextnet.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/contextnet.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/models/transducer/transformer.py` & `TensorFlowASR-2.0.1/tensorflow_asr/models/transducer/transformer.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/optimizers/accumulation.py` & `TensorFlowASR-2.0.1/tensorflow_asr/optimizers/accumulation.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/optimizers/regularizers.py` & `TensorFlowASR-2.0.1/tensorflow_asr/optimizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/optimizers/schedules.py` & `TensorFlowASR-2.0.1/tensorflow_asr/optimizers/schedules.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/schemas.py` & `TensorFlowASR-2.0.1/tensorflow_asr/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,7 +50,12 @@
     defaults=(None, None, None),
 )
 PredictOutput = collections.namedtuple(
     "PredictOutput",
     ("tokens", "next_tokens", "next_encoder_states", "next_decoder_states"),
     defaults=(None, None),
 )
+PredictOutputWithTranscript = collections.namedtuple(
+    "PredictOutputWithTranscript",
+    ("transcript", "tokens", "next_tokens", "next_encoder_states", "next_decoder_states"),
+    defaults=(None, None),
+)
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/tokenizers.py` & `TensorFlowASR-2.0.1/tensorflow_asr/tokenizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def corpus_generator(cls, decoder_config: DecoderConfig):
         for file_path in file_util.preprocess_paths(decoder_config.train_files):
             logger.info(f"Reading {file_path} ...")
             with tf.io.gfile.GFile(file_path, "r") as f:
                 temp_lines = f.read().splitlines()
                 for line in temp_lines[1:]:  # Skip the header of tsv file
                     data = line.split("\t", 2)[-1]  # get only transcript
-                    data = cls.normalize_text(data, decoder_config.normalization_form).numpy()
+                    data = cls.normalize_text(data, decoder_config).numpy()
                     yield data
 
     @property
     def shape(self) -> list:
         return [self.max_length if self.max_length > 0 else None]
 
     @property
@@ -131,17 +131,20 @@
     ):
         self.max_length = max(self.max_length, length)
 
     def reset_length(self):
         self.max_length = 0
 
     @classmethod
-    def normalize_text(cls, text: tf.Tensor, normalization_form: str = "NFKC"):
-        text = tft.normalize_utf8(text, normalization_form)
+    def normalize_text(cls, text: tf.Tensor, decoder_config: DecoderConfig):
+        text = tf.strings.regex_replace(text, b"\xe2\x81\x87".decode("utf-8"), "")
+        text = tft.normalize_utf8(text, decoder_config.normalization_form)
         text = tf.strings.regex_replace(text, r"\p{Cc}|\p{Cf}", " ")
+        text = tf.strings.regex_replace(text, decoder_config.unknown_token, "")
+        text = tf.strings.regex_replace(text, decoder_config.pad_token, "")
         text = tf.strings.regex_replace(text, r" +", " ")
         text = tf.strings.lower(text, encoding="utf-8")
         text = tf.strings.strip(text)  # remove trailing whitespace
         return text
 
     def add_scorer(self, scorer: any = None):
         """Add scorer to this instance"""
@@ -155,15 +158,15 @@
 
         Returns:
             tf.Tensor: normalized indices with shape same as indices
         """
         with tf.name_scope("normalize_indices"):
             minus_one = -1 * tf.ones_like(indices, dtype=tf.int32)
             blank_like = self.blank * tf.ones_like(indices, dtype=tf.int32)
-            return tf.where(indices == minus_one, blank_like, indices)
+            return tf.where(tf.equal(indices, minus_one), blank_like, indices)
 
     def prepand_blank(self, text: tf.Tensor) -> tf.Tensor:
         """Prepand blank index for transducer models"""
         return tf.concat([[self.blank], text], 0)
 
     def tokenize(self, text: str) -> tf.Tensor:
         raise NotImplementedError()
@@ -226,31 +229,32 @@
             vocab.update(text)
 
         write_vocab_file(decoder_config.vocabulary, vocab)
 
         return cls(decoder_config)
 
     def tokenize(self, text):
-        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        text = self.normalize_text(text, self.decoder_config)
         text = tf.strings.unicode_split(text, "UTF-8")
         return self.tokenizer.lookup(text)
 
     def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Convert list of indices to string
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
         indices = self.normalize_indices(indices)
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
         tokens = self.detokenizer.lookup(indices)
         tokens = tf.strings.reduce_join(tokens, axis=-1)
+        tokens = self.normalize_text(tokens, self.decoder_config)
         return tokens
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
     def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
@@ -303,34 +307,35 @@
             remove_extra_whitespaces=True,
             num_threads=multiprocessing.cpu_count(),
         )
 
         return cls(decoder_config)
 
     def tokenize(self, text: tf.Tensor) -> tf.Tensor:
-        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        text = self.normalize_text(text, self.decoder_config)
         indices = self.tokenizer.tokenize(text)
         indices = tf.cast(indices, tf.int32)
         return indices
 
     def detokenize(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Convert list of indices to string
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.bos_index))
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.eos_index))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.bos_index))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.eos_index))
         transcripts = self.tokenizer.detokenize(indices)
-        transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
+        transcripts = self.normalize_text(transcripts, self.decoder_config)
+        # transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
         return transcripts
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
     def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
@@ -395,15 +400,15 @@
             },
         )
         write_vocab_file(decoder_config.vocabulary, vocab)
 
         return cls(decoder_config)
 
     def tokenize(self, text: tf.Tensor) -> tf.Tensor:
-        text = self.normalize_text(text, self.decoder_config.normalization_form)
+        text = self.normalize_text(text, self.decoder_config)
         if self.decoder_config.keep_whitespace:
             text = tf.strings.regex_replace(text, " ", "| |")
             text = tf.strings.split(text, sep="|")
         else:
             text = tf.strings.split(text)
         indices = self.tokenizer.tokenize(text).merge_dims(0, 1)
         return indices
@@ -413,18 +418,19 @@
         Convert list of indices to string
         Args:
             indices: tf.Tensor with dim [B, None]
 
         Returns:
             transcripts: tf.Tensor of dtype tf.string with dim [B]
         """
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
-        indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.blank))
+        # indices = tf.ragged.boolean_mask(indices, tf.not_equal(indices, self.decoder_config.unknown_index))
         transcripts = self.tokenizer.detokenize(indices)
-        transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
+        transcripts = self.normalize_text(transcripts, self.decoder_config)
+        # transcripts = tf.strings.regex_replace(transcripts, r" +", " ")
         return transcripts
 
     @tf.function(input_signature=[tf.TensorSpec([None], dtype=tf.int32)])
     def detokenize_unicode_points(self, indices: tf.Tensor) -> tf.Tensor:
         """
         Transform Predicted Indices to Unicode Code Points (for using tflite)
         Args:
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/data_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/data_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/env_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/env_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/feature_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/feature_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/file_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/layer_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/layer_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/math_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/math_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 def masked_fill(
     tensor,
     mask,
     value=0,
 ):
     shape = shape_util.shape_list(tensor)
-    mask = tf.broadcast_to(mask, shape)
+    mask = tf.cast(tf.broadcast_to(mask, shape), dtype=tf.bool)
     values = tf.cast(tf.fill(shape, value), tensor.dtype)
     return tf.where(mask, tensor, values)
 
 
 def large_compatible_negative(
     tensor_type,
 ):
@@ -274,7 +274,19 @@
 def compute_time_length(
     tensor: tf.Tensor,
     dtype=tf.int32,
 ):
     with tf.name_scope("compute_time_length"):
         batch_size, time_length, *_ = shape_util.shape_list(tensor)
         return tf.cast(tf.repeat(time_length, batch_size, axis=0), dtype=dtype)
+
+
+def is_power_of_two(
+    x: int,
+):
+    return x != 0 and (x & (x - 1)) == 0
+
+
+def next_power_of_two(
+    x: int,
+):
+    return 1 if x == 0 else 2 ** math.ceil(math.log2(x))
```

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/metric_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/metric_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/plot_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/plot_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/shape_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/shape_util.py`

 * *Files identical despite different names*

### Comparing `TensorFlowASR-2.0.0/tensorflow_asr/utils/tf_util.py` & `TensorFlowASR-2.0.1/tensorflow_asr/utils/tf_util.py`

 * *Files identical despite different names*

