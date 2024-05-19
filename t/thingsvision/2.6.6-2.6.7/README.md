# Comparing `tmp/thingsvision-2.6.6.tar.gz` & `tmp/thingsvision-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.6.6.tar", last modified: Thu May 16 17:44:26 2024, max compression
+gzip compressed data, was "thingsvision-2.6.7.tar", last modified: Sun May 19 16:44:47 2024, max compression
```

## Comparing `thingsvision-2.6.6.tar` & `thingsvision-2.6.7.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.162964 thingsvision-2.6.6/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.6/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-16 17:44:26.162635 thingsvision-2.6.6/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16216 2024-04-24 14:58:04.000000 thingsvision-2.6.6/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-05-16 17:44:26.163042 thingsvision-2.6.6/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1725 2024-05-16 09:23:05.000000 thingsvision-2.6.6/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.122437 thingsvision-2.6.6/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.6/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.123924 thingsvision-2.6.6/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.6/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.125875 thingsvision-2.6.6/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.6/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.6/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.6/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2180 2024-05-16 09:23:05.000000 thingsvision-2.6.6/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.6/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-22 12:21:01.000000 thingsvision-2.6.6/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.6/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    12379 2024-05-16 09:23:05.000000 thingsvision-2.6.6/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.6/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.6/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.127093 thingsvision-2.6.6/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.6/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-05-16 17:44:14.000000 thingsvision-2.6.6/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.129094 thingsvision-2.6.6/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.6/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.131960 thingsvision-2.6.6/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.6/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.6/thingsvision/core/cka/cka_base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.6/thingsvision/core/cka/cka_numpy.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5957 2024-04-22 11:26:42.000000 thingsvision-2.6.6/thingsvision/core/cka/cka_torch.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.6/thingsvision/core/cka/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.137111 thingsvision-2.6.6/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-24 08:51:44.000000 thingsvision-2.6.6/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10927 2024-04-24 14:58:04.000000 thingsvision-2.6.6/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17360 2024-05-02 10:07:13.000000 thingsvision-2.6.6/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8453 2024-04-24 14:58:04.000000 thingsvision-2.6.6/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.6/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10948 2024-04-29 13:15:16.000000 thingsvision-2.6.6/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.138859 thingsvision-2.6.6/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.6/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.6/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.146813 thingsvision-2.6.6/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      355 2024-05-16 09:23:05.000000 thingsvision-2.6.6/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.6/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.6/thingsvision/custom_models/alexnet_salobjsub.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2024-05-16 09:23:05.000000 thingsvision-2.6.6/thingsvision/custom_models/align.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.150074 thingsvision-2.6.6/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.6/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.151110 thingsvision-2.6.6/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.6/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.6/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.152612 thingsvision-2.6.6/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.6/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.6/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.6/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.6/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.6/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.6/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3346 2024-05-16 17:44:14.000000 thingsvision-2.6.6/thingsvision/custom_models/sam.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.6/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.6/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.6/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.153231 thingsvision-2.6.6/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.6/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.154107 thingsvision-2.6.6/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.6/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.6/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.154591 thingsvision-2.6.6/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.6/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.156571 thingsvision-2.6.6/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.6/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.6/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.6/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.6/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.157291 thingsvision-2.6.6/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.157631 thingsvision-2.6.6/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.6/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.158949 thingsvision-2.6.6/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.6/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.6/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.6/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.160496 thingsvision-2.6.6/thingsvision/utils/models/mae/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.6/thingsvision/utils/models/mae/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.6/thingsvision/utils/models/mae/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.6/thingsvision/utils/models/mae/vit_mae.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.161306 thingsvision-2.6.6/thingsvision/utils/models/sam/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       43 2024-05-16 17:44:14.000000 thingsvision-2.6.6/thingsvision/utils/models/sam/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1478 2024-05-16 09:23:05.000000 thingsvision-2.6.6/thingsvision/utils/models/sam/common.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14419 2024-05-16 09:23:05.000000 thingsvision-2.6.6/thingsvision/utils/models/sam/image_encoder.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.161917 thingsvision-2.6.6/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.6/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.6/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 17:44:26.128902 thingsvision-2.6.6/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3079 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      346 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-05-16 17:44:25.000000 thingsvision-2.6.6/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.889469 thingsvision-2.6.7/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.7/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-19 16:44:47.889163 thingsvision-2.6.7/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16216 2024-04-24 14:58:04.000000 thingsvision-2.6.7/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-05-19 16:44:47.889546 thingsvision-2.6.7/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1725 2024-05-16 09:23:05.000000 thingsvision-2.6.7/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.839857 thingsvision-2.6.7/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.7/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.841119 thingsvision-2.6.7/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.7/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.843692 thingsvision-2.6.7/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.7/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.7/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.7/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2180 2024-05-16 09:23:05.000000 thingsvision-2.6.7/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.7/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-22 12:21:01.000000 thingsvision-2.6.7/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.7/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    12379 2024-05-16 09:23:05.000000 thingsvision-2.6.7/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.7/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.7/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.845227 thingsvision-2.6.7/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.7/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-05-19 16:44:37.000000 thingsvision-2.6.7/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.847330 thingsvision-2.6.7/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.7/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.848666 thingsvision-2.6.7/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.7/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-05-17 13:02:59.000000 thingsvision-2.6.7/thingsvision/core/cka/cka_base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3597 2024-05-19 16:44:37.000000 thingsvision-2.6.7/thingsvision/core/cka/cka_numpy.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     6084 2024-05-19 16:44:37.000000 thingsvision-2.6.7/thingsvision/core/cka/cka_torch.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      933 2024-05-19 16:44:37.000000 thingsvision-2.6.7/thingsvision/core/cka/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.851892 thingsvision-2.6.7/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-24 08:51:44.000000 thingsvision-2.6.7/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10927 2024-04-24 14:58:04.000000 thingsvision-2.6.7/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17360 2024-05-02 10:07:13.000000 thingsvision-2.6.7/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8453 2024-04-24 14:58:04.000000 thingsvision-2.6.7/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.7/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10948 2024-04-29 13:15:16.000000 thingsvision-2.6.7/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.853165 thingsvision-2.6.7/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.7/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.7/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.859770 thingsvision-2.6.7/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      355 2024-05-16 09:23:05.000000 thingsvision-2.6.7/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.7/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.7/thingsvision/custom_models/alexnet_salobjsub.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2024-05-16 09:23:05.000000 thingsvision-2.6.7/thingsvision/custom_models/align.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.862389 thingsvision-2.6.7/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.7/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.863242 thingsvision-2.6.7/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.7/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.7/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.875387 thingsvision-2.6.7/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.7/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.7/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.7/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.7/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.7/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.7/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3346 2024-05-16 17:44:14.000000 thingsvision-2.6.7/thingsvision/custom_models/sam.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.7/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.7/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.7/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.876272 thingsvision-2.6.7/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.7/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.877473 thingsvision-2.6.7/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.7/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.7/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.878265 thingsvision-2.6.7/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.7/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.880775 thingsvision-2.6.7/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.7/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.7/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.7/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.7/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.882149 thingsvision-2.6.7/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.882580 thingsvision-2.6.7/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.7/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.883990 thingsvision-2.6.7/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.7/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.7/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.7/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.885774 thingsvision-2.6.7/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.7/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.7/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.7/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.887367 thingsvision-2.6.7/thingsvision/utils/models/sam/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       43 2024-05-16 17:44:14.000000 thingsvision-2.6.7/thingsvision/utils/models/sam/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1478 2024-05-16 09:23:05.000000 thingsvision-2.6.7/thingsvision/utils/models/sam/common.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14419 2024-05-16 09:23:05.000000 thingsvision-2.6.7/thingsvision/utils/models/sam/image_encoder.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.888381 thingsvision-2.6.7/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.7/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.7/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-19 16:44:47.847095 thingsvision-2.6.7/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3079 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      346 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-05-19 16:44:47.000000 thingsvision-2.6.7/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.6.6/LICENSE` & `thingsvision-2.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/PKG-INFO` & `thingsvision-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.6
+Version: 2.6.7
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.6 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.7 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.6.6/README.md` & `thingsvision-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/setup.py` & `thingsvision-2.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.6.7/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.6.7/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.6.7/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.6.7/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/test_load_extractor.py` & `thingsvision-2.6.7/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/extractor/test_transformations.py` & `thingsvision-2.6.7/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/helper.py` & `thingsvision-2.6.7/tests/helper.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/test_features.py` & `thingsvision-2.6.7/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/tests/test_rest.py` & `thingsvision-2.6.7/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/cka/cka_base.py` & `thingsvision-2.6.7/thingsvision/core/cka/cka_base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/cka/cka_numpy.py` & `thingsvision-2.6.7/thingsvision/core/cka/cka_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,23 @@
             raise NotImplementedError
         return K
 
     def linear_kernel(self, X: Array) -> Array:
         """Use a linear kernel for computing the gram matrix."""
         return X @ X.T
 
