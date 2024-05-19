# Comparing `tmp/ragdaemon-0.5.0.tar.gz` & `tmp/ragdaemon-0.5.1.tar.gz`

## Comparing `ragdaemon-0.5.0.tar` & `ragdaemon-0.5.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0  1670456 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/app.py
--rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/context.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/locate.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0  1671121 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/app.py
+-rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/context.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/PKG-INFO
```

### Comparing `ragdaemon-0.5.0/scratch.ipynb` & `ragdaemon-0.5.1/scratch.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950418526785714%*

 * *Differences: {"'cells'": "{0: {'outputs': {2: {'text': {delete: [5, 4, 3, 2, 1, 0]}}, insert: [(0, "*

 * *            "OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', ['Initialized "*

 * *            'empty graph.\\n\', "Initializing annotators: [\'hierarchy\', \'chunker_llm\', '*

 * *            '\'call_graph\', \'diff\']...\\n", \'No Chroma HTTP client environment variables '*

 * *            "found. Defaulting to PersistentClient.\\n'])])), (1, OrderedDict([('name', 'stderr'), "*

 * *            "('output_type', 'stream' […]*

```diff
@@ -6,62 +6,97 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Initialized empty graph.\n",
-                        "Initializing annotators: ['hierarchy', 'chunker_llm', 'diff']...\n",
-                        "No parent node found for mentat/terminal/terminal_app.py:ContextContainer.update_context\n",
-                        "No parent node found for mentat/terminal/terminal_app.py:ContextContainer._build_sub_tree\n",
-                        "No parent node found for mentat/terminal/terminal_app.py:ContextContainer._build_path_tree\n",
-                        "No parent node found for mentat/terminal/terminal_app.py:ContextContainer._build_tree_widget\n",
+                        "Initializing annotators: ['hierarchy', 'chunker_llm', 'call_graph', 'diff']...\n",
+                        "No Chroma HTTP client environment variables found. Defaulting to PersistentClient.\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Chunking files...: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:01<00:00,  1.51s/it]\n",
+                        "Add of existing embedding ID: d3b64d9038fefc0fdcf43f32f48155ee\n",
+                        "Add of existing embedding ID: d6b3356e068d4ff7b6194987ba9a2ad3\n",
+                        "Add of existing embedding ID: 8b39ed49247c340ee68d75e5646ad741\n",
+                        "Add of existing embedding ID: fda570604098a162aa3cee2c5521582e\n",
+                        "Insert of existing embedding ID: d3b64d9038fefc0fdcf43f32f48155ee\n",
+                        "Insert of existing embedding ID: d6b3356e068d4ff7b6194987ba9a2ad3\n",
+                        "Insert of existing embedding ID: 8b39ed49247c340ee68d75e5646ad741\n",
+                        "Insert of existing embedding ID: fda570604098a162aa3cee2c5521582e\n",
+                        "Generating call graph: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00,  1.52it/s]"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
                         "Saved updated graph to /Users/granthawkins/.mentat/ragdaemon/ragdaemon-mentat.json\n"
                     ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
                 }
             ],
             "source": [
                 "from pathlib import Path\n",
                 "from ragdaemon.daemon import Daemon\n",
                 "\n",
                 "annotators = {\n",
                 "    \"hierarchy\": {},\n",
                 "    \"chunker_llm\": {},\n",
-                "    # \"call_graph\": {},\n",
+                "    \"call_graph\": {},\n",
                 "    # \"summarizer\": {},\n",
                 "    \"diff\": {},\n",
                 "}\n",
                 "\n",
                 "sample_dir = Path.home() / \"mentat\"\n",
                 "daemon = Daemon(\n",
                 "    sample_dir, \n",
                 "    annotators=annotators, \n",
                 "    verbose=True\n",
                 ")\n",
-                "await daemon.update()"
+                "await daemon.update(refresh=\"mentat/__main__.py\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'Develop and maintain the Mentat AI tool, which assists with coding tasks from the command line. Utilize the `mentat` directory to implement the core functionalities, including code context management, command-line interfaces, and version tracking. Extend capabilities to VSCode through the `mentat-vscode` directory. Benchmark performance and quality using a comprehensive set of scripts and tools in the `benchmarks` directory. Document and support the project with extensive guides and configurations located in the `docs` directory. Automate tests across the codebase with numerous test files in the `tests` directory and validate different aspects using the `testbed` directory. Define installation and configuration settings with files like `setup.py`, `requirements.txt`, and `pyproject.toml`. Facilitate community contributions and maintain CI/CD processes through guidelines and workflows in the `.github` directory.'"
+                            "{'id': 'mentat-vscode/src/webviews/context/WorkspaceRootContext.tsx',\n",
+                            " 'type': 'file',\n",
+                            " 'ref': 'mentat-vscode/src/webviews/context/WorkspaceRootContext.tsx',\n",
+                            " 'document': 'mentat-vscode/src/webviews/context/WorkspaceRootContext.tsx\\nimport { createContext } from \"react\";\\n\\nconst WorkspaceRootContext = createContext(\"\");\\nexport { WorkspaceRootContext };\\n',\n",
+                            " 'checksum': '3bdf225069530c9c50fe4004ebe78e59',\n",
+                            " 'active': False,\n",
+                            " 'calls': '{}',\n",
+                            " 'chunks_llm': [],\n",
+                            " 'summary': 'Create and export a React context named `WorkspaceRootContext`, initialized with an empty string.',\n",
+                            " 'summary_checksum': 'b06f596db3d940ad388a17f2b0b73899'}"
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "daemon.graph.nodes[\"ROOT\"][\"summary\"]"
+                "daemon.graph.nodes[\"mentat-vscode/src/webviews/context/WorkspaceRootContext.tsx\"]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
```

### Comparing `ragdaemon-0.5.0/tutorial.ipynb` & `ragdaemon-0.5.1/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/.github/workflows/run-tests.yml` & `ragdaemon-0.5.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/app.py` & `ragdaemon-0.5.1/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/context.py` & `ragdaemon-0.5.1/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/daemon.py` & `ragdaemon-0.5.1/ragdaemon/daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ragdaemon.annotators import annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.locate import locate
-from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, mentat_dir_path
+from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, mentat_dir_path, match_refresh
 
 
 def default_annotators():
     return {
         "hierarchy": {},
         "chunker_line": {"lines_per_chunk": 30},
         "diff": {},
@@ -99,20 +99,31 @@
         """Saves the graph to disk."""
         data = json_graph.node_link_data(self.graph)
         with open(self.graph_path, "w") as f:
             json.dump(data, f, indent=4)
         if self.verbose:
             print(f"Saved updated graph to {self.graph_path}")
 
-    async def update(self, refresh=False):
-        """Iteratively build the knowledge graph"""
+    async def update(self, refresh: str | bool = False):
+        """Iteratively build the knowledge graph
+
+        Refresh can be
+        - boolean to refresh all annotators/nodes
+        - string matching annotator names / node ids, e.g. ("chunker_llm")
+        - string with wildcard operators to fuzzy-match annotators/nodes, e.g. ("*diff*")
+        """
         _graph = self.graph.copy()
-        for annotator in self.pipeline.values():
-            if refresh or not annotator.is_complete(_graph, self.db):
-                _graph = await annotator.annotate(_graph, self.db, refresh=refresh)
+        for name, annotator in self.pipeline.items():
+            _refresh = (
+                match_refresh(refresh, name)
+                if isinstance(refresh, str) and refresh in self.pipeline
+                else refresh
+            )
+            if _refresh or not annotator.is_complete(_graph, self.db):
+                _graph = await annotator.annotate(_graph, self.db, refresh=_refresh)
         self.graph = _graph
         self.save()
 
     async def watch(self, interval=2, debounce=5):
         """Calls self.update interval debounce seconds after a file is modified."""
         paths = get_paths_for_directory(self.cwd)
         last_updated = 0
```

### Comparing `ragdaemon-0.5.0/ragdaemon/get_paths.py` & `ragdaemon-0.5.1/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/graph.py` & `ragdaemon-0.5.1/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/locate.py` & `ragdaemon-0.5.1/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/utils.py` & `ragdaemon-0.5.1/ragdaemon/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -184,7 +184,23 @@
                 refs.append(f"{start}-{end}")
             start = end = i
     if start == end:
         refs.append(str(start))
     else:
         refs.append(f"{start}-{end}")
     return ",".join(refs)
+
+
+def match_refresh(refresh: str | bool, target: str) -> bool:
+    if isinstance(refresh, bool):
+        return refresh
+
+    front_wildcard = refresh.startswith("*")
+    back_wildcard = refresh.endswith("*")
+    if front_wildcard and back_wildcard:
+        return refresh[1:-1] in target
+    elif front_wildcard:
+        return target.endswith(refresh[1:])
+    elif back_wildcard:
+        return target.startswith(refresh[:-1])
+    else:
+        return refresh == target
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/__init__.py` & `ragdaemon-0.5.1/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.5.1/ragdaemon/annotators/base_annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         self.spice_client = spice_client
         pass
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         raise NotImplementedError()
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         raise NotImplementedError()
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.5.1/ragdaemon/annotators/call_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database, remove_update_db_duplicates
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import (
     DEFAULT_CODE_EXTENSIONS,
     DEFAULT_COMPLETION_MODEL,
+    match_refresh,
     parse_path_ref,
     semaphore,
 )
 
 
 class CallGraph(Annotator):
     name = "call_graph"
@@ -181,15 +182,15 @@
                             if i > 1
                             else "Skipping."
                         )
 
         data[self.call_field_id] = calls
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         # Remove any existing call edges
         graph.remove_edges_from(
             [edge for edge in graph.edges(data=True) if edge[-1].get("type") == "call"]
         )
         # Get the list of nodes expected to have calls data
         files_with_calls = list[tuple[str, dict[str, Any]]]()
@@ -204,15 +205,18 @@
                 extension = Path(data["ref"]).suffix
                 if extension in self.call_extensions:
                     files_with_calls.append((node, data))
         # Generate/add call data for nodes that don't have it
         tasks = []
         files_just_updated = set()
         for node, data in files_with_calls:
-            if refresh or data.get(self.call_field_id, None) is None:
+            if (
+                match_refresh(refresh, node)
+                or data.get(self.call_field_id, None) is None
+            ):
                 checksum = data.get("checksum")
                 if checksum is None:
                     raise RagdaemonError(f"Node {node} has no checksum.")
                 tasks.append(self.get_file_call_data(node, data, graph))
                 files_just_updated.add(node)
         if len(tasks) > 0:
             if self.verbose:
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/chunker.py` & `ragdaemon-0.5.1/ragdaemon/annotators/chunker.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,40 @@
 from ragdaemon.database import (
     Database,
     remove_add_to_db_duplicates,
     remove_update_db_duplicates,
 )
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.graph import KnowledgeGraph
-from ragdaemon.utils import DEFAULT_CODE_EXTENSIONS, get_document, hash_str, truncate
+from ragdaemon.utils import (
+    DEFAULT_CODE_EXTENSIONS,
+    get_document,
+    hash_str,
+    match_refresh,
+    truncate,
+)
+
+
+def resolve_chunk_parent(id: str, nodes: set[str]) -> str | None:
+    file, chunk_str = id.split(":")
+    if chunk_str == "BASE":
+        return file
+    elif "." not in chunk_str:
+        return f"{file}:BASE"
+    else:
+        parts = chunk_str.split(".")
+        while True:
+            parent = f"{file}:{'.'.join(parts[:-1])}"
+            if parent in nodes:
+                return parent
+            parent_str = parent.split(":")[1]
+            if "." not in parent_str:
+                return None
+            # If intermediate parents are missing, skip them
+            parts = parent_str.split(".")
 
 
 class Chunker(Annotator):
     name = "chunker"
     chunk_field_id = "chunks"
 
     def __init__(self, *args, chunk_extensions: Optional[list[str]] = None, **kwargs):
@@ -78,15 +103,15 @@
             if self.verbose:
                 print(f"Error chunking {node}; skipping.")
             chunks = []
         chunks = sorted(chunks, key=lambda x: len(x["id"]))
         data[self.chunk_field_id] = chunks
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         # Select file nodes and remove all existing chunk nodes from graph.
         files_with_chunks = []
         all_nodes = list(graph.nodes(data=True))
         for node, data in all_nodes:
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
@@ -100,15 +125,18 @@
                     if extension in self.chunk_extensions:
                         files_with_chunks.append((node, data))
 
         # Generate/add chunk data for nodes that don't have it
         tasks = []
         files_just_chunked = set()
         for node, data in files_with_chunks:
-            if refresh or data.get(self.chunk_field_id, None) is None:
+            if (
+                match_refresh(refresh, node)
+                or data.get(self.chunk_field_id, None) is None
+            ):
                 tasks.append(self.get_file_chunk_data(node, data))
                 files_just_chunked.add(node)
             elif isinstance(data[self.chunk_field_id], str):
                 data[self.chunk_field_id] = json.loads(data[self.chunk_field_id])
         if len(tasks) > 0:
             if self.verbose:
                 await tqdm.gather(*tasks, desc="Chunking files...")
@@ -147,41 +175,27 @@
                     "type": "chunk",
                     "document": document,
                     "checksum": hash_str(document),
                     "active": False,
                 }
                 graph.add_node(id, **chunk_data)
                 all_chunk_ids.add(id)
