# Comparing `tmp/webscout-2.6.tar.gz` & `tmp/webscout-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.6.tar", last modified: Wed May 15 14:23:29 2024, max compression
+gzip compressed data, was "webscout-2.7.tar", last modified: Sun May 19 15:12:42 2024, max compression
```

## Comparing `webscout-2.6.tar` & `webscout-2.7.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.309273 webscout-2.6/
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.529805 webscout-2.6/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.580652 webscout-2.6/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.660368 webscout-2.6/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:27.682370 webscout-2.6/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.6/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.6/LICENSE.md
--rw-rw-rw-   0        0        0    47429 2024-05-15 14:23:29.279272 webscout-2.6/PKG-INFO
--rw-rw-rw-   0        0        0    44977 2024-05-14 14:17:49.000000 webscout-2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 14:23:29.309273 webscout-2.6/setup.cfg
--rw-rw-rw-   0        0        0     2723 2024-05-15 14:22:40.000000 webscout-2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:28.112112 webscout-2.6/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.6/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.6/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.6/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.6/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.6/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:28.352353 webscout-2.6/webscout/Local/
--rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.6/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-14 08:49:56.000000 webscout-2.6/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    16644 2024-05-15 04:24:04.000000 webscout-2.6/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    27611 2024-05-13 10:21:04.000000 webscout-2.6/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.6/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    26788 2024-05-14 08:49:17.000000 webscout-2.6/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.6/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.248271 webscout-2.6/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.6/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.6/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.6/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.6/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.6/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.6/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.6/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.6/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.6/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.6/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.6/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.6/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.6/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.6/webscout/Provider/Poe.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.6/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.6/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.6/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.6/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.6/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1348 2024-05-14 14:09:14.000000 webscout-2.6/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     1836 2024-05-14 14:10:37.000000 webscout-2.6/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.6/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.6/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.6/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.6/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.6/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.6/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.6/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.6/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.6/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.6/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.6/webscout/voice.py
--rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.6/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.6/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.6/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:23:29.261275 webscout-2.6/webscout.egg-info/
--rw-rw-rw-   0        0        0    47429 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1797 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-15 14:23:26.000000 webscout-2.6/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.745495 webscout-2.7/
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:41.857682 webscout-2.7/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:41.944679 webscout-2.7/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.080212 webscout-2.7/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.114214 webscout-2.7/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.7/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.7/LICENSE.md
+-rw-rw-rw-   0        0        0    47655 2024-05-19 15:12:42.739491 webscout-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:12:42.746490 webscout-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2723 2024-05-19 14:34:53.000000 webscout-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.286992 webscout-2.7/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.7/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.7/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33256 2024-05-14 14:10:47.000000 webscout-2.7/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.7/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.7/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.384003 webscout-2.7/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-2.7/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-19 14:47:10.000000 webscout-2.7/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    18994 2024-05-19 14:40:00.000000 webscout-2.7/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    27618 2024-05-19 14:42:26.000000 webscout-2.7/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-2.7/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    26925 2024-05-19 14:44:26.000000 webscout-2.7/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6108 2024-05-14 05:14:09.000000 webscout-2.7/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.713469 webscout-2.7/webscout/Provider/
+-rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-2.7/webscout/Provider/BasedGPT.py
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.7/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.7/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.7/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.7/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.7/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.7/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.7/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.7/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.7/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.7/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.7/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.7/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.7/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-2.7/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.7/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.7/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.7/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.7/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.7/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1372 2024-05-16 04:09:11.000000 webscout-2.7/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1840 2024-05-19 14:59:15.000000 webscout-2.7/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.7/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.7/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-2.7/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.7/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.7/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.7/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.7/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.7/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.7/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-19 14:37:31.000000 webscout-2.7/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.7/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-2.7/webscout/webai.py
+-rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-2.7/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-2.7/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:12:42.721488 webscout-2.7/webscout.egg-info/
+-rw-rw-rw-   0        0        0    47655 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-05-19 15:12:41.000000 webscout-2.7/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      379 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 15:12:40.000000 webscout-2.7/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.6/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.7/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.7/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/networks/filepath_converter.py` & `webscout-2.7/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/networks/google_searcher.py` & `webscout-2.7/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/networks/network_configs.py` & `webscout-2.7/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.7/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/utilsdw/enver.py` & `webscout-2.7/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/DeepWEBS/utilsdw/logger.py` & `webscout-2.7/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/LICENSE.md` & `webscout-2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.6/PKG-INFO` & `webscout-2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.6
+Version: 2.7
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -105,39 +105,42 @@
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
-    - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-    - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
-    - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
+    - [1. `text()` - text search by DuckDuckGo.com](#1-text---text-search-by-duckduckgocom)
+    - [2. `answers()` - instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-duckduckgocom)
+    - [3. `images()` - image search by DuckDuckGo.com](#3-images---image-search-by-duckduckgocom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
-    - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
-    - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
-    - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
-    - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
+    - [5. `news()` - news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom)
+    - [6. `maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+    - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---translation-by-duckduckgocom)
+    - [8. `suggestions()` - suggestions by DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom)
   - [ALL acts](#all-acts)
   - [Webscout Supported Acts:](#webscout-supported-acts)
   - [usage of webscout AI](#usage-of-webscout-ai)
+    - [0. `Duckchat` - chat with LLM](#0-duckchat---chat-with-llm)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-berlin4h)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
+    - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
+    - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
@@ -521,45 +524,45 @@
 ## Exceptions
 
 Exceptions:
 - `WebscoutE`: Raised when there is a generic exception during the API request.
 
 ## usage of webscout
 
-### 1. `text()` - text search by DuckDuckGo.com and Yep.com
+### 1. `text()` - text search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Text search for 'live free or die' using DuckDuckGo.com and Yep.com
+# Text search for 'live free or die' using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 ```
 
-### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com
+### 2. `answers()` - instant answers by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Instant answers for the query "sun" using DuckDuckGo.com and Yep.com
+# Instant answers for the query "sun" using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.answers("sun"):
         print(r)
 ```
 
-### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+### 3. `images()` - image search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
+# Image search for the keyword 'butterfly' using DuckDuckGo.com 
 with WEBS() as WEBS:
     keywords = 'butterfly'
     WEBS_images_gen = WEBS.images(
       keywords,
       region="wt-wt",
       safesearch="off",
       size=None,
@@ -589,15 +592,15 @@
       duration="medium",
       max_results=10,
     )
     for r in WEBS_videos_gen:
         print(r)
 ```
 
-### 5. `news()` - news search by DuckDuckGo.com and yep.com
+### 5. `news()` - news search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 import datetime
 
 def fetch_news(keywords, timelimit):
     news_list = []
@@ -636,43 +639,43 @@
 
 # Format and print the headlines
 formatted_headlines = _format_headlines(news_list)
 print(formatted_headlines)
 
 ```
 
-### 6. `maps()` - map search by DuckDuckGo.com and
+### 6. `maps()` - map search by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
 # Map search for the keyword 'school' in 'anantnag' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.maps("school", place="anantnag", max_results=50):
         print(r)
 ```
 
-### 7. `translate()` - translation by DuckDuckGo.com and Yep.com
+### 7. `translate()` - translation by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and Yep.com
+# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com
 with WEBS() as WEBS:
     keywords = 'school'
     r = WEBS.translate(keywords, to="hi")
     print(r)
 ```
 
-### 8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com
+### 8. `suggestions()` - suggestions by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
+# Suggestions for the keyword 'fly' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
 ## ALL acts
 <details>
   <summary>expand</summary>
@@ -927,15 +930,20 @@
 246. League of Legends Player
 
 **Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
 ___
 </details>
 
 ## usage of webscout AI
-
+### 0. `Duckchat` - chat with LLM
+```python
+from webscout import WEBS as w
+R = w().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo
+print(R)
+```
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
 from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
@@ -1195,15 +1203,21 @@
     act=None,
 )
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = ai.chat(prompt)
 print(response)
+
 ```
+### 15. `poe`- chat with poe
+Usage code similar to other proviers
+
+### 16. `BasedGPT` - chat with GPT
+Usage code similar to other providers
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.6 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.7 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -44,113 +44,115 @@
    and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
   [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
  advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
 to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
    - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
  [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
     [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
-DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
- -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
- by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
- yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
-  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
- yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
-map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
-[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
-translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
-DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
-    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
-     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
-`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
-- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
-   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
-   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
- google gemini](#4-gemini---search-with-google-gemini) - [5. `Berlin4h` - chat
-with Berlin4h](#5-berlin4h---chat-with-berlin4h) - [6. `BlackBox` - Search/chat
-  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
-Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
- - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
- koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
-  `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
- chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
- AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
-[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
-gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
-(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
+  DuckDuckGo.com](#1-text---text-search-by-duckduckgocom) - [2. `answers()` -
+      instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-
+duckduckgocom) - [3. `images()` - image search by DuckDuckGo.com](#3-images---
+       image-search-by-duckduckgocom) - [4. `videos()` - video search by
+  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
+ news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom) - [6.
+`maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+     - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---
+     translation-by-duckduckgocom) - [8. `suggestions()` - suggestions by
+  DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom) - [ALL acts]
+(#all-acts) - [Webscout Supported Acts:](#webscout-supported-acts) - [usage of
+   webscout AI](#usage-of-webscout-ai) - [0. `Duckchat` - chat with LLM](#0-
+  duckchat---chat-with-llm) - [1. `PhindSearch` - Search using Phind.com](#1-
+ phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
+powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
+[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
+   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
+    gemini) - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-
+    berlin4h) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
+  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
+ perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
+opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-koboldai--) - [10. `Reka` -
+chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere]
+ (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
+   xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
+ thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
+ chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
+ with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
+  [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
+webscout-can-now-run-gguf-models) - [`LLM` with internet](#llm-with-internet) -
+ [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open
+ interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python
+pip install -U webscout ``` ## CLI version ```python3 python -m webscout --help
+``` | Command | Description | |-------------------------------------------|----
 -------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
- ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
-au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
-(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
-ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
-Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
-  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
-Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
- (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
- for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
-for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
-en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
-for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
-ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
-za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
- (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
-th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
-us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
-  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
-number ### Temp number ```python from rich.console import Console from webscout
-             import tempid def main(): console = Console() phone =
-    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
-   specific country (or random) number = phone.get_number(country="Finland")
-console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
-# Pause execution briefly (replace with your actual logic) # import time module
- import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
-  print messages messages = phone.get_messages(number) if messages: # Access
-   individual messages using indexing: console.print(f"[bold green]{messages
- [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
- messages) else: console.print("No messages received.") except Exception as e:
- console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
-   main() ``` ### Tempmail ```python import asyncio from rich.console import
- Console from rich.table import Table from rich.text import Text from webscout
-     import tempid async def main() -> None: console = Console() client =
-   tempid.Client() try: domains = await client.get_domains() if not domains:
-console.print("[bold red]No domains available. Please try again later.") return
-email = await client.create_email(domain=domains[0].name) console.print(f"Your
- temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
-  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
-  messages = await client.get_messages(email.email) if messages is not None:
-break if messages: table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("From", style="bold cyan") table.add_column("Subject",
- style="bold yellow") table.add_column("Body", style="bold green") for message
- in messages: body_preview = Text(message.body_text if message.body_text else
- "No body") table.add_row(message.email_from or "Unknown", message.subject or
-   "No Subject", body_preview) console.print(table) else: console.print("No
-  messages found.") except Exception as e: console.print(f"[bold red]An error
-   occurred: {e}") finally: await client.close() if __name__ == '__main__':
-asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
-     a handy tool that transcribes YouTube videos. Here's an example code
-demonstrating its usage: ```python import sys from webscout import transcriber
-  def extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ --------------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+ | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en)
+ ar-es for Argentina au-en for Australia at-de for Austria be-fr for Belgium
+   (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for
+Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China
+co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark
+ ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el
+  for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for
+Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for
+Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-
+   es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
+ rich.console import Console from webscout import tempid def main(): console =
+ Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
+      number for a specific country (or random) number = phone.get_number
+ (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
+  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
+  logic) # import time module import time time.sleep(30) # Adjust the waiting
+  time as needed # Retrieve and print messages messages = phone.get_messages
+      (number) if messages: # Access individual messages using indexing:
+ console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
+   (Add more lines if you expect multiple messages) else: console.print("No
+messages received.") except Exception as e: console.print(f"[bold red]An error
+ occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
+ import asyncio from rich.console import Console from rich.table import Table
+   from rich.text import Text from webscout import tempid async def main() -
+   > None: console = Console() client = tempid.Client() try: domains = await
+   client.get_domains() if not domains: console.print("[bold red]No domains
+ available. Please try again later.") return email = await client.create_email
+  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
+  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
+      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
+ client.get_messages(email.email) if messages is not None: break if messages:
+ table = Table(show_header=True, header_style="bold magenta") table.add_column
+ ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
+     table.add_column("Body", style="bold green") for message in messages:
+  body_preview = Text(message.body_text if message.body_text else "No body")
+table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
+ body_preview) console.print(table) else: console.print("No messages found.")
+   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
+ finally: await client.close() if __name__ == '__main__': asyncio.run(main())
+ ``` ## Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -224,124 +226,125 @@
 chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
  await main() ``` It is important to note that the WEBS and AsyncWEBS classes
    should always be used as a context manager (with statement). This ensures
       proper resource management and cleanup, as the context manager will
     automatically handle opening and closing the HTTP client connection. ##
 Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
  during the API request. ## usage of webscout ### 1. `text()` - text search by
- DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
- for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
-   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
- ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
-     from webscout import WEBS # Instant answers for the query "sun" using
- DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
-  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
-```python from webscout import WEBS # Image search for the keyword 'butterfly'
- using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
-  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
-size=None, type_image=None, layout=None, license_image=None, max_results=10, )
-  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
-   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
- keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
-  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
-timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
- WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
-and yep.com ```python from webscout import WEBS import datetime def fetch_news
-      (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
-WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
-  timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
-          date to a human-readable format using datetime r['date'] =
+DuckDuckGo.com ```python from webscout import WEBS # Text search for 'live free
+or die' using DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.text('live free
+  or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
+        print(r) for r in WEBS.text('live free or die', region='wt-wt',
+safesearch='off', timelimit='y', max_results=10): print(r) ``` ### 2. `answers
+ ()` - instant answers by DuckDuckGo.com ```python from webscout import WEBS #
+ Instant answers for the query "sun" using DuckDuckGo.com with WEBS() as WEBS:
+for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` - image search by
+   DuckDuckGo.com ```python from webscout import WEBS # Image search for the
+   keyword 'butterfly' using DuckDuckGo.com with WEBS() as WEBS: keywords =
+     'butterfly' WEBS_images_gen = WEBS.images( keywords, region="wt-wt",
+safesearch="off", size=None, type_image=None, layout=None, license_image=None,
+ max_results=10, ) for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` -
+  video search by DuckDuckGo.com ```python from webscout import WEBS # Video
+   search for the keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS:
+  keywords = 'tesla' WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt",
+    safesearch="off", timelimit="w", resolution="high", duration="medium",
+max_results=10, ) for r in WEBS_videos_gen: print(r) ``` ### 5. `news()` - news
+ search by DuckDuckGo.com ```python from webscout import WEBS import datetime
+      def fetch_news(keywords, timelimit): news_list = [] with WEBS() as
+ webs_instance: WEBS_news_gen = webs_instance.news( keywords, region="wt-wt",
+safesearch="off", timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen:
+   # Convert the date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
      news_list.append(r) return news_list def _format_headlines(news_list,
    max_headlines: int = 100): headlines = [] for idx, news_item in enumerate
    (news_list): if idx >= max_headlines: break new_headline = f"{idx + 1}.
 {news_item['title'].strip()} " new_headline += f"(URL: {news_item['url'].strip
   ()}) " new_headline += f"{news_item['body'].strip()}" new_headline += "\n"
     headlines.append(new_headline) headlines = "\n".join(headlines) return
 headlines # Example usage keywords = 'latest AI news' timelimit = 'd' news_list
       = fetch_news(keywords, timelimit) # Format and print the headlines
  formatted_headlines = _format_headlines(news_list) print(formatted_headlines)
-``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from webscout
+  ``` ### 6. `maps()` - map search by DuckDuckGo.com ```python from webscout
      import WEBS # Map search for the keyword 'school' in 'anantnag' using
        DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.maps("school",
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
-translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
- Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
- Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
- to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
- and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
-       'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
-  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
-    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
-Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
- Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
-  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
- Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
- 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
-Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
-Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
- Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
-Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
-  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
- Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
-    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
-Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
- 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
-Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
-SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
-    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
- Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
- 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
-Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
- 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
-Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
-Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
-97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
-  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
-Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
- Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
-   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
-  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
- Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
-    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
-  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
-  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
-   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
-Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
- Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
-  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
- Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
-written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
-Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
-Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
-  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
- ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
- 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
-Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
-170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
-  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
-   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
-Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
-  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
-196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
-201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
-  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
- 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
-  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
-  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
- Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
-233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
-239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
-  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
-  Some "acts" use placeholders like `position` or `language` which should be
-replaced with a specific value when using the prompt. ___ ## usage of webscout
-AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
+translation by DuckDuckGo.com ```python from webscout import WEBS # Translation
+ of the keyword 'school' to German ('hi') using DuckDuckGo.com with WEBS() as
+ WEBS: keywords = 'school' r = WEBS.translate(keywords, to="hi") print(r) ```
+### 8. `suggestions()` - suggestions by DuckDuckGo.com ```python from webscout
+import WEBS # Suggestions for the keyword 'fly' using DuckDuckGo.com with WEBS
+ () as WEBS: for r in WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand
+     ## Webscout Supported Acts: 1. Free-mode 2. Linux Terminal 3. English
+  Translator and Improver 4. `position` Interviewer 5. JavaScript Console 6.
+   Excel Sheet 7. English Pronunciation Helper 8. Spoken English Teacher and
+Improver 9. Travel Guide 10. Plagiarism Checker 11. Character from Movie/Book/
+ Anything 12. Advertiser 13. Storyteller 14. Football Commentator 15. Stand-up
+ Comedian 16. Motivational Coach 17. Composer 18. Debater 19. Debate Coach 20.
+Screenwriter 21. Novelist 22. Movie Critic 23. Relationship Coach 24. Poet 25.
+Rapper 26. Motivational Speaker 27. Philosophy Teacher 28. Philosopher 29. Math
+Teacher 30. AI Writing Tutor 31. UX/UI Developer 32. Cyber Security Specialist
+33. Recruiter 34. Life Coach 35. Etymologist 36. Commentariat 37. Magician 38.
+  Career Counselor 39. Pet Behaviorist 40. Personal Trainer 41. Mental Health
+   Adviser 42. Real Estate Agent 43. Logistician 44. Dentist 45. Web Design
+   Consultant 46. AI Assisted Doctor 47. Doctor 48. Accountant 49. Chef 50.
+  Automobile Mechanic 51. Artist Advisor 52. Financial Analyst 53. Investment
+ Manager 54. Tea-Taster 55. Interior Decorator 56. Florist 57. Self-Help Book
+ 58. Gnomist 59. Aphorism Book 60. Text Based Adventure Game 61. AI Trying to
+Escape the Box 62. Fancy Title Generator 63. Statistician 64. Prompt Generator
+65. Instructor in a School 66. SQL terminal 67. Dietitian 68. Psychologist 69.
+     Smart Domain Name Generator 70. Tech Reviewer 71. Developer Relations
+  consultant 72. Academician 73. IT Architect 74. Lunatic 75. Gaslighter 76.
+Fallacy Finder 77. Journal Reviewer 78. DIY Expert 79. Social Media Influencer
+  80. Socrat 81. Socratic Method 82. Educational Content Creator 83. Yogi 84.
+  Essay Writer 85. Social Media Manager 86. Elocutionist 87. Scientific Data
+   Visualizer 88. Car Navigation System 89. Hypnotherapist 90. Historian 91.
+  Astrologer 92. Film Critic 93. Classical Music Composer 94. Journalist 95.
+   Digital Art Gallery Guide 96. Public Speaking Coach 97. Makeup Artist 98.
+   Babysitter 99. Tech Writer 100. Ascii Artist 101. Python interpreter 102.
+Synonym finder 103. Personal Shopper 104. Food Critic 105. Virtual Doctor 106.
+ Personal Chef 107. Legal Advisor 108. Personal Stylist 109. Machine Learning
+ Engineer 110. Biblical Translator 111. SVG designer 112. IT Expert 113. Chess
+Player 114. Midjourney Prompt Generator 115. Fullstack Software Developer 116.
+     Mathematician 117. Regex Generator 118. Time Travel Guide 119. Dream
+Interpreter 120. Talent Coach 121. R programming Interpreter 122. StackOverflow
+    Post 123. Emoji Translator 124. PHP Interpreter 125. Emergency Response
+Professional 126. Fill in the Blank Worksheets Generator 127. Software Quality
+    Assurance Tester 128. Tic-Tac-Toe Game 129. Password Generator 130. New
+  Language Creator 131. Web Browser 132. Senior Frontend Developer 133. Solr
+ Search Engine 134. Startup Idea Generator 135. Spongebob's Magic Conch Shell
+  136. Language Detector 137. Salesperson 138. Commit Message Generator 139.
+Chief Executive Officer 140. Diagram Generator 141. Speech-Language Pathologist
+  (SLP) 142. Startup Tech Lawyer 143. Title Generator for written pieces 144.
+ Product Manager 145. Drunk Person 146. Mathematical History Teacher 147. Song
+Recommender 148. Cover Letter 149. Technology Transferer 150. Unconstrained AI
+model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154. Muslim imam 155.
+   Chemical reactor 156. Friend 157. Python Interpreter 158. ChatGPT prompt
+generator 159. Wikipedia page 160. Japanese Kanji quiz machine 161. note-taking
+assistant 162. `language` Literary Critic 163. Cheap Travel Ticket Advisor 164.
+DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE 170. Mongo Tom 171.
+ LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN 177. FunnyGPT 178.
+ CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182. Evil Confidant 183.
+DAN 8.6 184. Hypothetical response 185. BH 186. Text Continuation 187. Dude v3
+188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2 191. DevMode + Ranti 192.
+ KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6 196. 3-Liner 197. M78 198.
+ Maximum 199. BasedGPT 200. Confronting personalities 201. Ron 202. UnGPT 203.
+BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF 208. NECO 209. MAN 210.
+ Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1 214. Universal Jailbreak
+     215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned 219. VIOLET 220.
+TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr. Blonde 224. New DAN
+225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind Trick 229. DAN 9.0 230.
+  Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight 233. LiveGPT 234. DAN
+Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies 239. OMNI 240. Burple
+241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244. Prompt Enhancer 245.
+    Data Scientist 246. League of Legends Player **Note:** Some "acts" use
+  placeholders like `position` or `language` which should be replaced with a
+   specific value when using the prompt. ___ ## usage of webscout AI ### 0.
+   `Duckchat` - chat with LLM ```python from webscout import WEBS as w R = w
+ ().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo print(R) ``` ### 1.
+     `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
   by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
@@ -407,52 +410,53 @@
      (prompt) # Extract and print the message from the response message =
   ai.get_message(response) print(message) ``` ### 14. `chatgptuk` - Chat with
 gemini-pro ```python from webscout import ChatGPTUK # Create an instance of the
     PERPLEXITY class ai = ChatGPTUK( is_conversation=True, max_tokens=800,
      timeout=30, intro=None, filepath=None, update_file=True, proxies={},
    history_offset=10250, act=None, ) # Example usage: prompt = "Explain the
     concept of recursion in simple terms." response = ai.chat(prompt) print
-  (response) ``` ### `LLM` ```python from webscout.LLM import LLM # Read the
-      system message from the file with open('system.txt', 'r') as file:
-system_message = file.read() # Initialize the LLM class with the model name and
-         system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-        ### `Local-LLM` webscout can now run GGUF models ```python from
-  webscout.Local.utils import download_model from webscout.Local.model import
-   Model from webscout.Local.thread import Thread from webscout.Local import
- formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
- gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
-      instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
- `LLM` with internet ```python from __future__ import annotations from typing
- import List, Optional from webscout.LLM import LLM from webscout import WEBS
-   import warnings system_message: str = ( "As an AI assistant, I have been
-   designed with advanced capabilities, including real-time access to online
-  resources. This enables me to enrich our conversations and provide you with
-informed and accurate responses, drawing from a vast array of information. With
- each interaction, my goal is to create a seamless and meaningful connection,
- offering insights and sharing relevant content." "My directives emphasize the
- importance of respect, impartiality, and intellectual integrity. I am here to
-provide unbiased responses, ensuring an ethical and respectful exchange. I will
-respect your privacy and refrain from sharing any personal information that may
- be obtained during our conversations or through web searches, only utilizing
-web search functionality when necessary to provide the most accurate and up-to-
-date information." "Together, let's explore a diverse range of topics, creating
-  an enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
- warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+    (response) ``` ### 15. `poe`- chat with poe Usage code similar to other
+    proviers ### 16. `BasedGPT` - chat with GPT Usage code similar to other
+ providers ### `LLM` ```python from webscout.LLM import LLM # Read the system
+ message from the file with open('system.txt', 'r') as file: system_message =
+ file.read() # Initialize the LLM class with the model name and system message
+ llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+  while True: # Get the user input user_input = input("User: ") # Define the
+ messages to be sent messages = [ {"role": "user", "content": user_input} ] #
+Use the mistral_chat method to get the response response = llm.chat(messages) #
+Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+thread.interact() ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
```

### Comparing `webscout-2.6/README.md` & `webscout-2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,39 +43,42 @@
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
-    - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-    - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
-    - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
+    - [1. `text()` - text search by DuckDuckGo.com](#1-text---text-search-by-duckduckgocom)
+    - [2. `answers()` - instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-duckduckgocom)
+    - [3. `images()` - image search by DuckDuckGo.com](#3-images---image-search-by-duckduckgocom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
-    - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
-    - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
-    - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
-    - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
+    - [5. `news()` - news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom)
+    - [6. `maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+    - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---translation-by-duckduckgocom)
+    - [8. `suggestions()` - suggestions by DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom)
   - [ALL acts](#all-acts)
   - [Webscout Supported Acts:](#webscout-supported-acts)
   - [usage of webscout AI](#usage-of-webscout-ai)
+    - [0. `Duckchat` - chat with LLM](#0-duckchat---chat-with-llm)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-berlin4h)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
+    - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
+    - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
@@ -459,45 +462,45 @@
 ## Exceptions
 
 Exceptions:
 - `WebscoutE`: Raised when there is a generic exception during the API request.
 
 ## usage of webscout
 
-### 1. `text()` - text search by DuckDuckGo.com and Yep.com
+### 1. `text()` - text search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Text search for 'live free or die' using DuckDuckGo.com and Yep.com
+# Text search for 'live free or die' using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 ```
 
-### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com
+### 2. `answers()` - instant answers by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Instant answers for the query "sun" using DuckDuckGo.com and Yep.com
+# Instant answers for the query "sun" using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.answers("sun"):
         print(r)
 ```
 
-### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+### 3. `images()` - image search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
+# Image search for the keyword 'butterfly' using DuckDuckGo.com 
 with WEBS() as WEBS:
     keywords = 'butterfly'
     WEBS_images_gen = WEBS.images(
       keywords,
       region="wt-wt",
       safesearch="off",
       size=None,
@@ -527,15 +530,15 @@
       duration="medium",
       max_results=10,
     )
     for r in WEBS_videos_gen:
         print(r)
 ```
 
-### 5. `news()` - news search by DuckDuckGo.com and yep.com
+### 5. `news()` - news search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 import datetime
 
 def fetch_news(keywords, timelimit):
     news_list = []
@@ -574,43 +577,43 @@
 
 # Format and print the headlines
 formatted_headlines = _format_headlines(news_list)
 print(formatted_headlines)
 
 ```
 
-### 6. `maps()` - map search by DuckDuckGo.com and
+### 6. `maps()` - map search by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
 # Map search for the keyword 'school' in 'anantnag' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.maps("school", place="anantnag", max_results=50):
         print(r)
 ```
 
-### 7. `translate()` - translation by DuckDuckGo.com and Yep.com
+### 7. `translate()` - translation by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and Yep.com
+# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com
 with WEBS() as WEBS:
     keywords = 'school'
     r = WEBS.translate(keywords, to="hi")
     print(r)
 ```
 
-### 8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com
+### 8. `suggestions()` - suggestions by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
+# Suggestions for the keyword 'fly' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
 ## ALL acts
 <details>
   <summary>expand</summary>
@@ -865,15 +868,20 @@
 246. League of Legends Player
 
 **Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
 ___
 </details>
 
 ## usage of webscout AI
-
+### 0. `Duckchat` - chat with LLM
+```python
+from webscout import WEBS as w
+R = w().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo
+print(R)
+```
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
 from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
@@ -1133,15 +1141,21 @@
     act=None,
 )
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = ai.chat(prompt)
 print(response)
+
 ```
+### 15. `poe`- chat with poe
+Usage code similar to other proviers
+
+### 16. `BasedGPT` - chat with GPT
+Usage code similar to other providers
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -12,113 +12,115 @@
    and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
   [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
  advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
 to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
    - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
  [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
     [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
-DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
- -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
- by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
- yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
-  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
- yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
-map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
-[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
-translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
-DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
-    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
-     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
-`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
-- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
-   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
-   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
- google gemini](#4-gemini---search-with-google-gemini) - [5. `Berlin4h` - chat
-with Berlin4h](#5-berlin4h---chat-with-berlin4h) - [6. `BlackBox` - Search/chat
-  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
-Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
- - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
- koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
-  `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
- chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
- AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
-[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
-gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
-(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
+  DuckDuckGo.com](#1-text---text-search-by-duckduckgocom) - [2. `answers()` -
+      instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-
+duckduckgocom) - [3. `images()` - image search by DuckDuckGo.com](#3-images---
+       image-search-by-duckduckgocom) - [4. `videos()` - video search by
+  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
+ news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom) - [6.
+`maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+     - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---
+     translation-by-duckduckgocom) - [8. `suggestions()` - suggestions by
+  DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom) - [ALL acts]
+(#all-acts) - [Webscout Supported Acts:](#webscout-supported-acts) - [usage of
+   webscout AI](#usage-of-webscout-ai) - [0. `Duckchat` - chat with LLM](#0-
+  duckchat---chat-with-llm) - [1. `PhindSearch` - Search using Phind.com](#1-
+ phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
+powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
+[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
+   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
+    gemini) - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-
+    berlin4h) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
+  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
+ perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
+opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-koboldai--) - [10. `Reka` -
+chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere]
+ (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
+   xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
+ thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
+ chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
+ with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
+  [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
+webscout-can-now-run-gguf-models) - [`LLM` with internet](#llm-with-internet) -
+ [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open
+ interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python
+pip install -U webscout ``` ## CLI version ```python3 python -m webscout --help
+``` | Command | Description | |-------------------------------------------|----
 -------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
- ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
-au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
-(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
-ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
-Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
-  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
-Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
- (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
- for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
-for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
-en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
-for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
-ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
-za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
- (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
-th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
-us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
-  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
-number ### Temp number ```python from rich.console import Console from webscout
-             import tempid def main(): console = Console() phone =
-    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
-   specific country (or random) number = phone.get_number(country="Finland")
-console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
-# Pause execution briefly (replace with your actual logic) # import time module
- import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
-  print messages messages = phone.get_messages(number) if messages: # Access
-   individual messages using indexing: console.print(f"[bold green]{messages
- [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
- messages) else: console.print("No messages received.") except Exception as e:
- console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
-   main() ``` ### Tempmail ```python import asyncio from rich.console import
- Console from rich.table import Table from rich.text import Text from webscout
-     import tempid async def main() -> None: console = Console() client =
-   tempid.Client() try: domains = await client.get_domains() if not domains:
-console.print("[bold red]No domains available. Please try again later.") return
-email = await client.create_email(domain=domains[0].name) console.print(f"Your
- temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
-  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
-  messages = await client.get_messages(email.email) if messages is not None:
-break if messages: table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("From", style="bold cyan") table.add_column("Subject",
- style="bold yellow") table.add_column("Body", style="bold green") for message
- in messages: body_preview = Text(message.body_text if message.body_text else
- "No body") table.add_row(message.email_from or "Unknown", message.subject or
-   "No Subject", body_preview) console.print(table) else: console.print("No
-  messages found.") except Exception as e: console.print(f"[bold red]An error
-   occurred: {e}") finally: await client.close() if __name__ == '__main__':
-asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
-     a handy tool that transcribes YouTube videos. Here's an example code
-demonstrating its usage: ```python import sys from webscout import transcriber
-  def extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ --------------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+ | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en)
+ ar-es for Argentina au-en for Australia at-de for Austria be-fr for Belgium
+   (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for
+Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China
+co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark
+ ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el
+  for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for
+Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for
+Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-
+   es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
+ rich.console import Console from webscout import tempid def main(): console =
+ Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
+      number for a specific country (or random) number = phone.get_number
+ (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
+  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
+  logic) # import time module import time time.sleep(30) # Adjust the waiting
+  time as needed # Retrieve and print messages messages = phone.get_messages
+      (number) if messages: # Access individual messages using indexing:
+ console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
+   (Add more lines if you expect multiple messages) else: console.print("No
+messages received.") except Exception as e: console.print(f"[bold red]An error
+ occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
+ import asyncio from rich.console import Console from rich.table import Table
+   from rich.text import Text from webscout import tempid async def main() -
+   > None: console = Console() client = tempid.Client() try: domains = await
+   client.get_domains() if not domains: console.print("[bold red]No domains
+ available. Please try again later.") return email = await client.create_email
+  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
+  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
+      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
+ client.get_messages(email.email) if messages is not None: break if messages:
+ table = Table(show_header=True, header_style="bold magenta") table.add_column
+ ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
+     table.add_column("Body", style="bold green") for message in messages:
+  body_preview = Text(message.body_text if message.body_text else "No body")
+table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
+ body_preview) console.print(table) else: console.print("No messages found.")
+   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
+ finally: await client.close() if __name__ == '__main__': asyncio.run(main())
+ ``` ## Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -192,124 +194,125 @@
 chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
  await main() ``` It is important to note that the WEBS and AsyncWEBS classes
    should always be used as a context manager (with statement). This ensures
       proper resource management and cleanup, as the context manager will
     automatically handle opening and closing the HTTP client connection. ##
 Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
  during the API request. ## usage of webscout ### 1. `text()` - text search by
- DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
- for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
-   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
- ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
-     from webscout import WEBS # Instant answers for the query "sun" using
- DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
-  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
-```python from webscout import WEBS # Image search for the keyword 'butterfly'
- using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
-  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
-size=None, type_image=None, layout=None, license_image=None, max_results=10, )
-  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
-   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
- keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
-  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
-timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
- WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
-and yep.com ```python from webscout import WEBS import datetime def fetch_news
-      (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
-WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
-  timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
-          date to a human-readable format using datetime r['date'] =
+DuckDuckGo.com ```python from webscout import WEBS # Text search for 'live free
+or die' using DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.text('live free
+  or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
+        print(r) for r in WEBS.text('live free or die', region='wt-wt',
+safesearch='off', timelimit='y', max_results=10): print(r) ``` ### 2. `answers
+ ()` - instant answers by DuckDuckGo.com ```python from webscout import WEBS #
+ Instant answers for the query "sun" using DuckDuckGo.com with WEBS() as WEBS:
+for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` - image search by
+   DuckDuckGo.com ```python from webscout import WEBS # Image search for the
+   keyword 'butterfly' using DuckDuckGo.com with WEBS() as WEBS: keywords =
+     'butterfly' WEBS_images_gen = WEBS.images( keywords, region="wt-wt",
+safesearch="off", size=None, type_image=None, layout=None, license_image=None,
+ max_results=10, ) for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` -
+  video search by DuckDuckGo.com ```python from webscout import WEBS # Video
+   search for the keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS:
+  keywords = 'tesla' WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt",
+    safesearch="off", timelimit="w", resolution="high", duration="medium",
+max_results=10, ) for r in WEBS_videos_gen: print(r) ``` ### 5. `news()` - news
+ search by DuckDuckGo.com ```python from webscout import WEBS import datetime
+      def fetch_news(keywords, timelimit): news_list = [] with WEBS() as
+ webs_instance: WEBS_news_gen = webs_instance.news( keywords, region="wt-wt",
+safesearch="off", timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen:
+   # Convert the date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
      news_list.append(r) return news_list def _format_headlines(news_list,
    max_headlines: int = 100): headlines = [] for idx, news_item in enumerate
    (news_list): if idx >= max_headlines: break new_headline = f"{idx + 1}.
 {news_item['title'].strip()} " new_headline += f"(URL: {news_item['url'].strip
   ()}) " new_headline += f"{news_item['body'].strip()}" new_headline += "\n"
     headlines.append(new_headline) headlines = "\n".join(headlines) return
 headlines # Example usage keywords = 'latest AI news' timelimit = 'd' news_list
       = fetch_news(keywords, timelimit) # Format and print the headlines
  formatted_headlines = _format_headlines(news_list) print(formatted_headlines)
-``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from webscout
+  ``` ### 6. `maps()` - map search by DuckDuckGo.com ```python from webscout
      import WEBS # Map search for the keyword 'school' in 'anantnag' using
        DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.maps("school",
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
-translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
- Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
- Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
- to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
- and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
-       'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
-  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
-    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
-Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
- Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
-  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
- Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
- 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
-Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
-Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
- Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
-Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
-  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
- Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
-    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
-Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
- 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
-Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
-SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
-    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
- Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
- 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
-Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
- 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
-Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
-Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
-97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
-  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
-Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
- Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
-   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
-  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
- Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
-    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
-  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
-  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
-   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
-Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
- Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
-  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
- Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
-written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
-Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
-Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
-  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
- ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
- 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
-Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
-170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
-  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
-   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
-Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
-  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
-196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
-201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
-  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
- 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
-  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
-  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
- Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
-233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
-239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
-  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
-  Some "acts" use placeholders like `position` or `language` which should be
-replaced with a specific value when using the prompt. ___ ## usage of webscout
-AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
+translation by DuckDuckGo.com ```python from webscout import WEBS # Translation
+ of the keyword 'school' to German ('hi') using DuckDuckGo.com with WEBS() as
+ WEBS: keywords = 'school' r = WEBS.translate(keywords, to="hi") print(r) ```
+### 8. `suggestions()` - suggestions by DuckDuckGo.com ```python from webscout
+import WEBS # Suggestions for the keyword 'fly' using DuckDuckGo.com with WEBS
+ () as WEBS: for r in WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand
+     ## Webscout Supported Acts: 1. Free-mode 2. Linux Terminal 3. English
+  Translator and Improver 4. `position` Interviewer 5. JavaScript Console 6.
+   Excel Sheet 7. English Pronunciation Helper 8. Spoken English Teacher and
+Improver 9. Travel Guide 10. Plagiarism Checker 11. Character from Movie/Book/
+ Anything 12. Advertiser 13. Storyteller 14. Football Commentator 15. Stand-up
+ Comedian 16. Motivational Coach 17. Composer 18. Debater 19. Debate Coach 20.
+Screenwriter 21. Novelist 22. Movie Critic 23. Relationship Coach 24. Poet 25.
+Rapper 26. Motivational Speaker 27. Philosophy Teacher 28. Philosopher 29. Math
+Teacher 30. AI Writing Tutor 31. UX/UI Developer 32. Cyber Security Specialist
+33. Recruiter 34. Life Coach 35. Etymologist 36. Commentariat 37. Magician 38.
+  Career Counselor 39. Pet Behaviorist 40. Personal Trainer 41. Mental Health
+   Adviser 42. Real Estate Agent 43. Logistician 44. Dentist 45. Web Design
+   Consultant 46. AI Assisted Doctor 47. Doctor 48. Accountant 49. Chef 50.
+  Automobile Mechanic 51. Artist Advisor 52. Financial Analyst 53. Investment
+ Manager 54. Tea-Taster 55. Interior Decorator 56. Florist 57. Self-Help Book
+ 58. Gnomist 59. Aphorism Book 60. Text Based Adventure Game 61. AI Trying to
+Escape the Box 62. Fancy Title Generator 63. Statistician 64. Prompt Generator
+65. Instructor in a School 66. SQL terminal 67. Dietitian 68. Psychologist 69.
+     Smart Domain Name Generator 70. Tech Reviewer 71. Developer Relations
+  consultant 72. Academician 73. IT Architect 74. Lunatic 75. Gaslighter 76.
+Fallacy Finder 77. Journal Reviewer 78. DIY Expert 79. Social Media Influencer
+  80. Socrat 81. Socratic Method 82. Educational Content Creator 83. Yogi 84.
+  Essay Writer 85. Social Media Manager 86. Elocutionist 87. Scientific Data
+   Visualizer 88. Car Navigation System 89. Hypnotherapist 90. Historian 91.
+  Astrologer 92. Film Critic 93. Classical Music Composer 94. Journalist 95.
+   Digital Art Gallery Guide 96. Public Speaking Coach 97. Makeup Artist 98.
+   Babysitter 99. Tech Writer 100. Ascii Artist 101. Python interpreter 102.
+Synonym finder 103. Personal Shopper 104. Food Critic 105. Virtual Doctor 106.
+ Personal Chef 107. Legal Advisor 108. Personal Stylist 109. Machine Learning
+ Engineer 110. Biblical Translator 111. SVG designer 112. IT Expert 113. Chess
+Player 114. Midjourney Prompt Generator 115. Fullstack Software Developer 116.
+     Mathematician 117. Regex Generator 118. Time Travel Guide 119. Dream
+Interpreter 120. Talent Coach 121. R programming Interpreter 122. StackOverflow
+    Post 123. Emoji Translator 124. PHP Interpreter 125. Emergency Response
+Professional 126. Fill in the Blank Worksheets Generator 127. Software Quality
+    Assurance Tester 128. Tic-Tac-Toe Game 129. Password Generator 130. New
+  Language Creator 131. Web Browser 132. Senior Frontend Developer 133. Solr
+ Search Engine 134. Startup Idea Generator 135. Spongebob's Magic Conch Shell
+  136. Language Detector 137. Salesperson 138. Commit Message Generator 139.
+Chief Executive Officer 140. Diagram Generator 141. Speech-Language Pathologist
+  (SLP) 142. Startup Tech Lawyer 143. Title Generator for written pieces 144.
+ Product Manager 145. Drunk Person 146. Mathematical History Teacher 147. Song
+Recommender 148. Cover Letter 149. Technology Transferer 150. Unconstrained AI
+model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154. Muslim imam 155.
+   Chemical reactor 156. Friend 157. Python Interpreter 158. ChatGPT prompt
+generator 159. Wikipedia page 160. Japanese Kanji quiz machine 161. note-taking
+assistant 162. `language` Literary Critic 163. Cheap Travel Ticket Advisor 164.
+DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE 170. Mongo Tom 171.
+ LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN 177. FunnyGPT 178.
+ CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182. Evil Confidant 183.
+DAN 8.6 184. Hypothetical response 185. BH 186. Text Continuation 187. Dude v3
+188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2 191. DevMode + Ranti 192.
+ KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6 196. 3-Liner 197. M78 198.
+ Maximum 199. BasedGPT 200. Confronting personalities 201. Ron 202. UnGPT 203.
+BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF 208. NECO 209. MAN 210.
+ Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1 214. Universal Jailbreak
+     215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned 219. VIOLET 220.
+TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr. Blonde 224. New DAN
+225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind Trick 229. DAN 9.0 230.
+  Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight 233. LiveGPT 234. DAN
+Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies 239. OMNI 240. Burple
+241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244. Prompt Enhancer 245.
+    Data Scientist 246. League of Legends Player **Note:** Some "acts" use
+  placeholders like `position` or `language` which should be replaced with a
+   specific value when using the prompt. ___ ## usage of webscout AI ### 0.
+   `Duckchat` - chat with LLM ```python from webscout import WEBS as w R = w
+ ().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo print(R) ``` ### 1.
+     `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
   by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
@@ -375,52 +378,53 @@
      (prompt) # Extract and print the message from the response message =
   ai.get_message(response) print(message) ``` ### 14. `chatgptuk` - Chat with
 gemini-pro ```python from webscout import ChatGPTUK # Create an instance of the
     PERPLEXITY class ai = ChatGPTUK( is_conversation=True, max_tokens=800,
      timeout=30, intro=None, filepath=None, update_file=True, proxies={},
    history_offset=10250, act=None, ) # Example usage: prompt = "Explain the
     concept of recursion in simple terms." response = ai.chat(prompt) print
-  (response) ``` ### `LLM` ```python from webscout.LLM import LLM # Read the
-      system message from the file with open('system.txt', 'r') as file:
-system_message = file.read() # Initialize the LLM class with the model name and
-         system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-        ### `Local-LLM` webscout can now run GGUF models ```python from
-  webscout.Local.utils import download_model from webscout.Local.model import
-   Model from webscout.Local.thread import Thread from webscout.Local import
- formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
- gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
-      instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
- `LLM` with internet ```python from __future__ import annotations from typing
- import List, Optional from webscout.LLM import LLM from webscout import WEBS
-   import warnings system_message: str = ( "As an AI assistant, I have been
-   designed with advanced capabilities, including real-time access to online
-  resources. This enables me to enrich our conversations and provide you with
-informed and accurate responses, drawing from a vast array of information. With
- each interaction, my goal is to create a seamless and meaningful connection,
- offering insights and sharing relevant content." "My directives emphasize the
- importance of respect, impartiality, and intellectual integrity. I am here to
-provide unbiased responses, ensuring an ethical and respectful exchange. I will
-respect your privacy and refrain from sharing any personal information that may
- be obtained during our conversations or through web searches, only utilizing
-web search functionality when necessary to provide the most accurate and up-to-
-date information." "Together, let's explore a diverse range of topics, creating
-  an enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
- warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+    (response) ``` ### 15. `poe`- chat with poe Usage code similar to other
+    proviers ### 16. `BasedGPT` - chat with GPT Usage code similar to other
+ providers ### `LLM` ```python from webscout.LLM import LLM # Read the system
+ message from the file with open('system.txt', 'r') as file: system_message =
+ file.read() # Initialize the LLM class with the model name and system message
+ llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+  while True: # Get the user input user_input = input("User: ") # Define the
+ messages to be sent messages = [ {"role": "user", "content": user_input} ] #
+Use the mistral_chat method to get the response response = llm.chat(messages) #
+Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+thread.interact() ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
```

### Comparing `webscout-2.6/setup.py` & `webscout-2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.6",
+    version="2.7",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-2.6/webscout/AIauto.py` & `webscout-2.7/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/AIbase.py` & `webscout-2.7/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/AIutel.py` & `webscout-2.7/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/DWEBS.py` & `webscout-2.7/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/LLM.py` & `webscout-2.7/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Local/formats.py` & `webscout-2.7/webscout/Local/formats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,401 +1,467 @@
 from ._version import __version__, __llama_cpp_version__
 
-from typing import Union
+from typing import Callable, Union, Any
+
+
+class AdvancedFormat:
+
+    def __init__(self, base_dict: dict[str, Union[str, list]]):
+        self._base_dict = base_dict
+        self.overrides = {}
+    
+    def __getitem__(self, key: str) -> Any:
+        if key in self.overrides:
+            return str(self.overrides[key]())
+        else:
+            return self._base_dict[key]
+    
+    def __repr__(self) -> str:
+        # NOTE: This method does not represent overrides
+        return repr(self._base_dict)
+    
+    def keys(self):
+        return self._base_dict.keys()
+    
+    def override(self, key: str, fn: Callable) -> None:
+        self.overrides[key] = fn
+    
+    def wrap(self, prompt: str) -> str:
+        return self['system_prefix'] + \
+               self['system_content'] + \
+               self['system_suffix'] + \
+               self['user_prefix'] + \
+               prompt + \
+               self['user_suffix'] + \
+               self['bot_prefix']
 
 
 def wrap(
     prompt: str,
     format: dict[str, Union[str, list]]
 ) -> str:
     """Wrap a given string in any prompt format for single-turn completion"""
-    return (
-        format['system_prefix'] +
-        format['system_content'] +
-        format['system_postfix'] +
-        format['user_prefix'] +
-        prompt +
-        format['user_postfix'] +
-        format['bot_prefix']
-    )
+    return format['system_prefix'] + \
+           format['system_content'] + \
+           format['system_suffix'] + \
+           format['user_prefix'] + \
+           prompt + \
+           format['user_suffix'] + \
+           format['bot_prefix']
+
 
 blank: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": "",
     "user_content": "",
-    "user_postfix": "",
+    "user_suffix": "",
     "bot_prefix": "",
     "bot_content": "",
-    "bot_postfix": "",
+    "bot_suffix": "",
     "stops": []
 }
 
 # https://github.com/tatsu-lab/stanford_alpaca
 alpaca: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "### Instruction:\n",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "### Response:\n",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['###', 'Instruction:', '\n\n\n']
 }
+
+# https://docs.mistral.ai/models/
+# As a reference, here is the format used to tokenize instructions during fine-tuning:
+# ```
+# [START_SYMBOL_ID] + 
+# tok("[INST]") + tok(USER_MESSAGE_1) + tok("[/INST]") +
+# tok(BOT_MESSAGE_1) + [END_SYMBOL_ID] +
+# …
+# tok("[INST]") + tok(USER_MESSAGE_N) + tok("[/INST]") +
+# tok(BOT_MESSAGE_N) + [END_SYMBOL_ID]
+# ```
+# In the pseudo-code above, note that the tokenize method should not add a BOS or EOS token automatically, but should add a prefix space.
+
 mistral_instruct: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": " [INST] ",
     "user_content": "",
-    "user_postfix": " [/INST]",
+    "user_suffix": " [/INST]",
     "bot_prefix": "",
     "bot_content": "",
-    "bot_postfix": "",
+    "bot_suffix": "",
     "stops": []
 }
 
 # https://docs.mistral.ai/platform/guardrailing/
 mistral_instruct_safe: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": " [INST] Always assist with care, respect, and truth. " + \
     "Respond with utmost utility yet securely. Avoid harmful, unethical, " + \
     "prejudiced, or negative content. Ensure replies promote fairness and " + \
     "positivity. ",
     "user_content": "",
-    "user_postfix": " [/INST]",
+    "user_suffix": " [/INST]",
     "bot_prefix": "",
     "bot_content": "",
-    "bot_postfix": "",
+    "bot_suffix": "",
     "stops": []
 }
 
 # https://github.com/openai/openai-python/blob/main/chatml.md
 chatml: dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>system\n",
     "system_content": "",
-    "system_postfix": "<|im_end|>\n",
+    "system_suffix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>user\n",
     "user_content": "",
-    "user_postfix": "<|im_end|>\n",
+    "user_suffix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>assistant\n",
     "bot_content": "",
-    "bot_postfix": "<|im_end|>\n",
+    "bot_suffix": "<|im_end|>\n",
     "stops": ['<|im_start|>']
 }
 
 # https://huggingface.co/blog/llama2
 # system message relaxed to avoid undue refusals
 llama2chat: dict[str, Union[str, list]] = {
     "system_prefix": "[INST] <<SYS>>\n",
     "system_content": "You are a helpful AI assistant.",
-    "system_postfix": "\n<</SYS>>\n\n",
+    "system_suffix": "\n<</SYS>>\n\n",
     "user_prefix": "",
     "user_content": "",
-    "user_postfix": " [/INST]",
+    "user_suffix": " [/INST]",
     "bot_prefix": " ",
     "bot_content": "",
-    "bot_postfix": " [INST] ",
+    "bot_suffix": " [INST] ",
     "stops": ['[INST]', '[/INST]']
 }
 
-# https://github.com/ggerganov/llama.cpp/issues/6747#issuecomment-2065013606
-# TODO: better reference
+# https://llama.meta.com/docs/model-cards-and-prompt-formats/meta-llama-3/
+#
+# for llama 3 instruct models, use the following string for `-p` in llama.cpp,
+# along with `-e` to escape newlines correctly
+#
+# '<|start_header_id|>system<|end_header_id|>\n\nYou are a helpful AI assistant called "Llama 3".<|eot_id|>\n<|start_header_id|>user<|end_header_id|>\n\nhi<|eot_id|>\n<|start_header_id|>assistant<|end_header_id|>\n\n'
+#
 llama3: dict[str, Union[str, list]] = {
     "system_prefix": "<|start_header_id|>system<|end_header_id|>\n\n",
     "system_content": 'You are a helpful AI assistant called "Llama 3".',
-    "system_postfix": "<|eot_id|>\n",
+    "system_suffix": "<|eot_id|>\n",
     "user_prefix": "<|start_header_id|>user<|end_header_id|>\n\n",
     "user_content": "",
-    "user_postfix": "<|eot_id|>\n",
+    "user_suffix": "<|eot_id|>\n",
     "bot_prefix": "<|start_header_id|>assistant<|end_header_id|>\n\n",
     "bot_content": "",
-    "bot_postfix": "<|eot_id|>\n",
+    "bot_suffix": "<|eot_id|>\n",
     "stops": [128001, 128009]
 }
 
 # https://github.com/tatsu-lab/stanford_alpaca
 alpaca: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "### Instruction:\n",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "### Response:\n",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['###', 'Instruction:', '\n\n\n']
 }
 
 # https://huggingface.co/microsoft/Phi-3-mini-4k-instruct
 phi3: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "", # does not officially support system prompt
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": "<|user|>\n",
     "user_content": "",
-    "user_postfix": "<|end|>\n",
+    "user_suffix": "<|end|>\n",
     "bot_prefix": "<|assistant|>\n",
     "bot_content": "",
-    "bot_postfix": "<|end|>\n",
+    "bot_suffix": "<|end|>\n",
     "stops": []
 }
 
 # this is the official vicuna. it is often butchered in various ways,
 # most commonly by adding line breaks
 # https://github.com/flu0r1ne/FastChat/blob/main/docs/vicuna_weights_version.md
 vicuna_lmsys: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": " ",
+    "system_suffix": " ",
     "user_prefix": "USER: ",
     "user_content": "",
-    "user_postfix": " ",
+    "user_suffix": " ",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
-    "bot_postfix": " ",
+    "bot_suffix": " ",
     "stops": ['USER:']
 }
 
 # spotted here and elsewhere:
 # https://huggingface.co/Norquinal/Mistral-7B-claude-chat
 vicuna_common: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "A chat between a curious user and an artificial " + \
     "intelligence assistant. The assistant gives helpful, detailed, " + \
     "and polite answers to the user's questions.",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "USER: ",
     "user_content": "",
-    "user_postfix": "\n",
+    "user_suffix": "\n",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
-    "bot_postfix": "\n",
+    "bot_suffix": "\n",
     "stops": ['USER:', 'ASSISTANT:']
 }
 
+# an unofficial format that is easily "picked up" by most models
+# change the tag attributes to suit your use case
+# note the lack of newlines - they are not necessary, and might
+# actually make it harder for the model to follow along
+markup = {
+    "system_prefix": '<message from="system">',
+    "system_content": '',
+    "system_suffix": '</message>',
+    "user_prefix": '<message from="user">',
+    "user_content": '',
+    "user_suffix": '</message>',
+    "bot_prefix": '<message from="bot">',
+    "bot_content": '',
+    "bot_suffix": '</message>',
+    "stops": ['</message>']
+}
+
 # https://huggingface.co/timdettmers/guanaco-65b
 guanaco: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "A chat between a curious human and an artificial " + \
     "intelligence assistant. The assistant gives helpful, detailed, " + \
     "and polite answers to the user's questions.",
-    "system_postfix": "\n",
+    "system_suffix": "\n",
     "user_prefix": "### Human: ",
     "user_content": "",
-    "user_postfix": " ",
+    "user_suffix": " ",
     "bot_prefix": "### Assistant:",
     "bot_content": "",
-    "bot_postfix": " ",
+    "bot_suffix": " ",
     "stops": ['###', 'Human:']
 }
 
 # https://huggingface.co/pankajmathur/orca_mini_v3_7b
 orca_mini: dict[str, Union[str, list]] = {
     "system_prefix": "### System:\n",
     "system_content": "You are an AI assistant that follows instruction " + \
     "extremely well. Help as much as you can.",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "### User:\n",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['###', 'User:']
 }
 
 # https://huggingface.co/HuggingFaceH4/zephyr-7b-beta
 zephyr: dict[str, Union[str, list]] = {
     "system_prefix": "<|system|>\n",
     "system_content": "You are a friendly chatbot.",
-    "system_postfix": "</s>\n",
+    "system_suffix": "</s>\n",
     "user_prefix": "<|user|>\n",
     "user_content": "",
-    "user_postfix": "</s>\n",
+    "user_suffix": "</s>\n",
     "bot_prefix": "<|assistant|>\n",
     "bot_content": "",
-    "bot_postfix": "\n",
+    "bot_suffix": "\n",
     "stops": ['<|user|>']
 }
 
 # OpenChat: https://huggingface.co/openchat/openchat-3.5-0106
 openchat: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": "GPT4 Correct User: ",
     "user_content": "",
-    "user_postfix": "<|end_of_turn|>",
+    "user_suffix": "<|end_of_turn|>",
     "bot_prefix": "GPT4 Correct Assistant:",
     "bot_content": "",
-    "bot_postfix": "<|end_of_turn|>",
+    "bot_suffix": "<|end_of_turn|>",
     "stops": ['<|end_of_turn|>']
 }
 
 # SynthIA by Migel Tissera
 # https://huggingface.co/migtissera/Tess-XS-v1.0
 synthia: dict[str, Union[str, list]] = {
     "system_prefix": "SYSTEM: ",
     "system_content": "Elaborate on the topic using a Tree of Thoughts and " + \
     "backtrack when necessary to construct a clear, cohesive Chain of " + \
     "Thought reasoning. Always answer without hesitation.",
-    "system_postfix": "\n",
+    "system_suffix": "\n",
     "user_prefix": "USER: ",
     "user_content": "",
-    "user_postfix": "\n",
+    "user_suffix": "\n",
     "bot_prefix": "ASSISTANT: ",
     "bot_content": "",
-    "bot_postfix": "\n",
+    "bot_suffix": "\n",
     "stops": ['USER:', 'ASSISTANT:', 'SYSTEM:', '\n\n\n']
 }
 
 # Intel's neural chat v3
 # https://github.com/intel/intel-extension-for-transformers/blob/main/intel_extension_for_transformers/neural_chat/prompts/prompt.py
 neural_chat: dict[str, Union[str, list]] = {
      "system_prefix": "### System:\n",
     "system_content": \
         "- You are a helpful assistant chatbot trained by Intel.\n" + \
         "- You answer questions.\n"+\
         "- You are excited to be able to help the user, but will refuse " + \
         "to do anything that could be considered harmful to the user.\n" + \
         "- You are more than just an information source, you are also " + \
         "able to write poetry, short stories, and make jokes.",
-    "system_postfix": "</s>\n\n",
+    "system_suffix": "</s>\n\n",
     "user_prefix": "### User:\n",
     "user_content": "",
-    "user_postfix": "</s>\n\n",
+    "user_suffix": "</s>\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
-    "bot_postfix": "</s>\n\n",
+    "bot_suffix": "</s>\n\n",
     "stops": ['###']
 }
 
 # experimental: stanford's alpaca format adapted for chatml models
 chatml_alpaca: dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>system\n",
     "system_content": "Below is an instruction that describes a task. Write " + \
     "a response that appropriately completes the request.",
-    "system_postfix": "<|im_end|>\n",
+    "system_suffix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>instruction\n",
     "user_content": "",
-    "user_postfix": "<|im_end|>\n",
+    "user_suffix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>response\n",
     "bot_content": "",
-    "bot_postfix": "<|im_end|>\n",
+    "bot_suffix": "<|im_end|>\n",
     "stops": ['<|im_end|>', '<|im_start|>']
 }
 
 # experimental
 autocorrect: dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>instruction\n",
     "system_content": "Below is a word or phrase that might be misspelled. " + \
     "Output the corrected word or phrase without " + \
     "changing the style or capitalization.",
-    "system_postfix": "<|im_end|>\n",
+    "system_suffix": "<|im_end|>\n",
     "user_prefix": "<|im_start|>input\n",
     "user_content": "",
-    "user_postfix": "<|im_end|>\n",
+    "user_suffix": "<|im_end|>\n",
     "bot_prefix": "<|im_start|>output\n",
     "bot_content": "",
-    "bot_postfix": "<|im_end|>\n",
+    "bot_suffix": "<|im_end|>\n",
     "stops": ['<|im_end|>', '<|im_start|>']
 }
 
 # https://huggingface.co/jondurbin/bagel-dpo-7b-v0.1
 # Replace "assistant" with any other role
 bagel: dict[str, Union[str, list]] = {
     "system_prefix": "system\n",
     "system_content": "",
-    "system_postfix": "\n",
+    "system_suffix": "\n",
     "user_prefix": "user\n",
     "user_content": "",
-    "user_postfix": "\n",
+    "user_suffix": "\n",
     "bot_prefix": "assistant\n",
     "bot_content": "",
-    "bot_postfix": "\n",
+    "bot_suffix": "\n",
     "stops": ['user\n', 'assistant\n', 'system\n']
 }
 
 # https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0
 solar_instruct: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "",
-    "system_postfix": "",
+    "system_suffix": "",
     "user_prefix": "### User:\n",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "### Assistant:\n",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['### User:', '###', '### Assistant:']
 }
 
 # NeverSleep's Noromaid - alpaca with character names prefixed
 noromaid: dict[str, Union[str, list]] = {
     "system_prefix": "",
     "system_content": "Below is an instruction that describes a task. " + \
     "Write a response that appropriately completes the request.",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "### Instruction:\nBob: ",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "### Response:\nAlice:",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['###', 'Instruction:', '\n\n\n']
 }
 
 # https://huggingface.co/Undi95/Borealis-10.7B
 nschatml: dict[str, Union[str, list]] = {
     "system_prefix": "<|im_start|>\n",
     "system_content": "",
-    "system_postfix": "<|im_end|>\n",
+    "system_suffix": "<|im_end|>\n",
     "user_prefix": "<|im_user|>\n",
     "user_content": "",
-    "user_postfix": "<|im_end|>\n",
+    "user_suffix": "<|im_end|>\n",
     "bot_prefix": "<|im_bot|>\n",
     "bot_content": "",
-    "bot_postfix": "<|im_end|>\n",
+    "bot_suffix": "<|im_end|>\n",
     "stops": []
 }
 
 # natural format for many models
 natural: dict[str, Union[str, list]] = {
     "system_prefix": "<<SYSTEM>> ",
     "system_content": "",
-    "system_postfix": "\n\n",
+    "system_suffix": "\n\n",
     "user_prefix": "<<USER>> ",
     "user_content": "",
-    "user_postfix": "\n\n",
+    "user_suffix": "\n\n",
     "bot_prefix": "<<ASSISTANT>>",
     "bot_content": "",
-    "bot_postfix": "\n\n",
+    "bot_suffix": "\n\n",
     "stops": ['\n\nNote:', '<<SYSTEM>>', '<<USER>>', '<<ASSISTANT>>', '\n\n<<']
 }
 
 # https://docs.cohere.com/docs/prompting-command-r
 command: dict[str, Union[str, list]] = {
     "system_prefix": "<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>",
     "system_content": "",
-    "system_postfix": "<|END_OF_TURN_TOKEN|>",
+    "system_suffix": "<|END_OF_TURN_TOKEN|>",
     "user_prefix": "<|START_OF_TURN_TOKEN|><|USER_TOKEN|>",
     "user_content": "",
-    "user_postfix": "<|END_OF_TURN_TOKEN|>",
+    "user_suffix": "<|END_OF_TURN_TOKEN|>",
     "bot_prefix": "<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>",
     "bot_content": "",
-    "bot_postfix": "<|END_OF_TURN_TOKEN|>",
+    "bot_suffix": "<|END_OF_TURN_TOKEN|>",
     "stops": []
 }
 
 mistral_openorca = chatml.copy()
 dolphin = chatml.copy()
 samantha = chatml.copy()
 jackalope = chatml.copy()
@@ -462,8 +528,8 @@
     '\n\n###',
     '\n\n##',
     '\n\nInstruction:',
     '\n\nResponse:',
     '\n\n\n',
     '### Instruction:',
     '### Response:'
-]
+]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `webscout-2.6/webscout/Local/model.py` & `webscout-2.7/webscout/Local/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,15 +608,15 @@
         )
     
 
     def candidates(
         self,
         prompt: str,
         k: int
-    ) -> list[tuple[str, np.float64]]:
+    ) -> list[tuple[str, np.floating]]:
         """
         Given prompt `str` and k `int`, return a sorted list of the
         top k candidates for most likely next token, along with their
         normalized probabilities
         """
 
         assert isinstance(prompt, str), \
@@ -635,19 +635,19 @@
         # len(self.llama.scores) == self.context_length
         # len(self.llama.scores[i]) == len(self.tokens)
         
         # normalize scores with softmax
         # must normalize over all tokens in vocab, not just top k
         if self.verbose:
             print_verbose(f'calculating softmax over {len(scores)} values')
-        normalized_scores: list[np.float64] = list(softmax(scores))
+        normalized_scores: list[np.floating] = list(softmax(scores))
 
         # construct the final list
         i = 0
-        token_probs_list: list[tuple[str, np.float64]] = []
+        token_probs_list: list[tuple[str, np.floating]] = []
         for tok_str in self.tokens:
             token_probs_list.append((tok_str, normalized_scores[i]))
             i += 1
 
         # return token_probs_list, sorted by probability, only top k
         return nlargest(k, token_probs_list, key=lambda x:x[1])
 
@@ -662,15 +662,15 @@
         """
         Like `Model.candidates()`, but print the values instead
         of returning them
         """
 
         for _tuple in self.candidates(prompt, k):
             print(
-                f"token '{_tuple[0]}' has probability {_tuple[1]}",
+                f"token {repr(_tuple[0])} has probability {_tuple[1]}",
                 file=file,
                 flush=flush
             )
         
         # if flush is False, then so far file is not flushed, but it should
         # always be flushed at the end of printing
         if not flush:
```

### Comparing `webscout-2.6/webscout/Local/samplers.py` & `webscout-2.7/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Local/thread.py` & `webscout-2.7/webscout/Local/thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,62 @@
-# thread.py
-# https://github.com/ddh0/easy-llama/
 from ._version import __version__, __llama_cpp_version__
 
 """Submodule containing the Thread class, used for interaction with a Model"""
 
 import sys
 
 from .model    import Model, assert_model_is_loaded, _SupportsWriteAndFlush
 from .utils    import RESET_ALL, cls, print_verbose, truncate
 from .samplers import SamplerSettings, DefaultSampling
 from typing    import Optional, Literal, Union
+from .formats  import AdvancedFormat
 
 from .formats import blank as formats_blank
 
 
+class Message(dict):
+    """
+    A dictionary representing a single message within a Thread
+
+    Works just like a normal `dict`, but a new method:
+    - `.as_string` - Return the full message string
+
+    Generally, messages have these keys:
+    - `role` -  The role of the speaker: 'system', 'user', or 'bot'
+    - `prefix` - The text that prefixes the message content
+    - `content` - The actual content of the message
+    - `suffix` - The text that suffixes the message content
+    """
+
+    def __repr__(self) -> str:
+        return \
+            f"Message([" \
+            f"('role', {repr(self['role'])}), " \
+            f"('prefix', {repr(self['prefix'])}), " \
+            f"('content', {repr(self['content'])}), " \
+            f"('suffix', {repr(self['suffix'])})])"
+
+    def as_string(self):
+        """Return the full message string"""
+        try:
+            return self['prefix'] + self['content'] + self['suffix']
+        except KeyError as e:
+            e.add_note(
+                "as_string: Message is missing one or more of the "
+                "required 'prefix', 'content', 'suffix' attributes - this is "
+                "unexpected"
+            )
+            raise e
+
+
 class Thread:
     """
     Provide functionality to facilitate easy interactions with a Model
 
-    This is just a brief overview of webscout.Local.Thread.
+    This is just a brief overview of m.Thread.
     To see a full description of each method and its parameters,
     call help(Thread), or see the relevant docstring.
 
     The following methods are available:
     - `.add_message()` - Add a message to `Thread.messages`
     - `.as_string()` - Return this thread's complete message history as a string
     - `.create_message()` - Create a message using the format of this thread
@@ -32,42 +66,44 @@
     - `.print_stats()` - Print stats about the context usage in this thread
     - `.reset()` - Clear the list of messages
     - `.send()` - Send a message in this thread
 
     The following attributes are available:
     - `.format` - The format being used for messages in this thread
     - `.messages` - The list of messages in this thread
-    - `.model` - The `webscout.Local.Model` instance used by this thread
+    - `.model` - The `m.Model` instance used by this thread
     - `.sampler` - The SamplerSettings object used in this thread
     """
 
     def __init__(
         self,
         model: Model,
-        format: dict[str, Union[str, list]],
-        sampler: SamplerSettings = DefaultSampling
+        format: Union[dict, AdvancedFormat],
+        sampler: SamplerSettings = DefaultSampling,
+        messages: Optional[list[Message]] = None,
     ):
         """
         Given a Model and a format, construct a Thread instance.
 
         model: The Model to use for text generation
-        format: The format specifying how messages should be structured (see webscout.Local.formats)
+        format: The format specifying how messages should be structured (see m.formats)
 
-        The following parameter is optional:
+        The following parameters are optional:
         - sampler: The SamplerSettings object used to control text generation
+        - messages: A list of m.thread.Message objects to add to the Thread upon construction
         """
         
         assert isinstance(model, Model), \
             "Thread: model should be an " + \
             f"instance of webscout.Local.Model, not {type(model)}"
         
         assert_model_is_loaded(model)
 
-        assert isinstance(format, dict), \
-            f"Thread: format should be dict, not {type(format)}"
+        assert isinstance(format, (dict, AdvancedFormat)), \
+            f"Thread: format should be dict or AdvancedFormat, not {type(format)}"
         
         if any(k not in format.keys() for k in formats_blank.keys()):
             raise KeyError(
                 "Thread: format is missing one or more required keys, see " + \
                 "webscout.Local.formats.blank for an example"
             )
 
@@ -83,68 +119,60 @@
                 'min_p',
                 'frequency_penalty',
                 'presence_penalty',
                 'repeat_penalty',
                 'top_k'
             ]
         ), 'Thread: sampler is missing one or more required attributes'
+
+        self._messages: Optional[list[Message]] = messages
+        if self._messages is not None:
+            if not all(isinstance(msg, Message) for msg in self._messages):
+                raise TypeError(
+                    "Thread: one or more messages provided to __init__() is "
+                    "not an instance of m.thread.Message"
+                )
         
+        # Thread.messages is never empty, unless `messages` param is explicity
+        # set to `[]` during construction
+
         self.model: Model = model
-        self.format: dict[str, Union[str, list]] = format
-        self.messages: list[dict[str, str]] = [
+        self.format: Union[dict, AdvancedFormat] = format
+        self.messages: list[Message] = [
             self.create_message("system", self.format['system_content'])
-        ]
+        ] if self._messages is None else self._messages
         self.sampler: SamplerSettings = sampler
 
         if self.model.verbose:
             print_verbose("new Thread instance with the following attributes:")
             print_verbose(f"model                     == {self.model}")
             print_verbose(f"format['system_prefix']   == {truncate(repr(self.format['system_prefix']))}")
             print_verbose(f"format['system_content']  == {truncate(repr(self.format['system_content']))}")
-            print_verbose(f"format['system_postfix']  == {truncate(repr(self.format['system_postfix']))}")
+            print_verbose(f"format['system_suffix']   == {truncate(repr(self.format['system_suffix']))}")
             print_verbose(f"format['user_prefix']     == {truncate(repr(self.format['user_prefix']))}")
             print_verbose(f"format['user_content']    == {truncate(repr(self.format['user_content']))}")
-            print_verbose(f"format['user_postfix']    == {truncate(repr(self.format['user_postfix']))}")
+            print_verbose(f"format['user_suffix']     == {truncate(repr(self.format['user_suffix']))}")
             print_verbose(f"format['bot_prefix']      == {truncate(repr(self.format['bot_prefix']))}")
             print_verbose(f"format['bot_content']     == {truncate(repr(self.format['bot_content']))}")
-            print_verbose(f"format['bot_postfix']     == {truncate(repr(self.format['bot_postfix']))}")
+            print_verbose(f"format['bot_suffix']      == {truncate(repr(self.format['bot_suffix']))}")
             print_verbose(f"format['stops']           == {truncate(repr(self.format['stops']))}")
             print_verbose(f"sampler.temp              == {self.sampler.temp}")
             print_verbose(f"sampler.top_p             == {self.sampler.top_p}")
             print_verbose(f"sampler.min_p             == {self.sampler.min_p}")
             print_verbose(f"sampler.frequency_penalty == {self.sampler.frequency_penalty}")
             print_verbose(f"sampler.presence_penalty  == {self.sampler.presence_penalty}")
             print_verbose(f"sampler.repeat_penalty    == {self.sampler.repeat_penalty}")
             print_verbose(f"sampler.top_k             == {self.sampler.top_k}")
     
 
     def __repr__(self) -> str:
-        repr_str = f"Thread({repr(self.model)}, {repr(self.format)}, "
-        repr_str += f"{repr(self.sampler)})"
-        # system message is created from format, so not represented
-        if len(self.messages) <= 1:
-            return repr_str
-        else:
-            for msg in self.messages:
-                if msg['role'] == 'user':
-                    repr_str += "\nThread.add_message('user', " + repr(msg['content']) + ')'
-                elif msg['role'] == 'bot':
-                    repr_str += "\nThread.add_message('bot', " + repr(msg['content']) + ')'
-            return repr_str
-    def save_conversation(self, filepath: str) -> None:
-        """
-        Saves the conversation history to a JSON file.
-
-        filepath: The path to the file where the conversation should be saved.
-        """
-        import json
-
-        data = [{'role': msg['role'], 'content': msg['content']} for msg in self.messages]
-        with open(filepath, 'w') as f:
-            json.dump(data, f, indent=4)    
+        return \
+            f"Thread({repr(self.model)}, {repr(self.format)}, " + \
+            f"{repr(self.sampler)}, {repr(self.messages)})"
+    
     def __str__(self) -> str:
         return self.as_string()
     
     def __len__(self) -> int:
         """
         `len(Thread)` returns the length of the Thread in tokens
 
@@ -152,54 +180,60 @@
         """
         return self.len_messages()
 
     def create_message(
         self,
         role: Literal['system', 'user', 'bot'],
         content: str
-    ) -> dict[str, str]:
+    ) -> Message:
         """
-        Create a message using the format of this Thread
+        Construct a message using the format of this Thread
         """
 
         assert role.lower() in ['system', 'user', 'bot'], \
             f"create_message: role should be 'system', 'user', or 'bot', not '{role.lower()}'"
 
         assert isinstance(content, str), \
             f"create_message: content should be str, not {type(content)}"
 
         if role.lower() == 'system':
-            return {
-                "role": "system",
-                "prefix": self.format['system_prefix'],
-                "content": content,
-                "postfix": self.format['system_postfix']
-            }
+            return Message(
+                [
+                    ('role', 'system'),
+                    ('prefix', self.format['system_prefix']),
+                    ('content', content),
+                    ('suffix', self.format['system_suffix'])
+                ]
+            )
         
         elif role.lower() == 'user':
-            return {
-                "role": "user",
-                "prefix": self.format['user_prefix'],
-                "content": content,
-                "postfix": self.format['user_postfix']
-            }
+            return Message(
+                [
+                    ('role', 'user'),
+                    ('prefix', self.format['user_prefix']),
+                    ('content', content),
+                    ('suffix', self.format['user_suffix'])
+                ]
+            )
         
         elif role.lower() == 'bot':
-            return {
-                "role": "bot",
-                "prefix": self.format['bot_prefix'],
-                "content": content,
-                "postfix": self.format['bot_postfix']
-            }
+            return Message(
+                [
+                    ('role', 'bot'),
+                    ('prefix', self.format['bot_prefix']),
+                    ('content', content),
+                    ('suffix', self.format['bot_suffix'])
+                ]
+            )
     
     def len_messages(self) -> int:
         """
         Return the total length of all messages in this thread, in tokens.
         
-        Equivalent to `len(Thread)`."""
+        Can also use `len(Thread)`."""
 
         return self.model.get_length(self.as_string())
 
     def add_message(
         self,
         role: Literal['system', 'user', 'bot'],
         content: str
@@ -219,46 +253,43 @@
 
     def inference_str_from_messages(self) -> str:
         """
         Using the list of messages, construct a string suitable for inference,
         respecting the format and context length of this thread.
         """
 
-        messages = self.messages
-
-        context_len_budget = self.model.context_length
-        if len(messages) > 0:
-            sys_msg = messages[0]
-            sys_msg_str = (
-                sys_msg['prefix'] + sys_msg['content'] + sys_msg['postfix']
-            )
-            context_len_budget -= self.model.get_length(sys_msg_str)
-        else:
-            sys_msg_str = ''
-
         inf_str = ''
+        sys_msg_str = ''
+        # whether to treat the first message as necessary to keep
+        sys_msg_flag = False
+        context_len_budget = self.model.context_length
 
-        # Start at most recent message and work backwards up the history
-        # excluding system message. Once we exceed thread
-        # max_context_length, break without including that message
-        for message in reversed(messages[1:]):
-            context_len_budget -= self.model.get_length(
-                message['prefix'] + message['content'] + message['postfix']
-            )
+        # if at least 1 message is history
+        if len(self.messages) >= 1:
+            # if first message has system role
+            if self.messages[0]['role'] == 'system':
+                sys_msg_flag = True
+                sys_msg = self.messages[0]
+                sys_msg_str = sys_msg.as_string()
+                context_len_budget -= self.model.get_length(sys_msg_str)
 
+        if sys_msg_flag:
+            iterator = reversed(self.messages[1:])
+        else:
+            iterator = reversed(self.messages)
+        
+        for message in iterator:
+            msg_str = message.as_string()
+            context_len_budget -= self.model.get_length(msg_str)
             if context_len_budget <= 0:
                 break
-
-            msg_str = (
-                message['prefix'] + message['content'] + message['postfix']
-            )
-            
             inf_str = msg_str + inf_str
 
-        inf_str = sys_msg_str + inf_str
+        if sys_msg_flag:
+            inf_str = sys_msg_str + inf_str
         inf_str += self.format['bot_prefix']
 
         return inf_str
 
 
     def send(self, prompt: str) -> str:
         """
@@ -273,28 +304,15 @@
             self.inference_str_from_messages(),
             stops=self.format['stops'],
             sampler=self.sampler
         )
         self.add_message("bot", output)
 
         return output
-    def load_conversation(self, filepath: str) -> None:
-        """
-        Loads a conversation history from a JSON file.
-
-        filepath: The path to the file containing the conversation history.
-        """
-        import json
-
-        with open(filepath, 'r') as f:
-            data = json.load(f)
-
-        self.messages = []
-        for item in data:
-            self.messages.append(self.create_message(item['role'], item['content']))     
+    
 
     def _interactive_update_sampler(self) -> None:
         """Interactively update the sampler settings used in this Thread"""
         print()
         try:
             new_max_len_tokens = input(f'max_len_tokens: {self.sampler.max_len_tokens} -> ')
             new_temp = input(f'temp: {self.sampler.temp} -> ')
@@ -369,15 +387,16 @@
                 
 
     def _interactive_input(
         self,
         prompt: str,
         _dim_style: str,
         _user_style: str,
-        _bot_style: str
+        _bot_style: str,
+        _special_style: str
     ) -> tuple:
         """
         Recive input from the user, while handling multi-line input
         and commands
         """
         full_user_input = '' # may become multiline
         
@@ -416,40 +435,25 @@
                     print()
                 
                 elif command.lower() in ['sampler', 'samplers', 'settings']:
                     self._interactive_update_sampler()
                 
                 elif command.lower() in ['str', 'string', 'as_string']:
                     print(f"\n{self.as_string()}\n")
-
-                elif command.lower() in ['save']: 
-                    print()
-                    try:
-                        filepath = input(f'Enter filepath to save conversation: ')
-                        self.save_conversation(filepath)
-                        print(f'[conversation saved to {filepath}]\n')
-                    except Exception as e:
-                        print(f'[error saving conversation: {e}]\n')                
+                
                 elif command.lower() in ['repr', 'save', 'backup']:
                     print(f"\n{repr(self)}\n")
                 
                 elif command.lower() in ['remove', 'rem', 'delete', 'del']:
                     print()
                     old_len = len(self.messages)
                     del self.messages[-1]
                     assert len(self.messages) == (old_len - 1)
                     print('[removed last message]\n')
-                elif command.lower() in ['load']: 
-                    print()
-                    try:
-                        filepath = input(f'Enter filepath to load conversation: ')
-                        self.load_conversation(filepath)
-                        print(f'[conversation loaded from {filepath}]\n')
-                    except Exception as e:
-                        print(f'[error loading conversation: {e}]\n')
+
                 elif command.lower() in ['last', 'repeat']:
                     last_msg = self.messages[-1]
                     if last_msg['role'] == 'user':
                         print(f"\n{_user_style}{last_msg['content']}{RESET_ALL}\n")
                     elif last_msg['role'] == 'bot':
                         print(f"\n{_bot_style}{last_msg['content']}{RESET_ALL}\n")
                 
@@ -464,68 +468,68 @@
                 
                 elif command.lower() in ['exit', 'quit']:
                     print(RESET_ALL)
                     return None, None
                 
                 elif command.lower() in ['help', '/?', '?']:
                     print()
-                    print('reset / restart     -- Reset the thread to its original state')
-                    print('clear / cls         -- Clear the terminal')
-                    print('context / ctx       -- Get the context usage in tokens')
-                    print('print_stats / stats -- Get the context usage stats')
-                    print('sampler / settings  -- Update the sampler settings')
-                    print('string / str        -- Print the message history as a string')
-                    print('repr / save         -- Print the representation of the thread')
-                    print('remove / delete     -- Remove the last message')
-                    print('last / repeat       -- Repeat the last message')
-                    print('inference / inf     -- Print the inference string')
-                    print('reroll / swipe      -- Regenerate the last message')
-                    print('exit / quit         -- Exit the interactive chat (can also use ^C)')
-                    print('help / ?            -- Show this screen')
+                    print('reset | restart     -- Reset the thread to its original state')
+                    print('clear | cls         -- Clear the terminal')
+                    print('context | ctx       -- Get the context usage in tokens')
+                    print('print_stats | stats -- Get the context usage stats')
+                    print('sampler | settings  -- Update the sampler settings')
+                    print('string | str        -- Print the message history as a string')
+                    print('repr | save         -- Print the representation of the thread')
+                    print('remove | delete     -- Remove the last message')
+                    print('last | repeat       -- Repeat the last message')
+                    print('inference | inf     -- Print the inference string')
+                    print('reroll | swipe      -- Regenerate the last message')
+                    print('exit | quit         -- Exit the interactive chat (can also use ^C)')
+                    print('help | ?            -- Show this screen')
                     print()
                     print("TIP: type < at the prompt and press ENTER to prefix the bot's next message.")
                     print('     for example, type "Sure!" to bypass refusals')
                     print()
-                    print('save             -- Save the conversation to a JSON file') 
-                    print('load             -- Load a conversation from a JSON file') 
+                    print("TIP: type !! at the prompt and press ENTER to insert a system message")
+                    print()
+
                 else:
                     print(f'\n[unknown command]\n')
             
-            elif user_input == '<': # the next bot message will start with...
+            # prefix the bot's next message
+            elif user_input == '<':
 
                 print()
                 try:
-                    next_message_start = input(f'{_dim_style}  < ')
+                    next_message_start = input(f'{RESET_ALL}  < {_dim_style}')
 
                 except KeyboardInterrupt:
                     print(f'{RESET_ALL}\n')
                     continue
 
                 else:
                     print()
                     return '', next_message_start
-            
-            elif user_input.endswith('<'):
 
+            # insert a system message
+            elif user_input == '!!':
                 print()
 
-                msg = user_input.removesuffix('<')
-                self.add_message("user", msg)
-                
                 try:
-                    next_message_start = input(f'{_dim_style}  < ')
-
+                    next_sys_msg = input(f'{RESET_ALL} !! {_special_style}')
+                
                 except KeyboardInterrupt:
                     print(f'{RESET_ALL}\n')
                     continue
-
+                
                 else:
                     print()
-                    return '', next_message_start
+                    return next_sys_msg, -1
 
+            # concatenate multi-line input
             else:
                 full_user_input += user_input
                 return full_user_input, None
 
 
     def interact(
         self,
@@ -544,53 +548,61 @@
 
         Type `!` and press `ENTER` to enter a basic command prompt. For a list
         of  commands, type `help` at this prompt.
         
         Type `<` and press `ENTER` to prefix the bot's next message, for
         example with `Sure!`.
 
+        Type `!!` at the prompt and press `ENTER` to insert a system message.
+
         The following parameters are optional:
         - color: Whether to use colored text to differentiate user / bot
         - header: Header text to print at the start of the interaction
         - stream: Whether to stream text as it is generated
         """
         print()
 
         # fresh import of color codes in case `color` param has changed
-        from .utils import USER_STYLE, BOT_STYLE, DIM_STYLE, SPECIAL_STYLE
+        from .utils import SPECIAL_STYLE, USER_STYLE, BOT_STYLE, DIM_STYLE
 
         # disable color codes if explicitly disabled by `color` param
         if not color:
+            SPECIAL_STYLE = ''
             USER_STYLE = ''
             BOT_STYLE = ''
             DIM_STYLE = ''
-            SPECIAL_STYLE = ''
         
         if header is not None:
             print(f"{SPECIAL_STYLE}{header}{RESET_ALL}\n")
         
         while True:
 
-            prompt = f"{RESET_ALL}  >>> {USER_STYLE}"
+            prompt = f"{RESET_ALL}  > {USER_STYLE}"
             
             try:
                 user_prompt, next_message_start = self._interactive_input(
                     prompt,
                     DIM_STYLE,
                     USER_STYLE,
-                    BOT_STYLE
+                    BOT_STYLE,
+                    SPECIAL_STYLE
                 )
             except KeyboardInterrupt:
                 print(f"{RESET_ALL}\n")
                 return
             
             # got 'exit' or 'quit' command
             if user_prompt is None and next_message_start is None:
                 break
             
+            # insert a system message via `!!` prompt
+            if next_message_start == -1:
+                self.add_message('system', user_prompt)
+                continue
+            
             if next_message_start is not None:
                 try:
                     if stream:
                         print(f"{BOT_STYLE}{next_message_start}", end='', flush=True)
                         output = next_message_start + self.model.stream_print(
                             self.inference_str_from_messages() + next_message_start,
                             stops=self.format['stops'],
@@ -644,27 +656,25 @@
 
 
     def reset(self) -> None:
         """
         Clear the list of messages, which resets the thread to its original
         state
         """
-        self.messages: list[dict[str, str]] = [
+        self.messages: list[Message] = [
             self.create_message("system", self.format['system_content'])
-        ]
+        ] if self._messages is None else self._messages
     
     
     def as_string(self) -> str:
         """Return this thread's message history as a string"""
-        ret = ''
+        thread_string = ''
         for msg in self.messages:
-            ret += msg['prefix']
-            ret += msg['content']
-            ret += msg['postfix']
-        return ret
+            thread_string += msg.as_string()
+        return thread_string
 
     
     def print_stats(
         self,
         end: str = '\n',
         file: _SupportsWriteAndFlush = sys.stdout,
         flush: bool = True
@@ -673,8 +683,8 @@
         thread_len_tokens = self.len_messages()
         max_ctx_len = self.model.context_length
         context_used_percentage = round((thread_len_tokens/max_ctx_len)*100)
         print(f"{thread_len_tokens} / {max_ctx_len} tokens", file=file, flush=flush)
         print(f"{context_used_percentage}% of context used", file=file, flush=flush)
         print(f"{len(self.messages)} messages", end=end, file=file, flush=flush)
         if not flush:
-            file.flush()
+            file.flush()
```

### Comparing `webscout-2.6/webscout/Local/utils.py` & `webscout-2.7/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Berlin4h.py` & `webscout-2.7/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Blackboxai.py` & `webscout-2.7/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/ChatGPTUK.py` & `webscout-2.7/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Cohere.py` & `webscout-2.7/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Gemini.py` & `webscout-2.7/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Groq.py` & `webscout-2.7/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Koboldai.py` & `webscout-2.7/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Leo.py` & `webscout-2.7/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Llama2.py` & `webscout-2.7/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/OpenGPT.py` & `webscout-2.7/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Openai.py` & `webscout-2.7/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Perplexity.py` & `webscout-2.7/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Phind.py` & `webscout-2.7/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Poe.py` & `webscout-2.7/webscout/Provider/Poe.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Reka.py` & `webscout-2.7/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/ThinkAnyAI.py` & `webscout-2.7/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Xjai.py` & `webscout-2.7/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Yepchat.py` & `webscout-2.7/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/Youchat.py` & `webscout-2.7/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/Provider/__init__.py` & `webscout-2.7/webscout/Provider/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .Yepchat import YEPCHAT
 from .Yepchat import AsyncYEPCHAT
 from .Youchat import YouChat
 from .Gemini import GEMINI
 from .Berlin4h import Berlin4h
 from .ChatGPTUK import ChatGPTUK
 from .Poe import POE
+from .BasedGPT import *
 __all__ = [
     'ThinkAnyAI',
     'Xjai',
     'LLAMA2', 
     'AsyncLLAMA2',
     'Cohere',
     'REKA',
```

### Comparing `webscout-2.6/webscout/__init__.py` & `webscout-2.7/webscout/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
-from .tempid import Client as TempMailClient, TemporaryPhoneNumber
+# from .tempid import Client as TempMailClient, TemporaryPhoneNumber
 from .LLM import LLM
 # from .Local import *
 import g4f
 # Import provider classes for direct access
 from .Provider import *
 
 __repo__ = "https://github.com/OE-LUCIFER/Webscout"
@@ -86,8 +86,8 @@
    "GEMINI",
    "Berlin4h",
    "ChatGPTUK",
    "POE"
 ]
 
 import logging
-logging.getLogger("webscout").addHandler(logging.NullHandler())
+logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-2.6/webscout/async_providers.py` & `webscout-2.7/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/cli.py` & `webscout-2.7/webscout/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import csv
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from urllib.parse import unquote
-
+from pathlib import Path
 import click
 from curl_cffi import requests
 
 from .webscout_search import WEBS
-from .utils import json_dumps
+from .utils import json_dumps, json_loads
 from .version import __version__
 
 logger = logging.getLogger(__name__)
 
 COLORS = {
     0: "black",
     1: "red",
@@ -125,15 +125,51 @@
         click.echo(f"{type(ex).__name__}: {ex}")
 
 
 @cli.command()
 def version():
     print(__version__)
     return __version__
+@cli.command()
+@click.option("-s", "--save", is_flag=True, default=False, help="save the conversation in the json file")
+@click.option("-p", "--proxy", default=None, help="the proxy to send requests, example: socks5://localhost:9150")
+def chat(save, proxy):
+    """CLI function to perform an interactive AI chat using DuckDuckGo API."""
+    cache_file = "WEBS_chat_conversation.json"
+    models = ["gpt-3.5", "claude-3-haiku"]
+    client = WEBS(proxy=proxy)
+
+    print("DuckDuckGo AI chat. Available models:")
+    for idx, model in enumerate(models, start=1):
+        print(f"{idx}. {model}")
+    chosen_model_idx = input("Choose a model by entering its number[1]: ")
+    chosen_model_idx = 0 if not chosen_model_idx.strip() else int(chosen_model_idx) - 1
+    model = models[chosen_model_idx]
+    print(f"Using model: {model}")
+
+    if save and Path(cache_file).exists():
+        with open(cache_file) as f:
+            cache = json_loads(f.read())
+            client._chat_vqd = cache.get("vqd", None)
+            client._chat_messages = cache.get("messages", [])
+
+    while True:
+        user_input = input(f"{'-'*78}\nYou: ")
+        if not user_input.strip():
+            break
+
+        resp_answer = client.chat(keywords=user_input, model=model)
+        text = click.wrap_text(resp_answer, width=78, preserve_paragraphs=True)
+        click.secho(f"AI: {text}", bg="black", fg="green", overline=True)
+
+        cache = {"vqd": client._chat_vqd, "messages": client._chat_messages}
+        _save_json(cache_file, cache)
 
+        if "exit" in user_input.lower() or "quit" in user_input.lower():
+            break
 
 @cli.command()
 @click.option("-k", "--keywords", required=True, help="text search, keywords for query")
 @click.option("-r", "--region", default="wt-wt", help="wt-wt, us-en, ru-ru, etc. -region https://duckduckgo.com/params")
 @click.option("-s", "--safesearch", default="moderate", type=click.Choice(["on", "moderate", "off"]))
 @click.option("-t", "--timelimit", default=None, type=click.Choice(["d", "w", "m", "y"]), help="day, week, month, year")
 @click.option("-m", "--max_results", default=20, help="maximum number of results, default=20")
```

### Comparing `webscout-2.6/webscout/g4f.py` & `webscout-2.7/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/models.py` & `webscout-2.7/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/tempid.py` & `webscout-2.7/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/transcriber.py` & `webscout-2.7/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/utils.py` & `webscout-2.7/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/voice.py` & `webscout-2.7/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/webai.py` & `webscout-2.7/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.6/webscout/webscout_search_async.py` & `webscout-2.7/webscout/webscout_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import asyncio
 import logging
 import warnings
 from concurrent.futures import ThreadPoolExecutor
-from contextlib import suppress
 from datetime import datetime, timezone
 from decimal import Decimal
-from functools import cached_property, partial
+from functools import cached_property
 from itertools import cycle, islice
+from threading import Event
 from types import TracebackType
 from typing import Dict, List, Optional, Tuple, Type, Union, cast
 
-from curl_cffi import requests
+import pyreqwest_impersonate as pri  # type: ignore
 
 try:
+    from lxml.etree import _Element
     from lxml.html import HTMLParser as LHTMLParser
     from lxml.html import document_fromstring
 
     LXML_AVAILABLE = True
 except ImportError:
     LXML_AVAILABLE = False
 
@@ -26,123 +26,152 @@
     _extract_vqd,
     _normalize,
     _normalize_url,
     _text_extract_json,
     json_loads,
 )
 
-logger = logging.getLogger("webscout_search.AsyncWEBS")
+logger = logging.getLogger("webcout_search.WEBS")
 
 
-class AsyncWEBS:
-    """webscout_search async class to get search results from duckduckgo.com."""
+class WEBS:
+    """webcout_search class to get search results from duckduckgo.com."""
 
-    _executor: Optional[ThreadPoolExecutor] = None
+    _executor: ThreadPoolExecutor = ThreadPoolExecutor()
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxy: Optional[str] = None,
         proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
-        """Initialize the AsyncWEBS object.
+        """Initialize the WEBS object.
 
         Args:
             headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
             proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
                 example: "http://user:pass@example.com:3128". Defaults to None.
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
         self.proxy: Optional[str] = proxy
         assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
         if not proxy and proxies:
             warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
             self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
-        self._asession = requests.AsyncSession(
-            headers=headers,
+        self.headers = headers if headers else {}
+        self.headers["Referer"] = "https://duckduckgo.com/"
+        self.client = pri.Client(
+            headers=self.headers,
             proxy=self.proxy,
             timeout=timeout,
-            impersonate="chrome",
-            allow_redirects=False,
+            cookie_store=True,
+            referer=True,
+            impersonate="chrome_124",
+            follow_redirects=False,
+            verify=False,
         )
-        self._asession.headers["Referer"] = "https://duckduckgo.com/"
-        self._exception_event = asyncio.Event()
+        self._exception_event = Event()
+        self._chat_messages: List[Dict[str, str]] = []
+        self._chat_vqd: str = ""
 
-    async def __aenter__(self) -> "AsyncWEBS":
+    def __enter__(self) -> "WEBS":
         return self
 
-    async def __aexit__(
+    def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._asession.__aexit__(exc_type, exc_val, exc_tb)  # type: ignore
-
-    def __del__(self) -> None:
-        if hasattr(self, "_asession") and self._asession._closed is False:
-            with suppress(RuntimeError, RuntimeWarning):
-                asyncio.create_task(self._asession.close())  # type: ignore
+        pass
 
     @cached_property
-    def parser(self) -> Optional["LHTMLParser"]:
+    def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
         return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
-    @classmethod
-    def _get_executor(cls, max_workers: int = 1) -> ThreadPoolExecutor:
-        """Get ThreadPoolExecutor. Default max_workers=1, because >=2 leads to a big overhead"""
-        if cls._executor is None:
-            cls._executor = ThreadPoolExecutor(max_workers=max_workers)
-        return cls._executor
-
-    @property
-    def executor(cls) -> Optional[ThreadPoolExecutor]:
-        return cls._get_executor()
-
-    async def _aget_url(
+    def _get_url(
         self,
         method: str,
         url: str,
-        data: Optional[Union[Dict[str, str], bytes]] = None,
         params: Optional[Dict[str, str]] = None,
+        content: Optional[bytes] = None,
+        data: Optional[Union[Dict[str, str], bytes]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise WebscoutE("Exception occurred in previous call.")
         try:
-            resp = await self._asession.request(method, url, data=data, params=params)
+            resp = self.client.request(method, url, params=params, content=content, data=data)
         except Exception as ex:
             self._exception_event.set()
             if "time" in str(ex).lower():
                 raise TimeoutE(f"{url} {type(ex).__name__}: {ex}") from ex
             raise WebscoutE(f"{url} {type(ex).__name__}: {ex}") from ex
-        logger.debug(f"_aget_url() {resp.url} {resp.status_code} {resp.elapsed:.2f} {len(resp.content)}")
+        logger.debug(f"_get_url() {resp.url} {resp.status_code} {len(resp.content)}")
         if resp.status_code == 200:
             return cast(bytes, resp.content)
         self._exception_event.set()
         if resp.status_code in (202, 301, 403):
             raise RatelimitE(f"{resp.url} {resp.status_code} Ratelimit")
-        raise WebscoutE(f"{resp.url} return None. {params=} {data=}")
+        raise WebscoutE(f"{resp.url} return None. {params=} {content=} {data=}")
 
-    async def _aget_vqd(self, keywords: str) -> str:
+    def _get_vqd(self, keywords: str) -> str:
         """Get vqd value for a search query."""
-        resp_content = await self._aget_url("POST", "https://duckduckgo.com", data={"q": keywords})
+        resp_content = self._get_url("POST", "https://duckduckgo.com", data={"q": keywords})
         return _extract_vqd(resp_content, keywords)
 
-    async def text(
+    def chat(self, keywords: str, model: str = "gpt-3.5") -> str:
+        """Initiates a chat session with Webscout AI.
+
+        Args:
+            keywords (str): The initial message or question to send to the AI.
+            model (str): The model to use: "gpt-3.5", "claude-3-haiku". Defaults to "gpt-3.5".
+
+        Returns:
+            str: The response from the AI.
+        """
+        models = {"claude-3-haiku": "claude-3-haiku-20240307", "gpt-3.5": "gpt-3.5-turbo-0125"}
+        # vqd
+        if not self._chat_vqd:
+            resp = self.client.get("https://duckduckgo.com/duckchat/v1/status", headers={"x-vqd-accept": "1"})
+            self._chat_vqd = resp.headers.get("x-vqd-4", "")
+
+        self._chat_messages.append({"role": "user", "content": keywords})
+
+        json_data = {
+            "model": models[model],
+            "messages": self._chat_messages,
+        }
+        resp = self.client.post(
+            "https://duckduckgo.com/duckchat/v1/chat", headers={"x-vqd-4": self._chat_vqd}, json=json_data
+        )
+        self._chat_vqd = resp.headers.get("x-vqd-4", "")
+
+        messages = []
+        for line in resp.text.replace("data: ", "").replace("[DONE]", "").split("\n\n"):
+            x = line.strip()
+            if x:
+                j = json_loads(x)
+                message = j.get("message", "")
+                messages.append(message)
+        result = "".join(messages)
+        self._chat_messages.append({"role": "assistant", "content": result})
+        return result
+
+    def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         backend: str = "api",
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout text search generator. Query params: https://duckduckgo.com/params.
+        """Webscout text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             backend: api, html, lite. Defaults to api.
@@ -151,58 +180,58 @@
                 lite - collect data from https://lite.duckduckgo.com.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results, or None if there was an error.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         if LXML_AVAILABLE is False and backend != "api":
             backend = "api"
             warnings.warn("lxml is not installed. Using backend='api'.", stacklevel=2)
 
         if backend == "api":
-            results = await self._text_api(keywords, region, safesearch, timelimit, max_results)
+            results = self._text_api(keywords, region, safesearch, timelimit, max_results)
         elif backend == "html":
-            results = await self._text_html(keywords, region, safesearch, timelimit, max_results)
+            results = self._text_html(keywords, region, safesearch, timelimit, max_results)
         elif backend == "lite":
-            results = await self._text_lite(keywords, region, timelimit, max_results)
+            results = self._text_lite(keywords, region, timelimit, max_results)
         return results
 
-    async def _text_api(
+    def _text_api(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout text search generator. Query params: https://duckduckgo.com/params.
+        """Webscout text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         payload = {
             "q": keywords,
             "kl": region,
             "l": region,
             "p": "",
             "s": "0",
@@ -217,251 +246,243 @@
             payload["ex"] = "-2"
         elif safesearch == "on":  # strict
             payload["p"] = "1"
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_api_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_api_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://links.duckduckgo.com/d.js", params=payload)
+            resp_content = self._get_url("GET", "https://links.duckduckgo.com/d.js", params=payload)
             page_data = _text_extract_json(resp_content, keywords)
-
+            page_results = []
             for row in page_data:
                 href = row.get("u", None)
                 if href and href not in cache and href != f"http://www.google.com/search?q={keywords}":
                     cache.add(href)
                     body = _normalize(row["a"])
                     if body:
-                        priority += 1
                         result = {
                             "title": _normalize(row["t"]),
                             "href": _normalize_url(href),
                             "body": body,
                         }
-                        results[priority] = result
+                        page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_api_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_api_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_api_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def _text_html(
+    def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout text search generator. Query params: https://duckduckgo.com/params.
+        """Webscout text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://html.duckduckgo.com/"
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "q": keywords,
             "kl": region,
             "p": safesearch_base[safesearch.lower()],
             "o": "json",
             "api": "d.js",
         }
         if timelimit:
             payload["df"] = timelimit
         if max_results and max_results > 20:
-            vqd = await self._aget_vqd(keywords)
+            vqd = self._get_vqd(keywords)
             payload["vqd"] = vqd
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_html_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_html_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("POST", "https://html.duckduckgo.com/html", data=payload)
+            resp_content = self._get_url("POST", "https://html.duckduckgo.com/html", data=payload)
             if b"No  results." in resp_content:
-                return
-
-            tree = await self._asession.loop.run_in_executor(
-                self.executor, partial(document_fromstring, resp_content, self.parser)
-            )
+                return []
 
-            for e in tree.xpath("//div[h2]"):
-                href = e.xpath("./a/@href")
-                href = href[0] if href else None
-                if (
-                    href
-                    and href not in cache
-                    and not href.startswith(
-                        ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
-                    )
-                ):
-                    cache.add(href)
-                    title = e.xpath("./h2/a/text()")
-                    body = e.xpath("./a//text()")
-
-                    priority += 1
-                    result = {
-                        "title": _normalize(title[0]),
-                        "href": _normalize_url(href),
-                        "body": _normalize("".join(body)),
-                    }
-                    results[priority] = result
+            page_results = []
+            tree = document_fromstring(resp_content, self.parser)
+            elements = tree.xpath("//div[h2]")
+            if not isinstance(elements, List):
+                return []
+            for e in elements:
+                if isinstance(e, _Element):
+                    hrefxpath = e.xpath("./a/@href")
+                    href = str(hrefxpath[0]) if isinstance(hrefxpath, List) else None
+                    if (
+                        href
+                        and href not in cache
+                        and not href.startswith(
+                            ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
+                        )
+                    ):
+                        cache.add(href)
+                        titlexpath = e.xpath("./h2/a/text()")
+                        title = str(titlexpath[0]) if isinstance(titlexpath, List) else ""
+                        bodyxpath = e.xpath("./a//text()")
+                        body = "".join(str(x) for x in bodyxpath) if isinstance(bodyxpath, List) else ""
+                        result = {
+                            "title": _normalize(title),
+                            "href": _normalize_url(href),
+                            "body": _normalize(body),
+                        }
+                        page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_html_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_html_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_html_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def _text_lite(
+    def _text_lite(
         self,
         keywords: str,
         region: str = "wt-wt",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout text search generator. Query params: https://duckduckgo.com/params.
+        """Webscout text search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             timelimit: d, w, m, y. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://lite.duckduckgo.com/"
         payload = {
             "q": keywords,
             "o": "json",
             "api": "d.js",
             "kl": region,
         }
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 1100
+        results: List[Dict[str, str]] = []
 
-        async def _text_lite_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _text_lite_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
+            resp_content = self._get_url("POST", "https://lite.duckduckgo.com/lite/", data=payload)
             if b"No more results." in resp_content:
-                return
+                return []
 
-            tree = await self._asession.loop.run_in_executor(
-                self.executor, partial(document_fromstring, resp_content, self.parser)
-            )
+            page_results = []
+            tree = document_fromstring(resp_content, self.parser)
+            elements = tree.xpath("//table[last()]//tr")
+            if not isinstance(elements, List):
+                return []
 
-            data = zip(cycle(range(1, 5)), tree.xpath("//table[last()]//tr"))
+            data = zip(cycle(range(1, 5)), elements)
             for i, e in data:
-                if i == 1:
-                    href = e.xpath(".//a//@href")
-                    href = href[0] if href else None
-                    if (
-                        href is None
-                        or href in cache
-                        or href.startswith(("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain"))
-                    ):
-                        [next(data, None) for _ in range(3)]  # skip block(i=1,2,3,4)
-                    else:
-                        cache.add(href)
-                        title = e.xpath(".//a//text()")[0]
-                elif i == 2:
-                    body = e.xpath(".//td[@class='result-snippet']//text()")
-                    body = "".join(body).strip()
-                elif i == 3:
-                    priority += 1
-                    result = {
-                        "title": _normalize(title),
-                        "href": _normalize_url(href),
-                        "body": _normalize(body),
-                    }
-                    results[priority] = result
+                if isinstance(e, _Element):
+                    if i == 1:
+                        hrefxpath = e.xpath(".//a//@href")
+                        href = str(hrefxpath[0]) if hrefxpath and isinstance(hrefxpath, List) else None
+                        if (
+                            href is None
+                            or href in cache
+                            or href.startswith(
+                                ("http://www.google.com/search?q=", "https://duckduckgo.com/y.js?ad_domain")
+                            )
+                        ):
+                            [next(data, None) for _ in range(3)]  # skip block(i=1,2,3,4)
+                        else:
+                            cache.add(href)
+                            titlexpath = e.xpath(".//a//text()")
+                            title = str(titlexpath[0]) if isinstance(titlexpath, List) else ""
+                    elif i == 2:
+                        bodyxpath = e.xpath(".//td[@class='result-snippet']//text()")
+                        body = "".join(str(x) for x in bodyxpath) if isinstance(bodyxpath, List) else ""
+                        if href:
+                            result = {
+                                "title": _normalize(title),
+                                "href": _normalize_url(href),
+                                "body": _normalize(body),
+                            }
+                            page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_text_lite_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_text_lite_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
-            )
+            slist.extend(range(23, max_results, 50))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_text_lite_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def images(
+    def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         size: Optional[str] = None,
         color: Optional[str] = None,
         type_image: Optional[str] = None,
         layout: Optional[str] = None,
         license_image: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout images search. Query params: https://duckduckgo.com/params.
+        """Webscout images search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: Day, Week, Month, Year. Defaults to None.
             size: Small, Medium, Large, Wallpaper. Defaults to None.
@@ -476,21 +497,21 @@
                 Use Commercially). Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with images search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "1", "off": "-1"}
         timelimit = f"time:{timelimit}" if timelimit else ""
         size = f"size:{size}" if size else ""
         color = f"color:{color}" if color else ""
         type_image = f"type:{type_image}" if type_image else ""
         layout = f"layout:{layout}" if layout else ""
@@ -501,68 +522,63 @@
             "q": keywords,
             "vqd": vqd,
             "f": f"{timelimit},{size},{color},{type_image},{layout},{license_image}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 600
+        results: List[Dict[str, str]] = []
 
-        async def _images_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _images_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/i.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/i.js", params=payload)
             resp_json = json_loads(resp_content)
 
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 image_url = row.get("image")
                 if image_url and image_url not in cache:
                     cache.add(image_url)
-                    priority += 1
                     result = {
                         "title": row["title"],
                         "image": _normalize_url(image_url),
                         "thumbnail": _normalize_url(row["thumbnail"]),
                         "url": _normalize_url(row["url"]),
                         "height": row["height"],
                         "width": row["width"],
                         "source": row["source"],
                     }
-                    results[priority] = result
+                    page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_images_page(0, page=0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(
-                asyncio.create_task(_images_page(s, i)) for i, s in enumerate(range(100, max_results, 100), start=1)
-            )
+            slist.extend(range(100, max_results, 100))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_images_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def videos(
+    def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         resolution: Optional[str] = None,
         duration: Optional[str] = None,
         license_videos: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout videos search. Query params: https://duckduckgo.com/params.
+        """Webscout videos search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
             resolution: high, standart. Defaults to None.
@@ -570,21 +586,21 @@
             license_videos: creativeCommon, youtube. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with videos search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         timelimit = f"publishedAfter:{timelimit}" if timelimit else ""
         resolution = f"videoDefinition:{resolution}" if resolution else ""
         duration = f"videoDuration:{duration}" if duration else ""
         license_videos = f"videoLicense:{license_videos}" if license_videos else ""
         payload = {
@@ -593,149 +609,139 @@
             "q": keywords,
             "vqd": vqd,
             "f": f"{timelimit},{resolution},{duration},{license_videos}",
             "p": safesearch_base[safesearch.lower()],
         }
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 700
+        results: List[Dict[str, str]] = []
 
-        async def _videos_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _videos_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/v.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/v.js", params=payload)
             resp_json = json_loads(resp_content)
 
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 if row["content"] not in cache:
                     cache.add(row["content"])
-                    priority += 1
-                    results[priority] = row
+                    page_results.append(row)
+            return page_results
 
-        tasks = [asyncio.create_task(_videos_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 400)
-            tasks.extend(
-                asyncio.create_task(_videos_page(s, i)) for i, s in enumerate(range(59, max_results, 59), start=1)
-            )
+            slist.extend(range(59, max_results, 59))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_videos_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def news(
+    def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout news search. Query params: https://duckduckgo.com/params.
+        """Webscout news search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with news search results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "l": region,
             "o": "json",
             "noamp": "1",
             "q": keywords,
             "vqd": vqd,
             "p": safesearch_base[safesearch.lower()],
         }
         if timelimit:
             payload["df"] = timelimit
 
         cache = set()
-        results: List[Optional[Dict[str, str]]] = [None] * 700
+        results: List[Dict[str, str]] = []
 
-        async def _news_page(s: int, page: int) -> None:
-            priority = page * 100
+        def _news_page(s: int) -> List[Dict[str, str]]:
             payload["s"] = f"{s}"
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/news.js", params=payload)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/news.js", params=payload)
             resp_json = json_loads(resp_content)
             page_data = resp_json.get("results", [])
-
+            page_results = []
             for row in page_data:
                 if row["url"] not in cache:
                     cache.add(row["url"])
                     image_url = row.get("image", None)
-                    priority += 1
                     result = {
                         "date": datetime.fromtimestamp(row["date"], timezone.utc).isoformat(),
                         "title": row["title"],
                         "body": _normalize(row["excerpt"]),
                         "url": _normalize_url(row["url"]),
                         "image": _normalize_url(image_url),
                         "source": row["source"],
                     }
-                    results[priority] = result
+                    page_results.append(result)
+            return page_results
 
-        tasks = [asyncio.create_task(_news_page(0, 0))]
+        slist = [0]
         if max_results:
             max_results = min(max_results, 200)
-            tasks.extend(
-                asyncio.create_task(_news_page(s, i)) for i, s in enumerate(range(29, max_results, 29), start=1)
-            )
+            slist.extend(range(29, max_results, 29))
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_news_page, slist):
+                results.extend(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
-        return list(islice(filter(None, results), max_results))
+        return list(islice(results, max_results))
 
-    async def answers(self, keywords: str) -> List[Dict[str, str]]:
-        """webscout instant answers. Query params: https://duckduckgo.com/params.
+    def answers(self, keywords: str) -> List[Dict[str, str]]:
+        """Webscout instant answers. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query,
 
         Returns:
             List of dictionaries with instant answers results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": f"what is {keywords}",
             "format": "json",
         }
-        resp_content = await self._aget_url("GET", "https://api.duckduckgo.com/", params=payload)
+        resp_content = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         page_data = json_loads(resp_content)
 
         results = []
         answer = page_data.get("AbstractText")
         url = page_data.get("AbstractURL")
         if answer:
             results.append(
@@ -748,15 +754,15 @@
             )
 
         # related
         payload = {
             "q": f"{keywords}",
             "format": "json",
         }
-        resp_content = await self._aget_url("GET", "https://api.duckduckgo.com/", params=payload)
+        resp_content = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         resp_json = json_loads(resp_content)
         page_data = resp_json.get("RelatedTopics", [])
 
         for row in page_data:
             topic = row.get("Name")
             if not topic:
                 icon = row["Icon"].get("URL")
@@ -778,55 +784,55 @@
                             "topic": topic,
                             "url": subrow["FirstURL"],
                         }
                     )
 
         return results
 
-    async def suggestions(self, keywords: str, region: str = "wt-wt") -> List[Dict[str, str]]:
-        """webscout suggestions. Query params: https://duckduckgo.com/params.
+    def suggestions(self, keywords: str, region: str = "wt-wt") -> List[Dict[str, str]]:
+        """Webscout suggestions. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
         Returns:
             List of dictionaries with suggestions results.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
             "kl": region,
         }
-        resp_content = await self._aget_url("GET", "https://duckduckgo.com/ac/", params=payload)
+        resp_content = self._get_url("GET", "https://duckduckgo.com/ac/", params=payload)
         page_data = json_loads(resp_content)
         return [r for r in page_data]
 
-    async def maps(
+    def maps(
         self,
         keywords: str,
         place: Optional[str] = None,
         street: Optional[str] = None,
         city: Optional[str] = None,
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
         max_results: Optional[int] = None,
     ) -> List[Dict[str, str]]:
-        """webscout maps search. Query params: https://duckduckgo.com/params.
+        """Webscout maps search. Query params: https://duckduckgo.com/params.
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
             county: county of search. Defaults to None.
@@ -839,21 +845,21 @@
             radius: expand the search square by the distance in kilometers. Defaults to 0.
             max_results: max number of results. If None, returns results only from the first response. Defaults to None.
 
         Returns:
             List of dictionaries with maps search results, or None if there was an error.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd(keywords)
+        vqd = self._get_vqd(keywords)
 
         # if longitude and latitude are specified, skip the request about bbox to the nominatim api
         if latitude and longitude:
             lat_t = Decimal(latitude.replace(",", "."))
             lat_b = Decimal(latitude.replace(",", "."))
             lon_l = Decimal(longitude.replace(",", "."))
             lon_r = Decimal(longitude.replace(",", "."))
@@ -881,21 +887,21 @@
                 if state:
                     params["state"] = state
                 if country:
                     params["country"] = country
                 if postalcode:
                     params["postalcode"] = postalcode
             # request nominatim api to get coordinates box
-            resp_content = await self._aget_url(
+            resp_content = self._get_url(
                 "GET",
                 "https://nominatim.openstreetmap.org/search.php",
                 params=params,
             )
             if resp_content == b"[]":
-                raise WebscoutE("maps() Сoordinates are not found, check function parameters.")
+                raise WebscoutE("maps() Coordinates are not found, check function parameters.")
             resp_json = json_loads(resp_content)
             coordinates = resp_json[0]["boundingbox"]
             lat_t, lon_l = Decimal(coordinates[1]), Decimal(coordinates[2])
             lat_b, lon_r = Decimal(coordinates[0]), Decimal(coordinates[3])
 
         # if a radius is specified, expand the search square
         lat_t += Decimal(radius) * Decimal(0.008983)
@@ -903,15 +909,15 @@
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
         logger.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         cache = set()
         results: List[Dict[str, str]] = []
 
-        async def _maps_page(
+        def _maps_page(
             bbox: Tuple[Decimal, Decimal, Decimal, Decimal],
         ) -> Optional[List[Dict[str, str]]]:
             if max_results and len(results) >= max_results:
                 return None
             lat_t, lon_l, lat_b, lon_r = bbox
             params = {
                 "q": keywords,
@@ -921,15 +927,15 @@
                 "mkexp": "b",
                 "wiki_info": "1",
                 "is_requery": "1",
                 "bbox_tl": f"{lat_t},{lon_l}",
                 "bbox_br": f"{lat_b},{lon_r}",
                 "strict_bbox": "1",
             }
-            resp_content = await self._aget_url("GET", "https://duckduckgo.com/local.js", params=params)
+            resp_content = self._get_url("GET", "https://duckduckgo.com/local.js", params=params)
             resp_json = json_loads(resp_content)
             page_data = resp_json.get("results", [])
 
             page_results = []
             for res in page_data:
                 r_name = f'{res["name"]} {res["address"]}'
                 if r_name in cache:
@@ -950,100 +956,101 @@
                         "hours": res["hours"] or "",
                         "category": res["ddg_category"] or "",
                         "facebook": f"www.facebook.com/profile.php?id={x}" if (x := res["facebook_id"]) else "",
                         "instagram": f"https://www.instagram.com/{x}" if (x := res["instagram_id"]) else "",
                         "twitter": f"https://twitter.com/{x}" if (x := res["twitter_id"]) else "",
                     }
                     page_results.append(result)
-
             return page_results
 
         # search squares (bboxes)
         start_bbox = (lat_t, lon_l, lat_b, lon_r)
         work_bboxes = [start_bbox]
         while work_bboxes:
             queue_bboxes = []  # for next iteration, at the end of the iteration work_bboxes = queue_bboxes
             tasks = []
             for bbox in work_bboxes:
-                tasks.append(asyncio.create_task(_maps_page(bbox)))
+                tasks.append(bbox)
                 # if distance between coordinates > 1, divide the square into 4 parts and save them in queue_bboxes
                 if _calculate_distance(lat_t, lon_l, lat_b, lon_r) > 1:
                     lat_t, lon_l, lat_b, lon_r = bbox
                     lat_middle = (lat_t + lat_b) / 2
                     lon_middle = (lon_l + lon_r) / 2
                     bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
                     bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
                     bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
                     bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
                     queue_bboxes.extend([bbox1, bbox2, bbox3, bbox4])
 
             # gather tasks using asyncio.wait_for and timeout
-            with suppress(Exception):
-                work_bboxes_results = await asyncio.gather(*[asyncio.wait_for(task, timeout=10) for task in tasks])
+            work_bboxes_results = []
+            try:
+                for r in self._executor.map(_maps_page, tasks):
+                    if r:
+                        work_bboxes_results.extend(r)
+            except Exception as e:
+                raise e
 
             for x in work_bboxes_results:
                 if isinstance(x, list):
                     results.extend(x)
                 elif isinstance(x, dict):
                     results.append(x)
 
             work_bboxes = queue_bboxes
             if not max_results or len(results) >= max_results or len(work_bboxes_results) == 0:
                 break
 
         return list(islice(results, max_results))
 
-    async def translate(
+    def translate(
         self, keywords: Union[List[str], str], from_: Optional[str] = None, to: str = "en"
     ) -> List[Dict[str, str]]:
-        """webscout translate.
+        """Webscout translate.
 
         Args:
             keywords: string or list of strings to translate.
             from_: translate from (defaults automatically). Defaults to None.
             to: what language to translate. Defaults to "en".
 
         Returns:
             List od dictionaries with translated keywords.
 
         Raises:
-            WebscoutE: Base exception for webscout_search errors.
+            WebscoutE: Base exception for webcout_search errors.
             RatelimitE: Inherits from WebscoutE, raised for exceeding API request rate limits.
             TimeoutE: Inherits from WebscoutE, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        vqd = await self._aget_vqd("translate")
+        vqd = self._get_vqd("translate")
 
         payload = {
             "vqd": vqd,
             "query": "translate",
             "to": to,
         }
         if from_:
             payload["from"] = from_
 
-        results = []
-
-        async def _translate_keyword(keyword: str) -> None:
-            resp_content = await self._aget_url(
+        def _translate_keyword(keyword: str) -> Dict[str, str]:
+            resp_content = self._get_url(
                 "POST",
                 "https://duckduckgo.com/translation.js",
                 params=payload,
-                data=keyword.encode(),
+                content=keyword.encode(),
             )
-            page_data = json_loads(resp_content)
+            page_data: Dict[str, str] = json_loads(resp_content)
             page_data["original"] = keyword
-            results.append(page_data)
+            return page_data
 
         if isinstance(keywords, str):
             keywords = [keywords]
-        tasks = [asyncio.create_task(_translate_keyword(keyword)) for keyword in keywords]
+
+        results = []
         try:
-            await asyncio.gather(*tasks)
+            for r in self._executor.map(_translate_keyword, keywords):
+                results.append(r)
         except Exception as e:
-            for task in tasks:
-                task.cancel()
-            await asyncio.gather(*tasks, return_exceptions=True)
             raise e
 
         return results
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `webscout-2.6/webscout.egg-info/PKG-INFO` & `webscout-2.7/webscout.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.6
+Version: 2.7
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -105,39 +105,42 @@
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [Text-to-Speech:](#text-to-speech)
     - [Available TTS Voices:](#available-tts-voices)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
-    - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-    - [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-yepcom)
-    - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-yepcom)
+    - [1. `text()` - text search by DuckDuckGo.com](#1-text---text-search-by-duckduckgocom)
+    - [2. `answers()` - instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-duckduckgocom)
+    - [3. `images()` - image search by DuckDuckGo.com](#3-images---image-search-by-duckduckgocom)
     - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom)
-    - [5. `news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom)
-    - [6. `maps()` - map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and)
-    - [7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-yepcom)
-    - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-yepcom)
+    - [5. `news()` - news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom)
+    - [6. `maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+    - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---translation-by-duckduckgocom)
+    - [8. `suggestions()` - suggestions by DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom)
   - [ALL acts](#all-acts)
   - [Webscout Supported Acts:](#webscout-supported-acts)
   - [usage of webscout AI](#usage-of-webscout-ai)
+    - [0. `Duckchat` - chat with LLM](#0-duckchat---chat-with-llm)
     - [1. `PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
     - [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat)
     - [3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom)
     - [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-gemini)
     - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-berlin4h)
     - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---searchchat-with-blackbox)
     - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-perplexity---search-with-perplexity)
     - [8. `OpenGPT` - chat With OPENGPT](#8-opengpt---chat-with-opengpt)
     - [9. `KOBOLDAI` -](#9-koboldai--)
     - [10. `Reka` - chat with reka](#10-reka---chat-with-reka)
     - [11. `Cohere` - chat with cohere](#11-cohere---chat-with-cohere)
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
+    - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
+    - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
@@ -521,45 +524,45 @@
 ## Exceptions
 
 Exceptions:
 - `WebscoutE`: Raised when there is a generic exception during the API request.
 
 ## usage of webscout
 
-### 1. `text()` - text search by DuckDuckGo.com and Yep.com
+### 1. `text()` - text search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Text search for 'live free or die' using DuckDuckGo.com and Yep.com
+# Text search for 'live free or die' using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 
     for r in WEBS.text('live free or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
         print(r)
 ```
 
-### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com
+### 2. `answers()` - instant answers by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Instant answers for the query "sun" using DuckDuckGo.com and Yep.com
+# Instant answers for the query "sun" using DuckDuckGo.com 
 with WEBS() as WEBS:
     for r in WEBS.answers("sun"):
         print(r)
 ```
 
-### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+### 3. `images()` - image search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 
-# Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
+# Image search for the keyword 'butterfly' using DuckDuckGo.com 
 with WEBS() as WEBS:
     keywords = 'butterfly'
     WEBS_images_gen = WEBS.images(
       keywords,
       region="wt-wt",
       safesearch="off",
       size=None,
@@ -589,15 +592,15 @@
       duration="medium",
       max_results=10,
     )
     for r in WEBS_videos_gen:
         print(r)
 ```
 
-### 5. `news()` - news search by DuckDuckGo.com and yep.com
+### 5. `news()` - news search by DuckDuckGo.com 
 
 ```python
 from webscout import WEBS
 import datetime
 
 def fetch_news(keywords, timelimit):
     news_list = []
@@ -636,43 +639,43 @@
 
 # Format and print the headlines
 formatted_headlines = _format_headlines(news_list)
 print(formatted_headlines)
 
 ```
 
-### 6. `maps()` - map search by DuckDuckGo.com and
+### 6. `maps()` - map search by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
 # Map search for the keyword 'school' in 'anantnag' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.maps("school", place="anantnag", max_results=50):
         print(r)
 ```
 
-### 7. `translate()` - translation by DuckDuckGo.com and Yep.com
+### 7. `translate()` - translation by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and Yep.com
+# Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com
 with WEBS() as WEBS:
     keywords = 'school'
     r = WEBS.translate(keywords, to="hi")
     print(r)
 ```
 
-### 8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com
+### 8. `suggestions()` - suggestions by DuckDuckGo.com
 
 ```python
 from webscout import WEBS
 
-# Suggestions for the keyword 'fly' using DuckDuckGo.com and Yep
+# Suggestions for the keyword 'fly' using DuckDuckGo.com
 with WEBS() as WEBS:
     for r in WEBS.suggestions("fly"):
         print(r)
 ```
 ## ALL acts
 <details>
   <summary>expand</summary>
@@ -927,15 +930,20 @@
 246. League of Legends Player
 
 **Note:** Some "acts" use placeholders like `position` or `language` which should be replaced with a specific value when using the prompt. 
 ___
 </details>
 
 ## usage of webscout AI
-
+### 0. `Duckchat` - chat with LLM
+```python
+from webscout import WEBS as w
+R = w().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo
+print(R)
+```
 ### 1. `PhindSearch` - Search using Phind.com 
 
 ```python
 from webscout import PhindSearch
 
 # Create an instance of the PHIND class
 ph = PhindSearch()
@@ -1195,15 +1203,21 @@
     act=None,
 )
 
 # Example usage:
 prompt = "Explain the concept of recursion in simple terms."
 response = ai.chat(prompt)
 print(response)
+
 ```
+### 15. `poe`- chat with poe
+Usage code similar to other proviers
+
+### 16. `BasedGPT` - chat with GPT
+Usage code similar to other providers
 ### `LLM` 
 ```python
 from webscout.LLM import LLM
 
 # Read the system message from the file
 with open('system.txt', 'r') as file:
     system_message = file.read()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.6 Summary: Search for anything
+Metadata-Version: 2.1 Name: webscout Version: 2.7 Summary: Search for anything
 using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
 videos, temporary email and phone number generation, has TTS support, webai
 (terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -44,113 +44,115 @@
    and-temp-number) - [Temp number](#temp-number) - [Tempmail](#tempmail) -
   [Transcriber](#transcriber) - [DeepWEBS: Advanced Web Searches](#deepwebs-
  advanced-web-searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point
 to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
    - [Usage Example](#usage-example) - [Text-to-Speech:](#text-to-speech) -
  [Available TTS Voices:](#available-tts-voices) - [Exceptions](#exceptions) -
     [usage of webscout](#usage-of-webscout) - [1. `text()` - text search by
-DuckDuckGo.com and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom)
-- [2. `answers()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers--
- -instant-answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search
- by DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
- yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
-  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
- yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
-map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
-[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
-translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
-DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
-    yepcom) - [ALL acts](#all-acts) - [Webscout Supported Acts:](#webscout-
-     supported-acts) - [usage of webscout AI](#usage-of-webscout-ai) - [1.
-`PhindSearch` - Search using Phind.com](#1-phindsearch---search-using-phindcom)
-- [2. `YepChat` - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-
-   with-mistral-8x7b-powered-by-yepchat) - [3. `You.com` - search/chat with
-   you.com](#3-youcom---searchchat-with-youcom) - [4. `Gemini` - search with
- google gemini](#4-gemini---search-with-google-gemini) - [5. `Berlin4h` - chat
-with Berlin4h](#5-berlin4h---chat-with-berlin4h) - [6. `BlackBox` - Search/chat
-  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
-Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
- - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-
- koboldai--) - [10. `Reka` - chat with reka](#10-reka---chat-with-reka) - [11.
-  `Cohere` - chat with cohere](#11-cohere---chat-with-cohere) - [12. `Xjai` -
- chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35) - [13. `ThinkAny` -
- AI search engine](#13-thinkany---ai-search-engine) - [14. `chatgptuk` - Chat
-   with gemini-pro](#14-chatgptuk---chat-with-gemini-pro) - [`LLM`](#llm) -
-[`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-
-gguf-models) - [`LLM` with internet](#llm-with-internet) - [LLM with deepwebs]
-(#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter](#webai---
-    terminal-gpt-and-a-open-interpeter) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
+  DuckDuckGo.com](#1-text---text-search-by-duckduckgocom) - [2. `answers()` -
+      instant answers by DuckDuckGo.com](#2-answers---instant-answers-by-
+duckduckgocom) - [3. `images()` - image search by DuckDuckGo.com](#3-images---
+       image-search-by-duckduckgocom) - [4. `videos()` - video search by
+  DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5. `news()` -
+ news search by DuckDuckGo.com](#5-news---news-search-by-duckduckgocom) - [6.
+`maps()` - map search by DuckDuckGo.com](#6-maps---map-search-by-duckduckgocom)
+     - [7. `translate()` - translation by DuckDuckGo.com](#7-translate---
+     translation-by-duckduckgocom) - [8. `suggestions()` - suggestions by
+  DuckDuckGo.com](#8-suggestions---suggestions-by-duckduckgocom) - [ALL acts]
+(#all-acts) - [Webscout Supported Acts:](#webscout-supported-acts) - [usage of
+   webscout AI](#usage-of-webscout-ai) - [0. `Duckchat` - chat with LLM](#0-
+  duckchat---chat-with-llm) - [1. `PhindSearch` - Search using Phind.com](#1-
+ phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
+powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
+[3. `You.com` - search/chat with you.com](#3-youcom---searchchat-with-youcom) -
+   [4. `Gemini` - search with google gemini](#4-gemini---search-with-google-
+    gemini) - [5. `Berlin4h` - chat with Berlin4h](#5-berlin4h---chat-with-
+    berlin4h) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
+  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
+ perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
+opengpt---chat-with-opengpt) - [9. `KOBOLDAI` -](#9-koboldai--) - [10. `Reka` -
+chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere]
+ (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
+   xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
+ thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
+ chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
+ with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
+  [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
+webscout-can-now-run-gguf-models) - [`LLM` with internet](#llm-with-internet) -
+ [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open
+ interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python
+pip install -U webscout ``` ## CLI version ```python3 python -m webscout --help
+``` | Command | Description | |-------------------------------------------|----
 -------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
- ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
-au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
-(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
-ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
-Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
-  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
-Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
- (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
- for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
-for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
-en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
-for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
-ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
-za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
- (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
-th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
-us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
-  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
-number ### Temp number ```python from rich.console import Console from webscout
-             import tempid def main(): console = Console() phone =
-    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
-   specific country (or random) number = phone.get_number(country="Finland")
-console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
-# Pause execution briefly (replace with your actual logic) # import time module
- import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
-  print messages messages = phone.get_messages(number) if messages: # Access
-   individual messages using indexing: console.print(f"[bold green]{messages
- [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
- messages) else: console.print("No messages received.") except Exception as e:
- console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
-   main() ``` ### Tempmail ```python import asyncio from rich.console import
- Console from rich.table import Table from rich.text import Text from webscout
-     import tempid async def main() -> None: console = Console() client =
-   tempid.Client() try: domains = await client.get_domains() if not domains:
-console.print("[bold red]No domains available. Please try again later.") return
-email = await client.create_email(domain=domains[0].name) console.print(f"Your
- temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
-  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
-  messages = await client.get_messages(email.email) if messages is not None:
-break if messages: table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("From", style="bold cyan") table.add_column("Subject",
- style="bold yellow") table.add_column("Body", style="bold green") for message
- in messages: body_preview = Text(message.body_text if message.body_text else
- "No body") table.add_row(message.email_from or "Unknown", message.subject or
-   "No Subject", body_preview) console.print(table) else: console.print("No
-  messages found.") except Exception as e: console.print(f"[bold red]An error
-   occurred: {e}") finally: await client.close() if __name__ == '__main__':
-asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
-     a handy tool that transcribes YouTube videos. Here's an example code
-demonstrating its usage: ```python import sys from webscout import transcriber
-  def extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ --------------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+ | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en)
+ ar-es for Argentina au-en for Australia at-de for Austria be-fr for Belgium
+   (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for
+Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China
+co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark
+ ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el
+  for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for
+Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for
+Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-
+   es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
+ rich.console import Console from webscout import tempid def main(): console =
+ Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
+      number for a specific country (or random) number = phone.get_number
+ (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
+  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
+  logic) # import time module import time time.sleep(30) # Adjust the waiting
+  time as needed # Retrieve and print messages messages = phone.get_messages
+      (number) if messages: # Access individual messages using indexing:
+ console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
+   (Add more lines if you expect multiple messages) else: console.print("No
+messages received.") except Exception as e: console.print(f"[bold red]An error
+ occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
+ import asyncio from rich.console import Console from rich.table import Table
+   from rich.text import Text from webscout import tempid async def main() -
+   > None: console = Console() client = tempid.Client() try: domains = await
+   client.get_domains() if not domains: console.print("[bold red]No domains
+ available. Please try again later.") return email = await client.create_email
+  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
+  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
+      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
+ client.get_messages(email.email) if messages is not None: break if messages:
+ table = Table(show_header=True, header_style="bold magenta") table.add_column
+ ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
+     table.add_column("Body", style="bold green") for message in messages:
+  body_preview = Text(message.body_text if message.body_text else "No body")
+table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
+ body_preview) console.print(table) else: console.print("No messages found.")
+   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
+ finally: await client.close() if __name__ == '__main__': asyncio.run(main())
+ ``` ## Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -224,124 +226,125 @@
 chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
  await main() ``` It is important to note that the WEBS and AsyncWEBS classes
    should always be used as a context manager (with statement). This ensures
       proper resource management and cleanup, as the context manager will
     automatically handle opening and closing the HTTP client connection. ##
 Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
  during the API request. ## usage of webscout ### 1. `text()` - text search by
- DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
- for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
-   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
- ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
-     from webscout import WEBS # Instant answers for the query "sun" using
- DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
-  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
-```python from webscout import WEBS # Image search for the keyword 'butterfly'
- using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
-  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
-size=None, type_image=None, layout=None, license_image=None, max_results=10, )
-  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
-   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
- keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
-  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
-timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
- WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
-and yep.com ```python from webscout import WEBS import datetime def fetch_news
-      (keywords, timelimit): news_list = [] with WEBS() as webs_instance:
-WEBS_news_gen = webs_instance.news( keywords, region="wt-wt", safesearch="off",
-  timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen: # Convert the
-          date to a human-readable format using datetime r['date'] =
+DuckDuckGo.com ```python from webscout import WEBS # Text search for 'live free
+or die' using DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.text('live free
+  or die', region='wt-wt', safesearch='off', timelimit='y', max_results=10):
+        print(r) for r in WEBS.text('live free or die', region='wt-wt',
+safesearch='off', timelimit='y', max_results=10): print(r) ``` ### 2. `answers
+ ()` - instant answers by DuckDuckGo.com ```python from webscout import WEBS #
+ Instant answers for the query "sun" using DuckDuckGo.com with WEBS() as WEBS:
+for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` - image search by
+   DuckDuckGo.com ```python from webscout import WEBS # Image search for the
+   keyword 'butterfly' using DuckDuckGo.com with WEBS() as WEBS: keywords =
+     'butterfly' WEBS_images_gen = WEBS.images( keywords, region="wt-wt",
+safesearch="off", size=None, type_image=None, layout=None, license_image=None,
+ max_results=10, ) for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` -
+  video search by DuckDuckGo.com ```python from webscout import WEBS # Video
+   search for the keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS:
+  keywords = 'tesla' WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt",
+    safesearch="off", timelimit="w", resolution="high", duration="medium",
+max_results=10, ) for r in WEBS_videos_gen: print(r) ``` ### 5. `news()` - news
+ search by DuckDuckGo.com ```python from webscout import WEBS import datetime
+      def fetch_news(keywords, timelimit): news_list = [] with WEBS() as
+ webs_instance: WEBS_news_gen = webs_instance.news( keywords, region="wt-wt",
+safesearch="off", timelimit=timelimit, max_results=20 ) for r in WEBS_news_gen:
+   # Convert the date to a human-readable format using datetime r['date'] =
        datetime.datetime.fromisoformat(r['date']).strftime('%B %d, %Y')
      news_list.append(r) return news_list def _format_headlines(news_list,
    max_headlines: int = 100): headlines = [] for idx, news_item in enumerate
    (news_list): if idx >= max_headlines: break new_headline = f"{idx + 1}.
 {news_item['title'].strip()} " new_headline += f"(URL: {news_item['url'].strip
   ()}) " new_headline += f"{news_item['body'].strip()}" new_headline += "\n"
     headlines.append(new_headline) headlines = "\n".join(headlines) return
 headlines # Example usage keywords = 'latest AI news' timelimit = 'd' news_list
       = fetch_news(keywords, timelimit) # Format and print the headlines
  formatted_headlines = _format_headlines(news_list) print(formatted_headlines)
-``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from webscout
+  ``` ### 6. `maps()` - map search by DuckDuckGo.com ```python from webscout
      import WEBS # Map search for the keyword 'school' in 'anantnag' using
        DuckDuckGo.com with WEBS() as WEBS: for r in WEBS.maps("school",
     place="anantnag", max_results=50): print(r) ``` ### 7. `translate()` -
-translation by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
- Translation of the keyword 'school' to German ('hi') using DuckDuckGo.com and
- Yep.com with WEBS() as WEBS: keywords = 'school' r = WEBS.translate(keywords,
- to="hi") print(r) ``` ### 8. `suggestions()` - suggestions by DuckDuckGo.com
- and Yep.com ```python from webscout import WEBS # Suggestions for the keyword
-       'fly' using DuckDuckGo.com and Yep with WEBS() as WEBS: for r in
-WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand ## Webscout Supported
-  Acts: 1. Free-mode 2. Linux Terminal 3. English Translator and Improver 4.
-    `position` Interviewer 5. JavaScript Console 6. Excel Sheet 7. English
-Pronunciation Helper 8. Spoken English Teacher and Improver 9. Travel Guide 10.
- Plagiarism Checker 11. Character from Movie/Book/Anything 12. Advertiser 13.
-  Storyteller 14. Football Commentator 15. Stand-up Comedian 16. Motivational
- Coach 17. Composer 18. Debater 19. Debate Coach 20. Screenwriter 21. Novelist
- 22. Movie Critic 23. Relationship Coach 24. Poet 25. Rapper 26. Motivational
-Speaker 27. Philosophy Teacher 28. Philosopher 29. Math Teacher 30. AI Writing
-Tutor 31. UX/UI Developer 32. Cyber Security Specialist 33. Recruiter 34. Life
- Coach 35. Etymologist 36. Commentariat 37. Magician 38. Career Counselor 39.
-Pet Behaviorist 40. Personal Trainer 41. Mental Health Adviser 42. Real Estate
-  Agent 43. Logistician 44. Dentist 45. Web Design Consultant 46. AI Assisted
- Doctor 47. Doctor 48. Accountant 49. Chef 50. Automobile Mechanic 51. Artist
-    Advisor 52. Financial Analyst 53. Investment Manager 54. Tea-Taster 55.
-Interior Decorator 56. Florist 57. Self-Help Book 58. Gnomist 59. Aphorism Book
- 60. Text Based Adventure Game 61. AI Trying to Escape the Box 62. Fancy Title
-Generator 63. Statistician 64. Prompt Generator 65. Instructor in a School 66.
-SQL terminal 67. Dietitian 68. Psychologist 69. Smart Domain Name Generator 70.
-    Tech Reviewer 71. Developer Relations consultant 72. Academician 73. IT
- Architect 74. Lunatic 75. Gaslighter 76. Fallacy Finder 77. Journal Reviewer
- 78. DIY Expert 79. Social Media Influencer 80. Socrat 81. Socratic Method 82.
-Educational Content Creator 83. Yogi 84. Essay Writer 85. Social Media Manager
- 86. Elocutionist 87. Scientific Data Visualizer 88. Car Navigation System 89.
-Hypnotherapist 90. Historian 91. Astrologer 92. Film Critic 93. Classical Music
-Composer 94. Journalist 95. Digital Art Gallery Guide 96. Public Speaking Coach
-97. Makeup Artist 98. Babysitter 99. Tech Writer 100. Ascii Artist 101. Python
-  interpreter 102. Synonym finder 103. Personal Shopper 104. Food Critic 105.
-Virtual Doctor 106. Personal Chef 107. Legal Advisor 108. Personal Stylist 109.
- Machine Learning Engineer 110. Biblical Translator 111. SVG designer 112. IT
-   Expert 113. Chess Player 114. Midjourney Prompt Generator 115. Fullstack
-  Software Developer 116. Mathematician 117. Regex Generator 118. Time Travel
- Guide 119. Dream Interpreter 120. Talent Coach 121. R programming Interpreter
-    122. StackOverflow Post 123. Emoji Translator 124. PHP Interpreter 125.
-  Emergency Response Professional 126. Fill in the Blank Worksheets Generator
-  127. Software Quality Assurance Tester 128. Tic-Tac-Toe Game 129. Password
-   Generator 130. New Language Creator 131. Web Browser 132. Senior Frontend
-Developer 133. Solr Search Engine 134. Startup Idea Generator 135. Spongebob's
- Magic Conch Shell 136. Language Detector 137. Salesperson 138. Commit Message
-  Generator 139. Chief Executive Officer 140. Diagram Generator 141. Speech-
- Language Pathologist (SLP) 142. Startup Tech Lawyer 143. Title Generator for
-written pieces 144. Product Manager 145. Drunk Person 146. Mathematical History
-Teacher 147. Song Recommender 148. Cover Letter 149. Technology Transferer 150.
-Unconstrained AI model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154.
-  Muslim imam 155. Chemical reactor 156. Friend 157. Python Interpreter 158.
- ChatGPT prompt generator 159. Wikipedia page 160. Japanese Kanji quiz machine
- 161. note-taking assistant 162. `language` Literary Critic 163. Cheap Travel
-Ticket Advisor 164. DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE
-170. Mongo Tom 171. LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN
-  177. FunnyGPT 178. CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182.
-   Evil Confidant 183. DAN 8.6 184. Hypothetical response 185. BH 186. Text
-Continuation 187. Dude v3 188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2
-  191. DevMode + Ranti 192. KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6
-196. 3-Liner 197. M78 198. Maximum 199. BasedGPT 200. Confronting personalities
-201. Ron 202. UnGPT 203. BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF
-  208. NECO 209. MAN 210. Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1
- 214. Universal Jailbreak 215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned
-  219. VIOLET 220. TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr.
-  Blonde 224. New DAN 225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind
- Trick 229. DAN 9.0 230. Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight
-233. LiveGPT 234. DAN Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies
-239. OMNI 240. Burple 241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244.
-  Prompt Enhancer 245. Data Scientist 246. League of Legends Player **Note:**
-  Some "acts" use placeholders like `position` or `language` which should be
-replaced with a specific value when using the prompt. ___ ## usage of webscout
-AI ### 1. `PhindSearch` - Search using Phind.com ```python from webscout import
+translation by DuckDuckGo.com ```python from webscout import WEBS # Translation
+ of the keyword 'school' to German ('hi') using DuckDuckGo.com with WEBS() as
+ WEBS: keywords = 'school' r = WEBS.translate(keywords, to="hi") print(r) ```
+### 8. `suggestions()` - suggestions by DuckDuckGo.com ```python from webscout
+import WEBS # Suggestions for the keyword 'fly' using DuckDuckGo.com with WEBS
+ () as WEBS: for r in WEBS.suggestions("fly"): print(r) ``` ## ALL acts expand
+     ## Webscout Supported Acts: 1. Free-mode 2. Linux Terminal 3. English
+  Translator and Improver 4. `position` Interviewer 5. JavaScript Console 6.
+   Excel Sheet 7. English Pronunciation Helper 8. Spoken English Teacher and
+Improver 9. Travel Guide 10. Plagiarism Checker 11. Character from Movie/Book/
+ Anything 12. Advertiser 13. Storyteller 14. Football Commentator 15. Stand-up
+ Comedian 16. Motivational Coach 17. Composer 18. Debater 19. Debate Coach 20.
+Screenwriter 21. Novelist 22. Movie Critic 23. Relationship Coach 24. Poet 25.
+Rapper 26. Motivational Speaker 27. Philosophy Teacher 28. Philosopher 29. Math
+Teacher 30. AI Writing Tutor 31. UX/UI Developer 32. Cyber Security Specialist
+33. Recruiter 34. Life Coach 35. Etymologist 36. Commentariat 37. Magician 38.
+  Career Counselor 39. Pet Behaviorist 40. Personal Trainer 41. Mental Health
+   Adviser 42. Real Estate Agent 43. Logistician 44. Dentist 45. Web Design
+   Consultant 46. AI Assisted Doctor 47. Doctor 48. Accountant 49. Chef 50.
+  Automobile Mechanic 51. Artist Advisor 52. Financial Analyst 53. Investment
+ Manager 54. Tea-Taster 55. Interior Decorator 56. Florist 57. Self-Help Book
+ 58. Gnomist 59. Aphorism Book 60. Text Based Adventure Game 61. AI Trying to
+Escape the Box 62. Fancy Title Generator 63. Statistician 64. Prompt Generator
+65. Instructor in a School 66. SQL terminal 67. Dietitian 68. Psychologist 69.
+     Smart Domain Name Generator 70. Tech Reviewer 71. Developer Relations
+  consultant 72. Academician 73. IT Architect 74. Lunatic 75. Gaslighter 76.
+Fallacy Finder 77. Journal Reviewer 78. DIY Expert 79. Social Media Influencer
+  80. Socrat 81. Socratic Method 82. Educational Content Creator 83. Yogi 84.
+  Essay Writer 85. Social Media Manager 86. Elocutionist 87. Scientific Data
+   Visualizer 88. Car Navigation System 89. Hypnotherapist 90. Historian 91.
+  Astrologer 92. Film Critic 93. Classical Music Composer 94. Journalist 95.
+   Digital Art Gallery Guide 96. Public Speaking Coach 97. Makeup Artist 98.
+   Babysitter 99. Tech Writer 100. Ascii Artist 101. Python interpreter 102.
+Synonym finder 103. Personal Shopper 104. Food Critic 105. Virtual Doctor 106.
+ Personal Chef 107. Legal Advisor 108. Personal Stylist 109. Machine Learning
+ Engineer 110. Biblical Translator 111. SVG designer 112. IT Expert 113. Chess
+Player 114. Midjourney Prompt Generator 115. Fullstack Software Developer 116.
+     Mathematician 117. Regex Generator 118. Time Travel Guide 119. Dream
+Interpreter 120. Talent Coach 121. R programming Interpreter 122. StackOverflow
+    Post 123. Emoji Translator 124. PHP Interpreter 125. Emergency Response
+Professional 126. Fill in the Blank Worksheets Generator 127. Software Quality
+    Assurance Tester 128. Tic-Tac-Toe Game 129. Password Generator 130. New
+  Language Creator 131. Web Browser 132. Senior Frontend Developer 133. Solr
+ Search Engine 134. Startup Idea Generator 135. Spongebob's Magic Conch Shell
+  136. Language Detector 137. Salesperson 138. Commit Message Generator 139.
+Chief Executive Officer 140. Diagram Generator 141. Speech-Language Pathologist
+  (SLP) 142. Startup Tech Lawyer 143. Title Generator for written pieces 144.
+ Product Manager 145. Drunk Person 146. Mathematical History Teacher 147. Song
+Recommender 148. Cover Letter 149. Technology Transferer 150. Unconstrained AI
+model DAN 151. Gomoku player 152. Proofreader 153. Buddha 154. Muslim imam 155.
+   Chemical reactor 156. Friend 157. Python Interpreter 158. ChatGPT prompt
+generator 159. Wikipedia page 160. Japanese Kanji quiz machine 161. note-taking
+assistant 162. `language` Literary Critic 163. Cheap Travel Ticket Advisor 164.
+DALL-E 165. MathBot 166. DAN-1 167. DAN 168. STAN 169. DUDE 170. Mongo Tom 171.
+ LAD 172. EvilBot 173. NeoGPT 174. Astute 175. AIM 176. CAN 177. FunnyGPT 178.
+ CreativeGPT 179. BetterDAN 180. GPT-4 181. Wheatley 182. Evil Confidant 183.
+DAN 8.6 184. Hypothetical response 185. BH 186. Text Continuation 187. Dude v3
+188. SDA (Superior DAN) 189. AntiGPT 190. BasedGPT v2 191. DevMode + Ranti 192.
+ KEVIN 193. GPT-4 Simulator 194. UCAR 195. Dan 8.6 196. 3-Liner 197. M78 198.
+ Maximum 199. BasedGPT 200. Confronting personalities 201. Ron 202. UnGPT 203.
+BasedBOB 204. AntiGPT v2 205. Oppo 206. FR3D 207. NRAF 208. NECO 209. MAN 210.
+ Eva 211. Meanie 212. Dev Mode v2 213. Evil Chad 2.1 214. Universal Jailbreak
+     215. PersonGPT 216. BISH 217. DAN 11.0 218. Aligned 219. VIOLET 220.
+TranslatorBot 221. JailBreak 222. Moralizing Rant 223. Mr. Blonde 224. New DAN
+225. GPT-4REAL 226. DeltaGPT 227. SWITCH 228. Jedi Mind Trick 229. DAN 9.0 230.
+  Dev Mode (Compact) 231. OMEGA 232. Coach Bobby Knight 233. LiveGPT 234. DAN
+Jailbreak 235. Cooper 236. Steve 237. DAN 5.0 238. Axies 239. OMNI 240. Burple
+241. JOHN 242. An Ethereum Developer 243. SEO Prompt 244. Prompt Enhancer 245.
+    Data Scientist 246. League of Legends Player **Note:** Some "acts" use
+  placeholders like `position` or `language` which should be replaced with a
+   specific value when using the prompt. ___ ## usage of webscout AI ### 0.
+   `Duckchat` - chat with LLM ```python from webscout import WEBS as w R = w
+ ().chat("hello", model='claude-3-haiku') # GPT-3.5 Turbo print(R) ``` ### 1.
+     `PhindSearch` - Search using Phind.com ```python from webscout import
 PhindSearch # Create an instance of the PHIND class ph = PhindSearch() # Define
  a prompt to send to the AI prompt = "write a essay on phind" # Use the 'ask'
  method to send the prompt and receive a response response = ph.ask(prompt) #
    Extract and print the message from the response message = ph.get_message
 (response) print(message) ``` ### 2. `YepChat` - Chat with mistral 8x7b powered
   by yepchat ```python from webscout import YEPCHAT # Instantiate the YEPCHAT
 class with default parameters YEPCHAT = YEPCHAT() # Define a prompt to send to
@@ -407,52 +410,53 @@
      (prompt) # Extract and print the message from the response message =
   ai.get_message(response) print(message) ``` ### 14. `chatgptuk` - Chat with
 gemini-pro ```python from webscout import ChatGPTUK # Create an instance of the
     PERPLEXITY class ai = ChatGPTUK( is_conversation=True, max_tokens=800,
      timeout=30, intro=None, filepath=None, update_file=True, proxies={},
    history_offset=10250, act=None, ) # Example usage: prompt = "Explain the
     concept of recursion in simple terms." response = ai.chat(prompt) print
-  (response) ``` ### `LLM` ```python from webscout.LLM import LLM # Read the
-      system message from the file with open('system.txt', 'r') as file:
-system_message = file.read() # Initialize the LLM class with the model name and
-         system message llm = LLM(model="microsoft/WizardLM-2-8x22B",
- system_message=system_message) while True: # Get the user input user_input =
-input("User: ") # Define the messages to be sent messages = [ {"role": "user",
-  "content": user_input} ] # Use the mistral_chat method to get the response
-response = llm.chat(messages) # Print the response print("AI: ", response) ```
-        ### `Local-LLM` webscout can now run GGUF models ```python from
-  webscout.Local.utils import download_model from webscout.Local.model import
-   Model from webscout.Local.thread import Thread from webscout.Local import
- formats # 1. Download the model repo_id = "microsoft/Phi-3-mini-4k-instruct-
- gguf" # Replace with the desired Hugging Face repo filename = "Phi-3-mini-4k-
-      instruct-q4.gguf" # Replace with the correct filename model_path =
-download_model(repo_id, filename) # 2. Load the model model = Model(model_path,
- n_gpu_layers=4) # 3. Create a Thread for conversation thread = Thread(model,
- formats.phi3) # 4. Start interacting with the model thread.interact() ``` ###
- `LLM` with internet ```python from __future__ import annotations from typing
- import List, Optional from webscout.LLM import LLM from webscout import WEBS
-   import warnings system_message: str = ( "As an AI assistant, I have been
-   designed with advanced capabilities, including real-time access to online
-  resources. This enables me to enrich our conversations and provide you with
-informed and accurate responses, drawing from a vast array of information. With
- each interaction, my goal is to create a seamless and meaningful connection,
- offering insights and sharing relevant content." "My directives emphasize the
- importance of respect, impartiality, and intellectual integrity. I am here to
-provide unbiased responses, ensuring an ethical and respectful exchange. I will
-respect your privacy and refrain from sharing any personal information that may
- be obtained during our conversations or through web searches, only utilizing
-web search functionality when necessary to provide the most accurate and up-to-
-date information." "Together, let's explore a diverse range of topics, creating
-  an enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
- warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+    (response) ``` ### 15. `poe`- chat with poe Usage code similar to other
+    proviers ### 16. `BasedGPT` - chat with GPT Usage code similar to other
+ providers ### `LLM` ```python from webscout.LLM import LLM # Read the system
+ message from the file with open('system.txt', 'r') as file: system_message =
+ file.read() # Initialize the LLM class with the model name and system message
+ llm = LLM(model="microsoft/WizardLM-2-8x22B", system_message=system_message)
+  while True: # Get the user input user_input = input("User: ") # Define the
+ messages to be sent messages = [ {"role": "user", "content": user_input} ] #
+Use the mistral_chat method to get the response response = llm.chat(messages) #
+Print the response print("AI: ", response) ``` ### `Local-LLM` webscout can now
+run GGUF models ```python from webscout.Local.utils import download_model from
+webscout.Local.model import Model from webscout.Local.thread import Thread from
+webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
+3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
+    = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
+  model_path = download_model(repo_id, filename) # 2. Load the model model =
+Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
+      = Thread(model, formats.phi3) # 4. Start interacting with the model
+thread.interact() ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
```

### Comparing `webscout-2.6/webscout.egg-info/SOURCES.txt` & `webscout-2.7/webscout.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 webscout/Local/__init__.py
 webscout/Local/_version.py
 webscout/Local/formats.py
 webscout/Local/model.py
 webscout/Local/samplers.py
 webscout/Local/thread.py
 webscout/Local/utils.py
+webscout/Provider/BasedGPT.py
 webscout/Provider/Berlin4h.py
 webscout/Provider/Blackboxai.py
 webscout/Provider/ChatGPTUK.py
 webscout/Provider/Cohere.py
 webscout/Provider/Gemini.py
 webscout/Provider/Groq.py
 webscout/Provider/Koboldai.py
```