-    def rbf_kernel(self, X: Array, sigma: float = 1.0) -> Array:
+    def rbf_kernel(self, X: Array) -> Array:
         """Use an rbf kernel for computing the gram matrix. Sigma defines the width."""
         GX = X @ X.T
         KX = np.diag(GX) - GX + (np.diag(GX) - GX).T
-        if sigma is None:
+        if self.sigma is None:
             mdist = np.median(KX[KX != 0])
             sigma = math.sqrt(mdist)
+        else:
+            sigma = self.sigma
         KX *= -0.5 / sigma**2
         KX = np.exp(KX)
         return KX
 
     def _hsic(self, X: Array, Y: Array) -> Array:
         """Compute the Hilbert-Schmidt independence criterion."""
         K = self.apply_kernel(X)
```

### Comparing `thingsvision-2.6.6/thingsvision/core/cka/cka_torch.py` & `thingsvision-2.6.7/thingsvision/core/cka/cka_torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,36 +14,37 @@
 class CKATorch(CKABase):
     def __init__(
         self,
         m: int,
         kernel: str,
         unbiased: bool = False,
         device: str = "cpu",
+        verbose: bool = False,
         sigma: Optional[float] = 1.0,
     ) -> None:
         """
         PyTorch implementation of CKA. Runs on CPU and CUDA.
         Args:
             m (int) - number of images / examples in a mini-batch or the full dataset;
             kernel (str) - 'linear' or 'rbf' kernel for computing the gram matrix;
             unbiased (bool) - whether to compute an unbiased version of CKA;
             device (str) - whether to perform CKA computation on CPU or GPU;
             sigma (float) - for 'rbf' kernel sigma defines the width of the Gaussian;
         """
         super().__init__(m=m, kernel=kernel, unbiased=unbiased, sigma=sigma)