-                # Locate the parent and add hierarchy edge
-                chunk_str = id.split(":")[1]
-                if chunk_str == "BASE":
-                    parent = file
-                elif "." not in chunk_str:
-                    parent = base_id
-                else:
-                    parts = chunk_str.split(".")
-                    while True:
-                        parent = f"{file}:{'.'.join(parts[:-1])}"
-                        if parent in graph:
-                            break
-                        parent_str = parent.split(":")[1]
-                        if "." not in parent_str:
-                            # If we can't find a parent, use the base node.
-                            if self.verbose:
-                                print(f"No parent node found for {id}")
-                            parent = base_id
-                            break
-                        # If intermediate parents are missing, skip them
-                        parts = parent_str.split(".")
+
+                all_nodes = set(graph.nodes)
+                parent = resolve_chunk_parent(id, all_nodes)
+                if parent is None:
+                    if self.verbose:
+                        print(f"No parent node found for {id}")
+                    parent = f"{file}:BASE"
                 graph.add_edge(parent, id, type="hierarchy")
 
         # 2. Get metadata for all chunks from db
-        all_chunk_checksums = [
-            graph.nodes[chunk]["checksum"] for chunk in all_chunk_ids
-        ]
+        all_chunk_checksums = list(
+            set(graph.nodes[chunk]["checksum"] for chunk in all_chunk_ids)
+        )
         response = db.get(ids=all_chunk_checksums, include=["metadatas"])
         db_data = {data["id"]: data for data in response["metadatas"]}
         add_to_db = {"ids": [], "documents": [], "metadatas": []}
         for chunk in all_chunk_ids:
             if chunk in db_data:
                 # 3. Add db metadata for nodes that have it
                 graph.nodes[chunk].update(db_data[chunk])
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.5.1/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.5.1/ragdaemon/annotators/chunker_llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,73 @@
-import asyncio
 import json
