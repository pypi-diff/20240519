# Comparing `tmp/article_to_podcast-0.1.6.tar.gz` & `tmp/article_to_podcast-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_to_podcast-0.1.6.tar", last modified: Wed May 15 06:08:28 2024, max compression
+gzip compressed data, was "article_to_podcast-0.1.9.tar", last modified: Wed May 15 09:32:44 2024, max compression
```

## Comparing `article_to_podcast-0.1.6.tar` & `article_to_podcast-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.261960 article_to_podcast-0.1.6/article_to_podcast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/article_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/article_to_podcast/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/article_to_podcast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 06:08:28.000000 article_to_podcast-0.1.6/article_to_podcast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:08:28.265960 article_to_podcast-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-15 06:08:06.000000 article_to_podcast-0.1.6/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/article_to_podcast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/article_to_podcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/article_to_podcast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/article_to_podcast/article_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/article_to_podcast/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/article_to_podcast/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/article_to_podcast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 09:32:44.000000 article_to_podcast-0.1.9/article_to_podcast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:32:44.041484 article_to_podcast-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-15 09:32:33.000000 article_to_podcast-0.1.9/tests/test_main.py
```

### Comparing `article_to_podcast-0.1.6/LICENSE.md` & `article_to_podcast-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `article_to_podcast-0.1.6/PKG-INFO` & `article_to_podcast-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-to-podcast
-Version: 0.1.6
+Version: 0.1.9
 Summary: CLI tool for converting articles to podcasts
 Author: Ivan Kovnatsky
 License: MIT
 Project-URL: Homepage, https://github.com/ivankovnatsky/article-to-podcast
 Project-URL: Changelog, https://github.com/ivankovnatsky/article-to-podcast/releases
 Project-URL: Issues, https://github.com/ivankovnatsky/article-to-podcast/issues
 Project-URL: CI, https://github.com/ivankovnatsky/article-to-podcast/actions
@@ -22,21 +22,25 @@
 Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cogapp; extra == "test"
 
 # Article to Podcast
 
-[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
+[![PyPI](https://img.shields.io/pypi/v/article-to-podcast.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
 [![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
+## Requirements
+
+You need to have ffmpeg install before running this CLI tool.
+
 ## Usage
 
 Install article-to-podcast with:
 
 ```console
 pipx install article-to-podcast
 ```
```

### Comparing `article_to_podcast-0.1.6/README.md` & `article_to_podcast-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Article to Podcast
 
