# Comparing `tmp/ragdaemon-0.5.1.tar.gz` & `tmp/ragdaemon-0.5.2.tar.gz`

## Comparing `ragdaemon-0.5.1.tar` & `ragdaemon-0.5.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0  1671121 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/app.py
--rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/context.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/app.py
+-rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/context.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.2/PKG-INFO
```

### Comparing `ragdaemon-0.5.1/tutorial.ipynb` & `ragdaemon-0.5.2/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/.github/workflows/run-tests.yml` & `ragdaemon-0.5.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/app.py` & `ragdaemon-0.5.2/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/context.py` & `ragdaemon-0.5.2/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/daemon.py` & `ragdaemon-0.5.2/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/get_paths.py` & `ragdaemon-0.5.2/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/graph.py` & `ragdaemon-0.5.2/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/locate.py` & `ragdaemon-0.5.2/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/utils.py` & `ragdaemon-0.5.2/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/__init__.py` & `ragdaemon-0.5.2/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.5.2/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.5.2/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/chunker.py` & `ragdaemon-0.5.2/ragdaemon/annotators/chunker.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 metadatas = {self.chunk_field_id: json.dumps(data[self.chunk_field_id])}
                 update_db["metadatas"].append(metadatas)
             update_db = remove_update_db_duplicates(**update_db)
             db.update(**update_db)
 
         # Process chunks
         # 1. Add all chunks to graph
-        all_chunk_ids = set()
+        checksums = dict[str, str]()
         for file, data in files_with_chunks:
             if len(data[self.chunk_field_id]) == 0:
                 continue
             # Sort such that "parents" are added before "children"
             base_id = f"{file}:BASE"
             chunks = [c for c in data[self.chunk_field_id] if c["id"] != base_id]
             chunks.sort(key=lambda x: len(x["id"]))
@@ -165,52 +165,50 @@
             if len(base_chunk) != 1:
                 raise RagdaemonError(f"Node {file} missing base chunk")
             chunks = base_chunk + chunks
             # Load chunks into graph
             for chunk in chunks:
                 id, ref = chunk["id"], chunk["ref"]
                 document = get_document(ref, Path(graph.graph["cwd"]))
+                checksum = hash_str(document)
                 chunk_data = {
                     "id": id,
                     "ref": ref,
                     "type": "chunk",
                     "document": document,
-                    "checksum": hash_str(document),
+                    "checksum": checksum,
                     "active": False,
                 }
                 graph.add_node(id, **chunk_data)
-                all_chunk_ids.add(id)
+                checksums[id] = checksum
 
                 all_nodes = set(graph.nodes)
                 parent = resolve_chunk_parent(id, all_nodes)
                 if parent is None:
                     if self.verbose:
                         print(f"No parent node found for {id}")
                     parent = f"{file}:BASE"
                 graph.add_edge(parent, id, type="hierarchy")
 
-        # 2. Get metadata for all chunks from db
-        all_chunk_checksums = list(
-            set(graph.nodes[chunk]["checksum"] for chunk in all_chunk_ids)
-        )
-        response = db.get(ids=all_chunk_checksums, include=["metadatas"])
-        db_data = {data["id"]: data for data in response["metadatas"]}
+        # Sync with remote DB
+        ids = list(set(checksums.values()))
+        response = db.get(ids=ids, include=["metadatas"])
+        db_data = {id: data for id, data in zip(response["ids"], response["metadatas"])}
         add_to_db = {"ids": [], "documents": [], "metadatas": []}
-        for chunk in all_chunk_ids:
-            if chunk in db_data:
-                # 3. Add db metadata for nodes that have it
-                graph.nodes[chunk].update(db_data[chunk])
+        for node, checksum in checksums.items():
+            if checksum in db_data:
+                data = db_data[checksum]
+                graph.nodes[node].update(data)
             else:
-                # 4. Add to db nodes that don't
-                data = deepcopy(graph.nodes[chunk])
+                data = deepcopy(graph.nodes[node])
                 document = data.pop("document")
                 document, truncate_ratio = truncate(document, db.embedding_model)
                 if truncate_ratio > 0 and self.verbose:
-                    print(f"Truncated {chunk} by {truncate_ratio:.2%}")
-                add_to_db["ids"].append(data["checksum"])
+                    print(f"Truncated {node} by {truncate_ratio:.2%}")
+                add_to_db["ids"].append(checksum)
                 add_to_db["documents"].append(document)
                 add_to_db["metadatas"].append(data)
         if len(add_to_db["ids"]) > 0:
             add_to_db = remove_add_to_db_duplicates(**add_to_db)
             db.add(**add_to_db)
 
         return graph
