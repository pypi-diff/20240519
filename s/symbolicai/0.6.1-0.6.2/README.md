# Comparing `tmp/symbolicai-0.6.1.tar.gz` & `tmp/symbolicai-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicai-0.6.1.tar", last modified: Thu Feb  1 18:48:34 2024, max compression
+gzip compressed data, was "symbolicai-0.6.2.tar", last modified: Sun May 19 07:56:49 2024, max compression
```

## Comparing `symbolicai-0.6.1.tar` & `symbolicai-0.6.2.tar`

### file list

```diff
@@ -1,254 +1,249 @@
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.126665 symbolicai-0.6.1/
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.088777 symbolicai-0.6.1/.github/
--rw-r--r--   0 xpitfire   (501) staff       (20)      883 2023-10-26 12:37:14.000000 symbolicai-0.6.1/.github/FUNDING.yml
--rw-r--r--   0 xpitfire   (501) staff       (20)     2018 2023-12-16 03:23:24.000000 symbolicai-0.6.1/.gitignore
--rw-r--r--   0 xpitfire   (501) staff       (20)      153 2023-11-24 20:52:59.000000 symbolicai-0.6.1/.readthedocs.yml
--rw-r--r--   0 xpitfire   (501) staff       (20)      435 2023-07-03 17:57:00.000000 symbolicai-0.6.1/CITATION.cff
--rw-r--r--   0 xpitfire   (501) staff       (20)     1643 2023-03-14 14:52:27.000000 symbolicai-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 xpitfire   (501) staff       (20)     1818 2023-12-19 02:22:54.000000 symbolicai-0.6.1/Dockerfile
--rw-r--r--   0 xpitfire   (501) staff       (20)     1539 2023-11-24 20:52:59.000000 symbolicai-0.6.1/LICENSE
--rw-r--r--   0 xpitfire   (501) staff       (20)       91 2023-03-14 14:52:27.000000 symbolicai-0.6.1/MANIFEST.in
--rw-r--r--   0 xpitfire   (501) staff       (20)    97153 2024-02-01 18:48:34.126464 symbolicai-0.6.1/PKG-INFO
--rw-r--r--   0 xpitfire   (501) staff       (20)    94590 2024-02-01 18:23:56.000000 symbolicai-0.6.1/README.md
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.081619 symbolicai-0.6.1/assets/
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.097945 symbolicai-0.6.1/assets/images/
--rw-r--r--   0 xpitfire   (501) staff       (20)    28719 2023-07-03 17:57:00.000000 symbolicai-0.6.1/assets/images/cat.jpg
--rw-r--r--   0 xpitfire   (501) staff       (20)    46058 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img1.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    91342 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img10.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    13911 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img2.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    11183 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img3.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    17206 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img4.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    55580 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img5.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    57683 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img6.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    77023 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img7.png
--rw-r--r--   0 xpitfire   (501) staff       (20)   211609 2023-03-14 14:52:27.000000 symbolicai-0.6.1/assets/images/img8.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    16559 2023-03-14 14:52:28.000000 symbolicai-0.6.1/assets/images/img9.png
--rw-r--r--   0 xpitfire   (501) staff       (20)  1277783 2023-03-14 14:52:28.000000 symbolicai-0.6.1/assets/images/preview.gif
--rw-r--r--   0 xpitfire   (501) staff       (20)   451461 2023-07-09 00:16:05.000000 symbolicai-0.6.1/assets/images/screen1.jpeg
--rw-r--r--   0 xpitfire   (501) staff       (20)   127115 2023-03-14 14:52:28.000000 symbolicai-0.6.1/assets/images/symai_logo.png
--rw-r--r--   0 xpitfire   (501) staff       (20)   103992 2023-10-25 18:32:43.000000 symbolicai-0.6.1/assets/images/symsh.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    42756 2023-08-04 06:12:51.000000 symbolicai-0.6.1/assets/images/vid1.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    78774 2023-08-04 06:12:51.000000 symbolicai-0.6.1/assets/images/vid2.png
--rw-r--r--   0 xpitfire   (501) staff       (20)   141729 2023-08-04 06:12:51.000000 symbolicai-0.6.1/assets/images/vid3.png
--rw-r--r--   0 xpitfire   (501) staff       (20)    59810 2023-08-04 06:12:51.000000 symbolicai-0.6.1/assets/images/vid4.png
--rw-r--r--   0 xpitfire   (501) staff       (20)   318171 2023-11-21 17:16:48.000000 symbolicai-0.6.1/assets/images/vid5.png
--rw-r--r--   0 xpitfire   (501) staff       (20)  1603606 2023-12-09 17:14:47.000000 symbolicai-0.6.1/assets/images/vid6.png
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.098977 symbolicai-0.6.1/bin/
--rw-r--r--   0 xpitfire   (501) staff       (20)     2149 2023-07-21 06:07:52.000000 symbolicai-0.6.1/bin/install.ps1
--rwxr-xr-x   0 xpitfire   (501) staff       (20)     3379 2023-07-21 06:07:52.000000 symbolicai-0.6.1/bin/install.sh
--rw-r--r--   0 xpitfire   (501) staff       (20)     2893 2023-12-19 02:22:54.000000 symbolicai-0.6.1/conf.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      251 2023-12-19 02:22:54.000000 symbolicai-0.6.1/docker-compose.yml
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.099101 symbolicai-0.6.1/docs/
--rw-r--r--   0 xpitfire   (501) staff       (20)      241 2023-07-03 17:57:00.000000 symbolicai-0.6.1/docs/requirements.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)      477 2023-07-06 10:23:44.000000 symbolicai-0.6.1/environment.yml
--rw-r--r--   0 xpitfire   (501) staff       (20)      251 2023-07-03 17:57:00.000000 symbolicai-0.6.1/index.rst
--rw-r--r--   0 xpitfire   (501) staff       (20)     1681 2023-12-09 17:14:47.000000 symbolicai-0.6.1/modules.rst
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.100950 symbolicai-0.6.1/notebooks/
--rw-r--r--   0 xpitfire   (501) staff       (20)    25155 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/Basics.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)     5660 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/ChatBot.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)     7315 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/Conversation.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)    22176 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/Indexer.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)    21040 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/News.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)    14881 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/Queries.ipynb
--rw-r--r--   0 xpitfire   (501) staff       (20)    18326 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/TTS_Persona.ipynb
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.103767 symbolicai-0.6.1/notebooks/examples/
--rw-r--r--   0 xpitfire   (501) staff       (20)     2235 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/a_star.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)     1512 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/examples/abstract.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    24045 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/audio.mp3
--rw-r--r--   0 xpitfire   (501) staff       (20)    66712 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/dbpedia_samples.jsonl
--rw-r--r--   0 xpitfire   (501) staff       (20)    52057 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/dbpedia_samples_prepared_train.jsonl
--rw-r--r--   0 xpitfire   (501) staff       (20)    13257 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/dbpedia_samples_prepared_valid.jsonl
--rw-r--r--   0 xpitfire   (501) staff       (20)     2718 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/examples/demo.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1961 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/demo_strategy.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     4529 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/docs.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      920 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/einsteins_puzzle.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)      495 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/file.json
--rw-r--r--   0 xpitfire   (501) staff       (20)     5190 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/examples/news.py
--rw-r--r--   0 xpitfire   (501) staff       (20)   762191 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/paper.pdf
--rw-r--r--   0 xpitfire   (501) staff       (20)     2671 2024-02-01 18:23:56.000000 symbolicai-0.6.1/notebooks/examples/paper.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2743 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/examples/sql.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.103902 symbolicai-0.6.1/notebooks/outputs/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-12-09 17:14:47.000000 symbolicai-0.6.1/notebooks/outputs/tmp.html.pkl
--rw-r--r--   0 xpitfire   (501) staff       (20)     2623 2024-02-01 18:23:56.000000 symbolicai-0.6.1/pyproject.toml
--rw-r--r--   0 xpitfire   (501) staff       (20)       38 2024-02-01 18:48:34.126707 symbolicai-0.6.1/setup.cfg
--rw-r--r--   0 xpitfire   (501) staff       (20)       37 2023-03-14 14:52:28.000000 symbolicai-0.6.1/setup.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.108402 symbolicai-0.6.1/symai/
--rw-r--r--   0 xpitfire   (501) staff       (20)    91409 2023-11-25 10:54:47.000000 symbolicai-0.6.1/symai/TERMS_OF_SERVICE.md
--rw-r--r--   0 xpitfire   (501) staff       (20)    18656 2024-02-01 18:43:37.000000 symbolicai-0.6.1/symai/__init__.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.108778 symbolicai-0.6.1/symai/backend/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-03-14 14:52:28.000000 symbolicai-0.6.1/symai/backend/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5836 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/base.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.108895 symbolicai-0.6.1/symai/backend/driver/
--rw-r--r--   0 xpitfire   (501) staff       (20)     7854 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/driver/webclient.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.109059 symbolicai-0.6.1/symai/backend/engines/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/engines/__init__.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.109233 symbolicai-0.6.1/symai/backend/engines/crawler/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3223 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/crawler/engine_selenium.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.109569 symbolicai-0.6.1/symai/backend/engines/embedding/
--rw-r--r--   0 xpitfire   (501) staff       (20)     2542 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/embedding/engine_openai.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      606 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/embedding/engine_plugin_embeddings.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.109715 symbolicai-0.6.1/symai/backend/engines/execute/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3736 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/engines/execute/engine_python.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.110152 symbolicai-0.6.1/symai/backend/engines/experiments/
--rw-r--r--   0 xpitfire   (501) staff       (20)     5321 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/experiments/engine_bard_wrapper.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      804 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/engines/experiments/engine_gptfinetuner.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5268 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/experiments/engine_llamacpp_completion.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.110326 symbolicai-0.6.1/symai/backend/engines/files/
--rw-r--r--   0 xpitfire   (501) staff       (20)     5588 2023-12-10 07:39:28.000000 symbolicai-0.6.1/symai/backend/engines/files/engine_io.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.110629 symbolicai-0.6.1/symai/backend/engines/imagecaptioning/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3124 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/imagecaptioning/engine_blip2.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6151 2023-12-18 14:52:06.000000 symbolicai-0.6.1/symai/backend/engines/imagecaptioning/engine_llavacpp_client.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.110813 symbolicai-0.6.1/symai/backend/engines/imagerendering/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3978 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/imagerendering/engine_dall_e.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.111377 symbolicai-0.6.1/symai/backend/engines/index/
--rw-r--r--   0 xpitfire   (501) staff       (20)     8787 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/index/engine_pinecone.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     7495 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/index/engine_vectordb.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.111940 symbolicai-0.6.1/symai/backend/engines/neurosymbolic/
--rw-r--r--   0 xpitfire   (501) staff       (20)     5605 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_nesy_client.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    17144 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_openai_gptX_chat.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    14096 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_openai_gptX_completion.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.112335 symbolicai-0.6.1/symai/backend/engines/ocr/
--rw-r--r--   0 xpitfire   (501) staff       (20)     2356 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/ocr/engine_apilayer.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.112479 symbolicai-0.6.1/symai/backend/engines/output/
--rw-r--r--   0 xpitfire   (501) staff       (20)      912 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/output/engine_stdout.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.112629 symbolicai-0.6.1/symai/backend/engines/search/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3513 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/search/engine_serpapi.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.112753 symbolicai-0.6.1/symai/backend/engines/speech_to_text/
--rw-r--r--   0 xpitfire   (501) staff       (20)     7355 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/engines/speech_to_text/engine_whisper.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.112919 symbolicai-0.6.1/symai/backend/engines/symbolic/
--rw-r--r--   0 xpitfire   (501) staff       (20)     1962 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/symbolic/engine_wolframalpha.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.113040 symbolicai-0.6.1/symai/backend/engines/text_to_speech/
--rw-r--r--   0 xpitfire   (501) staff       (20)     2117 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/text_to_speech/engine_openai.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.113172 symbolicai-0.6.1/symai/backend/engines/text_vision/
--rw-r--r--   0 xpitfire   (501) staff       (20)     3353 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/backend/engines/text_vision/engine_clip.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.113284 symbolicai-0.6.1/symai/backend/engines/userinput/
--rw-r--r--   0 xpitfire   (501) staff       (20)      744 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/engines/userinput/engine_console.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.113595 symbolicai-0.6.1/symai/backend/mixin/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-07-03 17:57:00.000000 symbolicai-0.6.1/symai/backend/mixin/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2972 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/backend/mixin/openai.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     4240 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/mixin/tracker.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.114123 symbolicai-0.6.1/symai/backend/services/
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.114527 symbolicai-0.6.1/symai/backend/services/configs/
--rw-r--r--   0 xpitfire   (501) staff       (20)      223 2023-10-25 18:32:43.000000 symbolicai-0.6.1/symai/backend/services/configs/huggingface_causallm.config.json
--rw-r--r--   0 xpitfire   (501) staff       (20)      223 2023-10-25 18:32:43.000000 symbolicai-0.6.1/symai/backend/services/configs/huggingface_seq2seqlm.config.json
--rw-r--r--   0 xpitfire   (501) staff       (20)     6581 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/services/huggingface_causallm_server.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      651 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/services/huggingface_client.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6103 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/backend/services/huggingface_seq2seqlm_server.py
--rw-r--r--   0 xpitfire   (501) staff       (20)       36 2023-11-02 17:40:09.000000 symbolicai-0.6.1/symai/backend/settings.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    13534 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/chat.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.115106 symbolicai-0.6.1/symai/collect/
--rw-r--r--   0 xpitfire   (501) staff       (20)      104 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/collect/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3928 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/collect/dynamic.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5385 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/collect/pipeline.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    14511 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/collect/stats.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    32534 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/components.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1641 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/constraints.py
--rw-r--r--   0 xpitfire   (501) staff       (20)   118582 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/core.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5640 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/core_ext.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.115387 symbolicai-0.6.1/symai/endpoints/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-11-21 00:42:40.000000 symbolicai-0.6.1/symai/endpoints/__init__py
--rw-r--r--   0 xpitfire   (501) staff       (20)    17772 2023-12-30 18:23:54.000000 symbolicai-0.6.1/symai/endpoints/api.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      165 2023-07-08 22:09:24.000000 symbolicai-0.6.1/symai/exceptions.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.118826 symbolicai-0.6.1/symai/extended/
--rw-r--r--   0 xpitfire   (501) staff       (20)      516 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6175 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/api_builder.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2155 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/arxiv_pdf_parser.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3739 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/bibtex_parser.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     9860 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/conversation.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      734 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/crawler.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1767 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/document.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2982 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/file_merger.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3317 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/graph.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3588 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/html_style_template.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.121192 symbolicai-0.6.1/symai/extended/interfaces/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-11-27 22:13:29.000000 symbolicai-0.6.1/symai/extended/interfaces/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      429 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/extended/interfaces/blip_2.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      458 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/clip.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      410 2023-07-21 06:07:56.000000 symbolicai-0.6.1/symai/extended/interfaces/console.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      500 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/dall_e.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      411 2023-11-29 12:56:27.000000 symbolicai-0.6.1/symai/extended/interfaces/file.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      403 2023-07-21 06:07:56.000000 symbolicai-0.6.1/symai/extended/interfaces/input.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      413 2023-12-14 18:07:49.000000 symbolicai-0.6.1/symai/extended/interfaces/llava.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      517 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/ocr.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      978 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/interfaces/pinecone.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      372 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/python.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      616 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/interfaces/selenium.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      477 2023-12-12 16:17:08.000000 symbolicai-0.6.1/symai/extended/interfaces/serpapi.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      352 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/interfaces/terminal.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      430 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/tts.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      978 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/interfaces/vectordb.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      495 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/whisper.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      443 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/interfaces/wolframalpha.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.121419 symbolicai-0.6.1/symai/extended/metrics/
--rw-r--r--   0 xpitfire   (501) staff       (20)       25 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/metrics/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3352 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/metrics/similarity.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3813 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/os_command.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.121892 symbolicai-0.6.1/symai/extended/packages/
--rw-r--r--   0 xpitfire   (501) staff       (20)       43 2023-07-05 23:54:39.000000 symbolicai-0.6.1/symai/extended/packages/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3662 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/packages/symdev.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2893 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/packages/sympkg.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5131 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/packages/symrun.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.122445 symbolicai-0.6.1/symai/extended/personas/
--rw-r--r--   0 xpitfire   (501) staff       (20)       95 2023-11-09 15:36:35.000000 symbolicai-0.6.1/symai/extended/personas/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3150 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/personas/builder.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5908 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/personas/dialogue.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6464 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/personas/persona.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.122781 symbolicai-0.6.1/symai/extended/personas/research/
--rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-17 07:30:18.000000 symbolicai-0.6.1/symai/extended/personas/research/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3876 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/personas/research/yann_lecun.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.123080 symbolicai-0.6.1/symai/extended/personas/sales/
--rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-08 00:13:09.000000 symbolicai-0.6.1/symai/extended/personas/sales/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5273 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/personas/sales/erik_james.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.123426 symbolicai-0.6.1/symai/extended/personas/student/
--rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-08 00:13:09.000000 symbolicai-0.6.1/symai/extended/personas/student/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3422 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/personas/student/max_tenner.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2246 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/repo_cloner.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2322 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/seo_query_optimizer.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    11983 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/solver.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.123710 symbolicai-0.6.1/symai/extended/strategies/
--rw-r--r--   0 xpitfire   (501) staff       (20)     1089 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/strategies/exceptremedy.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      476 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/extended/strategies/longtext.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      994 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/summarizer.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     4929 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/taypan_interpreter.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    15425 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/extended/vectordb.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6024 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/formatter.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    15099 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/functional.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5657 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/imports.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      972 2023-12-16 03:23:24.000000 symbolicai-0.6.1/symai/interfaces.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3684 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/memory.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.123960 symbolicai-0.6.1/symai/menu/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-11-24 19:11:53.000000 symbolicai-0.6.1/symai/menu/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    18779 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/menu/screen.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.124389 symbolicai-0.6.1/symai/misc/
--rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-07-06 14:48:25.000000 symbolicai-0.6.1/symai/misc/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     2892 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/misc/console.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1962 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/misc/loader.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1015 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/nesy_client.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      985 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/nesy_server.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.124794 symbolicai-0.6.1/symai/ops/
--rw-r--r--   0 xpitfire   (501) staff       (20)      634 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/ops/__init__.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     3679 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/ops/measures.py
--rw-r--r--   0 xpitfire   (501) staff       (20)   117783 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/ops/primitives.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6314 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/post_processors.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    15567 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/pre_processors.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1586 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/processor.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    74620 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/prompts.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     6237 2023-12-30 18:23:54.000000 symbolicai-0.6.1/symai/shell.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    33703 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/shellsv.py
--rw-r--r--   0 xpitfire   (501) staff       (20)      780 2023-12-09 17:14:47.000000 symbolicai-0.6.1/symai/strategy.py
--rw-r--r--   0 xpitfire   (501) staff       (20)    39406 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/symbol.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1245 2023-11-06 09:12:05.000000 symbolicai-0.6.1/symai/symsh.md
--rw-r--r--   0 xpitfire   (501) staff       (20)     3748 2024-02-01 18:23:56.000000 symbolicai-0.6.1/symai/utils.py
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.125733 symbolicai-0.6.1/symbolicai.egg-info/
--rw-r--r--   0 xpitfire   (501) staff       (20)    97153 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/PKG-INFO
--rw-r--r--   0 xpitfire   (501) staff       (20)     6247 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/SOURCES.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)        1 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/dependency_links.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)      296 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/entry_points.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)     1133 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/requires.txt
--rw-r--r--   0 xpitfire   (501) staff       (20)        6 2024-02-01 18:48:34.000000 symbolicai-0.6.1/symbolicai.egg-info/top_level.txt
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.085640 symbolicai-0.6.1/tests/
-drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-02-01 18:48:34.126165 symbolicai-0.6.1/tests/scripts/
--rw-r--r--   0 xpitfire   (501) staff       (20)      723 2023-07-03 17:57:00.000000 symbolicai-0.6.1/tests/scripts/download_models.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     5423 2023-12-09 17:14:47.000000 symbolicai-0.6.1/tests/scripts/evaluation.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1566 2023-12-09 17:14:47.000000 symbolicai-0.6.1/tests/scripts/single_run.py
--rw-r--r--   0 xpitfire   (501) staff       (20)     1113 2023-12-19 02:22:54.000000 symbolicai-0.6.1/trusted_repos.yml
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.675434 symbolicai-0.6.2/
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.645975 symbolicai-0.6.2/.github/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      883 2024-02-06 21:38:06.000000 symbolicai-0.6.2/.github/FUNDING.yml
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2018 2023-12-16 03:23:24.000000 symbolicai-0.6.2/.gitignore
+-rw-r--r--   0 xpitfire   (501) staff       (20)      153 2024-02-06 21:38:06.000000 symbolicai-0.6.2/.readthedocs.yml
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.646098 symbolicai-0.6.2/.symai/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      623 2024-05-19 07:55:06.000000 symbolicai-0.6.2/.symai/symsh.config.json
+-rw-r--r--   0 xpitfire   (501) staff       (20)      435 2024-02-06 21:38:06.000000 symbolicai-0.6.2/CITATION.cff
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1643 2024-02-06 21:38:06.000000 symbolicai-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1818 2024-02-06 21:38:06.000000 symbolicai-0.6.2/Dockerfile
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1539 2024-02-14 18:56:29.000000 symbolicai-0.6.2/LICENSE
+-rw-r--r--   0 xpitfire   (501) staff       (20)       91 2023-03-14 14:52:27.000000 symbolicai-0.6.2/MANIFEST.in
+-rw-r--r--   0 xpitfire   (501) staff       (20)    99618 2024-05-19 07:56:49.675201 symbolicai-0.6.2/PKG-INFO
+-rw-r--r--   0 xpitfire   (501) staff       (20)    94615 2024-05-19 07:55:06.000000 symbolicai-0.6.2/README.md
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.640163 symbolicai-0.6.2/assets/
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.650518 symbolicai-0.6.2/assets/images/
+-rw-r--r--   0 xpitfire   (501) staff       (20)    28719 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/cat.jpg
+-rw-r--r--   0 xpitfire   (501) staff       (20)    46058 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img1.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    91342 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img10.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    13911 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img2.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    11183 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img3.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    17206 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img4.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    55580 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img5.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    57683 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img6.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    77023 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img7.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)   211609 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img8.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    16559 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/img9.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)  1277783 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/preview.gif
+-rw-r--r--   0 xpitfire   (501) staff       (20)   451461 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/screen1.jpeg
+-rw-r--r--   0 xpitfire   (501) staff       (20)   127115 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/symai_logo.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)   103992 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/symsh.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    42756 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid1.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    78774 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid2.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)   141729 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid3.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)    59810 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid4.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)   318171 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid5.png
+-rw-r--r--   0 xpitfire   (501) staff       (20)  1603606 2024-02-06 21:38:06.000000 symbolicai-0.6.2/assets/images/vid6.png
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.651461 symbolicai-0.6.2/bin/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2149 2024-02-06 21:38:06.000000 symbolicai-0.6.2/bin/install.ps1
+-rwxr-xr-x   0 xpitfire   (501) staff       (20)     3379 2024-02-06 21:38:06.000000 symbolicai-0.6.2/bin/install.sh
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2893 2024-02-06 21:38:06.000000 symbolicai-0.6.2/conf.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      292 2024-05-19 07:55:06.000000 symbolicai-0.6.2/docker-compose.yml
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.651575 symbolicai-0.6.2/docs/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      241 2024-02-06 21:38:06.000000 symbolicai-0.6.2/docs/requirements.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)      477 2023-07-06 10:23:44.000000 symbolicai-0.6.2/environment.yml
+-rw-r--r--   0 xpitfire   (501) staff       (20)      251 2024-02-06 21:38:06.000000 symbolicai-0.6.2/index.rst
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1681 2024-02-06 21:38:06.000000 symbolicai-0.6.2/modules.rst
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.652603 symbolicai-0.6.2/notebooks/
+-rw-r--r--   0 xpitfire   (501) staff       (20)    25155 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/Basics.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5660 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/ChatBot.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)     7315 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/Conversation.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)    25381 2024-02-17 19:15:41.000000 symbolicai-0.6.2/notebooks/Indexer.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)    21040 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/News.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)    14881 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/Queries.ipynb
+-rw-r--r--   0 xpitfire   (501) staff       (20)    18326 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/TTS_Persona.ipynb
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.654963 symbolicai-0.6.2/notebooks/examples/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2235 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/a_star.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1512 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/abstract.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    24045 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/audio.mp3
+-rw-r--r--   0 xpitfire   (501) staff       (20)    66712 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/dbpedia_samples.jsonl
+-rw-r--r--   0 xpitfire   (501) staff       (20)    52057 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/dbpedia_samples_prepared_train.jsonl
+-rw-r--r--   0 xpitfire   (501) staff       (20)    13257 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/dbpedia_samples_prepared_valid.jsonl
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2718 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/demo.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1961 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/demo_strategy.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     4529 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/docs.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      920 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/einsteins_puzzle.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)      495 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/file.json
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5654 2024-02-14 18:57:55.000000 symbolicai-0.6.2/notebooks/examples/news.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)   762191 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/paper.pdf
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2671 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/paper.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2743 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/examples/sql.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.655076 symbolicai-0.6.2/notebooks/outputs/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2024-02-06 21:38:06.000000 symbolicai-0.6.2/notebooks/outputs/tmp.html.pkl
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2663 2024-05-19 07:55:06.000000 symbolicai-0.6.2/pyproject.toml
+-rw-r--r--   0 xpitfire   (501) staff       (20)       38 2024-05-19 07:56:49.675482 symbolicai-0.6.2/setup.cfg
+-rw-r--r--   0 xpitfire   (501) staff       (20)       37 2023-03-14 14:52:28.000000 symbolicai-0.6.2/setup.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.658569 symbolicai-0.6.2/symai/
+-rw-r--r--   0 xpitfire   (501) staff       (20)    91409 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/TERMS_OF_SERVICE.md
+-rw-r--r--   0 xpitfire   (501) staff       (20)    18764 2024-02-06 22:43:35.000000 symbolicai-0.6.2/symai/__init__.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.658910 symbolicai-0.6.2/symai/backend/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-03-14 14:52:28.000000 symbolicai-0.6.2/symai/backend/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5836 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/base.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.659034 symbolicai-0.6.2/symai/backend/driver/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     7854 2024-02-06 22:07:19.000000 symbolicai-0.6.2/symai/backend/driver/webclient.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.659181 symbolicai-0.6.2/symai/backend/engines/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/engines/__init__.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.659275 symbolicai-0.6.2/symai/backend/engines/crawler/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3223 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/crawler/engine_selenium.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.659516 symbolicai-0.6.2/symai/backend/engines/embedding/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3150 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/engines/embedding/engine_openai.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      606 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/backend/engines/embedding/engine_plugin_embeddings.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.659645 symbolicai-0.6.2/symai/backend/engines/execute/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3736 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/engines/execute/engine_python.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.660027 symbolicai-0.6.2/symai/backend/engines/experiments/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5321 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/experiments/engine_bard_wrapper.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      804 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/engines/experiments/engine_gptfinetuner.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5268 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/experiments/engine_llamacpp_completion.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.660172 symbolicai-0.6.2/symai/backend/engines/files/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6279 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/engines/files/engine_io.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.660433 symbolicai-0.6.2/symai/backend/engines/imagecaptioning/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3124 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/imagecaptioning/engine_blip2.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6151 2023-12-18 14:52:06.000000 symbolicai-0.6.2/symai/backend/engines/imagecaptioning/engine_llavacpp_client.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.660579 symbolicai-0.6.2/symai/backend/engines/imagerendering/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3978 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/imagerendering/engine_dall_e.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.660826 symbolicai-0.6.2/symai/backend/engines/index/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     8787 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/index/engine_pinecone.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     7826 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/engines/index/engine_vectordb.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.661299 symbolicai-0.6.2/symai/backend/engines/neurosymbolic/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5605 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_nesy_client.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    19154 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_openai_gptX_chat.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    13909 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_openai_gptX_completion.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.661502 symbolicai-0.6.2/symai/backend/engines/ocr/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2356 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/ocr/engine_apilayer.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.661626 symbolicai-0.6.2/symai/backend/engines/output/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      912 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/output/engine_stdout.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.661774 symbolicai-0.6.2/symai/backend/engines/search/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3513 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/backend/engines/search/engine_serpapi.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.661920 symbolicai-0.6.2/symai/backend/engines/symbolic/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1962 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/symbolic/engine_wolframalpha.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.662049 symbolicai-0.6.2/symai/backend/engines/text_to_speech/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2117 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/text_to_speech/engine_openai.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.662165 symbolicai-0.6.2/symai/backend/engines/text_vision/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3353 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/backend/engines/text_vision/engine_clip.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.662279 symbolicai-0.6.2/symai/backend/engines/userinput/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      744 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/engines/userinput/engine_console.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.662631 symbolicai-0.6.2/symai/backend/mixin/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-07-03 17:57:00.000000 symbolicai-0.6.2/symai/backend/mixin/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     4786 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/backend/mixin/openai.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     4240 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/mixin/tracker.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.663040 symbolicai-0.6.2/symai/backend/services/
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.663304 symbolicai-0.6.2/symai/backend/services/configs/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      223 2023-10-25 18:32:43.000000 symbolicai-0.6.2/symai/backend/services/configs/huggingface_causallm.config.json
+-rw-r--r--   0 xpitfire   (501) staff       (20)      223 2023-10-25 18:32:43.000000 symbolicai-0.6.2/symai/backend/services/configs/huggingface_seq2seqlm.config.json
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6581 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/services/huggingface_causallm_server.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      651 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/services/huggingface_client.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6103 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/backend/services/huggingface_seq2seqlm_server.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)       36 2023-11-02 17:40:09.000000 symbolicai-0.6.2/symai/backend/settings.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    13534 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/chat.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.663791 symbolicai-0.6.2/symai/collect/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      104 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/collect/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3928 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/collect/dynamic.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5385 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/collect/pipeline.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    14511 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/collect/stats.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    33797 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/components.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1641 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/constraints.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)   119003 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/core.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5640 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/core_ext.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.664077 symbolicai-0.6.2/symai/endpoints/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-11-21 00:42:40.000000 symbolicai-0.6.2/symai/endpoints/__init__py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    19289 2024-02-14 18:56:29.000000 symbolicai-0.6.2/symai/endpoints/api.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      165 2023-07-08 22:09:24.000000 symbolicai-0.6.2/symai/exceptions.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.666225 symbolicai-0.6.2/symai/extended/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      516 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6175 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/api_builder.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2155 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/arxiv_pdf_parser.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3739 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/bibtex_parser.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    12473 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/extended/conversation.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      734 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/crawler.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2279 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/extended/document.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2982 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/file_merger.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3317 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/graph.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3588 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/html_style_template.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.668324 symbolicai-0.6.2/symai/extended/interfaces/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-11-27 22:13:29.000000 symbolicai-0.6.2/symai/extended/interfaces/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      429 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/extended/interfaces/blip_2.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      458 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/clip.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      410 2023-07-21 06:07:56.000000 symbolicai-0.6.2/symai/extended/interfaces/console.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      500 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/dall_e.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      411 2023-11-29 12:56:27.000000 symbolicai-0.6.2/symai/extended/interfaces/file.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      403 2023-07-21 06:07:56.000000 symbolicai-0.6.2/symai/extended/interfaces/input.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      413 2023-12-14 18:07:49.000000 symbolicai-0.6.2/symai/extended/interfaces/llava.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      517 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/ocr.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      978 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/interfaces/pinecone.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      372 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/python.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      616 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/interfaces/selenium.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      477 2023-12-12 16:17:08.000000 symbolicai-0.6.2/symai/extended/interfaces/serpapi.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      352 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/interfaces/terminal.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      430 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/tts.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      978 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/interfaces/vectordb.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      501 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/extended/interfaces/whisper.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      443 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/interfaces/wolframalpha.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.668548 symbolicai-0.6.2/symai/extended/metrics/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       25 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/metrics/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3352 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/metrics/similarity.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3813 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/os_command.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.669012 symbolicai-0.6.2/symai/extended/packages/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       43 2023-07-05 23:54:39.000000 symbolicai-0.6.2/symai/extended/packages/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3662 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/packages/symdev.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2893 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/packages/sympkg.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5131 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/packages/symrun.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.669556 symbolicai-0.6.2/symai/extended/personas/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       95 2023-11-09 15:36:35.000000 symbolicai-0.6.2/symai/extended/personas/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3150 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/personas/builder.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5908 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/personas/dialogue.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6590 2024-02-06 22:43:35.000000 symbolicai-0.6.2/symai/extended/personas/persona.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.669859 symbolicai-0.6.2/symai/extended/personas/research/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-17 07:30:18.000000 symbolicai-0.6.2/symai/extended/personas/research/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3876 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/personas/research/yann_lecun.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.670133 symbolicai-0.6.2/symai/extended/personas/sales/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-08 00:13:09.000000 symbolicai-0.6.2/symai/extended/personas/sales/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5273 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/personas/sales/erik_james.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.670454 symbolicai-0.6.2/symai/extended/personas/student/
+-rw-r--r--   0 xpitfire   (501) staff       (20)       33 2023-11-08 00:13:09.000000 symbolicai-0.6.2/symai/extended/personas/student/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3422 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/personas/student/max_tenner.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2246 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/repo_cloner.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2322 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/seo_query_optimizer.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    11983 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/solver.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.670752 symbolicai-0.6.2/symai/extended/strategies/
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1089 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/strategies/exceptremedy.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      476 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/extended/strategies/longtext.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      994 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/summarizer.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     4929 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/extended/taypan_interpreter.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    15597 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/extended/vectordb.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     7519 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/formatter.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    14493 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/functional.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     5657 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/imports.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      972 2023-12-16 03:23:24.000000 symbolicai-0.6.2/symai/interfaces.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3684 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/memory.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.671047 symbolicai-0.6.2/symai/menu/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/menu/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    18779 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/menu/screen.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.671483 symbolicai-0.6.2/symai/misc/
+-rw-r--r--   0 xpitfire   (501) staff       (20)        0 2023-07-06 14:48:25.000000 symbolicai-0.6.2/symai/misc/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     2892 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/misc/console.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1962 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/misc/loader.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1015 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/nesy_client.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      985 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/nesy_server.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.671909 symbolicai-0.6.2/symai/ops/
+-rw-r--r--   0 xpitfire   (501) staff       (20)      634 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/ops/__init__.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3679 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/ops/measures.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)   119022 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/ops/primitives.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6314 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/post_processors.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    15567 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/pre_processors.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1586 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/processor.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    74620 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/prompts.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6237 2024-02-06 21:38:06.000000 symbolicai-0.6.2/symai/shell.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    33703 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/shellsv.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)      780 2023-12-09 17:14:47.000000 symbolicai-0.6.2/symai/strategy.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)    39839 2024-05-19 07:55:06.000000 symbolicai-0.6.2/symai/symbol.py
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1245 2023-11-06 09:12:05.000000 symbolicai-0.6.2/symai/symsh.md
+-rw-r--r--   0 xpitfire   (501) staff       (20)     3748 2024-02-01 18:23:56.000000 symbolicai-0.6.2/symai/utils.py
+drwxr-xr-x   0 xpitfire   (501) staff       (20)        0 2024-05-19 07:56:49.673025 symbolicai-0.6.2/symbolicai.egg-info/
+-rw-r--r--   0 xpitfire   (501) staff       (20)    99618 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/PKG-INFO
+-rw-r--r--   0 xpitfire   (501) staff       (20)     6128 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/SOURCES.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)        1 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/dependency_links.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)      296 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/entry_points.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1170 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/requires.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)        6 2024-05-19 07:56:49.000000 symbolicai-0.6.2/symbolicai.egg-info/top_level.txt
+-rw-r--r--   0 xpitfire   (501) staff       (20)     1113 2024-02-06 21:38:06.000000 symbolicai-0.6.2/trusted_repos.yml
```

### Comparing `symbolicai-0.6.1/.github/FUNDING.yml` & `symbolicai-0.6.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/.gitignore` & `symbolicai-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/CONTRIBUTING.md` & `symbolicai-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/Dockerfile` & `symbolicai-0.6.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/LICENSE` & `symbolicai-0.6.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, ExtensityAI, a AlphaCore AI e.U. brand.
+Copyright (c) 2024, ExtensityAI, a AlphaCore AI e.U. brand.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `symbolicai-0.6.1/PKG-INFO` & `symbolicai-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,16 @@
-Metadata-Version: 2.1
-Name: symbolicai
-Version: 0.6.1
-Summary: A Neuro-Symbolic Framework for Python
-Author-email: Marius-Constantin Dinu <office@alphacoreai.eu>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, ExtensityAI, a AlphaCore AI e.U. brand.
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of the copyright holder nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://alphacoreai.eu/
-Project-URL: GitHub, https://github.com/Xpitfire/symai
-Keywords: symbolic programming,machine learning
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: blip2
-Provides-Extra: wolframalpha
-Provides-Extra: whisper
-Provides-Extra: selenium
-Provides-Extra: serpapi
-Provides-Extra: pinecone
-Provides-Extra: bard
-Provides-Extra: services
-Provides-Extra: solver
-Provides-Extra: all
-License-File: LICENSE
-
 # **SymbolicAI**
 <img src="https://raw.githubusercontent.com/ExtensityAI/symbolicai/main/assets/images/symai_logo.png" width="200px">
 
 ## **A Neuro-Symbolic Perspective on Large Language Models (LLMs)**
 
 *Building applications with LLMs at the core using our `Symbolic API` facilitates the integration of classical and differentiable programming in Python.*
 
+Read [**full paper here**](https://arxiv.org/abs/2402.00854).
+
 Read further [**documentation here**](https://symbolicai.readthedocs.io/en/latest/README.html).
 
 [![PyPI version](https://badge.fury.io/py/symbolicai.svg)](https://badge.fury.io/py/symbolicai) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/dinumariusc.svg?style=social&label=Follow%20%40DinuMariusC)](https://twitter.com/DinuMariusC) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/symbolicapi.svg?style=social&label=Follow%20%40ExtensityAI)](https://twitter.com/ExtensityAI) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ExtensityAI/symbolicai/issues)
 [![Discord](https://img.shields.io/discord/768087161878085643?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/QYMNnh9ra8) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FXpitfire%2Fsymbolicai&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) [![GitHub forks](https://img.shields.io/github/forks/ExtensityAI/symbolicai.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai) [![GitHub stars](https://img.shields.io/github/stars/ExtensityAI/symbolicai.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai/stargazers/)
 
 
 
@@ -1359,39 +1306,31 @@
 array([[9.72840726e-01, 6.34790864e-03, 2.59368378e-03, 3.41371237e-03,
         3.71197984e-03, 8.53193272e-03, 1.03346225e-04, 2.08464009e-03,
         1.77942711e-04, 1.94185617e-04]], dtype=float32)
 ```
 
 ### Local Neuro-Symbolic Engine
 