-        device = self._check_device(device)
+        device = self._check_device(device, verbose)
         if device == "cpu":
             self.hsic = self._hsic
         else:
             # use JIT compilation on CUDA
             self.hsic = torch.compile(self._hsic)
         self.device = torch.device(device)
 
     @staticmethod
-    def _check_device(device: str) -> str:
+    def _check_device(device: str, verbose: bool) -> str:
         """Check whether the selected device is available on current compute node."""
         if device.startswith("cuda"):
             gpu_index = re.search(r"cuda:(\d+)", device)
 
             if not torch.cuda.is_available():
                 warnings.warn(
                     "\nCUDA is not available on your system. Switching to device='cpu'.\n",
@@ -54,16 +55,16 @@
                 warnings.warn(
                     f"\nGPU index {gpu_index.group(1)} is out of range. "
                     f"Available GPUs: {torch.cuda.device_count()}. "
                     f"Switching to device='cuda:0'.\n",
                     category=UserWarning,
                 )
                 device = "cuda:0"
-
-        print(f"\nUsing device: {device}\n")
+        if verbose:
+            print(f"\nUsing device: {device}\n")
         return device
 
     def centering(self, K: TensorType["m", "m"]) -> TensorType["m", "m"]:
         """Centering of the (square) gram matrix K."""
         # The below code block is mainly copied from Simon Kornblith's implementation;
         # see here: https://github.com/google-research/google-research/blob/master/representation_similarity/Demo.ipynb
         if not torch.allclose(K, K.T, rtol=1e-03, atol=1e-04):
@@ -100,22 +101,24 @@
     def linear_kernel(
         self, X: Union[TensorType["m", "d"], TensorType["m", "p"]]
     ) -> TensorType["m", "m"]:
         """Use a linear kernel for computing the gram matrix."""
         return X @ X.T
 
     def rbf_kernel(
-        self, X: TensorType["m", "d"], sigma: Optional[float] = 1.0
+        self, X: Union[TensorType["m", "d"], TensorType["m", "p"]]
     ) -> TensorType["m", "m"]:
         """Use an rbf kernel for computing the gram matrix. Sigma defines the width."""
         GX = X @ X.T
         KX = torch.diag(GX) - GX + (torch.diag(GX) - GX).T
-        if sigma is None:
+        if self.sigma is None:
             mdist = torch.median(KX[KX != 0])
             sigma = torch.sqrt(mdist)
+        else:
+            sigma = self.sigma
         KX *= -0.5 / sigma**2
         KX = KX.exp()
         return KX
 
     def _hsic(
         self, X: TensorType["m", "d"], Y: TensorType["m", "p"]
     ) -> TensorType["1"]:
```

### Comparing `thingsvision-2.6.6/thingsvision/core/cka/helpers.py` & `thingsvision-2.6.7/thingsvision/core/cka/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,26 @@
 def get_cka(
     backend: str,
     m: int,
     kernel: str = "linear",
     unbiased: bool = False,
     sigma: Optional[float] = 1.0,
     device: Optional[str] = None,
+    verbose: Optional[bool] = False,
 ) -> Union[CKANumPy, CKATorch]:
     """Return a NumPy or PyTorch implementation of CKA."""
     assert backend in BACKENDS, f"\nSupported backends are: {BACKENDS}\n"
     if backend == "numpy":
         cka = CKANumPy(m=m, kernel=kernel, unbiased=unbiased, sigma=sigma)
     else:
         assert isinstance(
             device, str
         ), "\nDevice must be set for using PyTorch backend.\n"
         cka = CKATorch(
-            m=m, kernel=kernel, unbiased=unbiased, device=device, sigma=sigma
+            m=m,
+            kernel=kernel,
+            unbiased=unbiased,
+            device=device,
+            sigma=sigma,
+            verbose=verbose,
         )
     return cka
```

### Comparing `thingsvision-2.6.6/thingsvision/core/extraction/base.py` & `thingsvision-2.6.7/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/extraction/extractors.py` & `thingsvision-2.6.7/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/extraction/helpers.py` & `thingsvision-2.6.7/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.6.7/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/extraction/torch.py` & `thingsvision-2.6.7/thingsvision/core/extraction/torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/core/rsa/helpers.py` & `thingsvision-2.6.7/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.6.7/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.6.7/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/align.py` & `thingsvision-2.6.7/thingsvision/custom_models/align.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.6.7/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.6.7/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.6.7/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.6.7/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.6.7/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/openclip.py` & `thingsvision-2.6.7/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.6.7/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/sam.py` & `thingsvision-2.6.7/thingsvision/custom_models/sam.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.6.7/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.6.7/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/thingsvision.py` & `thingsvision-2.6.7/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.6.7/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.6.7/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/data/__init__.py` & `thingsvision-2.6.7/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/data/data_loader.py` & `thingsvision-2.6.7/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/data/dataset.py` & `thingsvision-2.6.7/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/data/helpers.py` & `thingsvision-2.6.7/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.6.7/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.6.7/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.6.7/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/mae/utils.py` & `thingsvision-2.6.7/thingsvision/utils/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/mae/vit_mae.py` & `thingsvision-2.6.7/thingsvision/utils/models/mae/vit_mae.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/sam/common.py` & `thingsvision-2.6.7/thingsvision/utils/models/sam/common.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/models/sam/image_encoder.py` & `thingsvision-2.6.7/thingsvision/utils/models/sam/image_encoder.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision/utils/storing/helpers.py` & `thingsvision-2.6.7/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.6/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.6.7/thingsvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.6
+Version: 2.6.7
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.6 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.7 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.6.6/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.6.7/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

