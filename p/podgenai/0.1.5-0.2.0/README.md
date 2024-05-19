# Comparing `tmp/podgenai-0.1.5.tar.gz` & `tmp/podgenai-0.2.0.tar.gz`

## Comparing `podgenai-0.1.5.tar` & `podgenai-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 podgenai-0.1.5/.python-version
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.5/requirements-dev.lock
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.5/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/__main__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/config.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/exceptions.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/podgenai.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/work.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/audio.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/subtopics.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/topic.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/tts.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/voice.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/continuation_first.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/continuation_next.txt
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/generate_subtopic.txt
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/list_subtopics.txt
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/select_voice.txt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/tts_disclaimer.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/binascii.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/input.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/openai.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/semantic_text_splitter.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/sys.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.1.5/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.1.5/LICENSE
--rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 podgenai-0.1.5/README.md
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 podgenai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 podgenai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 podgenai-0.2.0/.python-version
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.2.0/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/__main__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/config.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/exceptions.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/podgenai.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/work.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/content/audio.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/content/subtopics.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/content/topic.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/content/tts.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/content/voice.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/continuation_first.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/continuation_next.txt
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/generate_subtopic.txt
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/list_subtopics.txt
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/select_voice.txt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/prompts/tts_disclaimer.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/util/binascii.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/util/input.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/util/openai.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/util/semantic_text_splitter.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.2.0/src/podgenai/util/sys.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.2.0/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.2.0/LICENSE
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 podgenai-0.2.0/README.md
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 podgenai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 podgenai-0.2.0/PKG-INFO
```

### Comparing `podgenai-0.1.5/requirements-dev.lock` & `podgenai-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/requirements.lock` & `podgenai-0.2.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/__main__.py` & `podgenai-0.2.0/src/podgenai/__main__.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/config.py` & `podgenai-0.2.0/src/podgenai/config.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/podgenai.py` & `podgenai-0.2.0/src/podgenai/podgenai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/work.py` & `podgenai-0.2.0/src/podgenai/work.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/content/audio.py` & `podgenai-0.2.0/src/podgenai/content/audio.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/content/subtopics.py` & `podgenai-0.2.0/src/podgenai/content/subtopics.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/content/topic.py` & `podgenai-0.2.0/src/podgenai/content/topic.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/content/tts.py` & `podgenai-0.2.0/src/podgenai/content/tts.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/content/voice.py` & `podgenai-0.2.0/src/podgenai/content/voice.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/prompts/generate_subtopic.txt` & `podgenai-0.2.0/src/podgenai/prompts/generate_subtopic.txt`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/prompts/list_subtopics.txt` & `podgenai-0.2.0/src/podgenai/prompts/list_subtopics.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Produce a list of contiguously numbered points for a lengthy 1-hour long audiobook podcast episode on the given topic. Do not provide a nested hierarchy of points; emit only a flattened single-level instead of a hierarchy, even if it means duplicating a few words. Accordingly, do not emit any bullet points either. Moreover, each numbered point must be a relevant self-sufficient subtopic of the given topic. Being factual is of course important, so list only the subtopics you actually know to be well-documented, eschewing unverified ones, even if this means that the podcast will be smaller. In case you have nothing at all, just say "None."
 
 Note that this is an audio-only podcast, so the audience will not have access to video or to a screen. For technical topics, avoid software code and fancy mathematical equations as they are hard to vocalize. Also note that the audience is a mixed audience with an interest in the topic, operating at a variety of skill levels (student / junior / mid / senior). The audience relies on the podcast to learn skills to earn their living, so they must learn everything that they need to know; their interest is both academic and pragmatic. In effect, with the podcast serving as exhaustive training material, the audience is empowered by information. Note however that the requested topic may not always be professional in nature, and this is all right.
 
-You do not need to cover any prerequisite or foundational topics because they would be covered in a different podcast, so please skip them, and focus exclusively on the given topic. Do not otherwise comment on the task in any way because your response will be parsed by a machine.
+You do not need to cover any prerequisite or foundational topics because they would be covered in a different podcast, so please skip them, and focus exclusively on the given topic. Avoid fluff or filler content. Do not otherwise comment on the task in any way because your response will be parsed by a machine.
 
 For your information, in a subsequent step, I will ask you to generate the corresponding text for each of the listed subtopic points, one point at a time. As such, it would help for each of the points you list to exclusively be those that you can subsequently expound upon at significant length.
 
 The topic for the podcast is:
 
 {topic}
```