-You can use a locally hosted instance for the Neuro-Symbolic Engine. Out of the box, we provide a Hugging Face client-server backend and host the model `openlm-research/open_llama_13b` to perform the inference. As the name suggests, this is a six billion parameter model and requires a GPU with ~16GB RAM to run properly. The following example shows how to host and configure the usage of the local Neuro-Symbolic Engine.
-
-First, we start the backend server:
+You can use a locally hosted instance for the Neuro-Symbolic Engine. We build on top of [llama.cpp](https://github.com/ggerganov/llama.cpp/tree/master) through [llama-cpp-python](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file). Please follow the `llama-cpp-python` installation instructions. We make the assumption the user has experience running `llama.cpp` prior to using our API for local hosting.
 
+For instance, let's suppose you want to set as a Neuro-Symbolic Engine the latest Llama 3 model. Download the model and start the server:
 ```bash
-# optional: set cache folder for transformers (Linux/MacOS)
-export TRANSFORMERS_CACHE="<path-to-cache-folder>"
-# start server backend (default model is openlm-research/open_llama_13b)
-symsvr
-# initialize server with client call
-symclient
+python -m llama_cpp.server --model [your llama.cpp folder]/models/llama-pro-8b-instruct.Q4_K_M.gguf --n_gpu_layers -1 --chat_format llama-3 --port 8000 --host localhost
 ```
 
-Then, use the following code once to set up the local engine:
+Then, in your `symai.config.json` file, set the `NEUROSYMBOLIC_ENGINE_API_KEY` to `http://localhost:8000` (following the `--port` and `--host` you set in the previous step) and `NEUROSYMBOLIC_ENGINE_MODEL` to `llama.cpp`.
 
-```python
-from symai.backend.engines.neurosymbolic.engine_nesy_client import NeSyClientEngine
-from symai.functional import EngineRepository
-# setup local engine
-engine = NeSyClientEngine()
-EngineRepository.register('neurosymbolic', engine)
+```json
+{
+  "NEUROSYMBOLIC_ENGINE_API_KEY": "http://localhost:8000",
+  "NEUROSYMBOLIC_ENGINE_MODEL": "llama.cpp"
+}
 ```
+Now you are set to use the local engine.
 
-
-Now you can use the local engine to perform symbolic computation:
 ```python
 # do some symbolic computation with the local engine
 sym = Symbol('cats are cute')
 res = sym.compose()
 ...
 ```
 
@@ -1565,15 +1504,15 @@
 * We view operators/methods as being able to move along a spectrum between prompting and fine-tuning, based on task-specific requirements and data availability. We believe this approach is more general compared to prompting frameworks.
 * We propose a general method for handling large context sizes and transforming a data stream problem into a search problem, related to **reasoning as a search problem** in [Search and Reasoning in Problem Solving](https://www.sciencedirect.com/science/article/abs/pii/S0004370283800034).
 
 We hope that our work can be seen as complementary and offer a future outlook on how we would like to use machine learning models as an integral part of programming languages and their entire computational stack.
 
 ### Acknowledgements
 
-We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback; and to [Dynatrace Research](https://engineering.dynatrace.com/research/) for supporting this project. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community). Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
+We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community) for supporting this project. Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
 
 Finally, we would like to thank the open-source community for making their APIs and tools publicly available, including (but not limited to) [PyTorch](https://pytorch.org/), [Hugging Face](https://huggingface.co/), [OpenAI](https://openai.com/), [GitHub](https://github.com/), [Microsoft Research](https://www.microsoft.com/en-us/research/), and many others.
 
 Special thanks are owed to [Kajetan Schweighofer](https://www.linkedin.com/in/kajetan-schweighofer-a61113202/?originalSubdomain=at), [Markus Hofmarcher](https://www.linkedin.com/in/markus-hofmarcher-2722141b8/?originalSubdomain=at), [Thomas Natschläger](https://www.linkedin.com/in/thomas-natschlaeger/?originalSubdomain=at), and [Sepp Hochreiter](https://scholar.google.at/citations?user=tvUH3WMAAAAJ&hl=en).
 
 ### Contribution
```

### Comparing `symbolicai-0.6.1/README.md` & `symbolicai-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,131 @@
+Metadata-Version: 2.1
+Name: symbolicai
+Version: 0.6.2
+Summary: A Neuro-Symbolic Framework for Python
+Author-email: Marius-Constantin Dinu <office@alphacoreai.eu>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2024, ExtensityAI, a AlphaCore AI e.U. brand.
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://alphacoreai.eu/
+Project-URL: GitHub, https://github.com/Xpitfire/symai
+Keywords: symbolic programming,machine learning
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: setuptools>=67.7.2
+Requires-Dist: toml>=0.10.2
+Requires-Dist: natsort>=8.3.1
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: python-box>=7.0.1
+Requires-Dist: rpyc>=5.3.1
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchaudio>=2.0.1
+Requires-Dist: torchvision>=0.15.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: transformers>=4.30.2
+Requires-Dist: sympy>=1.12
+Requires-Dist: openai>=1.1.0
+Requires-Dist: PyPDF2>=3.0.1
+Requires-Dist: ipython>=8.14.0
+Requires-Dist: accelerate>=0.20.3
+Requires-Dist: sentencepiece>=0.1.99
+Requires-Dist: tiktoken>=0.7.0
+Requires-Dist: tika>=2.6.0
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: GitPython>=3.1.32
+Requires-Dist: pathos>=0.3.1
+Requires-Dist: prompt-toolkit>=3.0.39
+Requires-Dist: pydub
+Requires-Dist: opencv-python
+Requires-Dist: pymongo==3.12.3
+Requires-Dist: pymongo[srv]
+Requires-Dist: requests_toolbelt
+Requires-Dist: pyvis
+Requires-Dist: beartype>=0.17.2
+Provides-Extra: blip2
+Requires-Dist: bitsandbytes>=0.39.1; extra == "blip2"
+Requires-Dist: decord; extra == "blip2"
+Requires-Dist: salesforce-lavis; extra == "blip2"
+Provides-Extra: wolframalpha
+Requires-Dist: wolframalpha>=5.0.0; extra == "wolframalpha"
+Provides-Extra: whisper
+Requires-Dist: openai-whisper>=20231117; extra == "whisper"
+Provides-Extra: selenium
+Requires-Dist: selenium>=4.10.0; extra == "selenium"
+Requires-Dist: webdriver-manager>=4.0.1; extra == "selenium"
+Requires-Dist: chromedriver-autoinstaller>=0.4.0; extra == "selenium"
+Provides-Extra: serpapi
+Requires-Dist: google-search-results>=2.4.2; extra == "serpapi"
+Provides-Extra: pinecone
+Requires-Dist: pinecone-client>=2.2.2; extra == "pinecone"
+Provides-Extra: bard
+Requires-Dist: bardapi>=0.1.24; extra == "bard"
+Provides-Extra: services
+Requires-Dist: fastapi>=0.104.1; extra == "services"
+Requires-Dist: redis>=5.0.1; extra == "services"
+Requires-Dist: uvicorn>=0.24.0.post1; extra == "services"
+Provides-Extra: solver
+Requires-Dist: z3-solver; extra == "solver"
+Provides-Extra: all
+Requires-Dist: wolframalpha>=5.0.0; extra == "all"
+Requires-Dist: openai-whisper>=20231117; extra == "all"
+Requires-Dist: selenium>=4.10.0; extra == "all"
+Requires-Dist: webdriver-manager>=4.0.1; extra == "all"
+Requires-Dist: chromedriver-autoinstaller>=0.4.0; extra == "all"
+Requires-Dist: google-search-results>=2.4.2; extra == "all"
+Requires-Dist: pinecone-client>=2.2.2; extra == "all"
+Requires-Dist: fastapi>=0.104.1; extra == "all"
+Requires-Dist: redis>=5.0.1; extra == "all"
+Requires-Dist: uvicorn>=0.24.0.post1; extra == "all"
+Requires-Dist: z3-solver; extra == "all"
+
 # **SymbolicAI**
 <img src="https://raw.githubusercontent.com/ExtensityAI/symbolicai/main/assets/images/symai_logo.png" width="200px">
 
 ## **A Neuro-Symbolic Perspective on Large Language Models (LLMs)**
 
 *Building applications with LLMs at the core using our `Symbolic API` facilitates the integration of classical and differentiable programming in Python.*
 
+Read [**full paper here**](https://arxiv.org/abs/2402.00854).
+
 Read further [**documentation here**](https://symbolicai.readthedocs.io/en/latest/README.html).
 
 [![PyPI version](https://badge.fury.io/py/symbolicai.svg)](https://badge.fury.io/py/symbolicai) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/dinumariusc.svg?style=social&label=Follow%20%40DinuMariusC)](https://twitter.com/DinuMariusC) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/symbolicapi.svg?style=social&label=Follow%20%40ExtensityAI)](https://twitter.com/ExtensityAI) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ExtensityAI/symbolicai/issues)
 [![Discord](https://img.shields.io/discord/768087161878085643?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/QYMNnh9ra8) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FXpitfire%2Fsymbolicai&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) [![GitHub forks](https://img.shields.io/github/forks/ExtensityAI/symbolicai.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai) [![GitHub stars](https://img.shields.io/github/stars/ExtensityAI/symbolicai.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai/stargazers/)
 
 
 
@@ -1304,39 +1421,31 @@
 array([[9.72840726e-01, 6.34790864e-03, 2.59368378e-03, 3.41371237e-03,
         3.71197984e-03, 8.53193272e-03, 1.03346225e-04, 2.08464009e-03,
         1.77942711e-04, 1.94185617e-04]], dtype=float32)
 ```
 
 ### Local Neuro-Symbolic Engine
 
-You can use a locally hosted instance for the Neuro-Symbolic Engine. Out of the box, we provide a Hugging Face client-server backend and host the model `openlm-research/open_llama_13b` to perform the inference. As the name suggests, this is a six billion parameter model and requires a GPU with ~16GB RAM to run properly. The following example shows how to host and configure the usage of the local Neuro-Symbolic Engine.
-
-First, we start the backend server:
+You can use a locally hosted instance for the Neuro-Symbolic Engine. We build on top of [llama.cpp](https://github.com/ggerganov/llama.cpp/tree/master) through [llama-cpp-python](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file). Please follow the `llama-cpp-python` installation instructions. We make the assumption the user has experience running `llama.cpp` prior to using our API for local hosting.
 
+For instance, let's suppose you want to set as a Neuro-Symbolic Engine the latest Llama 3 model. Download the model and start the server:
 ```bash
-# optional: set cache folder for transformers (Linux/MacOS)
-export TRANSFORMERS_CACHE="<path-to-cache-folder>"
-# start server backend (default model is openlm-research/open_llama_13b)
-symsvr
-# initialize server with client call
-symclient
+python -m llama_cpp.server --model [your llama.cpp folder]/models/llama-pro-8b-instruct.Q4_K_M.gguf --n_gpu_layers -1 --chat_format llama-3 --port 8000 --host localhost
 ```
 
-Then, use the following code once to set up the local engine:
+Then, in your `symai.config.json` file, set the `NEUROSYMBOLIC_ENGINE_API_KEY` to `http://localhost:8000` (following the `--port` and `--host` you set in the previous step) and `NEUROSYMBOLIC_ENGINE_MODEL` to `llama.cpp`.
 
-```python
-from symai.backend.engines.neurosymbolic.engine_nesy_client import NeSyClientEngine
-from symai.functional import EngineRepository
-# setup local engine
-engine = NeSyClientEngine()
-EngineRepository.register('neurosymbolic', engine)
+```json
+{
+  "NEUROSYMBOLIC_ENGINE_API_KEY": "http://localhost:8000",
+  "NEUROSYMBOLIC_ENGINE_MODEL": "llama.cpp"
+}
 ```
+Now you are set to use the local engine.
 
-
-Now you can use the local engine to perform symbolic computation:
 ```python
 # do some symbolic computation with the local engine
 sym = Symbol('cats are cute')
 res = sym.compose()
 ...
 ```
 
@@ -1510,15 +1619,15 @@
 * We view operators/methods as being able to move along a spectrum between prompting and fine-tuning, based on task-specific requirements and data availability. We believe this approach is more general compared to prompting frameworks.
 * We propose a general method for handling large context sizes and transforming a data stream problem into a search problem, related to **reasoning as a search problem** in [Search and Reasoning in Problem Solving](https://www.sciencedirect.com/science/article/abs/pii/S0004370283800034).
 
 We hope that our work can be seen as complementary and offer a future outlook on how we would like to use machine learning models as an integral part of programming languages and their entire computational stack.
 
 ### Acknowledgements
 
-We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback; and to [Dynatrace Research](https://engineering.dynatrace.com/research/) for supporting this project. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community). Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
+We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community) for supporting this project. Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
 
 Finally, we would like to thank the open-source community for making their APIs and tools publicly available, including (but not limited to) [PyTorch](https://pytorch.org/), [Hugging Face](https://huggingface.co/), [OpenAI](https://openai.com/), [GitHub](https://github.com/), [Microsoft Research](https://www.microsoft.com/en-us/research/), and many others.
 
 Special thanks are owed to [Kajetan Schweighofer](https://www.linkedin.com/in/kajetan-schweighofer-a61113202/?originalSubdomain=at), [Markus Hofmarcher](https://www.linkedin.com/in/markus-hofmarcher-2722141b8/?originalSubdomain=at), [Thomas Natschläger](https://www.linkedin.com/in/thomas-natschlaeger/?originalSubdomain=at), and [Sepp Hochreiter](https://scholar.google.at/citations?user=tvUH3WMAAAAJ&hl=en).
 
 ### Contribution
```

### Comparing `symbolicai-0.6.1/assets/images/cat.jpg` & `symbolicai-0.6.2/assets/images/cat.jpg`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img1.png` & `symbolicai-0.6.2/assets/images/img1.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img10.png` & `symbolicai-0.6.2/assets/images/img10.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img2.png` & `symbolicai-0.6.2/assets/images/img2.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img3.png` & `symbolicai-0.6.2/assets/images/img3.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img4.png` & `symbolicai-0.6.2/assets/images/img4.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img5.png` & `symbolicai-0.6.2/assets/images/img5.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img6.png` & `symbolicai-0.6.2/assets/images/img6.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img7.png` & `symbolicai-0.6.2/assets/images/img7.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img8.png` & `symbolicai-0.6.2/assets/images/img8.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/img9.png` & `symbolicai-0.6.2/assets/images/img9.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/preview.gif` & `symbolicai-0.6.2/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/screen1.jpeg` & `symbolicai-0.6.2/assets/images/screen1.jpeg`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/symai_logo.png` & `symbolicai-0.6.2/assets/images/symai_logo.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/symsh.png` & `symbolicai-0.6.2/assets/images/symsh.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid1.png` & `symbolicai-0.6.2/assets/images/vid1.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid2.png` & `symbolicai-0.6.2/assets/images/vid2.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid3.png` & `symbolicai-0.6.2/assets/images/vid3.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid4.png` & `symbolicai-0.6.2/assets/images/vid4.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid5.png` & `symbolicai-0.6.2/assets/images/vid5.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/assets/images/vid6.png` & `symbolicai-0.6.2/assets/images/vid6.png`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/bin/install.ps1` & `symbolicai-0.6.2/bin/install.ps1`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/bin/install.sh` & `symbolicai-0.6.2/bin/install.sh`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/conf.py` & `symbolicai-0.6.2/conf.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/modules.rst` & `symbolicai-0.6.2/modules.rst`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/Basics.ipynb` & `symbolicai-0.6.2/notebooks/Basics.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/ChatBot.ipynb` & `symbolicai-0.6.2/notebooks/ChatBot.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/Conversation.ipynb` & `symbolicai-0.6.2/notebooks/Conversation.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/Indexer.ipynb` & `symbolicai-0.6.2/notebooks/Indexer.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857638888888889%*

 * *Differences: {"'cells'": "{16: {'execution_count': 4}, insert: [(14, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', 2), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            '["sym = Symbol(\'test\')"])])), (15, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', 3), ('metadata', OrderedDict()), ('outputs', "*

 * *            "[OrderedDict([('data', OrderedDict([('text/plain', ['(1, 768)'])])), "*

 * *            "('execution_count', 3), ('metadata', OrderedDict()),  […]*

```diff
@@ -366,19 +366,105 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
+                "sym = Symbol('test')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "(1, 768)"
+                        ]
+                    },
+                    "execution_count": 3,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "sym.embedding.shape"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "indexer = Indexer()"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "index = indexer()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<ul><li><a href=\"src/evals/snippets/einstein_puzzle_logic_solution.txt\"><b>src/evals/snippets/einstein_puzzle_logic_solution.txt</a></b><br># Determine who owns the fish\n",
+                            "    query = Const(\"query\", Nationality)\n",
+                            "    fact1 (lambda i: And(n(i) == query, p(i) == Fish))</li>\n",
+                            "<li><a href=\"src/evals/snippets/einstein_puzzle_logic_solution.txt\"><b>src/evals/snippets/einstein_puzzle_logic_solution.txt</a></b><br># Assert a new fact. Defines a synonym for add to make the code more readable\n",
+                            "    def fact0(f):\n",
+                            "        S.add(f)</li>\n",
+                            "<li><a href=\"src/evals/snippets/latex_templating_solution_1.txt\"><b>src/evals/snippets/latex_templating_solution_1.txt</a></b><br># Prepare table content\n",
+                            "    benchmark_rows = {bench_name: \"\" for bench_name in BENCHMARK_NAME_MAPPING.values()}\n",
+                            "    for bench_name in BENCHMARK_NAME_MAPPING.values():\n",
+                            "        if bench_name not in str(list(data.values())):\n",
+                            "            print(f\"Skipping benchmark because not all results are computed. Did not find `{bench_name}` in `{data.keys()}`\")\n",
+                            "            return\n",
+                            "        # Initialize list to keep the scores for this benchmark to find the best model\n",
+                            "        scores = [(model, values[bench_name]['performance']) for model, values in data.items()]\n",
+                            "        best_score = max(scores, key=lambda x: x[1])[1]</li>\n",
+                            "<li><a href=\"src/evals/snippets/einstein_puzzle_logic_solution.txt\"><b>src/evals/snippets/einstein_puzzle_logic_solution.txt</a></b><br># Assert a fact about two variables\n",
+                            "    def fact2(f):\n",
+                            "        i = variable()\n",
+                            "        j = variable()\n",
+                            "        S.add(i != j)\n",
+                            "        S.add(f(i, j))</li>\n",
+                            "<li><a href=\"src/evals/snippets/einstein_puzzle_logic_solution.txt\"><b>src/evals/snippets/einstein_puzzle_logic_solution.txt</a></b><br># Assert a fact about a new variable\n",
+                            "    def fact1(f):\n",
+                            "        i = variable()\n",
+                            "        S.add(f(i))</li>\n",
+                            "</ul>"
+                        ],
+                        "text/plain": [
+                            "<class symai.backend.engines.index.engine_vectordb.VectorDBResult at 0x7f8169133850>(value=['# ----[FILE_START]<PART ... c_solution.txt\\n\\n'])"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "index('test', raw_result=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
```

### Comparing `symbolicai-0.6.1/notebooks/News.ipynb` & `symbolicai-0.6.2/notebooks/News.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/Queries.ipynb` & `symbolicai-0.6.2/notebooks/Queries.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/TTS_Persona.ipynb` & `symbolicai-0.6.2/notebooks/TTS_Persona.ipynb`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/a_star.txt` & `symbolicai-0.6.2/notebooks/examples/a_star.txt`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/abstract.py` & `symbolicai-0.6.2/notebooks/examples/abstract.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/audio.mp3` & `symbolicai-0.6.2/notebooks/examples/audio.mp3`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/dbpedia_samples.jsonl` & `symbolicai-0.6.2/notebooks/examples/dbpedia_samples.jsonl`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/dbpedia_samples_prepared_train.jsonl` & `symbolicai-0.6.2/notebooks/examples/dbpedia_samples_prepared_train.jsonl`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/dbpedia_samples_prepared_valid.jsonl` & `symbolicai-0.6.2/notebooks/examples/dbpedia_samples_prepared_valid.jsonl`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/demo.py` & `symbolicai-0.6.2/notebooks/examples/demo.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/demo_strategy.py` & `symbolicai-0.6.2/notebooks/examples/demo_strategy.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/docs.py` & `symbolicai-0.6.2/notebooks/examples/docs.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/einsteins_puzzle.txt` & `symbolicai-0.6.2/notebooks/examples/einsteins_puzzle.txt`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/news.py` & `symbolicai-0.6.2/notebooks/examples/news.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,27 @@
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>News</title>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
   </head>
   <body>
-  <h1>News Headlines</h1>
   {{placeholder}}
 
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
   </body>
 </html>"""
 
 HTML_STREAM_STYLE_DESCRIPTION = f"""Style the elements according to the bootstrap library.
-Replace the list items with a summary title and the item text.
-Add highlighting animations.
-Use best practices for colors, text font, etc.
-Assume the elements are inside the `placeholder` tag of the following HTML template:
+Create sections, listings, paragraphs, and headings based on the news data.
+Add emphasis and animations to elements if appropriate. Organize the content in tiles or cards.
+Use best practices for colors, text font, etc. and try to make the web app look professional and modern.
+Output the html output within a ```html\n ... \n``` code block.
+Do not remove any content from the news data.
+Assume the elements are inside the body `placeholder` tag of the following HTML template:
 {HTML_TEMPLATE}"""
 
 class News(Expression):
     """The `News` class sub-classes `Expression` and provides a way to fetch and render news from a given url. It uses a `Stream` object to process the news data, with a sequence of `Clean`, `Translate`, `Outline`, and `Compose` expressions.
     It also defines a `Style` for the header, and a `Symbol` for the HTML templates.
     """
     def __init__(self, url: str, pattern: str, filters: List[Expression] = [], render: bool = False, **kwargs):
@@ -49,36 +50,39 @@
         self.render_ = render
         filters = filters if isinstance(filters, List) or isinstance(filters, tuple) else [filters]
         self.data_stream = Stream(Sequence(
             Clean(),
             Translate(),
             Outline(),
             *filters,
-            Compose(f'Compose news paragraphs. Combine only facts that belong topic-wise together:\n'),
+            Compose(f'Compose a comprehensive news article. Group all facts that belong together topics-wise:\n'),
         ))
-
         self.html_stream = Stream(
             Sequence(
                 Template(template=HTML_TEMPLATE),
                 Style(description=HTML_STREAM_STYLE_DESCRIPTION,
                       libraries=['https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css',
                                  'https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js',
                                  'https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js']),
             )
         )
+        self.post_processors = ProcessorPipeline([StripPostProcessor(), CodeExtractPostProcessor()])
+        self.writer = FileWriter('tmp/news.html')
 
     def render(self, sym: Symbol, **kwargs) -> Symbol:
         """The `render` method takes a `Symbol` as an argument and returns a `Symbol` containing the rendered news.
         It first sets the `html_template_seq` property of the `html_stream` to the result of applying the `header_style` to the `html_template`.
         It then iterates through the `data_stream` and collects the strings resulting from each expression.
         These strings are combined into a single `Symbol` object which is then clustered.
         Finally, the `render` method applies the `html_template` to the clustered `Symbol` and returns the result.
         """
         res = '\n'.join([str(s) for s in self.html_stream(sym, **kwargs)])
+        res = self.post_processors(str(res), None)
         res = Symbol(str(HTML_TEMPLATE).replace('{{placeholder}}', res))
+        self.writer(res)
         return res
 
     def forward(self, **kwargs) -> Symbol:
         """The `forward` method is used to fetch and process the news data.
         It first calls the `fetch` method with the `url` and `pattern` arguments.
         It then iterates through the `data_stream` and collects the `Symbol` object resulting from each expression.
         These `Symbol` objects are then combined into a single `Symbol` object which is then mapped.
```

### Comparing `symbolicai-0.6.1/notebooks/examples/paper.pdf` & `symbolicai-0.6.2/notebooks/examples/paper.pdf`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/paper.py` & `symbolicai-0.6.2/notebooks/examples/paper.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/notebooks/examples/sql.py` & `symbolicai-0.6.2/notebooks/examples/sql.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/pyproject.toml` & `symbolicai-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "setuptools>=67.7.2", "toml>=0.10.2", "natsort>=8.3.1", "numpy>=1.24.3", "tqdm>=4.65.0", "python-box>=7.0.1", "rpyc>=5.3.1", "pandas>=2.0.2",
     "scikit-learn>=1.2.2", "torch>=2.0.0", "torchaudio>=2.0.1", "torchvision>=0.15.0", "PyYAML>=6.0", "transformers>=4.30.2", "sympy>=1.12",
     "openai>=1.1.0", "PyPDF2>=3.0.1", "ipython>=8.14.0", "accelerate>=0.20.3", "sentencepiece>=0.1.99",
-    "tiktoken>=0.3.3", "tika>=2.6.0", "beautifulsoup4>=4.12.2", "colorama>=0.4.6", "GitPython>=3.1.32", "pathos>=0.3.1", "prompt-toolkit>=3.0.39",
-    "pydub", "opencv-python", "pymongo==3.12.3", "pymongo[srv]", "requests_toolbelt", "pyvis"
+    "tiktoken>=0.7.0", "tika>=2.6.0", "beautifulsoup4>=4.12.2", "colorama>=0.4.6", "GitPython>=3.1.32", "pathos>=0.3.1", "prompt-toolkit>=3.0.39",
+    "pydub", "opencv-python", "pymongo==3.12.3", "pymongo[srv]", "requests_toolbelt", "pyvis", "beartype>=0.17.2"
 ]
 
 [project.optional-dependencies]
 blip2 = ["bitsandbytes>=0.39.1", "decord", "salesforce-lavis"]
 wolframalpha = ["wolframalpha>=5.0.0"]
-whisper = ["openai-whisper"]
+whisper = ["openai-whisper>=20231117"]
 selenium = ["selenium>=4.10.0", "webdriver-manager>=4.0.1", "chromedriver-autoinstaller>=0.4.0"]
 serpapi = ["google-search-results>=2.4.2"]
 pinecone = ["pinecone-client>=2.2.2"]
 bard = ["bardapi>=0.1.24"]
 services = ["fastapi>=0.104.1", "redis>=5.0.1", "uvicorn>=0.24.0.post1"]
 solver = ["z3-solver"]
-all = ["wolframalpha>=5.0.0", "openai-whisper", "selenium>=4.10.0", "webdriver-manager>=4.0.1", "chromedriver-autoinstaller>=0.4.0", "google-search-results>=2.4.2", "pinecone-client>=2.2.2", "fastapi>=0.104.1", "redis>=5.0.1", "uvicorn>=0.24.0.post1", "z3-solver"]
+all = ["wolframalpha>=5.0.0", "openai-whisper>=20231117", "selenium>=4.10.0", "webdriver-manager>=4.0.1", "chromedriver-autoinstaller>=0.4.0", "google-search-results>=2.4.2", "pinecone-client>=2.2.2", "fastapi>=0.104.1", "redis>=5.0.1", "uvicorn>=0.24.0.post1", "z3-solver"]
 
 [tool.setuptools.dynamic]
 version = {attr = "symai.SYMAI_VERSION"}
 
 [tool.setuptools.package-data]
 "*" = ["*.json", "*.md"]
```

### Comparing `symbolicai-0.6.1/symai/TERMS_OF_SERVICE.md` & `symbolicai-0.6.2/symai/TERMS_OF_SERVICE.md`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/__init__.py` & `symbolicai-0.6.2/symai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 # do not remove - hides the libraries' debug messages
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("tika").setLevel(logging.ERROR)
 logging.getLogger("httpx").setLevel(logging.ERROR)
 logging.getLogger("httpcore").setLevel(logging.ERROR)
 
+# set the environment variable for the transformers library
+os.environ['TOKENIZERS_PARALLELISM'] = "false"
 
-SYMAI_VERSION = "0.6.1"
+
+SYMAI_VERSION = "0.6.2"
 __version__   = SYMAI_VERSION
 __root_dir__  = Path.home() / '.symai'
 
 
 def _start_symai():
     global _symai_config_
     global _symsh_config_
```

### Comparing `symbolicai-0.6.1/symai/backend/base.py` & `symbolicai-0.6.2/symai/backend/base.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/driver/webclient.py` & `symbolicai-0.6.2/symai/backend/driver/webclient.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/crawler/engine_selenium.py` & `symbolicai-0.6.2/symai/backend/engines/crawler/engine_selenium.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/embedding/engine_openai.py` & `symbolicai-0.6.2/symai/backend/engines/embedding/engine_openai.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import numpy as np
 import openai
 
 from typing import Optional
 
 from ...base import Engine
 from ...mixin.openai import OpenAIMixin
 from ...settings import SYMAI_CONFIG
@@ -16,20 +17,20 @@
 
 
 class EmbeddingEngine(Engine, OpenAIMixin):
     def __init__(self, api_key: Optional[str] = None, model: Optional[str] = None):
         super().__init__()
         logger = logging.getLogger('openai')
         logger.setLevel(logging.WARNING)
-        self.config             = SYMAI_CONFIG
-        openai.api_key          = self.config['EMBEDDING_ENGINE_API_KEY'] if api_key is None else api_key
-        self.model              = self.config['EMBEDDING_ENGINE_MODEL'] if model is None else model
-        self.pricing            = self.api_pricing()
-        self.max_tokens         = self.api_max_tokens()
-        self.embedding_dim      = 1536
+        self.config        = SYMAI_CONFIG
+        openai.api_key     = self.config['EMBEDDING_ENGINE_API_KEY'] if api_key is None else api_key
+        self.model         = self.config['EMBEDDING_ENGINE_MODEL'] if model is None else model
+        self.pricing       = self.api_pricing()
+        self.max_tokens    = self.api_max_tokens()
+        self.embedding_dim = self.api_embedding_dims()
 
     def id(self) -> str:
         if  self.config['EMBEDDING_ENGINE_API_KEY']:
             return 'embedding'
         return super().id() # default to unregistered
 
     def command(self, *args, **kwargs):
@@ -37,30 +38,46 @@
         if 'EMBEDDING_ENGINE_API_KEY' in kwargs:
             openai.api_key = kwargs['EMBEDDING_ENGINE_API_KEY']
         if 'EMBEDDING_ENGINE_MODEL' in kwargs:
             self.model = kwargs['EMBEDDING_ENGINE_MODEL']
 
     def forward(self, argument):
         prepared_input = argument.prop.prepared_input
-        args            = argument.args
-        kwargs          = argument.kwargs
+        args           = argument.args
+        kwargs         = argument.kwargs
 
-        input_          = prepared_input if isinstance(prepared_input, list) else [prepared_input]
-        except_remedy   = kwargs['except_remedy'] if 'except_remedy' in kwargs else None
+        input_        = prepared_input if isinstance(prepared_input, list) else [prepared_input]
+        except_remedy = kwargs.get('except_remedy')
+        new_dim       = kwargs.get('new_dim')
 
         try:
             res = openai.embeddings.create(model=self.model,
                                            input=input_)
         except Exception as e:
             if except_remedy is None:
                 raise e
             callback = openai.embeddings.create
             res = except_remedy(e, input_, callback, self, *args, **kwargs)
 
-        rsp = [r.embedding for r in res.data]
+        if new_dim:
+            mn = min(new_dim, self.embedding_dim) #@NOTE: new_dim should be less than or equal to the original embedding dim
+            rsp = [self._normalize_l2(r.embedding[:mn]) for r in res.data]
+        else:
+            rsp = [r.embedding for r in res.data]
 
         metadata = {}
         return [rsp], metadata
 
     def prepare(self, argument):
         assert not argument.prop.processed_input, "EmbeddingEngine does not support processed_input."
         argument.prop.prepared_input = argument.prop.entries
+
+    def _normalize_l2(self, x):
+        x = np.array(x)
+        if x.ndim == 1:
+            norm = np.linalg.norm(x)
+            if norm == 0:
+                return x.tolist()
+            return (x / norm).tolist()
+        else:
+            norm = np.linalg.norm(x, 2, axis=1, keepdims=True)
+            return np.where(norm == 0, x, x / norm).tolist()
```

### Comparing `symbolicai-0.6.1/symai/backend/engines/embedding/engine_plugin_embeddings.py` & `symbolicai-0.6.2/symai/backend/engines/embedding/engine_plugin_embeddings.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/execute/engine_python.py` & `symbolicai-0.6.2/symai/backend/engines/execute/engine_python.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/experiments/engine_bard_wrapper.py` & `symbolicai-0.6.2/symai/backend/engines/experiments/engine_bard_wrapper.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/experiments/engine_gptfinetuner.py` & `symbolicai-0.6.2/symai/backend/engines/experiments/engine_gptfinetuner.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/experiments/engine_llamacpp_completion.py` & `symbolicai-0.6.2/symai/backend/engines/experiments/engine_llamacpp_completion.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/files/engine_io.py` & `symbolicai-0.6.2/symai/core_ext.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,195 @@
+import functools
+import traceback
 import os
+import os
+import pickle
+import random
+import time
 import logging
-import PyPDF2
-import tika
-
-from tika import unpack
-
-from ...base import Engine
+import dill
+import multiprocessing as mp
 
-
-# initialize tika server
-tika.initVM()
-# suppress tika logging
-logging.getLogger('tika').setLevel(logging.CRITICAL)
-
-
-class FileEngine(Engine):
-    def __init__(self):
-        super().__init__()
-
-    def id(self) -> str:
-        return 'files'
-
-    def _read_slice_file(self, file_path: str) -> str:
-        # check if file is empty
-        if file_path is None or file_path.strip() == '':
-            return None
-
-        # check if file slice is used
-        slices_ = None
-        if '[' in file_path and ']' in file_path:
-            file_parts = file_path.split('[')
-            file_path = file_parts[0]
-            # remove string up to '[' and after ']'
-            slices_s = file_parts[1].split(']')[0].split(',')
-            slices_ = []
-            for s in slices_s:
-                if s == '':
-                    continue
-                elif ':' in s:
-                    s_split = s.split(':')
-                    if len(s_split) == 2:
-                        start_slice = int(s_split[0]) if s_split[0] != '' else None
-                        end_slice = int(s_split[1]) if s_split[1] != '' else None
-                        slices_.append(slice(start_slice, end_slice, None))
-                    elif len(s_split) == 3:
-                        start_slice = int(s_split[0]) if s_split[0] != '' else None
-                        end_slice = int(s_split[1]) if s_split[1] != '' else None
-                        step_slice = int(s_split[2]) if s_split[2] != '' else None
-                        slices_.append(slice(start_slice, end_slice, step_slice))
-                else:
-                    slices_.append(int(s))
-
-        # check if file exists
-        assert os.path.exists(file_path), f'File does not exist: {file_path}'
-
-        # verify if file is empty
-        if os.path.getsize(file_path) <= 0:
-            return ''
-
-        file_ = unpack.from_file(str(file_path))
-        if 'content' in file_:
-            content = file_['content']
-        else:
-            content = str(file_)
-
-        if content is None:
-            return None
-        content = content.split('\n')
-
-        if slices_ is not None:
-            new_content = []
-            for s in slices_:
-                new_content.extend(content[s])
-            content = new_content
-        content = '\n'.join(content)
-        return content
-
-
-    def reset_eof_of_pdf_return_stream(self, pdf_stream_in: list):
-        actual_line = len(pdf_stream_in)  # Predefined value in case EOF not found
-        # find the line position of the EOF
-        for i, x in enumerate(pdf_stream_in[::-1]):
-            if b'%%EOF' in x:
-                actual_line = len(pdf_stream_in)-i
-                print(f'EOF found at line position {-i} = actual {actual_line}, with value {x}')
-                break
-
-        # return the list up to that point
-        return pdf_stream_in[:actual_line]
-
-    def fix_pdf(self, file_path: str):
-        # opens the file for reading
-        with open(file_path, 'rb') as p:
-            txt = (p.readlines())
-
-        # get the new list terminating correctly
-        txtx = self.reset_eof_of_pdf_return_stream(txt)
-
-        # write to new pdf
-        new_file_path = f'{file_path}_fixed.pdf'
-        with open(new_file_path, 'wb') as f:
-            f.writelines(txtx)
-
-        fixed_pdf = PyPDF2.PdfReader(new_file_path)
-        return fixed_pdf
-
-    def read_text(self, pdf_reader, range_):
-        txt = ''
-        n_pages = len(pdf_reader.pages)
-        if range_ is None:
-            for i in range(n_pages):
-                page = pdf_reader.pages[i]
-                txt += page.extract_text()
-        else:
-            for i in range(n_pages)[range_]:
-                page = pdf_reader.pages[i]
-                txt += page.extract_text()
-        return txt
-
-    def forward(self, argument):
-        kwargs        = argument.kwargs
-        path          = argument.prop.prepared_input
-
-        if '.pdf' in path:
-            range_ = None
-            if 'slice' in kwargs:
-                range_ = kwargs['slice']
-                if isinstance(range_, tuple) or isinstance(range_, list):
-                    range_ = slice(*range_)
-
-            rsp = ''
-            try:
-                with open(str(path), 'rb') as f:
-                    # creating a pdf reader object
-                    pdf_reader = PyPDF2.PdfReader(f)
-                    rsp = self.read_text(pdf_reader, range_)
-            except Exception as e:
-                print(f'Error reading PDF: {e} | {path}')
-                if 'fix_pdf' not in kwargs or not kwargs['fix_pdf']:
-                    raise e
-                fixed_pdf = self.fix_pdf(str(path))
-                pdf_reader_fixed = PyPDF2.PdfReader(fixed_pdf)
-                rsp = self.read_text(pdf_reader_fixed, range_)
-        else:
+from . import __root_dir__
+from typing import Callable, List
+from pathlib import Path
+from pathos.multiprocessing import ProcessingPool as PPool
+
+from .functional import EngineRepository
+
+
+logging.getLogger("multiprocessing").setLevel(logging.ERROR)
+
+
+def _run_in_process(expr, func, args, kwargs):
+    # Unpickling the expression using dill
+    expr = dill.loads(expr)
+    func = dill.loads(func)
+    return func(expr, *args, **kwargs)
+
+def _parallel(func: Callable, expressions: List[Callable], worker: int = mp.cpu_count() // 2):
+    def proxy_function(*args, **kwargs):
+        # Pickle the expressions using dill
+        pickled_exprs = [dill.dumps(expr) for expr in expressions]
+        pickled_func = dill.dumps(func)
+        with mp.Pool(processes=worker) as pool:
+            # We map the _run_in_process function to each pickled expression
+            results = pool.starmap(_run_in_process, [(expr, pickled_func, args, kwargs) for expr in pickled_exprs])
+        return results
+    return proxy_function
+
+# Decorator
+def parallel(expressions: List[Callable], worker: int = mp.cpu_count() // 2):
+    def decorator_parallel(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            # Run expressions in parallel
+            parallel_func = _parallel(func, expressions, worker=worker)
+            # Call the proxy function to execute in parallel and capture results
+            results = parallel_func(*args, **kwargs)
+            return results
+        return wrapper
+    return decorator_parallel
+
+def bind(engine: str, property: str):
+    '''
+    Bind to an engine and retrieve one of its properties.
+    '''
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            return EngineRepository.bind_property(
+                    engine=engine,
+                    property=property
+                )
+        return wrapper
+    return decorator
+
+
+def retry(
+    exceptions=Exception,
+    tries=-1,
+    delay=0,
+    max_delay=-1,
+    backoff=1,
+    jitter=0
+):
+    '''
+    Returns a retry decorator.
+
+    :param exceptions: an exception or a tuple of exceptions to catch. default: Exception.
+    :param tries:      the maximum number of attempts. default: -1 (infinite).
+    :param delay:      initial delay between attempts. default: 0.
+    :param max_delay:  the maximum value of delay. default: -1 (no limit).
+    :param backoff:    multiplier applied to delay between attempts. default: 1 (no backoff).
+    :param jitter:     extra seconds added to delay between attempts. default: 0.
+                       fixed if a number, random if a range tuple (min, max)
+
+    Credits to invlpg (https://pypi.org/project/retry)
+    '''
+
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            return _retry_func(
+                    functools.partial(func, *args, **kwargs),
+                    exceptions=exceptions,
+                    tries=tries,
+                    delay=delay,
+                    max_delay=max_delay,
+                    backoff=backoff,
+                    jitter=jitter
+                )
+        return wrapper
+    return decorator
+
+
+def _retry_func(
+    func: callable,
+    exceptions: Exception,
+    tries: int,
+    delay: int,
+    max_delay: int,
+    backoff=int,
+    jitter=int
+):
+    _tries, _delay = tries, delay
+    while _tries:
+        try:
+            return func()
+        except exceptions as e:
+            _tries -= 1
+            if not _tries:
+                raise
+
+            time.sleep(_delay)
+            _delay *= backoff
+
+            if isinstance(jitter, tuple):
+                _delay += random.uniform(*jitter)
+            else:
+                _delay += jitter
+
+            if max_delay >= 0:
+                _delay = min(_delay, max_delay)
+
+
+def cache(
+    in_memory:  bool,
+    cache_path: str = __root_dir__ / 'cache'
+):
+    '''
+    Cache the result of a *any* function call. This is very useful in cost optimization (e.g. computing embeddings).
+    '''
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(instance):
+            return _cache_registry_func(
+                    in_memory,
+                    cache_path,
+                    func,
+                    instance
+                )
+        return wrapper
+    return decorator
+
+
+def _cache_registry_func(
+        in_memory: bool,
+        cache_path: str,
+        func: Callable,
+        *args, **kwargs
+    ):
+
+    if not os.path.exists(cache_path): os.makedirs(cache_path)
+
+    if in_memory and os.path.exists(Path(cache_path) / func.__qualname__):
+        with open(Path(cache_path) / func.__qualname__, 'rb') as f:
+            call = pickle.load(f)
+
+        return call
+
+    call = func(*args, **kwargs)
+    with open(Path(cache_path) / func.__qualname__, 'wb') as f:
+        pickle.dump(call , f)
+
+    return call
+
+def error_logging(debug: bool = False):
+    '''
+    Log the error of a function call.
+    '''
+    def dec(func):
+        @functools.wraps(func)
+        def _dec(*args, **kwargs):
             try:
-                rsp = self._read_slice_file(path)
+                return func(*args, **kwargs)
             except Exception as e:
-                print(f'Error reading empty file: {e} | {path}')
+                logging.error(e)
+                if debug:
+                    # Simple message:
+                    print('Function: {} call failed. Error: {}'.format(func.__name__, e))
+                    # print traceback
+                    traceback.print_exc()
                 raise e
-
-        if rsp is None:
-            raise Exception(f'Error reading file - empty result: {path}')
-
-        # ensure encoding is utf8
-        rsp = rsp.encode('utf8', 'ignore').decode('utf8', 'ignore')
-
-        metadata = {}
-
-        return [rsp], metadata
-
-    def prepare(self, argument):
-        assert not argument.prop.processed_input, "FileEngine does not support processed_input."
-        path = argument.prop.path
-        path = path.replace('\\', '')
-        argument.prop.prepared_input = path
+        return _dec
+    return dec
```

### Comparing `symbolicai-0.6.1/symai/backend/engines/imagecaptioning/engine_blip2.py` & `symbolicai-0.6.2/symai/backend/engines/imagecaptioning/engine_blip2.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/imagecaptioning/engine_llavacpp_client.py` & `symbolicai-0.6.2/symai/backend/engines/imagecaptioning/engine_llavacpp_client.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/imagerendering/engine_dall_e.py` & `symbolicai-0.6.2/symai/backend/engines/imagerendering/engine_dall_e.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/index/engine_pinecone.py` & `symbolicai-0.6.2/symai/backend/engines/index/engine_pinecone.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/index/engine_vectordb.py` & `symbolicai-0.6.2/symai/backend/engines/index/engine_vectordb.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         ):
         super().__init__()
         self.index_name     = index_name
         self.index_dims     = index_dims
         self.index_top_k    = index_top_k
         self.index_metric   = index_metric
         self.storage_file   = index_storage_file
+        self.model          = None
         # Initialize an instance of VectorDB
         # Note that embedding_function and vectors are not passed as VectorDB will compute it on the fly
         self.index = index_dict
 
     def id(self) -> str:
         if not SYMAI_CONFIG['INDEXING_ENGINE_API_KEY'] or SYMAI_CONFIG['INDEXING_ENGINE_API_KEY'] == '':
             return 'index'
@@ -121,15 +122,15 @@
         top_k        = argument.prop.top_k or self.index_top_k
         metric       = argument.prop.metric or self.index_metric
         kwargs       = argument.kwargs
         similarities = argument.prop.similarities or False
         storage_file = argument.prop.storage_file or self.storage_file
         rsp          = None
 
-        self._init(top_k, index_dims, metric)
+        self._init(index_name, top_k, index_dims, metric)
 
         # Process each operation
         if operation == 'search':
             # Get the query text from the prepared input
             query_vector = embedding[0]
             # Perform search in the VectorDB
             results = self.index[index_name](vector=query_vector, top_k=top_k, return_similarities=similarities)
@@ -143,44 +144,46 @@
                 vectors.append(vector)
                 documents.append(document['text'])
             self.index[index_name].add(documents=documents, vectors=vectors)
 
         elif operation == 'config':
             # Handle any configurations if needed (not applicable for in-memory VectorDB)
             assert kwargs, 'Please provide a configuration dictionary.'
-            assert storage_file, 'Please provide a `storage_file` path to load the pre-computed index.'
             # Check if the index is to be persisted or loaded
             if argument.prop.load:
+                assert storage_file, 'Please provide a `storage_file` path to load the pre-computed index.'
                 # Load the pre-computed index from the provided path
                 self.index[index_name] = VectorDB(
                     index_dims=index_dims,
                     top_k=top_k,
                     similarity_metric=metric,
                     load_on_init=storage_file,
                     index_name=index_name
                 )
             else:
                 # Save the pre-computed index to the provided path
                 self.index[index_name].save(storage_file)
 
         else:
-            raise ValueError('Invalid operation')
+            raise ValueError('Invalid operation; please use either "search", "add", or "config".')
 
         metadata = {}
 
         rsp = VectorDBResult(rsp, query, None)
         return [rsp], metadata
 
-    def _init(self, top_k, index_dims, metric):
+    def _init(self, index_name, top_k, index_dims, metric, embedding_model=not None):
         # Initialize the VectorDB if not already initialized
-        if self.index_name not in self.index:
-            self.index[self.index_name] = VectorDB(
+        if index_name not in self.index:
+            self.index[index_name] = VectorDB(
+                index_name=index_name,
                 index_dims=index_dims,
                 top_k=top_k,
-                similarity_metric=metric
+                similarity_metric=metric,
+                embedding_model=embedding_model #@NOTE: the VectorDBIndexEngine class uses precomputed embeddings so the model is not needed in the VectorDB class
             )
 
     def prepare(self, argument):
         assert not argument.prop.processed_input, 'VectorDB indexing engine does not support processed_input.'
         argument.prop.prepared_input = argument.prop.prompt
 
     def save(self, index_name = None, storage_file = None):
```

### Comparing `symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_nesy_client.py` & `symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_nesy_client.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_openai_gptX_chat.py` & `symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_openai_gptX_chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import openai
 
 from typing import List, Optional
 
 from ...base import Engine
 from ...mixin.openai import OpenAIMixin
 from ...settings import SYMAI_CONFIG
-from ....utils import encode_frames_file
+from ....utils import encode_frames_file, CustomUserWarning
 from ....misc.console import ConsoleStyle
 from ....symbol import Symbol
 
 
 logging.getLogger("openai").setLevel(logging.ERROR)
 logging.getLogger("requests").setLevel(logging.ERROR)
 logging.getLogger("urllib").setLevel(logging.ERROR)
@@ -21,37 +21,28 @@
 
 
 class InvalidRequestErrorRemedyChatStrategy:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __call__(self, engine, error, callback, argument):
-        openai_kwargs = {}
         kwargs              = argument.kwargs
         prompts_            = argument.prop.prepared_input
 
-        # send prompt to GPT-X Chat-based
-        stop                = kwargs['stop'] if 'stop' in kwargs else None
-        model               = kwargs['model'] if 'model' in kwargs else None
-
         msg = str(error)
         handle = None
         try:
             if "This model's maximum context length is" in msg:
                 handle = 'type1'
-                max_ = engine.max_tokens
+                max_ = engine.max_context_tokens
                 usr = msg.split('tokens. ')[1].split(' ')[-1]
                 overflow_tokens = int(usr) - int(max_)
             elif "is less than the minimum" in msg:
                 handle = 'type2'
-                # extract number until 'is'
-                msg_ = msg.split("is less than the minimum")[0]
-                # remove until the first `-`
-                msg_ = msg_.split(': "-')[-1]
-                overflow_tokens = int(msg_)
+                overflow_tokens = engine.max_response_tokens
             else:
                 raise Exception(msg) from error
         except Exception as e:
             raise e from error
 
         prompts = [p for p in prompts_ if p['role'] == 'user']
         system_prompt = [p for p in prompts_ if p['role'] == 'system']
@@ -60,183 +51,227 @@
             truncated_prompts_ = [{'role': p['role'], 'content': c} for p, c in zip(prompts, truncated_content_)]
             with ConsoleStyle('warn') as console:
                 console.print(f"WARNING: Overflow tokens detected. Reducing prompt size by {overflow_tokens} characters.")
         elif handle == 'type2':
             user_prompts = [p['content'] for p in prompts]
             new_prompt   = [*system_prompt]
             new_prompt.extend([{'role': p['role'], 'content': c} for p, c in zip(prompts, user_prompts)])
-            overflow_tokens = engine.compute_required_tokens(new_prompt) - int(engine.max_tokens * 0.70)
+            overflow_tokens = engine.compute_required_tokens(new_prompt) - int(engine.max_context_tokens * 0.70)
             if overflow_tokens > 0:
-                print('WARNING: Overflow tokens detected. Reducing prompt size to 70% of max_tokens.')
+                CustomUserWarning(f'WARNING: Overflow tokens detected. Reducing prompt size to 70% of model context size ({engine.max_context_tokens}).')
                 for i, content in enumerate(user_prompts):
                     token_ids = engine.tokenizer.encode(content)
                     if overflow_tokens >= len(token_ids):
                         overflow_tokens -= len(token_ids)
                         user_prompts[i] = ''
                     else:
                         new_content = engine.tokenizer.decode(token_ids[:-overflow_tokens])
                         user_prompts[i] = new_content
                         overflow_tokens = 0
                         break
 
             new_prompt = [*system_prompt]
             new_prompt.extend([{'role': p['role'], 'content': c} for p, c in zip(prompts, user_prompts)])
-            assert engine.compute_required_tokens(new_prompt) <= engine.max_tokens, \
-                f"Token overflow: prompts exceed {engine.max_tokens} tokens after truncation"
+            assert engine.compute_required_tokens(new_prompt) <= engine.max_context_tokens, \
+                f"Token overflow: prompts exceed {engine.max_context_tokens} tokens after truncation"
 
             truncated_prompts_ = [{'role': p['role'], 'content': c.strip()} for p, c in zip(prompts, user_prompts) if c.strip()]
         else:
             raise Exception('Invalid handle case for remedy strategy.') from error
 
         truncated_prompts_ = [*system_prompt, *truncated_prompts_]
 
-        # convert map to list of strings
-        max_tokens          = kwargs['max_tokens'] if 'max_tokens' in kwargs else engine.compute_remaining_tokens(truncated_prompts_)
-        temperature         = kwargs['temperature'] if 'temperature' in kwargs else 1
-        frequency_penalty   = kwargs['frequency_penalty'] if 'frequency_penalty' in kwargs else 0
-        presence_penalty    = kwargs['presence_penalty'] if 'presence_penalty' in kwargs else 0
-        top_p               = kwargs['top_p'] if 'top_p' in kwargs else 1
-        functions           = kwargs['functions'] if 'functions' in kwargs else None
-        function_call       = "auto" if functions is not None else None
-
-        if stop is not None:
-            openai_kwargs['stop'] = stop
-        if functions is not None:
-            openai_kwargs['functions'] = functions
-        if function_call is not None:
-            openai_kwargs['function_call'] = function_call
-
-        return callback(model=model,
-                        messages=truncated_prompts_,
-                        max_tokens=max_tokens,
-                        temperature=temperature,
-                        frequency_penalty=frequency_penalty,
-                        presence_penalty=presence_penalty,
-                        top_p=top_p,
-                        n=1,
-                        **openai_kwargs)
+        model             = kwargs.get('model',             engine.model)
+        seed              = kwargs.get('seed',              engine.seed)
+        max_tokens        = kwargs.get('max_tokens',        engine.compute_remaining_tokens(truncated_prompts_))
+        stop              = kwargs.get('stop')
+        temperature       = kwargs.get('temperature',       1)
+        frequency_penalty = kwargs.get('frequency_penalty', 0)
+        presence_penalty  = kwargs.get('presence_penalty',  0)
+        top_p             = kwargs.get('top_p',             1)
+        n                 = kwargs.get('n',                 1)
+        logit_bias        = kwargs.get('logit_bias')
+        logprobs          = kwargs.get('logprobs',          False)
+        top_logprobs      = kwargs.get('top_logprobs')
+        tools             = kwargs.get('tools')
+        tool_choice       = kwargs.get('tool_choice')
+        response_format   = kwargs.get('response_format')
+
+        return callback(
+                model=model,
+                messages=truncated_prompts_,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                frequency_penalty=frequency_penalty,
+                presence_penalty=presence_penalty,
+                top_p=top_p,
+                n=n,
+                logit_bias=logit_bias,
+                logprobs=logprobs,
+                top_logprobs=top_logprobs,
+                tools=tools,
+                tool_choice=tool_choice,
+                response_format=response_format,
+                seed=seed,
+                stop=stop
+            )
 
 
 class GPTXChatEngine(Engine, OpenAIMixin):
     def __init__(self, api_key: Optional[str] = None, model: Optional[str] = None):
         super().__init__()
-        logger              = logging.getLogger('openai')
+        logger = logging.getLogger('openai')
         logger.setLevel(logging.WARNING)
-        self.config         = SYMAI_CONFIG
-        openai.api_key      = self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] if api_key is None else api_key
-        self.model          = self.config['NEUROSYMBOLIC_ENGINE_MODEL'] if model is None else model
-        self.tokenizer      = tiktoken.encoding_for_model(self.model)
-        self.pricing        = self.api_pricing()
-        self.max_tokens     = self.api_max_tokens() - 100 # TODO: account for tolerance. figure out how their magic number works to compute reliably the precise max token size
-        self.seed           = None
-        self.except_remedy  = None
+        self.config = SYMAI_CONFIG
+        if self.id() != 'neurosymbolic':
+            return # do not initialize if not neurosymbolic; avoids conflict with llama.cpp check in EngineRepository.register_from_package
+        openai.api_key           = self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] if api_key is None else api_key
+        self.model               = self.config['NEUROSYMBOLIC_ENGINE_MODEL'] if model is None else model
+        self.tokenizer           = tiktoken.encoding_for_model(self.model)
+        self.pricing             = self.api_pricing()
+        self.max_context_tokens  = self.api_max_context_tokens()
+        self.max_response_tokens = self.api_max_response_tokens()
+        self.seed                = None
+        self.except_remedy       = None
 
     def id(self) -> str:
-        if   self.config['NEUROSYMBOLIC_ENGINE_MODEL'] and \
-            (self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('gpt-3.5') or \
-             self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('gpt-4')):
+        if   self.config.get('NEUROSYMBOLIC_ENGINE_MODEL') and \
+            (self.config.get('NEUROSYMBOLIC_ENGINE_MODEL').startswith('gpt-3.5') or \
+             self.config.get('NEUROSYMBOLIC_ENGINE_MODEL').startswith('gpt-4')):
             return 'neurosymbolic'
         return super().id() # default to unregistered
 
     def command(self, *args, **kwargs):
         super().command(*args, **kwargs)
         if 'NEUROSYMBOLIC_ENGINE_API_KEY' in kwargs:
             openai.api_key = kwargs['NEUROSYMBOLIC_ENGINE_API_KEY']
         if 'NEUROSYMBOLIC_ENGINE_MODEL' in kwargs:
             self.model     = kwargs['NEUROSYMBOLIC_ENGINE_MODEL']
         if 'seed' in kwargs:
             self.seed      = kwargs['seed']
         if 'except_remedy' in kwargs:
             self.except_remedy = kwargs['except_remedy']
 
-    def compute_required_tokens(self, prompts: dict) -> int:
-        # iterate over prompts and compute number of tokens
-        prompts_ = [role['content'] for role in prompts]
-        if self.model == 'gpt-4-vision-preview':
-            eval_prompt = ''
-            for p in prompts_:
-                if type(p) == str:
-                    eval_prompt += p
-                else:
-                    for p_ in p:
-                        if p_['type'] == 'text':
-                            eval_prompt += p_['text']
-            prompt = eval_prompt
+    def compute_required_tokens(self, messages):
+        """Return the number of tokens used by a list of messages."""
+
+        if self.model in {
+            "gpt-3.5-turbo-0613",
+            "gpt-3.5-turbo-16k-0613",
+            "gpt-4-0314",
+            "gpt-4-32k-0314",
+            "gpt-4-0613",
+            "gpt-4-32k-0613",
+            "gpt-4-turbo",
+            "gpt-4o"
+            }:
+            tokens_per_message = 3
+            tokens_per_name = 1
+        elif self.model == "gpt-3.5-turbo-0301":
+            tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
+            tokens_per_name = -1    # if there's a name, the role is omitted
+        elif self.model == "gpt-3.5-turbo":
+            CustomUserWarning("Warning: gpt-3.5-turbo may update over time. Returning num tokens assuming gpt-3.5-turbo-0613.")
+            tokens_per_message = 3
+            tokens_per_name = 1
+            self.tokenizer = tiktoken.encoding_for_model("gpt-3.5-turbo-0613")
+        elif self.model == "gpt-4":
+            tokens_per_message = 3
+            tokens_per_name = 1
+            CustomUserWarning("Warning: gpt-4 may update over time. Returning num tokens assuming gpt-4-0613.")
+            self.tokenizer = tiktoken.encoding_for_model("gpt-4-0613")
         else:
-            prompt = ''.join(prompts_)
-        val = len(self.tokenizer.encode(prompt, disallowed_special=()))
-        return val
+            raise NotImplementedError(
+                f"""num_tokens_from_messages() is not implemented for model {self.model}. See https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken for information on how messages are converted to tokens."""
+            )
+
+        num_tokens = 0
+        for message in messages:
+            num_tokens += tokens_per_message
+            for key, value in message.items():
+                if type(value) == str:
+                    num_tokens += len(self.tokenizer.encode(value, disallowed_special=()))
+                else:
+                    for v in value:
+                        if v['type'] == 'text':
+                            num_tokens += len(self.tokenizer.encode(v['text'], disallowed_special=()))
+                if key == "name":
+                    num_tokens += tokens_per_name
+        num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
+        return num_tokens
 
     def compute_remaining_tokens(self, prompts: list) -> int:
         val = self.compute_required_tokens(prompts)
-        if 'gpt-4-1106-preview' == self.model or 'gpt-4-vision-preview' == self.model: # models can only output 4_096 tokens
-            return min(int((self.max_tokens - val) * 0.99), 4_096)
-        return int((self.max_tokens - val) * 0.99) # TODO: figure out how their magic number works to compute reliably the precise max token size
+        #@NOTE: this will obviously fail if val is greater than max_context_tokens
+        #       the remedy strategy should handle this case
+        return min(self.max_context_tokens - val, self.max_response_tokens)
 
     def forward(self, argument):
-        kwargs              = argument.kwargs
-        prompts_            = argument.prop.prepared_input
+        kwargs        = argument.kwargs
+        prompts_      = argument.prop.prepared_input
 
-        openai_kwargs = {}
-
-        # send prompt to GPT-X Chat-based
-        stop                = kwargs['stop'] if 'stop' in kwargs else None
-        model               = kwargs['model'] if 'model' in kwargs else self.model
-        seed                = kwargs['seed'] if 'seed' in kwargs else self.seed
-
-        # convert map to list of strings
-        max_tokens          = kwargs['max_tokens'] if 'max_tokens' in kwargs else self.compute_remaining_tokens(prompts_)
-        temperature         = kwargs['temperature'] if 'temperature' in kwargs else 1
-        frequency_penalty   = kwargs['frequency_penalty'] if 'frequency_penalty' in kwargs else 0
-        presence_penalty    = kwargs['presence_penalty'] if 'presence_penalty' in kwargs else 0
-        top_p               = kwargs['top_p'] if 'top_p' in kwargs else 1
-        except_remedy       = kwargs['except_remedy'] if 'except_remedy' in kwargs else self.except_remedy
-        functions           = kwargs['functions'] if 'functions' in kwargs else None
-        function_call       = "auto" if functions is not None else None
-
-        if stop is not None:
-            openai_kwargs['stop'] = stop
-        if functions is not None:
-            openai_kwargs['functions'] = functions
-        if function_call is not None:
-            openai_kwargs['function_call'] = function_call
-        if seed is not None:
-            openai_kwargs['seed'] = seed
+        model             = kwargs.get('model',             self.model)
+        seed              = kwargs.get('seed',              self.seed)
+        except_remedy     = kwargs.get('except_remedy',     self.except_remedy)
+        max_tokens        = kwargs.get('max_tokens',        self.compute_remaining_tokens(prompts_))
+        stop              = kwargs.get('stop',              '')
+        temperature       = kwargs.get('temperature',       1)
+        frequency_penalty = kwargs.get('frequency_penalty', 0)
+        presence_penalty  = kwargs.get('presence_penalty',  0)
+        top_p             = kwargs.get('top_p',             1)
+        n                 = kwargs.get('n',                 1)
+        logit_bias        = kwargs.get('logit_bias')
+        logprobs          = kwargs.get('logprobs')
+        top_logprobs      = kwargs.get('top_logprobs')
+        tools             = kwargs.get('tools')
+        tool_choice       = kwargs.get('tool_choice')
+        response_format   = kwargs.get('response_format')
 
         try:
-            res = openai.chat.completions.create(model=model,
-                                                 messages=prompts_,
-                                                 max_tokens=max_tokens,
-                                                 temperature=temperature,
-                                                 frequency_penalty=frequency_penalty,
-                                                 presence_penalty=presence_penalty,
-                                                 top_p=top_p,
-                                                 n=1,
-                                                 **openai_kwargs)
+            res = openai.chat.completions.create(
+                    model=model,
+                    messages=prompts_,
+                    max_tokens=max_tokens,
+                    temperature=temperature,
+                    frequency_penalty=frequency_penalty,
+                    presence_penalty=presence_penalty,
+                    top_p=top_p,
+                    n=n,
+                    logit_bias=logit_bias,
+                    logprobs=logprobs,
+                    top_logprobs=top_logprobs,
+                    tools=tools,
+                    tool_choice=tool_choice,
+                    response_format=response_format,
+                    seed=seed,
+                    stop=stop
+                )
 
         except Exception as e:
             if openai.api_key is None or openai.api_key == '':
                 msg = 'OpenAI API key is not set. Please set it in the config file or pass it as an argument to the command method.'
                 logging.error(msg)
-                raise Exception(msg) from e
+                if self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] is None or self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] == '':
+                    raise Exception(msg) from e
+                openai.api_key = self.config['NEUROSYMBOLIC_ENGINE_API_KEY']
 
             callback = openai.chat.completions.create
             kwargs['model'] = kwargs['model'] if 'model' in kwargs else self.model
             if except_remedy is not None:
                 res = except_remedy(self, e, callback, argument)
             else:
                 try:
                     # implicit remedy strategy
                     except_remedy = InvalidRequestErrorRemedyChatStrategy()
                     res = except_remedy(self, e, callback, argument)
                 except Exception as e2:
                     ex = Exception(f'Failed to handle exception: {e}. Also failed implicit remedy strategy after retry: {e2}')
                     raise ex from e
 
-        metadata = {}
+        metadata = {'raw_output': res}
 
         rsp    = [r.message.content for r in res.choices]
         output = rsp if isinstance(prompts_, list) else rsp[0]
         return output, metadata
 
     def prepare(self, argument):
         if argument.prop.raw_input:
@@ -247,49 +282,57 @@
             if type(value) != list:
                 if type(value) != dict:
                     value = {'role': 'user', 'content': str(value)}
                 value = [value]
             argument.prop.prepared_input = value
             return
 
-        _non_verbose_output = """[META INSTRUCTIONS START]\nYou do not output anything else, like verbose preambles or post explanation, such as "Sure, let me...", "Hope that was helpful...", "Yes, I can help you with that...", etc. Consider well formatted output, e.g. for sentences use punctuation, spaces etc. or for code use indentation, etc. Never add meta instructions information to your output!\n"""
+        _non_verbose_output = """<META_INSTRUCTION/>\nYou do not output anything else, like verbose preambles or post explanation, such as "Sure, let me...", "Hope that was helpful...", "Yes, I can help you with that...", etc. Consider well formatted output, e.g. for sentences use punctuation, spaces etc. or for code use indentation, etc. Never add meta instructions information to your output!\n\n"""
         user:   str = ""
         system: str = ""
 
         if argument.prop.suppress_verbose_output:
             system += _non_verbose_output
         system = f'{system}\n' if system and len(system) > 0 else ''
 
+        if argument.prop.response_format:
+            system += '<JSON_RESPONSE/>\n You will output JSON!\n\n'
+
         ref = argument.prop.instance
         static_ctxt, dyn_ctxt = ref.global_context
         if len(static_ctxt) > 0:
-            system += f"[STATIC CONTEXT]\n{static_ctxt}\n\n"
+            system += f"<STATIC CONTEXT/>\n{static_ctxt}\n\n"
 
         if len(dyn_ctxt) > 0:
-            system += f"[DYNAMIC CONTEXT]\n{dyn_ctxt}\n\n"
+            system += f"<DYNAMIC CONTEXT/>\n{dyn_ctxt}\n\n"
 
         payload = argument.prop.payload
         if argument.prop.payload:
-            system += f"[ADDITIONAL CONTEXT]\n{str(payload)}\n\n"
+            system += f"<ADDITIONAL CONTEXT/>\n{str(payload)}\n\n"
 
         examples: List[str] = argument.prop.examples
         if examples and len(examples) > 0:
-            system += f"[EXAMPLES]\n{str(examples)}\n\n"
+            system += f"<EXAMPLES/>\n{str(examples)}\n\n"
 
         def extract_pattern(text):
             pattern = r'<<vision:(.*?):>>'
             return re.findall(pattern, text)
 
         def remove_pattern(text):
             pattern = r'<<vision:(.*?):>>'
             return re.sub(pattern, '', text)
 
         image_files = []
         # pre-process prompt if contains image url
-        if self.model == 'gpt-4-vision-preview' and '<<vision:' in str(argument.prop.processed_input):
+        if (self.model == 'gpt-4-vision-preview' or \
+            self.model == 'gpt-4-turbo-2024-04-09' or \
+            self.model == 'gpt-4-turbo' or \
+            self.model == 'gpt-4o') \
+            and '<<vision:' in str(argument.prop.processed_input):
+
             parts = extract_pattern(str(argument.prop.processed_input))
             for p in parts:
                 img_ = p.strip()
                 if img_.startswith('http'):
                     image_files.append(img_)
                 elif img_.startswith('data:image'):
                     image_files.append(img_)
@@ -315,40 +358,48 @@
                     else:
                         print('No frames found or error in encoding frames')
 
         if argument.prop.prompt is not None and len(argument.prop.prompt) > 0:
             val = str(argument.prop.prompt)
             if len(image_files) > 0:
                 val = remove_pattern(val)
-            system += f"[INSTRUCTION]\n{val}"
+            system += f"<INSTRUCTION/>\n{val}\n\n"
 
         suffix: str = str(argument.prop.processed_input)
         if len(image_files) > 0:
             suffix = remove_pattern(suffix)
 
         if '[SYSTEM_INSTRUCTION::]: <<<' in suffix and argument.prop.parse_system_instructions:
             parts = suffix.split('\n>>>\n')
             # first parts are the system instructions
             c = 0
             for i, p in enumerate(parts):
                 if 'SYSTEM_INSTRUCTION' in p:
-                    system += f"{p}\n"
+                    system += f"<{p}/>\n\n"
                     c += 1
                 else:
                     break
             # last part is the user input
             suffix = '\n>>>\n'.join(parts[c:])
         user += f"{suffix}"
 
         if argument.prop.template_suffix:
-            user += f"\n[[PLACEHOLDER]]\n{str(argument.prop.template_suffix)}\n\n"
-            user += f"Only generate content for the placeholder `[[PLACEHOLDER]]` following the instructions and context information. Do NOT write `[[PLACEHOLDER]]` or anything else in your output.\n\n"
+            system += f' You will only generate content for the placeholder `{str(argument.prop.template_suffix)}` following the instructions and the provided context information.\n\n'
 
-        images = [{ 'type': 'image', "image_url": { "url": file, "detail": "auto" }} for file in image_files]
         if self.model == 'gpt-4-vision-preview':
+           images = [{ 'type': 'image', "image_url": { "url": file }} for file in image_files]
+           user_prompt = { "role": "user", "content": [
+                *images,
+                { 'type': 'text', 'text': user }
+            ]}
+        elif self.model == 'gpt-4-turbo-2024-04-09' or \
+             self.model == 'gpt-4-turbo' or \
+             self.model == 'gpt-4o':
+
+            images = [{ 'type': 'image_url', "image_url": { "url": file }} for file in image_files]
             user_prompt = { "role": "user", "content": [
                 *images,
                 { 'type': 'text', 'text': user }
             ]}
         else:
             user_prompt = { "role": "user", "content": user }
```

### Comparing `symbolicai-0.6.1/symai/backend/engines/neurosymbolic/engine_openai_gptX_completion.py` & `symbolicai-0.6.2/symai/backend/engines/neurosymbolic/engine_openai_gptX_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tiktoken
 
 from typing import List, Optional
 
 from ...base import Engine
 from ...mixin.openai import OpenAIMixin
 from ...settings import SYMAI_CONFIG
+from ....utils import CustomUserWarning
 from ....misc.console import ConsoleStyle
 
 
 logging.getLogger("openai").setLevel(logging.ERROR)
 logging.getLogger("requests").setLevel(logging.ERROR)
 logging.getLogger("urllib").setLevel(logging.ERROR)
 logging.getLogger("httpx").setLevel(logging.ERROR)
@@ -19,35 +20,31 @@
 
 class InvalidRequestErrorRemedyCompletionStrategy:
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __call__(self, engine, error, callback, argument):
         openai_kwargs = {}
-        kwargs              = argument.kwargs
-        prompts_            = argument.prop.prepared_input
+        kwargs   = argument.kwargs
+        prompts_ = argument.prop.prepared_input
         # send prompt to GPT-X Completion-based
-        stop                = kwargs['stop'] if 'stop' in kwargs else None
-        model               = kwargs['model'] if 'model' in kwargs else None
+        stop  = kwargs['stop'] if 'stop' in kwargs else None
+        model = kwargs['model'] if 'model' in kwargs else None
 
         msg = str(error)
         handle = None
         try:
             if "This model's maximum context length is" in msg:
                 handle = 'type1'
-                max_ = engine.max_tokens
+                max_ = engine.max_context_tokens
                 usr = msg.split('tokens. ')[1].split(' ')[-1]
                 overflow_tokens = int(usr) - int(max_)
             elif "is less than the minimum" in msg:
                 handle = 'type2'
-                # extract number until 'is'
-                msg_ = msg.split("is less than the minimum")[0]
-                # remove until the first `-`
-                msg_ = msg_.split(': "-')[-1]
-                overflow_tokens = int(msg_)
+                overflow_tokens = engine.max_response_tokens
             else:
                 raise Exception(msg) from error
         except Exception as e:
             raise e from error
 
         # unify the format to use same remedy strategy for both chat and completion
         values = prompts_[0].replace('---------SYSTEM BEHAVIOR--------\n', '').split('\n\n---------USER REQUEST--------\n')
@@ -61,43 +58,43 @@
             prompts_ = [role['content'] for role in prompts]
             prompt = ''.join(prompts_)
             val = len(engine.tokenizer.encode(prompt, disallowed_special=()))
             return val
 
         def compute_remaining_tokens(prompts: list) -> int:
             val = compute_required_tokens(prompts)
-            return int((engine.max_tokens - val) * 0.99)
+            return int((engine.max_context_tokens - val) * 0.99)
 
         if handle == 'type1':
             truncated_content_ = [p['content'][overflow_tokens:] for p in prompts]
             truncated_prompts_ = [{'role': p['role'], 'content': c} for p, c in zip(prompts, truncated_content_)]
             with ConsoleStyle('warn') as console:
                 console.print(f"WARNING: Overflow tokens detected. Reducing prompt size by {overflow_tokens} characters.")
         elif handle == 'type2':
             user_prompts = [p['content'] for p in prompts]
             new_prompt   = [*system_prompt]
             new_prompt.extend([{'role': p['role'], 'content': c} for p, c in zip(prompts, user_prompts)])
-            overflow_tokens = compute_required_tokens(new_prompt) - int(engine.max_tokens * 0.70)
+            overflow_tokens = compute_required_tokens(new_prompt) - int(engine.max_context_tokens * 0.70)
             if overflow_tokens > 0:
-                print('WARNING: Overflow tokens detected. Reducing prompt size to 70% of max_tokens.')
+                CustomUserWarning(f'WARNING: Overflow tokens detected. Reducing prompt size to 70% of model context size ({engine.max_context_tokens}).')
                 for i, content in enumerate(user_prompts):
                     token_ids = engine.tokenizer.encode(content)
                     if overflow_tokens >= len(token_ids):
                         overflow_tokens -= len(token_ids)
                         user_prompts[i] = ''
                     else:
                         new_content = engine.tokenizer.decode(token_ids[:-overflow_tokens])
                         user_prompts[i] = new_content
                         overflow_tokens = 0
                         break
 
             new_prompt = [*system_prompt]
             new_prompt.extend([{'role': p['role'], 'content': c} for p, c in zip(prompts, user_prompts)])
-            assert compute_required_tokens(new_prompt) <= engine.max_tokens, \
-                f"Token overflow: prompts exceed {engine.max_tokens} tokens after truncation"
+            assert compute_required_tokens(new_prompt) <= engine.max_context_tokens, \
+                f"Token overflow: prompts exceed {engine.max_context_tokens} tokens after truncation"
 
             truncated_prompts_ = [{'role': p['role'], 'content': c.strip()} for p, c in zip(prompts, user_prompts) if c.strip()]
         else:
             raise Exception('Invalid handle case for remedy strategy.') from error
 
         truncated_prompts_ = [*system_prompt, *truncated_prompts_]
 
@@ -128,23 +125,26 @@
                         **openai_kwargs)
 
 
 
 class GPTXCompletionEngine(Engine, OpenAIMixin):
     def __init__(self, api_key: Optional[str] = None, model: Optional[str] = None):
         super().__init__()
-        logger              = logging.getLogger('openai')
+        logger = logging.getLogger('openai')
         logger.setLevel(logging.WARNING)
-        self.config         = SYMAI_CONFIG
-        openai.api_key      = self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] if api_key is None else api_key
-        self.model          = self.config['NEUROSYMBOLIC_ENGINE_MODEL'] if model is None else model
-        self.tokenizer      = tiktoken.encoding_for_model(self.model)
-        self.pricing        = self.api_pricing()
-        self.max_tokens     = self.api_max_tokens() - 100 # TODO: account for tolerance. figure out how their magic number works to compute reliably the precise max token size
-        self.except_remedy  = None
+        self.config = SYMAI_CONFIG
+        if self.id() != 'neurosymbolic':
+            return # do not initialize if not neurosymbolic; avoids conflict with llama.cpp check in EngineRepository.register_from_package
+        openai.api_key           = self.config['NEUROSYMBOLIC_ENGINE_API_KEY'] if api_key is None else api_key
+        self.model               = self.config['NEUROSYMBOLIC_ENGINE_MODEL'] if model is None else model
+        self.tokenizer           = tiktoken.encoding_for_model(self.model)
+        self.pricing             = self.api_pricing()
+        self.max_context_tokens  = self.api_max_context_tokens()
+        self.max_response_tokens = self.api_max_response_tokens()
+        self.except_remedy       = None
 
     def id(self) -> str:
         if   self.config['NEUROSYMBOLIC_ENGINE_MODEL'] and \
             (self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('text-') or \
              self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('davinci') or \
              self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('curie') or \
              self.config['NEUROSYMBOLIC_ENGINE_MODEL'].startswith('babbage') or \
@@ -165,35 +165,33 @@
        # iterate over prompts and compute number of tokens
         prompt = prompts[0] # index 0 is correct since we only have one prompt in legacy mode
         val = len(self.tokenizer.encode(prompt, disallowed_special=()))
         return val
 
     def compute_remaining_tokens(self, prompts: list) -> int:
         val = self.compute_required_tokens(prompts)
-        return int((self.max_tokens - val) * 0.99) # TODO: figure out how their magic number works to compute reliably the precise max token size
+        return min(self.max_context_tokens - val, self.max_response_tokens)
 
     def forward(self, argument):
         kwargs              = argument.kwargs
         prompts_            = argument.prop.prepared_input
 
         # send prompt to GPT-3
         max_tokens          = kwargs['max_tokens'] if 'max_tokens' in kwargs else self.compute_remaining_tokens(prompts_)
         stop                = kwargs['stop'] if 'stop' in kwargs else None
         model               = kwargs['model'] if 'model' in kwargs else self.model
-        suffix              = kwargs['template_suffix'] if 'template_suffix' in kwargs else None
         temperature         = kwargs['temperature'] if 'temperature' in kwargs else 0.7
         frequency_penalty   = kwargs['frequency_penalty'] if 'frequency_penalty' in kwargs else 0
         presence_penalty    = kwargs['presence_penalty'] if 'presence_penalty' in kwargs else 0
         top_p               = kwargs['top_p'] if 'top_p' in kwargs else 1
         except_remedy       = kwargs['except_remedy'] if 'except_remedy' in kwargs else self.except_remedy
 
         try:
             res = openai.completions.create(model=model,
                                             prompt=prompts_,
-                                            suffix=suffix,
                                             max_tokens=max_tokens,
                                             temperature=temperature,
                                             frequency_penalty=frequency_penalty,
                                             presence_penalty=presence_penalty,
                                             top_p=top_p,
                                             stop=stop,
                                             n=1)
```

### Comparing `symbolicai-0.6.1/symai/backend/engines/ocr/engine_apilayer.py` & `symbolicai-0.6.2/symai/backend/engines/ocr/engine_apilayer.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/output/engine_stdout.py` & `symbolicai-0.6.2/symai/backend/engines/output/engine_stdout.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/search/engine_serpapi.py` & `symbolicai-0.6.2/symai/backend/engines/search/engine_serpapi.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/symbolic/engine_wolframalpha.py` & `symbolicai-0.6.2/symai/backend/engines/symbolic/engine_wolframalpha.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/text_to_speech/engine_openai.py` & `symbolicai-0.6.2/symai/backend/engines/text_to_speech/engine_openai.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/text_vision/engine_clip.py` & `symbolicai-0.6.2/symai/backend/engines/text_vision/engine_clip.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/engines/userinput/engine_console.py` & `symbolicai-0.6.2/symai/backend/engines/userinput/engine_console.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/mixin/tracker.py` & `symbolicai-0.6.2/symai/backend/mixin/tracker.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/services/huggingface_causallm_server.py` & `symbolicai-0.6.2/symai/backend/services/huggingface_causallm_server.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/services/huggingface_client.py` & `symbolicai-0.6.2/symai/backend/services/huggingface_client.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/backend/services/huggingface_seq2seqlm_server.py` & `symbolicai-0.6.2/symai/backend/services/huggingface_seq2seqlm_server.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/chat.py` & `symbolicai-0.6.2/symai/chat.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/collect/dynamic.py` & `symbolicai-0.6.2/symai/collect/dynamic.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/collect/pipeline.py` & `symbolicai-0.6.2/symai/collect/pipeline.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/collect/stats.py` & `symbolicai-0.6.2/symai/collect/stats.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/components.py` & `symbolicai-0.6.2/symai/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import numpy as np
 
 from tqdm import tqdm
 from pathlib import Path
 from random import sample
 from string import ascii_lowercase, ascii_uppercase
-from typing import Callable, Iterator, List, Optional, Type
+from typing import Callable, Iterator, List, Optional, Type, Union
 from pyvis.network import Network
 
 from . import core
 from . import core_ext
 from .constraints import DictFormatConstraint
 from .formatter import ParagraphFormatter
 from .symbol import Expression, Symbol, Metadata
@@ -458,31 +458,42 @@
         self.exclude = exclude
 
     def forward(self, sym: Symbol, **kwargs) -> Symbol:
         sym = self._to_symbol(sym)
         return sym.filter(self.exclude, include=False, **kwargs)
 
 
+class FileWriter(Expression):
+    def __init__(self, path: str, **kwargs):
+        super().__init__(**kwargs)
+        self.path = path
+
+    def forward(self, sym: Symbol, **kwargs) -> Symbol:
+        sym = self._to_symbol(sym)
+        with open(self.path, 'w') as f:
+            f.write(str(sym))
+
+
 class FileReader(Expression):
-    @classmethod
-    def exists(cls, path: str) -> bool:
+    @staticmethod
+    def exists(path: str) -> bool:
         # remove slicing if any
         _tmp     = path
         _splits  = _tmp.split('[')
         if '[' in _tmp:
             _tmp = _splits[0]
         assert len(_splits) == 1 or len(_splits) == 2, 'Invalid file link format.'
         _tmp     = Path(_tmp)
         # check if file exists and is a file
         if os.path.exists(_tmp) and os.path.isfile(_tmp):
             return True
         return False
 
-    @classmethod
-    def extract_files(cls, cmds: str) -> List[str]:
+    @staticmethod
+    def extract_files(cmds: str) -> List[str]:
         # Use the updated regular expression to match quoted and non-quoted paths
         pattern = r'''(?:"((?:\\.|[^"\\])*)"|'((?:\\.|[^'\\])*)'|`((?:\\.|[^`\\])*)`|((?:\\ |[^ ])+))'''
 
         # Use the updated regular expression to split and handle quoted and non-quoted paths
         matches = re.findall(pattern, cmds)
 
         # Process the matches to handle quoted paths and normal paths
@@ -508,21 +519,36 @@
                 files.append(FileReader.expand_user_path(path))
             elif non_quoted:
                 # For non-quoted paths, we simply add them to the list after expanding
                 files.append(FileReader.expand_user_path(non_quoted))
 
         return files
 
-    @classmethod
-    def expand_user_path(cls, path: str) -> str:
+    @staticmethod
+    def expand_user_path(path: str) -> str:
         return path.replace('~', os.path.expanduser('~'))
 
-    def forward(self, path: str, **kwargs) -> Expression:
-        return self.open(path, **kwargs)
+    @staticmethod
+    def integrity_check(files: List[str]) -> List[str]:
+        not_skipped = []
+        for file in tqdm(files):
+            if FileReader.exists(file):
+                not_skipped.append(file)
+            else:
+                CustomUserWarning(f'Skipping file: {file}')
+        return not_skipped
 
+    def forward(self, files: Union[str, List[str]], **kwargs) -> Expression:
+        if isinstance(files, str):
+            return self.open(files, **kwargs)
+        if isinstance(files, list):
+            if kwargs.get('run_integrity_check'):
+                files = self.integrity_check(files)
+            return self.sym_return_type([self.open(f, **kwargs).value for f in files])
+        raise ValueError('Invalid input type. Please provide a string (file path) or a list of strings (file paths).')
 
 class FileQuery(Expression):
     def __init__(self, path: str, filter: str, **kwargs):
         super().__init__(**kwargs)
         self.path = path
         file_open = FileReader()
         self.query_stream = Stream(Sequence(
@@ -805,24 +831,35 @@
         index = str(index)
         index = index.replace('-', '')
         index = index.replace('_', '')
         index = index.replace(' ', '')
         index = index.lower()
         return index
 
-    def __init__(self, index_name: str = DEFAULT, top_k: int = 8, batch_size: int = 20, formatter: Callable = ParagraphFormatter(), auto_add=False, raw_result=True, **kwargs):
+    def __init__(
+            self,
+            index_name: str = DEFAULT,
+            top_k: int = 8,
+            batch_size: int = 20,
+            formatter: Callable = ParagraphFormatter(),
+            auto_add=False,
+            raw_result: bool = False,
+            new_dim: int = None,
+            **kwargs
+        ):
         super().__init__(**kwargs)
         index_name = Indexer.replace_special_chars(index_name)
         self.index_name = index_name
         self.elements   = []
         self.batch_size = batch_size
         self.top_k      = top_k
         self.retrieval  = None
         self.formatter  = formatter
         self.raw_result = raw_result
+        self.new_dim    = new_dim
         self.sym_return_type = Expression
 
         # append index name to indices.txt in home directory .symai folder (default)
         self.path = Path.home() / '.symai' / 'indices.txt'
         if not self.path.exists():
             self.path.parent.mkdir(parents=True, exist_ok=True)
             self.path.touch()
@@ -849,28 +886,33 @@
         if not path.exists():
             return False
         with open(path, 'r') as f:
             indices = f.read().split('\n')
             if self.index_name in indices:
                 return True
 
-    def forward(self, data: Optional[Symbol] = None, raw_result: bool = False) -> Symbol:
+    def forward(
+            self,
+            data: Optional[Symbol] = None,
+            raw_result: bool = False,
+        ) -> Symbol:
         that = self
         if data is not None:
             data = self._to_symbol(data)
-            # split text paragraph-wise and index each paragraph separately
             self.elements = self.formatter(data).value
             # run over the elments in batches
             for i in tqdm(range(0, len(self.elements), self.batch_size)):
-                val = Symbol(self.elements[i:i+self.batch_size]).zip()
+                val = Symbol(self.elements[i:i+self.batch_size]).zip(new_dim=self.new_dim)
                 that.add(val, index_name=that.index_name)
+            that.config(None, index_name=that.index_name)
 
         def _func(query, *args, **kwargs):
-            query_emb = Symbol(query).embed().value
+            raw_result = kwargs.get('raw_result') or that.raw_result
+            query_emb = Symbol(query).embed(new_dim=that.new_dim).value
             res = that.get(query_emb, index_name=that.index_name, index_top_k=that.top_k, ori_query=query, **kwargs)
             that.retrieval = res
-            if that.raw_result or raw_result or ('raw_result' in kwargs and kwargs['raw_result']):
+            if raw_result:
                 return res
             rsp = res.query(query, *args, **kwargs)
             return rsp
 
         return _func
```

### Comparing `symbolicai-0.6.1/symai/constraints.py` & `symbolicai-0.6.2/symai/constraints.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/core.py` & `symbolicai-0.6.2/symai/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 
+from box import Box
 from typing import Callable, Dict, List, Optional, Any
 
 from . import post_processors as post
 from . import pre_processors as pre
 from . import prompts as prm
 from .functional import EngineRepository
 from .symbol import Expression, Metadata
@@ -25,18 +26,22 @@
         self._set_all_kwargs_as_properties()
         # Set default values if not specified for backend processing
         # Reserved keywords
         if 'preview' not in self.kwargs:
             self.prop.preview           = False
         if 'raw_input' not in self.kwargs:
             self.prop.raw_input         = False
+        if 'raw_output' not in self.kwargs:
+            self.prop.raw_output        = False
         if 'logging' not in self.kwargs:
             self.prop.logging           = False
         if 'verbose' not in self.kwargs:
             self.prop.verbose           = False
+        if 'response_format' not in self.kwargs:
+            self.prop.response_format   = None
         if 'log_level' not in self.kwargs:
             self.prop.log_level         = None
         if 'time_clock' not in self.kwargs:
             self.prop.time_clock        = None
         if 'payload' not in self.kwargs:
             self.prop.payload           = None
         if 'processed_input' not in self.kwargs:
@@ -54,15 +59,21 @@
 
     def _set_all_kwargs_as_properties(self):
         for key, value in self.kwargs.items():
             setattr(self.prop, key, value)
 
     @property
     def value(self):
-        return self.prop
+        return Box({
+            'args': self.args,
+            'signature_kwargs': self.signature_kwargs,
+            'decorator_kwargs': self.decorator_kwargs,
+            'kwargs': self.kwargs,
+            'prop': self.prop
+        })
 
     def _construct_kwargs(self, signature_kwargs, decorator_kwargs):
         '''
         Combines and overrides the decorator args and kwargs with the runtime signature args and kwargs.
 
         Args:
             signature_kwargs (Dict): The signature kwargs.
```

### Comparing `symbolicai-0.6.1/symai/endpoints/api.py` & `symbolicai-0.6.2/symai/endpoints/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import importlib
 import inspect
 import pickle
 import redis
 
 from redis.exceptions import ConnectionError
-from fastapi import FastAPI, APIRouter, HTTPException
+from fastapi import FastAPI, APIRouter, HTTPException, Security, status
+from fastapi.security import APIKeyHeader
+from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 from typing import Any, Generic, TypeVar, Dict, List, Optional, Union
 
+from symai.backend import settings
+
 from .. import core_ext
 from ..symbol import Symbol, Expression
 
 
 # Configure Redis server connection parameters and executable path
 HOST  = 'localhost'
 PORT  = 6379
 DEBUG = True
-
+API_KEY = settings.SYMAI_CONFIG.get('FASTAPI_API_KEY', None)
 
 def is_redis_running(host: str, port: int) -> bool:
     """Check if a Redis server is running at the given host and port."""
     try:
         r = redis.Redis(host=host, port=port)
         r.ping()
         print(f"Redis server is running at {host}:{port}")
@@ -98,26 +102,28 @@
     host=HOST,   # Or use the host where your Redis server is running
     port=PORT,   # The default Redis port number
     db=0         # The default database index
 )
 
 # Initialize the FastAPI app and API router
 app                           = FastAPI(title="SymbolicAI API", version="1.0")
+api_key_header                = APIKeyHeader(name="X-API-Key")
 router                        = APIRouter()
 use_redis                     = is_redis_running(HOST, PORT)
 
 # Instantiate the generic repositories with the counter keys
 symbol_repository             = GenericRepository[Symbol](redis_client, "sym_id", use_redis=use_redis)
 expression_repository         = GenericRepository[Expression](redis_client, "expr_id", use_redis=use_redis)
 # Register all types which subclass Expression and offer a get() method with default=None
 component_class_types = {
     name: cls for name, cls in inspect.getmembers(importlib.import_module('symai.components'), inspect.isclass) if issubclass(cls, Expression)
 }
 component_instance_repository = GenericRepository[Union[Symbol, Expression]](redis_client, "comp_id", use_redis=use_redis)
 
+app.add_middleware(CORSMiddleware, allow_origins=["*"], allow_credentials=True, allow_methods=["*"], allow_headers=["*"])
 
 ### Symbols Endpoints ###
 
 
 class CreateSymbolRequest(BaseModel):
     value: Optional[Any]          = None
     static_context: Optional[str] = ''
@@ -128,53 +134,62 @@
     static_context: str = None
 
 
 class SymbolMethodRequest(BaseModel):
     args: List[Any] = []
     kwargs: Dict[str, Any] = {}
 
+def get_api_key(api_key_header: str = Security(api_key_header) if API_KEY else None) -> str:
+    if API_KEY == None:
+        return True
+    if api_key_header == API_KEY:
+        return api_key_header
+    raise HTTPException(
+        status_code=status.HTTP_401_UNAUTHORIZED,
+        detail="Invalid or missing API Key",
+    )
 
 @app.post("/symbol/")
-def create_symbol(symbol_request: CreateSymbolRequest):
+def create_symbol(symbol_request: CreateSymbolRequest, api_key: str = Security(get_api_key)):
     symbol = Symbol(symbol_request.value, static_context=symbol_request.static_context)
     symbol_id = symbol_repository.uid()
     symbol_repository.set(symbol_id, symbol)
     return {"id": symbol_id, **symbol.json()}
 
 
 @app.get("/symbol/{symbol_id}/")
-def get_symbol(symbol_id: str):
+def get_symbol(symbol_id: str, api_key: str = Security(get_api_key)):
     symbol = symbol_repository.get(symbol_id)
     if symbol is None:
         raise HTTPException(status_code=404, detail="Symbol not found")
     return symbol.json()
 
 
 @app.patch("/symbol/{symbol_id}/")
-def update_symbol(symbol_id: str, update_request: UpdateSymbolRequest):
+def update_symbol(symbol_id: str, update_request: UpdateSymbolRequest, api_key: str = Security(get_api_key)):
     symbol = symbol_repository.get(symbol_id)
     if symbol is None:
         raise HTTPException(status_code=404, detail="Symbol not found")
     for attr, value in update_request.model_dump(exclude_unset=True).items():
         setattr(symbol, attr, value)
     symbol_repository.set(symbol_id, symbol)
     return symbol.json()
 
 
 @app.delete("/symbol/{symbol_id}/")
-def delete_symbol(symbol_id: str):
+def delete_symbol(symbol_id: str, api_key: str = Security(get_api_key)):
     symbol = symbol_repository.delete(symbol_id)
     if symbol is None:
         raise HTTPException(status_code=404, detail="Symbol not found")
     return {"message": "Symbol deleted successfully"}
 
 
 @app.post("/symbol/{symbol_id}/{method_name}/")
 @core_ext.error_logging(debug=DEBUG)
-def operate_on_symbol(symbol_id: str, method_name: str, method_request: SymbolMethodRequest):
+def operate_on_symbol(symbol_id: str, method_name: str, method_request: SymbolMethodRequest, api_key: str = Security(get_api_key)):
     symbol = symbol_repository.get(symbol_id)
     if symbol is None:
         raise HTTPException(status_code=404, detail="Symbol not found")
     method = getattr(symbol, method_name, None)
     if method is None or not callable(method):
         raise HTTPException(status_code=404, detail=f"Method {method_name} not found or is not callable")
     result = method(*method_request.args, **method_request.kwargs)
@@ -189,66 +204,66 @@
 
 
 class UpdateExpressionRequest(BaseModel):
     value: Any = None
 
 
 @app.post("/expression/")
-def create_expression(expression_request: CreateExpressionRequest):
+def create_expression(expression_request: CreateExpressionRequest, api_key: str = Security(get_api_key)):
     expression = Expression(expression_request.value)
     expression_id = expression_repository.uid()
     expression_repository.set(expression_id, expression)
     return {"id": expression_id, **expression.json()}
 
 
 @app.get("/expression/{expression_id}/")
-def get_expression(expression_id: str):
+def get_expression(expression_id: str, api_key: str = Security(get_api_key)):
     expression = expression_repository.get(expression_id)
     if expression is None:
         raise HTTPException(status_code=404, detail="Expression not found")
     return expression.json()
 
 
 @app.post("/expression/{expression_id}/call/")
 @core_ext.error_logging(debug=DEBUG)
-def call_expression(expression_id: str, method_request: SymbolMethodRequest):
+def call_expression(expression_id: str, method_request: SymbolMethodRequest, api_key: str = Security(get_api_key)):
     # Retrieve the expression instance by ID
     expression = expression_repository.get(expression_id)
     if expression is None:
         raise HTTPException(status_code=404, detail="Expression not found")
     result = expression(*method_request.args, **method_request.kwargs)
     return {"result": result.json() if isinstance(result, Symbol) else result}
 
 
 @app.post("/expression/{expression_id}/{method_name}/")
 @core_ext.error_logging(debug=DEBUG)
-def operate_on_expression(expression_id: str, method_name: str, method_request: SymbolMethodRequest):
+def operate_on_expression(expression_id: str, method_name: str, method_request: SymbolMethodRequest, api_key: str = Security(get_api_key)):
     expression = expression_repository.get(expression_id)
     if expression is None:
         raise HTTPException(status_code=404, detail="Expression not found")
     method = getattr(expression, method_name, None)
     if method is None or not callable(method):
         raise HTTPException(status_code=404, detail=f"Method {method_name} not found or is not callable")
     result = method(*method_request.args, **method_request.kwargs)
     return {"result": result.json() if isinstance(result, Symbol) else result}
 
 
 @app.patch("/expression/{expression_id}/")
-def update_expression(expression_id: str, update_request: UpdateExpressionRequest):
+def update_expression(expression_id: str, update_request: UpdateExpressionRequest, api_key: str = Security(get_api_key)):
     expression = expression_repository.get(expression_id)
     if expression is None:
         raise HTTPException(status_code=404, detail="Expression not found")
     for attr, value in update_request.model_dump(exclude_unset=True).items():
         setattr(expression, attr, value)
     expression_repository.set(expression_id, expression)
     return expression.json()
 
 
 @app.delete("/expression/{expression_id}/")
-def delete_expression(expression_id: str):
+def delete_expression(expression_id: str, api_key: str = Security(get_api_key)):
     expression = expression_repository.delete(expression_id)
     if expression is None:
         raise HTTPException(status_code=404, detail="Expression not found")
     return {"message": "Expression deleted successfully"}
 
 
 #### Generic Component Endpoints ####
@@ -277,40 +292,40 @@
 
 
 class UpdateComponentRequest(BaseModel):
     update_kwargs: Dict[str, Any] = {}
 
 
 @app.post("/components/")
-def create_component(request: CreateComponentGenericRequest):
+def create_component(request: CreateComponentGenericRequest, api_key: str = Security(get_api_key)):
     # Retrieve the class from the repository
     cls = component_class_types.get(request.class_name)
     if cls is None:
         raise HTTPException(status_code=404, detail="Component class not found")
     # Instantiate the class and execute the command
     instance = cls(*request.init_args, **request.init_kwargs)
     # Store the instance with a generated ID and return the ID
     instance_id = component_instance_repository.uid()
     component_instance_repository.set(instance_id, instance)  # Assuming component_instance_repository exists
     return {"id": instance_id}
 
 
 @app.get("/components/{instance_id}/")
-def get_component(instance_id: str):
+def get_component(instance_id: str, api_key: str = Security(get_api_key)):
     # Retrieve an instance by its ID from the repository
     instance = component_instance_repository.get(instance_id)
     if instance is None:
         raise HTTPException(status_code=404, detail="Component instance not found")
     return instance.json()  # Assuming __dict__ can be used to serialize the instance
 
 
 # Endpoint to execute a command on a component instance
 @app.post("/components/call/")
 @core_ext.error_logging(debug=DEBUG)
-def generic_forward(request: GenericRequest):
+def generic_forward(request: GenericRequest, api_key: str = Security(get_api_key)):
     # Dynamically import the class from components module based on request.class_name
     components_module = importlib.import_module('.components', package='symai')
     cls = getattr(components_module, request.class_name)
     # Check if cls is subclass of Expression and instantiate
     if not issubclass(cls, components_module.Expression):
         raise ValueError("The provided class name must be a subclass of Expression")
     # Initialize the class with provided init_args, requiring unpacking **kwargs
@@ -320,26 +335,26 @@
     # Assume result is a components.Symbol instance, you need to return a serializable format
     if isinstance(result, components_module.Symbol):
         return result.json()
     return result  # If result is already a serializable type
 
 
 @app.patch("/components/{instance_id}/")
-def update_component(instance_id: str, update_request: UpdateComponentRequest):
+def update_component(instance_id: str, update_request: UpdateComponentRequest, api_key: str = Security(get_api_key)):
     instance = component_instance_repository.get(instance_id)
     if instance is None:
         raise HTTPException(status_code=404, detail="Component instance not found")
     for attr, value in update_request.update_kwargs.items():
         setattr(instance, attr, value)
     component_instance_repository.set(instance_id, instance)
     return instance.json()
 
 
 @app.delete("/components/{instance_id}/")
-def delete_component(instance_id: str):
+def delete_component(instance_id: str, api_key: str = Security(get_api_key)):
     instance = component_instance_repository.delete(instance_id)
     if instance is None:
         raise HTTPException(status_code=404, detail="Component instance not found")
     return {"message": "Component instance deleted successfully"}
 
 
 ### Selectively register the endpoints with the API router ###
@@ -366,15 +381,15 @@
 
 class UpdateExtendedRequest(BaseModel):
     update_kwargs: Dict[str, Any] = {}
 
 
 # Create endpoints for each of the extended classes
 @app.post("/extended/")
-def create_extended(request: CreateExtendedRequest):
+def create_extended(request: CreateExtendedRequest, api_key: str = Security(get_api_key)):
     # Dynamically retrieve the extended class
     extended_class = extended_class_types.get(request.class_name)
     if extended_class is None:
         raise HTTPException(status_code=404, detail=f"{request.class_name} class not found")
     # Instantiate the extended class with the provided arguments
     extended_instance = extended_class(*request.init_args, **request.init_kwargs)
     # Store the instance and return the instance ID and details
@@ -382,15 +397,15 @@
     extended_instance_repository.set(instance_id, extended_instance)
     return {"id": instance_id, **extended_instance.json()}
 
 
 # Endpoint to execute a command on a component instance
 @app.post("/extended/call/")
 @core_ext.error_logging(debug=DEBUG)
-def extended_forward(request: GenericRequest):
+def extended_forward(request: GenericRequest, api_key: str = Security(get_api_key)):
     # Dynamically import the class from components module based on request.class_name
     try:
         # get request.class_name from extended_types if it's a type of extended_types
         cls = extended_class_types.get(request.class_name)
         # look for the class in the extended module if not found in extended_types
         # iterate over the extended_type Union and check if the class name is in the __dict__
         if cls is None:
@@ -412,37 +427,37 @@
     except TypeError as e:
         raise HTTPException(status_code=422, detail=str(e))
     except Exception as e:
         raise HTTPException(status_code=500, detail=f"An error occurred: {str(e)}")
 
 
 @app.get("/extended/{instance_id}/")
-def get_extended(instance_id: str):
+def get_extended(instance_id: str, api_key: str = Security(get_api_key)):
     # Retrieve an instance by its ID
     extended_instance = extended_instance_repository.get(instance_id)
     if extended_instance is None:
         raise HTTPException(status_code=404, detail="Extended instance not found")
     return extended_instance.json()
 
 
 @app.patch("/extended/{instance_id}/")
-def update_extended(instance_id: str, update_request: UpdateExtendedRequest):
+def update_extended(instance_id: str, update_request: UpdateExtendedRequest, api_key: str = Security(get_api_key)):
     # Retrieve the instance by its ID
     extended_instance = extended_instance_repository.get(instance_id)
     if extended_instance is None:
         raise HTTPException(status_code=404, detail="Extended instance not found")
     # Update the instance with the provided arguments
     for attr, value in update_request.update_kwargs.items():
         setattr(extended_instance, attr, value)
     extended_instance_repository.set(instance_id, extended_instance)
     return extended_instance.json()
 
 
 @app.delete("/extended/{instance_id}/")
-def delete_extended(instance_id: str):
+def delete_extended(instance_id: str, api_key: str = Security(get_api_key)):
     # Attempt to delete the instance by its ID
     success = extended_instance_repository.delete(instance_id)
     if not success:
         raise HTTPException(status_code=404, detail="Extended instance not found or already deleted")
     return {"message": "Extended instance deleted successfully"}
```

### Comparing `symbolicai-0.6.1/symai/extended/__init__.py` & `symbolicai-0.6.2/symai/extended/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/api_builder.py` & `symbolicai-0.6.2/symai/extended/api_builder.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/arxiv_pdf_parser.py` & `symbolicai-0.6.2/symai/extended/arxiv_pdf_parser.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/bibtex_parser.py` & `symbolicai-0.6.2/symai/extended/bibtex_parser.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/conversation.py` & `symbolicai-0.6.2/symai/extended/conversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 import os
 import pickle
 
 from datetime import datetime
 from typing import Any, Callable, Optional, List
+from pathlib import Path
 
 from .seo_query_optimizer import SEOQueryOptimizer
+from ..formatter import TextContainerFormatter
 from ..components import Indexer, FileReader
 from ..memory import SlidingWindowStringConcatMemory
 from ..symbol import Symbol
 from ..interfaces import Interface
 
 
 class CodeFormatter:
     def __call__(self, value: str, *args: Any, **kwds: Any) -> Any:
         # extract code from chat conversations or ```<language>\n{code}\n``` blocks
         return Symbol(value).extract('Only extract code without ``` block markers or chat conversations')
 
 
 class Conversation(SlidingWindowStringConcatMemory):
-    def __init__(self, init:     Optional[str] = None,
-                 file_link:      Optional[List[str]] = None,
-                 url_link:       Optional[List[str]] = None,
-                 index_name:     Optional[str] = None,
-                 auto_print:     bool          = True,
-                 token_ratio:    float         = 0.6,
-                 *args, **kwargs):
+    def __init__(
+            self,
+            init:          Optional[str]       = None,
+            file_link:     Optional[List[str]] = None,
+            url_link:      Optional[List[str]] = None,
+            index_name:    Optional[str]       = None,
+            auto_print:    bool                = True,
+            token_ratio:   float               = 0.6,
+            with_metadata: bool                = False,
+            *args, **kwargs
+        ):
         super().__init__(token_ratio, *args, **kwargs)
         self.token_ratio = token_ratio
         self.auto_print  = auto_print
         if file_link and isinstance(file_link, str):
             file_link    = [file_link]
         if url_link and isinstance(url_link, str):
             url_link     = [url_link]
         self.file_link   = file_link
         self.url_link    = url_link
         self.index_name  = index_name
         self.seo_opt     = SEOQueryOptimizer()
-        self.reader      = FileReader()
+        self.reader      = FileReader(with_metadata=with_metadata)
         self.crawler     = Interface('selenium')
         self.user_tag    = 'USER::'
         self.bot_tag     = 'ASSISTANT::'
 
         if init is not None:
             self.store_system_message(init, *args, **kwargs)
         if file_link is not None:
@@ -49,15 +55,15 @@
         if url_link is not None:
             for url in url_link:
                 self.store_url(url, *args, **kwargs)
         self.indexer     = None
         self.index       = None
         if index_name is not None:
             self.indexer = Indexer(index_name=index_name)
-            self.index   = self.indexer(raw_result=True)
+            self.index   = self.indexer(raw_result=kwargs.get('raw_result', False))
 
     def __getstate__(self):
         state = super().__getstate__().copy()
         # Remove the unpickleable entries such as the `indexer` attribute because it is not serializable
         state.pop('seo_opt', None)
         state.pop('indexer', None)
         state.pop('index', None)
@@ -174,25 +180,27 @@
             length_memory_shards = len(memory_shards)
             if length_memory_shards <= 3:
                 memory_shards = memory_shards
             elif length_memory_shards <= 5:
                 memory_shards = memory_shards[:2] + memory_shards[-(length_memory_shards-2):]
             else:
                 memory_shards = memory_shards[:2] + memory_shards[-3:]
-            search_query = '\n'.join(memory_shards) # join with newlines
-            search_query = self.seo_opt(f'[Query]:' | query | '\n' | search_query)
+
+            search_query = query | '\n' | '\n'.join(memory_shards)
+            if kwargs.get('use_seo_opt'):
+                search_query = self.seo_opt(f'[Query]:' | search_query)
             memory = self.index(search_query, *args, **kwargs)
+
             if 'raw_result' in kwargs:
                 print(memory)
 
         payload = ''
         # if payload is set, then add it to the memory
         if 'payload' in kwargs:
-            payload           = kwargs['payload']
-            kwargs['payload'] = f'[Conversation Payload]:\n{payload}\n'
+            payload  = f"[Conversation Payload]:\n{kwargs.pop('payload')}\n"
 
         index_memory = ''
         # if index is set, then add it to the memory
         if memory:
             index_memory = f'[Index Retrieval]:\n{str(memory)[:1500]}\n'
 
         payload = f'{index_memory}{payload}'
@@ -229,10 +237,73 @@
 
 [Program Instructions]
 If the user requests functions or instructions, you will process the user queries based on the results of the retrieval augmented memory and only return content about the retrieval augmented memory, conversation data and files content.
 """
 
 
 class RetrievalAugmentedConversation(Conversation):
+    def __init__(
+            self,
+            folder_path: Optional[str] = None,
+            *,
+            index_name:  Optional[str] = None,
+            max_depth:   Optional[int] = 0,
+            auto_print:  bool          = True,
+            token_ratio: float         = 0.9,
+            top_k                      = 5,
+            formatter: Callable        = TextContainerFormatter(),
+            overwrite: bool            = False,
+            with_metadata: bool        = False,
+            raw_result: Optional[bool] = False,
+            new_dim: Optional[int]     = None,
+            **kwargs
+        ):
+
+        super().__init__(auto_print=auto_print, with_metadata=with_metadata, token_ratio=token_ratio, **kwargs)
+        self.folder_path   = folder_path
+        self.max_depth     = max_depth
+        self.index_name    = index_name
+        self.auto_print    = auto_print
+        self.token_ratio   = token_ratio
+        self.top_k         = top_k
+        self.formatter     = formatter
+        self.overwrite     = overwrite
+        self.with_metadata = with_metadata
+        self.raw_result    = raw_result
+        self.new_dim       = new_dim
+
+        indexer = Indexer(index_name=index_name, top_k=top_k, formatter=formatter, auto_add=False, new_dim=new_dim)
+        if folder_path and (not indexer.exists() or overwrite):
+            files = self.get_files(folder_path, max_depth)
+            indexer.register()
+            text = self.reader(files, with_metadata=with_metadata, **kwargs)
+
+            self.index = indexer(
+                    data=text,
+                    raw_result=raw_result,
+                    **kwargs
+                )
+        else:
+            self.index = indexer(
+                    raw_result=raw_result,
+                    **kwargs
+                )
+
     @property
     def static_context(self) -> str:
         return RETRIEVAL_CONTEXT
+
+    def get_files(self, folder_path, max_depth):
+        accepted_formats = ['.pdf', '.md', '.txt']
+
+        folder = Path(folder_path)
+        files = []
+        for file_path in folder.rglob("*"):
+            if file_path.is_file() and file_path.suffix in accepted_formats:
+                relative_path = file_path.relative_to(folder)
+                depth = len(relative_path.parts) - 1
+                if depth <= max_depth:
+                    files.append(file_path.as_posix())
+        return files
+
+    def forward(self, query: str, *args, **kwargs):
+        return super().forward(query, *args, **kwargs)
```

### Comparing `symbolicai-0.6.1/symai/extended/crawler.py` & `symbolicai-0.6.2/symai/extended/crawler.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/document.py` & `symbolicai-0.6.2/symai/extended/document.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,41 +4,67 @@
 
 from ..symbol import Expression, Symbol
 from ..components import FileReader, Indexer
 from ..formatter import ParagraphFormatter
 
 
 class DocumentRetriever(Expression):
-    def __init__(self, index_name: str = Indexer.DEFAULT, file = None, top_k = 5, formatter: Callable = ParagraphFormatter(), overwrite: bool = False, raw_result: bool = False, **kwargs):
+    def __init__(
+            self,
+            index_name: str = Indexer.DEFAULT,
+            file = None,
+            top_k = 5,
+            formatter: Callable = ParagraphFormatter(),
+            overwrite: bool = False,
+            with_metadata: bool = False,
+            raw_result: Optional[bool] = False,
+            new_dim: Optional[int] = None,
+            **kwargs
+        ):
         super().__init__(**kwargs)
-        indexer      = Indexer(index_name=index_name, top_k=top_k, formatter=formatter, auto_add=False, raw_result=raw_result)
-        self.indexer = indexer
-        text         = None
+        indexer = Indexer(index_name=index_name, top_k=top_k, formatter=formatter, auto_add=False, new_dim=new_dim)
+        text    = None
+
         if not indexer.exists() or overwrite:
             indexer.register()
             if type(file) is str:
                 file_path = file
                 reader = FileReader()
-                text = reader(file_path, **kwargs)
+                text = reader(file_path, with_metadata=with_metadata, **kwargs)
             else:
                 text = str(file)
-            self.index = indexer(text, **kwargs)
+
+            self.index = indexer(
+                    data=text, #@NOTE: we write the text to the index
+                    raw_result=raw_result,
+                    **kwargs
+                )
         else:
-            self.index = indexer(**kwargs)
+            self.index = indexer(
+                    raw_result=raw_result,
+                    **kwargs
+                    )
 
         self.text = Symbol(text)
         if text is not None:
             # save in home directory
             path = os.path.join(os.path.expanduser('~'), '.symai', 'temp', index_name)
             # create the directory if it does not exist
             if not os.path.exists(path):
                 os.makedirs(path)
             self.dump(os.path.join(path, 'dump_file'), replace=True)
 
-    def forward(self, query: Optional[Symbol], raw_result: bool = False) -> Symbol:
-        return self.index(query, raw_result=raw_result)
+    def forward(
+            self,
+            query: Symbol,
+            raw_result: Optional[bool] = False,
+        ) -> Symbol:
+        return self.index(
+                query,
+                raw_result=raw_result,
+                )
 
     def dump(self, path: str, replace: bool = True) -> Symbol:
         if self.text is None:
             raise ValueError('No text to save.')
         # save the text to a file
         self.text.save(path, replace=replace)
```

### Comparing `symbolicai-0.6.1/symai/extended/file_merger.py` & `symbolicai-0.6.2/symai/extended/file_merger.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/graph.py` & `symbolicai-0.6.2/symai/extended/graph.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/html_style_template.py` & `symbolicai-0.6.2/symai/extended/html_style_template.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/interfaces/ocr.py` & `symbolicai-0.6.2/symai/extended/interfaces/ocr.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/interfaces/pinecone.py` & `symbolicai-0.6.2/symai/extended/interfaces/pinecone.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/interfaces/selenium.py` & `symbolicai-0.6.2/symai/extended/interfaces/selenium.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/interfaces/vectordb.py` & `symbolicai-0.6.2/symai/extended/interfaces/vectordb.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/metrics/similarity.py` & `symbolicai-0.6.2/symai/extended/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/os_command.py` & `symbolicai-0.6.2/symai/extended/os_command.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/packages/symdev.py` & `symbolicai-0.6.2/symai/extended/packages/symdev.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/packages/sympkg.py` & `symbolicai-0.6.2/symai/extended/packages/sympkg.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/packages/symrun.py` & `symbolicai-0.6.2/symai/extended/packages/symrun.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/personas/builder.py` & `symbolicai-0.6.2/symai/extended/personas/builder.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/personas/dialogue.py` & `symbolicai-0.6.2/symai/extended/personas/dialogue.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/personas/persona.py` & `symbolicai-0.6.2/symai/extended/personas/persona.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,16 +130,22 @@
                         pre_processors=pre_processors,
                         post_processors=post_processors)
 
         tag = self.bot_tag if source is None else source
         if not tag.endswith('::'):
             tag = f'{tag}::'
         user_query = self.build_tag(self.user_tag, query)
+
+        payload = ''
+        if 'payload' in kwargs:
+            p = kwargs.pop('payload')
+            payload = f'{p}[PERSONA BIO]\n{self.bio()}'
+
         res = func(user_query,
-                   payload=f'[PERSONA BIO]\n{self.bio()}',
+                   payload=payload,
                    tag=tag,
                    thoughts=thoughts,
                    stop=['>>>'],
                    parse_system_instructions=True,
                    *args, **kwargs,)
 
         if 'preview' in kwargs and kwargs['preview']:
```

### Comparing `symbolicai-0.6.1/symai/extended/personas/research/yann_lecun.py` & `symbolicai-0.6.2/symai/extended/personas/research/yann_lecun.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/personas/sales/erik_james.py` & `symbolicai-0.6.2/symai/extended/personas/sales/erik_james.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/personas/student/max_tenner.py` & `symbolicai-0.6.2/symai/extended/personas/student/max_tenner.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/repo_cloner.py` & `symbolicai-0.6.2/symai/extended/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/seo_query_optimizer.py` & `symbolicai-0.6.2/symai/extended/seo_query_optimizer.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/solver.py` & `symbolicai-0.6.2/symai/extended/solver.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/strategies/exceptremedy.py` & `symbolicai-0.6.2/symai/extended/strategies/exceptremedy.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/summarizer.py` & `symbolicai-0.6.2/symai/extended/summarizer.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/taypan_interpreter.py` & `symbolicai-0.6.2/symai/extended/taypan_interpreter.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/extended/vectordb.py` & `symbolicai-0.6.2/symai/extended/vectordb.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
     Parameters
     ----------
     documents : list, optional
         A list of documents to add to the database.
     vectors : list, optional
         A list of vectors to add to the database.
-    embedding_model : str, optional
-        The reference to an embedding model to use when embedding documents into vectors.
-    embedding_function : function, optional
-        A function that takes in a list of documents and returns a list of vectors.
+    embedding_model : callable, optional
+        The reference to a callable embedding model used in the default `embedding_function`; defaults to `ExtensityAI/embeddings` which is `all-mpnet-base-v2` based.
+    embedding_function : callable, optional
+        A function that takes in a list of documents and returns a list of vectors; defaults to `_get_embedding` which uses the callable `embedding_model`.
     similarity_metric : str, optional
         The similarity metric to use when querying the database. Can be either 'dot', 'cosine', 'euclidean', 'adams', or 'derrida'.
     batch_size : int, optional
         The batch size to use when embedding documents into vectors.
     load_on_init : bool, optional
         Whether or not to load the database from a file on initialization.
     index_dims : int, optional
@@ -75,17 +75,18 @@
     load(storage_file)
         Loads the database from a file.
     forward(query_text, top_k=5, return_similarities=True)
         Queries the database for similar documents.
 
     Examples
     --------
-    >>> from symai.extended import LocalVectorDB
-    >>> db = LocalVectorDB()
-    >>> db.add("Hello, world!")
+    >>> from symai.extended import VectorDB
+    >>> db = VectorDB()
+    >>> db.add("Hello, World!")
+    >>> db("Hello, World!")
     """
     _default_documents          = []
     _default_vectors            = None
     _default_embedding_model    = None
     _default_batch_size         = MAX_BATCH_SIZE
     _default_similarity_metric  = "cosine"
     _default_embedding_function = None
```

### Comparing `symbolicai-0.6.1/symai/formatter.py` & `symbolicai-0.6.2/symai/formatter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import json
 import re
-from typing import List, Dict
+
+from beartype import beartype
+from beartype.typing import Any, Dict, List
+from tqdm import tqdm
 
 from . import core_ext
-from .symbol import Symbol, Expression
+from .symbol import Expression, Symbol
 
 
 class ParagraphFormatter(Expression):
     def __init__(self, value=None, **kwargs):
         super().__init__(value, **kwargs)
         self.NEWLINES_RE = re.compile(r"\n{2,}")  # two or more "\n" characters
         self._has_file_start = False
@@ -131,7 +135,52 @@
         return sentences
 
     def forward(self, sym: Symbol, *args, **kwargs) -> Symbol:
         sym = self._to_symbol(sym)
         # split text sentence-wise and index each sentence separately
         self.elements = self.split_sentences(sym.value)
         return self._to_symbol(self.elements)
+
+
+class TextContainerFormatter(Expression):
+    def __init__(
+            self,
+            value: Any = None,
+            key: str ="text",
+            text_split: int = 4,
+            **kwargs
+        ):
+        super().__init__(value, **kwargs)
+        self.key = key
+        self.text_split = text_split
+
+    @beartype
+    def forward(self, sym: Symbol, *args, **kwargs) -> Symbol:
+        if isinstance(sym.value, list):
+            containers = [container for pdf in sym.value for container in pdf]
+        chunks = [text for container in tqdm(containers) for text in self._chunk(container)]
+        return self._to_symbol(chunks)
+
+    def _chunk(self, container: 'TextContainer') -> List[str]:
+        text = container.text
+        step = len(text) // self.text_split
+        splits = []
+        i = c = 0
+        while c < self.text_split:
+            if c == self.text_split - 1:
+                # Unify the last chunk with the previous one if necessary
+                splits.append(self._as_str(text[i:], container))
+                break
+            splits.append(self._as_str(text[i:i+step], container))
+            i += step
+            c += 1
+        return splits
+
+    def _as_str(self, text: str, container: 'TextContainer') -> str:
+        return (
+            '---\n'
+            f"id: {container.id}\n"
+            f"page: {container.page}\n"
+            '---\n'
+            f"{text}"
+        )
+
```

### Comparing `symbolicai-0.6.1/symai/functional.py` & `symbolicai-0.6.2/symai/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
     while try_cnt < trials:
         try_cnt += 1
         try:
             rsp, metadata = _execute_query(engine, post_processors, return_constraint, argument)
             # return preview of the command if preview is set
             if argument.prop.preview:
                 return rsp
+
+            if argument.prop.raw_output:
+                return metadata.get('raw_output')
+
         except Exception as e:
             logging.error(f"Failed to execute query: {str(e)}")
             traceback.print_exc()
             if try_cnt < trials:
                 continue # repeat if query unsuccessful
             # if max retries reached, return default or raise exception
             # execute default function implementation as fallback
@@ -218,27 +222,17 @@
             cls._instance.__init__()  # Explicitly call __init__
         return cls._instance
 
     @staticmethod
     def register(id: str, engine_instance: Engine, allow_engine_override: bool = False, *args, **kwargs) -> None:
         self = EngineRepository()
         # Check if the engine is already registered
-        if id in self._engines.keys() and not allow_engine_override:
+        if id in self._engines and not allow_engine_override:
             raise ValueError(f"Engine {id} is already registered. Set allow_engine_override to True to override.")
-        elif id in self._engines:
-            reg_eng = self.get(id)
-            # prompt message if engine is already registered and allow_engine_override is not explicitly set to True
-            if not allow_engine_override:
-                with ConsoleStyle('warn', logging=True) as console:
-                    console.print(f"Engine {id} is already registered. Overriding engine: {reg_eng} with {str(str(engine_instance))}")
-        # debug
-        # else:
-        #     with ConsoleStyle('debug', logging=False) as console:
-        #         console.print(f"Registering engine: {id} >> {str(engine_instance)}")
-        # Create an instance of the engine class and store it
+
         self._engines[id] = engine_instance
 
     @staticmethod
     def register_from_plugin(id: str, plugin: str, selected_engine: Optional[str] = None, args = [], kwargs = {}, allow_engine_override: bool = False, *func_args, **func_kwargs) -> None:
         from .imports import Import
         types = Import.load_module_class(plugin)
         # filter out engine class type
@@ -284,15 +278,15 @@
     def get(engine_name: str, *args, **kwargs) -> Engine:
         self = EngineRepository()
         # try first time load of engine
         if engine_name not in self._engines.keys():
             # get subpackage name from engine name
             subpackage_name = engine_name.replace('-', '_')
             # get subpackage
-            subpackage = subpackage = importlib.import_module(f"{engines.__package__}.{subpackage_name}", None)
+            subpackage = importlib.import_module(f"{engines.__package__}.{subpackage_name}", None)
             # raise exception if subpackage is not found
             if subpackage is None:
                 raise ValueError(f"The symbolicai library does not contain the engine named {engine_name}. Verify your configuration or if you have initialized the respective engine.")
             self._instance.register_from_package(subpackage)
         engine = self._engines.get(engine_name, None)
         # raise exception if engine is not registered
         if engine is None:
```

### Comparing `symbolicai-0.6.1/symai/imports.py` & `symbolicai-0.6.2/symai/imports.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/interfaces.py` & `symbolicai-0.6.2/symai/interfaces.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/memory.py` & `symbolicai-0.6.2/symai/memory.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/menu/screen.py` & `symbolicai-0.6.2/symai/menu/screen.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/misc/console.py` & `symbolicai-0.6.2/symai/misc/console.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/misc/loader.py` & `symbolicai-0.6.2/symai/misc/loader.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/nesy_client.py` & `symbolicai-0.6.2/symai/nesy_client.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/nesy_server.py` & `symbolicai-0.6.2/symai/nesy_server.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/ops/__init__.py` & `symbolicai-0.6.2/symai/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/ops/measures.py` & `symbolicai-0.6.2/symai/ops/measures.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/ops/primitives.py` & `symbolicai-0.6.2/symai/ops/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -2152,14 +2152,15 @@
             ValueError: If the Expression object exceeds the maximum allowed tokens.
         '''
         @core_ext.bind(engine='neurosymbolic', property='max_tokens')
         def _max_tokens(_): pass
 
         max_ctxt_tokens = int(_max_tokens(self) * token_ratio)
         prev = expr(self, preview=True, **kwargs)
+        prev = str(prev)
 
         if len(prev) > _max_tokens(self):
             n_splits = (len(prev) // max_ctxt_tokens) + 1
 
             for i in range(n_splits):
                 tokens_sliced = self.tokens[i * max_ctxt_tokens: (i + 1) * max_ctxt_tokens]
                 r = self._to_symbol(self.tokenizer().decode(tokens_sliced))
@@ -2643,42 +2644,78 @@
 
         Args:
             message (str, optional): The message displayed to request the user input. Defaults to 'Please add more information'.
             **kwargs: Additional keyword arguments to be passed to the `@core.userinput` decorator.
 
         Returns:
             Symbol: The resulting Symbol after receiving the user input.
+
+        Examples:
+        --------
+        >>> from symai import Symbol
+        >>> s = Symbol().input('Please enter your name')
+        >>> [output: 'John']
+
+        >>> s = Symbol('I was born in')
+        >>> s = s.input('Please enter the year of your birth')
+        >>> [output: 'I was born in 1990'] # if Symbol has a <str> value inputs will be concatenated
+
+        # Works identically for the `Expression` class
         '''
         @core.userinput(**kwargs)
         def _func(_, message) -> str:
             pass
-        return self.sym_return_type(_func(self, message))
 
-    def open(self, path: str, **kwargs) -> 'Symbol':
+        res = _func(self, message)
+        condition = self.value is not None and isinstance(self.value, str)
+
+        if hasattr(self, 'sym_return_type'):
+            return self.sym_return_type(self.value if condition else '') | res
+        return self._to_symbol(self.value if condition else '') | self._to_symbol(res)
+
+    def open(self, path: str = None, **kwargs) -> 'Symbol':
         '''
         Open a file and store its content in an Expression object as a string.
 
         Args:
             path (str): The path to the file that needs to be opened.
             **kwargs: Arbitrary keyword arguments to be used by the core.opening decorator.
 
         Returns:
             Symbol: An Expression object containing the content of the file as a string value.
+
+        Examples:
+        --------
+        >>> from symai import Symbol
+        >>> s = Symbol().open('file.txt')
+
+        >>> s = Symbol('file.txt')
+        >>> s = s.open()
+
+        # Works identically for the `Expression` class
         '''
+
+        path = path if path is not None else self.value
+        if path is None:
+            raise ValueError('Path is not provided; either provide a path or set the value of the Symbol to the path')
+
         @core.opening(path=path, **kwargs)
-        def _func(_) -> str:
+        def _func(_):
             pass
-        return self.sym_return_type(_func(self))
+
+        if hasattr(self, 'sym_return_type'):
+            return self.sym_return_type(_func(self))
+        return self._to_symbol(_func(self))
 
 
 class IndexingPrimitives(Primitive):
     '''
     This mixin contains functionalities related to indexing symbols.
     '''
-    def index(self, path: str, index_name: str, **kwargs) -> 'Symbol':
+    def config(self, path: str, index_name: str, **kwargs) -> 'Symbol':
         '''
         Execute a configuration operation on the index.
 
         Args:
             path (str): Index configuration path.
             **kwargs: Arbitrary keyword arguments to be used by the core.index decorator.
```

### Comparing `symbolicai-0.6.1/symai/post_processors.py` & `symbolicai-0.6.2/symai/post_processors.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/pre_processors.py` & `symbolicai-0.6.2/symai/pre_processors.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/processor.py` & `symbolicai-0.6.2/symai/processor.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/prompts.py` & `symbolicai-0.6.2/symai/prompts.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/shell.py` & `symbolicai-0.6.2/symai/shell.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/shellsv.py` & `symbolicai-0.6.2/symai/shellsv.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/strategy.py` & `symbolicai-0.6.2/symai/strategy.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/symbol.py` & `symbolicai-0.6.2/symai/symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,26 @@
         Delete a metadata attribute by name.
 
         Args:
             name (str): The name of the metadata attribute to delete.
         '''
         self.__delattr__(name)
 
+    def __str__(self) -> str:
+        '''
+        Get the string representation of the Symbol's value.
+
+        Returns:
+            str: The string representation of the Symbol's value.
+        '''
+        _val = ''
+        if self.value is not None:
+            _val += str(self.value)
+        return _val + f"Properties({str({k: str(v) for k, v in self.__dict__.items() if not k.startswith('_')})})"
+
     def __repr__(self) -> str:
         '''
         Get the representation of the Symbol object as a string.
 
         Returns:
             str: The representation of the Symbol object.
         '''
@@ -719,15 +731,15 @@
             res (Any): The result of the forward method.
             **kwargs: Arbitrary keyword arguments.
 
         Returns:
             Any: The result of the forward method.
         '''
         # transport results to the root node for global access
-        if not self is self.root:
+        if not self is self.root and not self.metadata.detach:
             ref = self.root.metadata
             if ref.root_link is None:
                 ref.root_link = Linker()
             if ref.root_link.results is None:
                 ref.root_link.results = {}
             prev = None
             if len(ref.root_link.results) > 0:
```

### Comparing `symbolicai-0.6.1/symai/symsh.md` & `symbolicai-0.6.2/symai/symsh.md`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symai/utils.py` & `symbolicai-0.6.2/symai/utils.py`

 * *Files identical despite different names*

### Comparing `symbolicai-0.6.1/symbolicai.egg-info/PKG-INFO` & `symbolicai-0.6.2/symbolicai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: symbolicai
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Neuro-Symbolic Framework for Python
 Author-email: Marius-Constantin Dinu <office@alphacoreai.eu>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, ExtensityAI, a AlphaCore AI e.U. brand.
+        Copyright (c) 2024, ExtensityAI, a AlphaCore AI e.U. brand.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -37,33 +37,95 @@
 Project-URL: GitHub, https://github.com/Xpitfire/symai
 Keywords: symbolic programming,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: setuptools>=67.7.2
+Requires-Dist: toml>=0.10.2
+Requires-Dist: natsort>=8.3.1
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: python-box>=7.0.1
+Requires-Dist: rpyc>=5.3.1
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchaudio>=2.0.1
+Requires-Dist: torchvision>=0.15.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: transformers>=4.30.2
+Requires-Dist: sympy>=1.12
+Requires-Dist: openai>=1.1.0
+Requires-Dist: PyPDF2>=3.0.1
+Requires-Dist: ipython>=8.14.0
+Requires-Dist: accelerate>=0.20.3
+Requires-Dist: sentencepiece>=0.1.99
+Requires-Dist: tiktoken>=0.7.0
+Requires-Dist: tika>=2.6.0
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: GitPython>=3.1.32
+Requires-Dist: pathos>=0.3.1
+Requires-Dist: prompt-toolkit>=3.0.39
+Requires-Dist: pydub
+Requires-Dist: opencv-python
+Requires-Dist: pymongo==3.12.3
+Requires-Dist: pymongo[srv]
+Requires-Dist: requests_toolbelt
+Requires-Dist: pyvis
+Requires-Dist: beartype>=0.17.2
 Provides-Extra: blip2
+Requires-Dist: bitsandbytes>=0.39.1; extra == "blip2"
+Requires-Dist: decord; extra == "blip2"
+Requires-Dist: salesforce-lavis; extra == "blip2"
 Provides-Extra: wolframalpha
+Requires-Dist: wolframalpha>=5.0.0; extra == "wolframalpha"
 Provides-Extra: whisper
+Requires-Dist: openai-whisper>=20231117; extra == "whisper"
 Provides-Extra: selenium
+Requires-Dist: selenium>=4.10.0; extra == "selenium"
+Requires-Dist: webdriver-manager>=4.0.1; extra == "selenium"
+Requires-Dist: chromedriver-autoinstaller>=0.4.0; extra == "selenium"
 Provides-Extra: serpapi
+Requires-Dist: google-search-results>=2.4.2; extra == "serpapi"
 Provides-Extra: pinecone
+Requires-Dist: pinecone-client>=2.2.2; extra == "pinecone"
 Provides-Extra: bard
+Requires-Dist: bardapi>=0.1.24; extra == "bard"
 Provides-Extra: services
+Requires-Dist: fastapi>=0.104.1; extra == "services"
+Requires-Dist: redis>=5.0.1; extra == "services"
+Requires-Dist: uvicorn>=0.24.0.post1; extra == "services"
 Provides-Extra: solver
+Requires-Dist: z3-solver; extra == "solver"
 Provides-Extra: all
-License-File: LICENSE
+Requires-Dist: wolframalpha>=5.0.0; extra == "all"
+Requires-Dist: openai-whisper>=20231117; extra == "all"
+Requires-Dist: selenium>=4.10.0; extra == "all"
+Requires-Dist: webdriver-manager>=4.0.1; extra == "all"
+Requires-Dist: chromedriver-autoinstaller>=0.4.0; extra == "all"
+Requires-Dist: google-search-results>=2.4.2; extra == "all"
+Requires-Dist: pinecone-client>=2.2.2; extra == "all"
+Requires-Dist: fastapi>=0.104.1; extra == "all"
+Requires-Dist: redis>=5.0.1; extra == "all"
+Requires-Dist: uvicorn>=0.24.0.post1; extra == "all"
+Requires-Dist: z3-solver; extra == "all"
 
 # **SymbolicAI**
 <img src="https://raw.githubusercontent.com/ExtensityAI/symbolicai/main/assets/images/symai_logo.png" width="200px">
 
 ## **A Neuro-Symbolic Perspective on Large Language Models (LLMs)**
 
 *Building applications with LLMs at the core using our `Symbolic API` facilitates the integration of classical and differentiable programming in Python.*
 
+Read [**full paper here**](https://arxiv.org/abs/2402.00854).
+
 Read further [**documentation here**](https://symbolicai.readthedocs.io/en/latest/README.html).
 
 [![PyPI version](https://badge.fury.io/py/symbolicai.svg)](https://badge.fury.io/py/symbolicai) [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/dinumariusc.svg?style=social&label=Follow%20%40DinuMariusC)](https://twitter.com/DinuMariusC) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/symbolicapi.svg?style=social&label=Follow%20%40ExtensityAI)](https://twitter.com/ExtensityAI) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ExtensityAI/symbolicai/issues)
 [![Discord](https://img.shields.io/discord/768087161878085643?label=Discord&logo=Discord&logoColor=white)](https://discord.gg/QYMNnh9ra8) [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FXpitfire%2Fsymbolicai&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) [![GitHub forks](https://img.shields.io/github/forks/ExtensityAI/symbolicai.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai) [![GitHub stars](https://img.shields.io/github/stars/ExtensityAI/symbolicai.svg?style=social&label=Star&maxAge=2592000)](https://GitHub.com/ExtensityAI/symbolicai/stargazers/)
 
 
 
@@ -1359,39 +1421,31 @@
 array([[9.72840726e-01, 6.34790864e-03, 2.59368378e-03, 3.41371237e-03,
         3.71197984e-03, 8.53193272e-03, 1.03346225e-04, 2.08464009e-03,
         1.77942711e-04, 1.94185617e-04]], dtype=float32)
 ```
 
 ### Local Neuro-Symbolic Engine
 
-You can use a locally hosted instance for the Neuro-Symbolic Engine. Out of the box, we provide a Hugging Face client-server backend and host the model `openlm-research/open_llama_13b` to perform the inference. As the name suggests, this is a six billion parameter model and requires a GPU with ~16GB RAM to run properly. The following example shows how to host and configure the usage of the local Neuro-Symbolic Engine.
-
-First, we start the backend server:
+You can use a locally hosted instance for the Neuro-Symbolic Engine. We build on top of [llama.cpp](https://github.com/ggerganov/llama.cpp/tree/master) through [llama-cpp-python](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file). Please follow the `llama-cpp-python` installation instructions. We make the assumption the user has experience running `llama.cpp` prior to using our API for local hosting.
 
+For instance, let's suppose you want to set as a Neuro-Symbolic Engine the latest Llama 3 model. Download the model and start the server:
 ```bash
-# optional: set cache folder for transformers (Linux/MacOS)
-export TRANSFORMERS_CACHE="<path-to-cache-folder>"
-# start server backend (default model is openlm-research/open_llama_13b)
-symsvr
-# initialize server with client call
-symclient
+python -m llama_cpp.server --model [your llama.cpp folder]/models/llama-pro-8b-instruct.Q4_K_M.gguf --n_gpu_layers -1 --chat_format llama-3 --port 8000 --host localhost
 ```
 
-Then, use the following code once to set up the local engine:
+Then, in your `symai.config.json` file, set the `NEUROSYMBOLIC_ENGINE_API_KEY` to `http://localhost:8000` (following the `--port` and `--host` you set in the previous step) and `NEUROSYMBOLIC_ENGINE_MODEL` to `llama.cpp`.
 
-```python
-from symai.backend.engines.neurosymbolic.engine_nesy_client import NeSyClientEngine
-from symai.functional import EngineRepository
-# setup local engine
-engine = NeSyClientEngine()
-EngineRepository.register('neurosymbolic', engine)
+```json
+{
+  "NEUROSYMBOLIC_ENGINE_API_KEY": "http://localhost:8000",
+  "NEUROSYMBOLIC_ENGINE_MODEL": "llama.cpp"
+}
 ```
+Now you are set to use the local engine.
 
-
-Now you can use the local engine to perform symbolic computation:
 ```python
 # do some symbolic computation with the local engine
 sym = Symbol('cats are cute')
 res = sym.compose()
 ...
 ```
 
@@ -1565,15 +1619,15 @@
 * We view operators/methods as being able to move along a spectrum between prompting and fine-tuning, based on task-specific requirements and data availability. We believe this approach is more general compared to prompting frameworks.
 * We propose a general method for handling large context sizes and transforming a data stream problem into a search problem, related to **reasoning as a search problem** in [Search and Reasoning in Problem Solving](https://www.sciencedirect.com/science/article/abs/pii/S0004370283800034).
 
 We hope that our work can be seen as complementary and offer a future outlook on how we would like to use machine learning models as an integral part of programming languages and their entire computational stack.
 
 ### Acknowledgements
 
-We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback; and to [Dynatrace Research](https://engineering.dynatrace.com/research/) for supporting this project. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community). Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
+We have a long list of acknowledgements. Special thanks go to our colleagues and friends at the [Institute for Machine Learning at Johannes Kepler University (JKU), Linz](https://www.jku.at/institut-fuer-machine-learning/) for their exceptional support and feedback. We are also grateful to the [AI Austria RL Community](https://aiaustria.com/rl-community) for supporting this project. Additionally, we appreciate all contributors to this project, regardless of whether they provided feedback, bug reports, code, or simply used the framework. Your support is highly valued.
 
 Finally, we would like to thank the open-source community for making their APIs and tools publicly available, including (but not limited to) [PyTorch](https://pytorch.org/), [Hugging Face](https://huggingface.co/), [OpenAI](https://openai.com/), [GitHub](https://github.com/), [Microsoft Research](https://www.microsoft.com/en-us/research/), and many others.
 
 Special thanks are owed to [Kajetan Schweighofer](https://www.linkedin.com/in/kajetan-schweighofer-a61113202/?originalSubdomain=at), [Markus Hofmarcher](https://www.linkedin.com/in/markus-hofmarcher-2722141b8/?originalSubdomain=at), [Thomas Natschläger](https://www.linkedin.com/in/thomas-natschlaeger/?originalSubdomain=at), and [Sepp Hochreiter](https://scholar.google.at/citations?user=tvUH3WMAAAAJ&hl=en).
 
 ### Contribution
```

### Comparing `symbolicai-0.6.1/symbolicai.egg-info/SOURCES.txt` & `symbolicai-0.6.2/symbolicai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 environment.yml
 index.rst
 modules.rst
 pyproject.toml
 setup.py
 trusted_repos.yml
 .github/FUNDING.yml
+.symai/symsh.config.json
 assets/images/cat.jpg
 assets/images/img1.png
 assets/images/img10.png
 assets/images/img2.png
 assets/images/img3.png
 assets/images/img4.png
 assets/images/img5.png
@@ -107,15 +108,14 @@
 symai/backend/engines/index/engine_vectordb.py
 symai/backend/engines/neurosymbolic/engine_nesy_client.py
 symai/backend/engines/neurosymbolic/engine_openai_gptX_chat.py
 symai/backend/engines/neurosymbolic/engine_openai_gptX_completion.py
 symai/backend/engines/ocr/engine_apilayer.py
 symai/backend/engines/output/engine_stdout.py
 symai/backend/engines/search/engine_serpapi.py
-symai/backend/engines/speech_to_text/engine_whisper.py
 symai/backend/engines/symbolic/engine_wolframalpha.py
 symai/backend/engines/text_to_speech/engine_openai.py
 symai/backend/engines/text_vision/engine_clip.py
 symai/backend/engines/userinput/engine_console.py
 symai/backend/mixin/__init__.py
 symai/backend/mixin/openai.py
 symai/backend/mixin/tracker.py
@@ -192,11 +192,8 @@
 symai/ops/measures.py
 symai/ops/primitives.py
 symbolicai.egg-info/PKG-INFO
 symbolicai.egg-info/SOURCES.txt
 symbolicai.egg-info/dependency_links.txt
 symbolicai.egg-info/entry_points.txt
 symbolicai.egg-info/requires.txt
-symbolicai.egg-info/top_level.txt
-tests/scripts/download_models.py
-tests/scripts/evaluation.py
-tests/scripts/single_run.py
+symbolicai.egg-info/top_level.txt
```

### Comparing `symbolicai-0.6.1/symbolicai.egg-info/requires.txt` & `symbolicai-0.6.2/symbolicai.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,32 @@
 transformers>=4.30.2
 sympy>=1.12
 openai>=1.1.0
 PyPDF2>=3.0.1
 ipython>=8.14.0
 accelerate>=0.20.3
 sentencepiece>=0.1.99
-tiktoken>=0.3.3
+tiktoken>=0.7.0
 tika>=2.6.0
 beautifulsoup4>=4.12.2
 colorama>=0.4.6
 GitPython>=3.1.32
 pathos>=0.3.1
 prompt-toolkit>=3.0.39
 pydub
 opencv-python
 pymongo==3.12.3
 pymongo[srv]
 requests_toolbelt
 pyvis
+beartype>=0.17.2
 
 [all]
 wolframalpha>=5.0.0
-openai-whisper
+openai-whisper>=20231117
 selenium>=4.10.0
 webdriver-manager>=4.0.1
 chromedriver-autoinstaller>=0.4.0
 google-search-results>=2.4.2
 pinecone-client>=2.2.2
 fastapi>=0.104.1
 redis>=5.0.1
@@ -69,11 +70,11 @@
 redis>=5.0.1
 uvicorn>=0.24.0.post1
 
 [solver]
 z3-solver
 
 [whisper]
-openai-whisper
+openai-whisper>=20231117
 
 [wolframalpha]
 wolframalpha>=5.0.0
```

### Comparing `symbolicai-0.6.1/trusted_repos.yml` & `symbolicai-0.6.2/trusted_repos.yml`

 * *Files identical despite different names*

