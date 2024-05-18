# Comparing `tmp/mychamp-0.0.0.tar.gz` & `tmp/mychamp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mychamp-0.0.0.tar", last modified: Tue Aug 29 18:13:58 2023, max compression
+gzip compressed data, was "mychamp-0.0.2.tar", last modified: Sat May 18 21:58:43 2024, max compression
```

## Comparing `mychamp-0.0.0.tar` & `mychamp-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,59 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-29 18:13:58.041757 mychamp-0.0.0/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1071 2023-08-29 17:48:19.000000 mychamp-0.0.0/LICENSE
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      172 2023-08-29 18:13:58.041757 mychamp-0.0.0/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     8049 2023-08-29 17:48:50.000000 mychamp-0.0.0/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-29 18:13:58.041757 mychamp-0.0.0/machop/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       84 2023-08-29 17:48:19.000000 mychamp-0.0.0/machop/__main__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      301 2023-08-29 17:48:19.000000 mychamp-0.0.0/machop/main.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2023-08-29 18:13:58.041757 mychamp-0.0.0/mychamp.egg-info/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      172 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      254 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       58 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/entry_points.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        6 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        7 2023-08-29 18:13:58.000000 mychamp-0.0.0/mychamp.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      409 2023-08-29 18:13:46.000000 mychamp-0.0.0/pyproject.toml
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2023-08-29 18:13:58.041757 mychamp-0.0.0/setup.cfg
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1168 2024-05-16 23:57:35.000000 mychamp-0.0.2/LICENSE
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       55 2024-05-18 21:58:40.000000 mychamp-0.0.2/MANIFEST.in
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)     1327 2024-05-18 21:58:43.677727 mychamp-0.0.2/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      934 2024-05-18 21:57:31.000000 mychamp-0.0.2/README.md
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.581728 mychamp-0.0.2/mychamp/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 23:25:03.000000 mychamp-0.0.2/mychamp/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      553 2024-05-18 21:53:16.000000 mychamp-0.0.2/mychamp/__main__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.581728 mychamp-0.0.2/mychamp/data/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-16 23:25:03.000000 mychamp-0.0.2/mychamp/data/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       82 2024-05-16 23:25:03.000000 mychamp-0.0.2/mychamp/data/quote.txt
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.669727 mychamp-0.0.2/mychamp/machamp/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/__init__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.669727 mychamp-0.0.2/mychamp/machamp/dataset_readers/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      155 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      927 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/basic_tokenizer.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     3944 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/lemma_edit.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    25511 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/machamp_universal_reader.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     3058 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/reader_utils.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     7719 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/dataset_readers/sequence_multilabel_field.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.673727 mychamp-0.0.2/mychamp/machamp/metrics/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       50 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/metrics/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    14951 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/metrics/multi_span_based_f1_measure.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1075 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/metrics/perplexity.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.673727 mychamp-0.0.2/mychamp/machamp/models/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      497 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    10720 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/crf_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    28080 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/dependency_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    10144 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/machamp_model.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     6112 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/mlm_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    21698 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/multiseq_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     5145 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/sentence_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    23655 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/seq2seq_decoder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     7302 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/models/tag_decoder.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/mychamp/machamp/modules/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      394 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/modules/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    11335 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/modules/bucket_batch_sampler.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)    16203 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/modules/pretrained_transformer_embedder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     4769 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/modules/pretrained_transformer_mismatched_embedder.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     5483 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/modules/pretrained_transformer_mixmatched_indexer.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/mychamp/machamp/predictor/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       57 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/predictor/__init__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     5341 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/predictor/predictor.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     9431 2024-05-17 01:38:52.000000 mychamp-0.0.2/mychamp/machamp/util.py
+-rw-------   0 jstrieb   (1012) jstrieb   (1012)     1086 2024-05-17 03:00:05.000000 mychamp-0.0.2/mychamp/meta.py
+-rwx------   0 jstrieb   (1012) jstrieb   (1012)     1420 2024-05-18 21:55:03.000000 mychamp-0.0.2/mychamp/meta.sh
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/mychamp/predict/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     4311 2024-05-17 02:26:57.000000 mychamp-0.0.2/mychamp/predict/__main__.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/mychamp/train/
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     4085 2024-05-18 06:10:16.000000 mychamp-0.0.2/mychamp/train/__main__.py
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     4482 2024-05-18 03:10:55.000000 mychamp-0.0.2/mychamp/train/arguments.py
+drwxrwxr-x   0 jstrieb   (1012) jstrieb   (1012)        0 2024-05-18 21:58:43.677727 mychamp-0.0.2/mychamp.egg-info/
+-rw-r--r--   0 jstrieb   (1012) jstrieb   (1012)     1327 2024-05-18 21:58:43.000000 mychamp-0.0.2/mychamp.egg-info/PKG-INFO
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)     1625 2024-05-18 21:58:43.000000 mychamp-0.0.2/mychamp.egg-info/SOURCES.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        1 2024-05-18 21:58:43.000000 mychamp-0.0.2/mychamp.egg-info/dependency_links.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)       50 2024-05-18 21:58:43.000000 mychamp-0.0.2/mychamp.egg-info/entry_points.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)        8 2024-05-18 21:58:43.000000 mychamp-0.0.2/mychamp.egg-info/top_level.txt
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      557 2024-05-18 21:58:40.000000 mychamp-0.0.2/pyproject.toml
+-rw-rw-r--   0 jstrieb   (1012) jstrieb   (1012)      152 2024-05-18 21:58:43.677727 mychamp-0.0.2/setup.cfg
```

### Comparing `mychamp-0.0.0/LICENSE` & `mychamp-0.0.2/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 MIT License
 
-Copyright (c) 2023 Jacob Striebel
+Copyright (c) 2024 Jacob Striebel
+Copyright (c) 2020 Rob van der Goot, Ahmet Ustun, Alan Ramponi
+Copyright (c) 2019 Dan Kondratyuk
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