### Comparing `podgenai-0.1.5/src/podgenai/util/input.py` & `podgenai-0.2.0/src/podgenai/util/input.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/src/podgenai/util/openai.py` & `podgenai-0.2.0/src/podgenai/util/openai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/.gitignore` & `podgenai-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/LICENSE` & `podgenai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.5/README.md` & `podgenai-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # podgenai
 **podgenai** is a Python 3.12 application to generate approximately an hour-long informational single-speaker audiobook/podcast mp3 file on a given topic using the GPT-4 LLM. A funded [OpenAI API key](https://platform.openai.com/api-keys) is required.
 
+## Links
+| Caption     | Link                                               |
+|-------------|----------------------------------------------------|
+| Repo        | https://github.com/impredicative/podgenai          |
+| Changelog   | https://github.com/impredicative/podgenai/releases |
+| Package     | https://pypi.org/project/podgenai/                 |
+| Podcast     | https://podcasters.spotify.com/pod/podgenai        |
+| Podcast RSS | https://anchor.fm/s/f4868644/podcast/rss           |
+
 ## Approach
 The `gpt-4-0125-preview` and `tts-1` models are used. For a given topic, the high-level reference approach is:
 
 * Applicable subtopics are listed using the LLM. If however the topic is unknown to the LLM, the process is aborted.
 * The voice is selected using the LLM from four choices.
 * Concurrently for each subtopic, the corresponding text and speech are generated using the LLM and TTS respectively.
 * The speech files are concatenated using `ffmpeg`.
```

### Comparing `podgenai-0.1.5/pyproject.toml` & `podgenai-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "podgenai"
-version = "0.1.5"
+version = "0.2.0"
 description = "GPT-4 based informational audiobook/podcast mp3 generator"
 authors = [
     { name = "Ouroboros Chrysopoeia", email = "impredicative@users.noreply.github.com" }
 ]
 dependencies = [
     "fire>=0.6.0",
     "openai>=1.27.0",
```

### Comparing `podgenai-0.1.5/PKG-INFO` & `podgenai-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: podgenai
-Version: 0.1.5
+Version: 0.2.0
 Summary: GPT-4 based informational audiobook/podcast mp3 generator
 Project-URL: Repository, https://github.com/impredicative/podgenai
 Author-email: Ouroboros Chrysopoeia <impredicative@users.noreply.github.com>
 License-File: LICENSE
 Keywords: GPT-4,aicast,audiobook,mp3,podcast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -18,14 +18,23 @@
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: semantic-text-splitter>=0.13.1
 Description-Content-Type: text/markdown
 
 # podgenai
 **podgenai** is a Python 3.12 application to generate approximately an hour-long informational single-speaker audiobook/podcast mp3 file on a given topic using the GPT-4 LLM. A funded [OpenAI API key](https://platform.openai.com/api-keys) is required.
 
+## Links
+| Caption     | Link                                               |
+|-------------|----------------------------------------------------|
+| Repo        | https://github.com/impredicative/podgenai          |
+| Changelog   | https://github.com/impredicative/podgenai/releases |
+| Package     | https://pypi.org/project/podgenai/                 |
+| Podcast     | https://podcasters.spotify.com/pod/podgenai        |
+| Podcast RSS | https://anchor.fm/s/f4868644/podcast/rss           |
+
 ## Approach
 The `gpt-4-0125-preview` and `tts-1` models are used. For a given topic, the high-level reference approach is:
 
 * Applicable subtopics are listed using the LLM. If however the topic is unknown to the LLM, the process is aborted.
 * The voice is selected using the LLM from four choices.
 * Concurrently for each subtopic, the corresponding text and speech are generated using the LLM and TTS respectively.
 * The speech files are concatenated using `ffmpeg`.
```