+from functools import partial
 from json.decoder import JSONDecodeError
 from typing import Any, Dict, List, Optional
 
 from spice import SpiceMessages
 from spice.models import TextModel
 
-from ragdaemon.annotators.chunker import Chunker
+from ragdaemon.annotators.chunker import Chunker, resolve_chunk_parent
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, lines_set_to_ref, semaphore
 
 
-def is_chunk_valid(chunk: dict, last_valid_line: int):
-    if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
-        raise RagdaemonError(f"Chunk is missing fields: {chunk}")
-    halves = chunk["id"].split(":")
-    if len(halves) != 2 or not halves[0] or not halves[1]:
-        raise RagdaemonError(f"Chunk ID is not in the correct format: {chunk}")
-    start, end = chunk.get("start_line"), chunk.get("end_line")
-    if start is None or end is None:
-        raise RagdaemonError(f"Chunk lines are missing: {chunk}")
-    # Sometimes output is int, sometimes string. This accomodates either.
-    start, end = str(start), str(end)
-    if not start.isdigit() or not end.isdigit():
-        raise RagdaemonError(f"Chunk lines are not valid: {chunk}")
-    start, end = int(start), int(end)
-    if not 1 <= start <= end <= last_valid_line:
-        raise RagdaemonError(f"Chunk lines are out of bounds: {chunk}")
-    # TODO: Validate the ref, i.e. a parent chunk exists
+def validate(
+    response: str,
+    file: str,
+    max_line: int,
+    file_chunks: set[str] | None,
+    last_chunk: Optional[dict[str, Any]],
+):
+    try:
+        chunks = json.loads(response).get("chunks")
+    except JSONDecodeError:
+        return False
+    if not isinstance(chunks, list):
+        return False
+    if not all(isinstance(chunk, dict) for chunk in chunks):
+        return False
+
+    for chunk in chunks:
+        if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
+            return False  # Chunk is missing fields
+
+        halves = chunk["id"].split(":")
+        if len(halves) != 2 or not halves[0] or not halves[1]:
+            return False  # Chunk ID is not in the correct format
+        if halves[0] != file:
+            return False
+
+        start, end = chunk.get("start_line"), chunk.get("end_line")
+        if start is None or end is None:
+            return False  # Chunk lines are missing
+
+        # Sometimes output is int, sometimes string. This accomodates either.
+        start, end = str(start), str(end)
+        if not start.isdigit() or not end.isdigit():
+            return False  # Chunk lines are not valid
+        start, end = int(start), int(end)
+
+        if not 1 <= start <= end <= max_line:
+            return False  # Chunk lines are out of bounds
+        # TODO: Validate the ref, i.e. a parent chunk exists
+
+    if last_chunk is not None:
+        if not any(chunk["id"] == last_chunk["id"] for chunk in chunks):
+            return False
+
+    if file_chunks is not None:
+        valid_parents = file_chunks.copy()
+        chunks_shortest_first = sorted(chunks, key=lambda x: len(x["id"]))
+        for chunk in chunks_shortest_first:
+            if not resolve_chunk_parent(chunk["id"], valid_parents):
+                return False
+            valid_parents.add(chunk["id"])
+
+    return True
 
 
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
     chunk_field_id = "chunks_llm"
 
     def __init__(
@@ -45,14 +81,15 @@
         self.batch_size = batch_size
         self.model = model
 
     async def get_llm_response(
         self,
         file: str,
         file_lines: list[str],
+        file_chunks: set[str],
         last_chunk: Optional[dict[str, Any]] = None,
     ) -> List[Dict[str, Any]]:
         """Get one chunking response from the LLM model."""
         if self.spice_client is None:
             raise RagdaemonError("Spice client is not initialized.")
 
         messages = SpiceMessages(self.spice_client)
@@ -61,83 +98,96 @@
             messages.add_system_prompt(
                 "chunker_llm.continuation", last_chunk=last_chunk
             )
         messages.add_user_prompt(
             "chunker_llm.user", path=file, code="\n".join(file_lines)
         )
 
+        max_line = int(file_lines[-1].split(":")[0])  # Extract line number
+        validator = partial(
+            validate,
+            file=file,
+            max_line=max_line,
+            file_chunks=file_chunks,
+            last_chunk=last_chunk,
+        )
         async with semaphore:
-            response = await self.spice_client.get_response(
-                messages=messages,
-                model=self.model,
-                response_format={"type": "json_object"},
-            )
-        try:
-            chunks = json.loads(response.text)["chunks"]
-        except JSONDecodeError:
-            raise RagdaemonError(
-                "Failed to parse JSON response. This could mean that the output is too "
-                "long, i.e. there are too many functions to chunk in one pass. If this "
-                "is the case, decrease the batch size and try again."
+            try:
+                response = await self.spice_client.get_response(
+                    messages=messages,
+                    model=self.model,
+                    response_format={"type": "json_object"},
+                    validator=validator,
+                    retries=2,
+                )
+                return json.loads(response.text).get("chunks")
+            except ValueError:
+                pass
+            # It's possible the parent chunk just doens't exist. So try once more and
+            # disregard that - it will just be linked to the BASE chunk instead.
+            validator = partial(
+                validate,
+                file=file,
+                max_line=max_line,
+                file_chunks=None,
+                last_chunk=last_chunk,
             )
-        last_valid_line = int(file_lines[-1].split(":")[0])
-        for chunk in chunks:
-            is_chunk_valid(chunk, last_valid_line)
-        if last_chunk is not None:
-            if not any(chunk["id"] == last_chunk["id"] for chunk in chunks):
-                raise RagdaemonError(
-                    f"Last chunk replacement ({last_chunk['id']}) not found in response."
+            try:
+                response = await self.spice_client.get_response(
+                    messages=messages,
+                    model=self.model,
+                    response_format={"type": "json_object"},
+                    validator=validator,
+                    retries=1,
                 )
-        return chunks
+                return json.loads(response.text).get("chunks")
+            except ValueError:
+                if self.verbose:
+                    print(
+                        f"Failed to get response for {file} batch ending at line {max_line}."
+                    )
+                return []
 
-    async def chunk_document(
-        self, document: str, retries: int = 1
-    ) -> list[dict[str, Any]]:
+    async def chunk_document(self, document: str) -> list[dict[str, Any]]:
         """Parse file_lines into a list of {id, ref} chunks."""
         lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if not file_lines or not any(line for line in file_lines):
             return []
         file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
 
         # Get raw llm output: {id, start_line, end_line}
         chunks = list[dict[str, Any]]()
         n_batches = (len(file_lines) + self.batch_size - 1) // self.batch_size
         for i in range(n_batches):
             batch_lines = file_lines[i * self.batch_size : (i + 1) * self.batch_size]
+            file_chunks = set(chunk["id"] for chunk in chunks)
             last_chunk = chunks.pop() if chunks else None
-            for j in range(retries + 1, 0, -1):
-                try:
-                    _chunks = await self.get_llm_response(file, batch_lines, last_chunk)
-                    chunks.extend(_chunks)
-                    break
-                except RagdaemonError as e:
-                    if self.verbose:
-                        print(
-                            f"Error chunking {file} batch {i+1}/{n_batches}:\n{e}\n"
-                            + f"{j-1} retries left."
-                            if j > 1
-                            else "Skipping."
-                        )
-                    if j == 1:
-                        return []
+            _chunks = await self.get_llm_response(
+                file, batch_lines, file_chunks, last_chunk
+            )
+            chunks.extend(_chunks)
 
         # Convert to {id: set(lines)} for easier manipulation
         chunks = {
             c["id"]: set(range(c["start_line"], c["end_line"] + 1)) for c in chunks
         }
 
         def update_parent_nodes(id: str, _chunks: dict[str, set[int]]):
             parent_lines = _chunks[id]
             child_chunks = {k: v for k, v in _chunks.items() if k.startswith(id + ".")}
             if child_chunks:
                 # Make sure end_line of each 'parent' chunk covers all children
                 start_line = min(parent_lines)
-                end_line = max(max(v) for v in child_chunks.values())
+                end_line = start_line
+                for child_lines in child_chunks.values():
+                    if not child_lines:
+                        continue
+                    end_line = max(end_line, max(child_lines))
                 parent_lines = set(range(start_line, end_line + 1))
                 # Remove child lines from parent lines
                 for child_lines in child_chunks.values():
                     parent_lines -= child_lines
                 _chunks[id] = parent_lines
             return _chunks
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/diff.py` & `ragdaemon-0.5.1/ragdaemon/annotators/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             return True
 
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         return self.id in graph and graph.nodes[self.id]["checksum"] == checksum
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         cwd = Path(graph.graph["cwd"])
         if not get_git_root_for_path(cwd, raise_error=False):
             return graph
 
         graph_nodes = {
             node
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.5.1/ragdaemon/annotators/hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         cwd = Path(graph.graph["cwd"])
         return graph.graph.get("files_checksum") == files_checksum(
             cwd, self.ignore_patterns
         )
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         """Build a graph of active files and directories with hierarchy edges."""
 
         # Initialize a new graph from scratch with same cwd
         cwd = Path(graph.graph["cwd"])
         graph = KnowledgeGraph()
         graph.graph["cwd"] = str(cwd)
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.5.1/ragdaemon/annotators/layout_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 return False
         return True
 
     async def annotate(
         self,
         graph: KnowledgeGraph,
         db: Database,
-        refresh: bool = False,
+        refresh: str | bool = False,
         iterations: int = 40,
     ) -> KnowledgeGraph:
         """
         a. Regenerate x/y/z for all nodes
         b. Update all nodes
         c. Save to chroma
         """
```

### Comparing `ragdaemon-0.5.0/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.5.1/ragdaemon/annotators/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import Database, remove_update_db_duplicates
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, hash_str, semaphore, truncate
+from ragdaemon.utils import (
+    DEFAULT_COMPLETION_MODEL,
+    hash_str,
+    match_refresh,
+    semaphore,
+    truncate,
+)
 
 
 def count_leaf_nodes_any_depth(
     graph: KnowledgeGraph,
     node: str,
     edge_type: str = "hierarchy",
     seen: Optional[set[str]] = None,
@@ -220,32 +226,33 @@
         return True
 
     async def generate_summary(
         self,
         node: str,
         graph: KnowledgeGraph,
         loading_bar: Optional[tqdm] = None,
-        refresh: bool = False,
+        refresh: str | bool = False,
     ):
         """Asynchronously generate summary and update graph"""
         if self.spice_client is None:
             raise RagdaemonError("Spice client not initialized")
 
         document, context = get_document_and_context(
             node, graph, summary_field_id=self.summary_field_id, model=self.model
         )
         summary_checksum = hash_str(document + context)
         data = graph.nodes[node]
+        _refresh = match_refresh(refresh, node)
         if (
-            refresh
+            _refresh
             or data.get(self.summary_field_id) is None
             or summary_checksum != data.get(self.checksum_field_id)
         ):
             subprompt = "root" if node == "ROOT" else data.get("type", "")
-            previous_summary = "" if refresh else data.get(self.summary_field_id, "")
+            previous_summary = "" if _refresh else data.get(self.summary_field_id, "")
 
             messages = SpiceMessages(self.spice_client)
             messages.add_system_prompt(
                 name=f"summarizer.{subprompt}", previous_summary=previous_summary
             )
             messages.add_user_prompt(
                 name=f"summarizer.user",
@@ -268,30 +275,30 @@
             loading_bar.update(1)
 
     async def dfs(
         self,
         node: str,
         graph: KnowledgeGraph,
         loading_bar: Optional[tqdm] = None,
-        refresh: bool = False,
+        refresh: str | bool = False,
     ):
         """Depth-first search to generate summaries for all nodes"""
         children = [
             edge[1]
             for edge in graph.out_edges(node, data=True)
             if edge[-1].get("type") == "hierarchy"
             and graph.nodes[edge[1]].get("type") in self.summarize_nodes
         ]
         if children:
             tasks = [self.dfs(child, graph, loading_bar, refresh) for child in children]
             await asyncio.gather(*tasks)
         await self.generate_summary(node, graph, loading_bar, refresh)
 
     async def annotate(
-        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+        self, graph: KnowledgeGraph, db: Database, refresh: str | bool = False
     ) -> KnowledgeGraph:
         """Asynchronously generate or fetch summaries and add to graph/db"""
         summaries = dict[str, str]()
         for node, data in graph.nodes(data=True):
             if data is not None and data.get("type") in self.summarize_nodes:
                 summaries[node] = data.get(self.checksum_field_id, "")
```

### Comparing `ragdaemon-0.5.0/ragdaemon/database/__init__.py` & `ragdaemon-0.5.1/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/database/chroma_database.py` & `ragdaemon-0.5.1/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/database/database.py` & `ragdaemon-0.5.1/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/database/lite_database.py` & `ragdaemon-0.5.1/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.5.1/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.5.1/ragdaemon/prompts/chunker_llm.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 2. `start_line` - where the function, class or method begins
 3. `end_line` - where it ends - INCLUSIVE
 
 The code may be provided in BATCHES, so you might see incomplete functions 
 or function signatures at the end of the file. Return them as if they were 
 complete functions, and they'll be repaired later.
 
+For items without an explicit name, e.g. anonymous functions, if/for/while 
+loops, direct callback assignments, entry points etc., do not count them as 
+chunks.
+
 EXAMPLE:
 --------------------------------------------------------------------------------
 <path>
 example/graph.py
 </path>
 
 <code>
@@ -52,15 +56,16 @@
 with any necessary updates. 
 
 Do your best to infer the correct position from the LAST CHUNK. For example:
 - If the last chunk was a class method and your first chunk also appears to be a class method,
 use the class name from the LAST CHUNK in your first chunk's `id`. Do your best to infer from
 context, spacing or other clues whether it is a continuation or a new section.
 - If the `end_line` of the last chunk is the last line before the provided code file,
-it may be a continuation of the LAST CHUNK, so return it with updated `end_line`."""
+it may be a continuation of the LAST CHUNK, so return it with updated `end_line`.
+- The current code might contain no new chunks! In that case just return the duplicated last chunk."""
 
 user="""\
 <path>
 {{ path }}
 </path>
 
 <code>
```

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/locate.toml` & `ragdaemon-0.5.1/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/favicon.ico` & `ragdaemon-0.5.1/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.5.1/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/js/main.js` & `ragdaemon-0.5.1/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.5.1/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/js/three/node.js` & `ragdaemon-0.5.1/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.5.1/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/ragdaemon/templates/index.html` & `ragdaemon-0.5.1/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/conftest.py` & `ragdaemon-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/test_comments.py` & `ragdaemon-0.5.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/test_context.py` & `ragdaemon-0.5.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/test_daemon.py` & `ragdaemon-0.5.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/test_get_paths.py` & `ragdaemon-0.5.1/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/test_sample.py` & `ragdaemon-0.5.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_chunker.py` & `ragdaemon-0.5.1/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.5.1/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_diff.py` & `ragdaemon-0.5.1/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_hierarchy.py` & `ragdaemon-0.5.1/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.5.1/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/annotators/test_summarizer.py` & `ragdaemon-0.5.1/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/chunker_graph.json` & `ragdaemon-0.5.1/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/context_message.txt` & `ragdaemon-0.5.1/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/diff_graph.json` & `ragdaemon-0.5.1/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/hard_to_chunk.txt` & `ragdaemon-0.5.1/tests/data/hard_to_chunk.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     def subtract_numbers(self):
         return self.a - self.b
     
     def exp_numbers(self):
         return math.pow(self.a, self.b)
     
-    def call():
+    def call(self):
         if self.operation == "add":
             return self.add_numbers()
         elif self.operation == "subtract":
             return self.subtract_numbers()
         elif self.operation == "exp":
             return self.multiply_numbers()
         else:
```

### Comparing `ragdaemon-0.5.0/tests/data/hierarchy_graph.json` & `ragdaemon-0.5.1/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.5.1/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/data/summarizer_graph.json` & `ragdaemon-0.5.1/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/tests/sample/src/interface.py` & `ragdaemon-0.5.1/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/LICENSE` & `ragdaemon-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/README.md` & `ragdaemon-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.0/pyproject.toml` & `ragdaemon-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.5.0"
+version = "0.5.1"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.5.0/PKG-INFO` & `ragdaemon-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.5.0
+Version: 0.5.1
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