```

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.5.2/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.5.2/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/diff.py` & `ragdaemon-0.5.2/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.5.2/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.5.2/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.5.2/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/database/__init__.py` & `ragdaemon-0.5.2/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/database/chroma_database.py` & `ragdaemon-0.5.2/ragdaemon/database/chroma_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Optional, cast
+from typing import Any, Optional, cast
 
 import dotenv
 from chromadb.config import Settings
 from spice import Spice
 
 from ragdaemon import __version__
 from ragdaemon.database.database import Database
@@ -50,14 +50,15 @@
         embedding_model: str,
         embedding_provider: Optional[str] = None,
         verbose: bool = False,
     ) -> None:
         self.cwd = cwd
         self.db_path = db_path
         self.embedding_model = embedding_model
+        self.verbose = verbose
 
         import chromadb  # Imports are slow so do it lazily
         from chromadb.api.types import (
             Embeddable,
             EmbeddingFunction,
             Embeddings,
         )
@@ -94,15 +95,15 @@
                 host=host,
                 port=port,
                 ssl=port == 443,
                 headers={"Authorization": basic_auth(username, password)},
                 settings=Settings(allow_reset=True, anonymized_telemetry=False),
             )
         except KeyError:
-            if verbose:
+            if self.verbose:
                 print(
                     "No Chroma HTTP client environment variables found. Defaulting to PersistentClient."
                 )
             _client = chromadb.PersistentClient(path=str(db_path))
 
         minor_version = ".".join(__version__.split(".")[:2])
         name = f"ragdaemon-{minor_version}-{self.embedding_model}"
@@ -148,8 +149,25 @@
             return []
         # Parse results. Return results for the 'first query' only
         results = [
             {"checksum": id, "distance": distance}
             for id, distance in zip(response["ids"][0], response["distances"][0])
         ]
         results = sorted(results, key=lambda x: x["distance"])
+
+        # If a query is interrupted before removing the flags, or if two queries
+        # are sent at the same times, the active flags can get messed up. This is
+        # a workaround to ensure the flags are always correct.
+        if any(result["checksum"] not in valid_checksums for result in results):
+            if self.verbose:
+                print(
+                    f"Corrupt records found in {self.cwd.name}. Resetting active flags."
+                )
+            corrupt_records = self._collection.get(include=[])["ids"]
+            updates = {
+                "ids": corrupt_records,
+                "metadatas": [{"active": False} for _ in corrupt_records],
+            }
+            self._collection.update(**updates)
+            return self.query(query, active_checksums)
+
         return results
```

### Comparing `ragdaemon-0.5.1/ragdaemon/database/database.py` & `ragdaemon-0.5.2/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/database/lite_database.py` & `ragdaemon-0.5.2/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.5.2/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.5.2/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/locate.toml` & `ragdaemon-0.5.2/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.5.2/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.5.2/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.5.2/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.5.2/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.5.2/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/favicon.ico` & `ragdaemon-0.5.2/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.5.2/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/js/main.js` & `ragdaemon-0.5.2/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.5.2/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/js/three/node.js` & `ragdaemon-0.5.2/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.5.2/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/ragdaemon/templates/index.html` & `ragdaemon-0.5.2/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/conftest.py` & `ragdaemon-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/test_comments.py` & `ragdaemon-0.5.2/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/test_context.py` & `ragdaemon-0.5.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/test_daemon.py` & `ragdaemon-0.5.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/test_get_paths.py` & `ragdaemon-0.5.2/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/test_sample.py` & `ragdaemon-0.5.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_chunker.py` & `ragdaemon-0.5.2/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.5.2/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_diff.py` & `ragdaemon-0.5.2/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_hierarchy.py` & `ragdaemon-0.5.2/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.5.2/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/annotators/test_summarizer.py` & `ragdaemon-0.5.2/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/chunker_graph.json` & `ragdaemon-0.5.2/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/context_message.txt` & `ragdaemon-0.5.2/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/diff_graph.json` & `ragdaemon-0.5.2/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/hard_to_chunk.txt` & `ragdaemon-0.5.2/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/hierarchy_graph.json` & `ragdaemon-0.5.2/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.5.2/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/data/summarizer_graph.json` & `ragdaemon-0.5.2/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/tests/sample/src/interface.py` & `ragdaemon-0.5.2/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/LICENSE` & `ragdaemon-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/README.md` & `ragdaemon-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.1/pyproject.toml` & `ragdaemon-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.5.1"
+version = "0.5.2"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.5.1/PKG-INFO` & `ragdaemon-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.5.1
+Version: 0.5.2
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