-[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
+[![PyPI](https://img.shields.io/pypi/v/article-to-podcast.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
 [![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
+## Requirements
+
+You need to have ffmpeg install before running this CLI tool.
+
 ## Usage
 
 Install article-to-podcast with:
 
 ```console
 pipx install article-to-podcast
 ```
```

### Comparing `article_to_podcast-0.1.6/article_to_podcast/cli.py` & `article_to_podcast-0.1.9/article_to_podcast/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,25 @@
     fable:   A narrative and storytelling voice.
     onyx:    A deep and resonant voice.
     nova:    A bright and energetic voice.
     shimmer: A soft and soothing voice.
     Experiment with different voices to find one that matches your desired tone and audience. The current voices are optimized for English.
     """,
 )
-def cli(url, directory, audio_format, model, voice):
+@click.option(
+    "--shrink",
+    type=click.IntRange(0, 100),
+    default=100,
+    help="Percentage of the text to process. 0-100%. Default is 100%.",
+)
+def cli(url, directory, audio_format, model, voice, shrink):
     text, title = get_article_content(url)
-    filename = format_filename(title, audio_format)
-    filepath = Path(directory) / filename
-    process_article(text, str(filepath), model, voice)
+
+    if shrink < 100:
+        end_idx = len(text) * shrink // 100
+        text = text[:end_idx]  # Limit the text based on the percentage
+    filename = Path(directory) / f"{format_filename(title, audio_format)}"
+    process_article(text, filename, model, voice)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `article_to_podcast-0.1.6/article_to_podcast/main.py` & `article_to_podcast-0.1.9/article_to_podcast/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import io
 from pathlib import Path
 from openai import OpenAI
 from pydub import AudioSegment
 
 TEXT_SEND_LIMIT = 4096  # Constant for the text limit
```

### Comparing `article_to_podcast-0.1.6/article_to_podcast.egg-info/PKG-INFO` & `article_to_podcast-0.1.9/article_to_podcast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-to-podcast
-Version: 0.1.6
+Version: 0.1.9
 Summary: CLI tool for converting articles to podcasts
 Author: Ivan Kovnatsky
 License: MIT
 Project-URL: Homepage, https://github.com/ivankovnatsky/article-to-podcast
 Project-URL: Changelog, https://github.com/ivankovnatsky/article-to-podcast/releases
 Project-URL: Issues, https://github.com/ivankovnatsky/article-to-podcast/issues
 Project-URL: CI, https://github.com/ivankovnatsky/article-to-podcast/actions
@@ -22,21 +22,25 @@
 Requires-Dist: lxml[html_clean]
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: cogapp; extra == "test"
 
 # Article to Podcast
 
-[![PyPI](https://img.shields.io/pypi/v/ospeak.svg)](https://pypi.org/project/article-to-podcast/)
+[![PyPI](https://img.shields.io/pypi/v/article-to-podcast.svg)](https://pypi.org/project/article-to-podcast/)
 [![Changelog](https://img.shields.io/github/release/ivankovnatsky/article-to-podcast.svg)](https://github.com/ivankovnatsky/article-to-podcast/releases)
 [![Tests](https://github.com/ivankovnatsky/article-to-podcast/workflows/Test/badge.svg)](https://github.com/ivankovnatsky/article-to-podcast/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/github/license/ivankovnatsky/article-to-podcast)](https://github.com/ivankovnatsky/article-to-podcast/blob/main/LICENSE.md)
 
 CLI tool for converting articles to podcasts using OpenAI's Text-to-Speech API.
 
+## Requirements
+
+You need to have ffmpeg install before running this CLI tool.
+
 ## Usage
 
 Install article-to-podcast with:
 
 ```console
 pipx install article-to-podcast
 ```
```

### Comparing `article_to_podcast-0.1.6/pyproject.toml` & `article_to_podcast-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "article-to-podcast"
-version = "0.1.6"
+version = "0.1.9"
 description = "CLI tool for converting articles to podcasts"
 readme = "README.md"
 authors = [{name = "Ivan Kovnatsky"}]
 license = {text = "MIT"}
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License"
```

### Comparing `article_to_podcast-0.1.6/tests/test_main.py` & `article_to_podcast-0.1.9/tests/test_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from click.testing import CliRunner
 from article_to_podcast.cli import cli
 from article_to_podcast.main import TEXT_SEND_LIMIT, split_text
 from article_to_podcast.article_fetcher import get_article_content
 from pathlib import Path
-import pytest
 
 ARTICLE_URL = "https://blog.kubetools.io/kopylot-an-ai-powered-kubernetes-assistant-for-devops-developers/"
 
 
 def test_split_text():
     text = "This is a test text. " * 300  # Creating a long text to ensure it gets split
     chunks = split_text(text)
@@ -38,29 +37,21 @@
             "/tmp",
             "--audio-format",
             "mp3",
             "--model",
             "tts-1",
             "--voice",
             "alloy",
+            "--shrink",
+            "1",  # Use 5% of the text to reduce costs during testing
         ],
         catch_exceptions=False,  # Allow exceptions to propagate
     )
 
-    if result.exception:
-        print(f"Exception: {result.exception}")
-        import traceback
-
-        traceback.print_exception(
-            type(result.exception), result.exception, result.exception.__traceback__
-        )
-
-    # Ensure test fails if there's an exception
-    assert result.exception is None or "429" in str(result.exception)
-
-    output_audio_paths = list(Path("/tmp").glob("*.mp3"))
-    if output_audio_paths:
-        for output_audio_path in output_audio_paths:
-            assert not output_audio_path.exists()  # Ensure no partial files are saved
-            # Clean up
-            if output_audio_path.exists():
-                output_audio_path.unlink()
+    assert result.exit_code == 0
+    output_audio_path = list(Path("/tmp").glob("*.mp3"))[
+        0
+    ]  # Find the generated audio file
+    assert output_audio_path.exists()
+
+    # Clean up
+    # output_audio_path.unlink()
```

