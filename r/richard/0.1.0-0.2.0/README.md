# Comparing `tmp/richard-0.1.0.tar.gz` & `tmp/richard-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richard-0.1.0.tar", last modified: Sun May 12 05:52:20 2024, max compression
+gzip compressed data, was "richard-0.2.0.tar", last modified: Sun May 19 08:12:10 2024, max compression
```

## Comparing `richard-0.1.0.tar` & `richard-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,100 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.676252 richard-0.1.0/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1083 2024-05-04 21:29:27.000000 richard-0.1.0/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      444 2024-05-12 05:52:20.676252 richard-0.1.0/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      180 2024-05-05 13:05:24.000000 richard-0.1.0/README.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.664251 richard-0.1.0/docs/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/docs/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.664251 richard-0.1.0/richard/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1400 2024-05-11 15:19:23.000000 richard-0.1.0/richard/Pipeline.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:28:03.000000 richard-0.1.0/richard/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      459 2024-05-04 06:40:05.000000 richard-0.1.0/richard/constants.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.668251 richard-0.1.0/richard/entity/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1668 2024-05-11 15:18:34.000000 richard-0.1.0/richard/entity/GrammarRule.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1383 2024-05-11 15:18:45.000000 richard-0.1.0/richard/entity/GrammarRules.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      242 2024-05-04 19:20:05.000000 richard-0.1.0/richard/entity/Log.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      188 2024-05-11 15:19:23.000000 richard-0.1.0/richard/entity/ParseResult.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1330 2024-05-11 15:19:23.000000 richard-0.1.0/richard/entity/ParseTreeNode.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1319 2024-05-11 06:24:19.000000 richard-0.1.0/richard/entity/Record.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      772 2024-05-11 15:19:23.000000 richard-0.1.0/richard/entity/RecordSet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      566 2024-05-11 15:19:23.000000 richard-0.1.0/richard/entity/RuleConstituent.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1428 2024-05-11 15:19:23.000000 richard-0.1.0/richard/entity/SentenceRequest.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/entity/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.668251 richard-0.1.0/richard/interface/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      287 2024-05-11 15:19:23.000000 richard-0.1.0/richard/interface/SomeLanguageSelector.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      200 2024-05-11 06:53:06.000000 richard-0.1.0/richard/interface/SomeLogger.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      625 2024-05-11 15:19:23.000000 richard-0.1.0/richard/interface/SomeParser.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      475 2024-05-11 06:46:50.000000 richard-0.1.0/richard/interface/SomeProcessor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      303 2024-05-11 15:19:23.000000 richard-0.1.0/richard/interface/SomeSemanticComposer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      288 2024-05-11 15:19:23.000000 richard-0.1.0/richard/interface/SomeSemanticExecutor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      571 2024-05-11 15:19:23.000000 richard-0.1.0/richard/interface/SomeTokenizer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/interface/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.668251 richard-0.1.0/richard/processor/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 17:13:33.000000 richard-0.1.0/richard/processor/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.668251 richard-0.1.0/richard/processor/language_selector/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      733 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/language_selector/LanguageSelector.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1225 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/language_selector/Multilingual.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/language_selector/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/parser/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/BasicParser.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/parser/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/parser/earley/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7572 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/earley/EarleyParser.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/parser/earley/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/parser/earley/entity/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2089 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/earley/entity/Chart.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1400 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/earley/entity/ChartState.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:03:37.000000 richard-0.1.0/richard/processor/parser/earley/entity/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3203 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/earley/tree_extract.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      845 2024-05-06 06:25:41.000000 richard-0.1.0/richard/processor/parser/earley/unknown_word.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/parser/helper/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1808 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/parser/helper/SimpleGrammarRulesParser.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/parser/helper/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/semantic_composer/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1877 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/semantic_composer/SemanticComposer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/semantic_composer/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/semantic_executor/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      859 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/semantic_executor/SemanticExecutor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/semantic_executor/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/processor/tokenizer/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      387 2024-05-11 15:19:23.000000 richard-0.1.0/richard/processor/tokenizer/BasicTokenizer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/processor/tokenizer/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.672251 richard-0.1.0/richard/semantics/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/semantics/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      570 2024-05-10 18:39:43.000000 richard-0.1.0/richard/semantics/commands.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.676252 richard-0.1.0/richard/store/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      830 2024-05-11 15:19:23.000000 richard-0.1.0/richard/store/MemoryDb.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/store/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.676252 richard-0.1.0/richard/type/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       19 2024-05-02 18:35:12.000000 richard-0.1.0/richard/type/PositionType.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      102 2024-05-11 15:19:23.000000 richard-0.1.0/richard/type/SimpleGrammar.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       56 2024-05-09 08:30:11.000000 richard-0.1.0/richard/type/SimpleGrammarRule.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.1.0/richard/type/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.664251 richard-0.1.0/richard.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      444 2024-05-12 05:52:20.000000 richard-0.1.0/richard.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2160 2024-05-12 05:52:20.000000 richard-0.1.0/richard.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2024-05-12 05:52:20.000000 richard-0.1.0/richard.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       19 2024-05-12 05:52:20.000000 richard-0.1.0/richard.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2024-05-12 05:52:20.676252 richard-0.1.0/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      550 2024-05-12 05:50:12.000000 richard-0.1.0/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-12 05:52:20.676252 richard-0.1.0/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3830 2024-05-11 15:19:23.000000 richard-0.1.0/tests/EarleyParser_test.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2142 2024-05-11 15:19:23.000000 richard-0.1.0/tests/Multilingual_test.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1097 2024-05-11 15:19:23.000000 richard-0.1.0/tests/Parser_test.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3422 2024-05-11 15:19:23.000000 richard-0.1.0/tests/Quantifier_test.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 17:14:10.000000 richard-0.1.0/tests/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.038690 richard-0.2.0/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1083 2024-05-04 21:29:27.000000 richard-0.2.0/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      444 2024-05-19 08:12:10.038690 richard-0.2.0/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      853 2024-05-19 08:11:25.000000 richard-0.2.0/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.026690 richard-0.2.0/docs/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/docs/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.026690 richard-0.2.0/richard/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1225 2024-05-17 18:23:39.000000 richard-0.2.0/richard/Domain.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1283 2024-05-18 18:49:45.000000 richard-0.2.0/richard/Pipeline.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:28:03.000000 richard-0.2.0/richard/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.030690 richard-0.2.0/richard/block/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1489 2024-05-18 18:49:45.000000 richard-0.2.0/richard/block/FindAll.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1252 2024-05-18 18:49:45.000000 richard-0.2.0/richard/block/FindOne.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      422 2024-05-18 18:49:45.000000 richard-0.2.0/richard/block/Succeed.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1074 2024-05-18 18:49:45.000000 richard-0.2.0/richard/block/TryFirst.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-18 18:49:45.000000 richard-0.2.0/richard/block/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      485 2024-05-18 18:49:45.000000 richard-0.2.0/richard/constants.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.030690 richard-0.2.0/richard/entity/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      128 2024-05-18 18:49:45.000000 richard-0.2.0/richard/entity/BlockResult.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      507 2024-05-18 18:49:45.000000 richard-0.2.0/richard/entity/ControlBlock.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      116 2024-05-17 06:26:32.000000 richard-0.2.0/richard/entity/Entity.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1640 2024-05-14 18:36:11.000000 richard-0.2.0/richard/entity/GrammarRule.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1383 2024-05-11 15:18:45.000000 richard-0.2.0/richard/entity/GrammarRules.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      242 2024-05-04 19:20:05.000000 richard-0.2.0/richard/entity/Log.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1330 2024-05-11 15:19:23.000000 richard-0.2.0/richard/entity/ParseTreeNode.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      158 2024-05-18 18:49:45.000000 richard-0.2.0/richard/entity/ProcessResult.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      131 2024-05-16 18:47:24.000000 richard-0.2.0/richard/entity/Relation.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      566 2024-05-11 15:19:23.000000 richard-0.2.0/richard/entity/RuleConstituent.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2024-05-18 18:49:45.000000 richard-0.2.0/richard/entity/SentenceRequest.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/entity/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.030690 richard-0.2.0/richard/interface/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      287 2024-05-11 15:19:23.000000 richard-0.2.0/richard/interface/SomeLanguageSelector.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      200 2024-05-11 06:53:06.000000 richard-0.2.0/richard/interface/SomeLogger.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      625 2024-05-11 15:19:23.000000 richard-0.2.0/richard/interface/SomeParser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      548 2024-05-18 18:49:45.000000 richard-0.2.0/richard/interface/SomeProcessor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      303 2024-05-11 15:19:23.000000 richard-0.2.0/richard/interface/SomeSemanticComposer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      288 2024-05-11 15:19:23.000000 richard-0.2.0/richard/interface/SomeSemanticExecutor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      571 2024-05-11 15:19:23.000000 richard-0.2.0/richard/interface/SomeTokenizer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/interface/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.030690 richard-0.2.0/richard/processor/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 17:13:33.000000 richard-0.2.0/richard/processor/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/language_selector/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      828 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/language_selector/LanguageSelector.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/language_selector/Multilingual.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/language_selector/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/parser/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1196 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/parser/BasicParser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/parser/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/parser/earley/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7601 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/parser/earley/EarleyParser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/parser/earley/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/parser/earley/entity/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2099 2024-05-14 17:16:08.000000 richard-0.2.0/richard/processor/parser/earley/entity/Chart.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1400 2024-05-11 15:19:23.000000 richard-0.2.0/richard/processor/parser/earley/entity/ChartState.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:03:37.000000 richard-0.2.0/richard/processor/parser/earley/entity/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3267 2024-05-14 17:27:17.000000 richard-0.2.0/richard/processor/parser/earley/tree_extract.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      845 2024-05-06 06:25:41.000000 richard-0.2.0/richard/processor/parser/earley/unknown_word.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/parser/helper/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1807 2024-05-17 21:38:55.000000 richard-0.2.0/richard/processor/parser/helper/SimpleGrammarRulesParser.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/parser/helper/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/semantic_composer/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2198 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/semantic_composer/SemanticComposer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/semantic_composer/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/semantic_executor/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      959 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/semantic_executor/SemanticExecutor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/semantic_executor/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/processor/tokenizer/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      721 2024-05-18 18:49:45.000000 richard-0.2.0/richard/processor/tokenizer/BasicTokenizer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/processor/tokenizer/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/semantics/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/semantics/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      576 2024-05-15 18:03:31.000000 richard-0.2.0/richard/semantics/commands.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/store/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1102 2024-05-18 18:49:45.000000 richard-0.2.0/richard/store/MemoryDb.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1394 2024-05-15 12:45:19.000000 richard-0.2.0/richard/store/Record.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      837 2024-05-17 18:31:03.000000 richard-0.2.0/richard/store/RecordSet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/store/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.034690 richard-0.2.0/richard/type/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       19 2024-05-02 18:35:12.000000 richard-0.2.0/richard/type/PositionType.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      102 2024-05-11 15:19:23.000000 richard-0.2.0/richard/type/SimpleGrammar.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       56 2024-05-09 08:30:11.000000 richard-0.2.0/richard/type/SimpleGrammarRule.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 18:01:27.000000 richard-0.2.0/richard/type/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.026690 richard-0.2.0/richard.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      444 2024-05-19 08:12:09.000000 richard-0.2.0/richard.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2532 2024-05-19 08:12:09.000000 richard-0.2.0/richard.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2024-05-19 08:12:09.000000 richard-0.2.0/richard.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       19 2024-05-19 08:12:09.000000 richard-0.2.0/richard.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2024-05-19 08:12:10.038690 richard-0.2.0/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      550 2024-05-19 08:09:41.000000 richard-0.2.0/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-19 08:12:10.038690 richard-0.2.0/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3799 2024-05-19 07:39:42.000000 richard-0.2.0/tests/Chat80_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3090 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Composer_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3845 2024-05-18 18:49:45.000000 richard-0.2.0/tests/EarleyParser_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2540 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Executor_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2211 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Multilingual_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Parser_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1252 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Postgres_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3915 2024-05-18 18:49:45.000000 richard-0.2.0/tests/Quantifier_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      789 2024-05-19 07:49:52.000000 richard-0.2.0/tests/Tokenizer_test.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2024-05-11 17:14:10.000000 richard-0.2.0/tests/__init__.py
```

### Comparing `richard-0.1.0/LICENSE` & `richard-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/Pipeline.py` & `richard-0.2.0/richard/processor/language_selector/Multilingual.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from dataclasses import dataclass
-
+from richard.entity.ProcessResult import ProcessResult
 from richard.entity.SentenceRequest import SentenceRequest
-from .interface.SomeProcessor import SomeProcessor
+from richard.interface.SomeLanguageSelector import SomeLanguageSelector
+from richard.interface.SomeProcessor import SomeProcessor
 
 
-@dataclass(frozen=True)
-class Pipeline:
+class Multilingual(SomeProcessor):
     """
-    This class contains all processors involved in the processing of a sentence.
-    The number and type of processors depend on the purpose of the application.
-    When a new sentence comes in, it creates a request for it ans sends it trough the pipeline of processors.
-    Each processor generates one or more alternative interpretations (ambiguity), and the pipeline processes these one by one.
-    Each processor has access to the active alternative interpretations of its predecessors.
+    This compositing processor takes other processors as input and uses the processor of the active language when asks to `process` input
+    It can be used to combine any combinations of processors, like tokenization processors or parsing processors
     """
     
-    processors: list[SomeProcessor]
+    processors: dict[str, SomeProcessor]
+    language_selector: SomeLanguageSelector
+
+    def __init__(self, processors: dict[str, SomeProcessor], language_selector: SomeLanguageSelector) -> None:
+        super().__init__()
+        self.processors = processors
+        self.language_selector = language_selector
+
+        
+    def process(self, request: SentenceRequest) -> ProcessResult:
 
+        locale = self.language_selector.get_locale(request)
 
-    def enter(self, request: SentenceRequest):
-        self.try_processor(0, request)
+        if locale not in self.processors:
+            raise Exception("No processor available for locale " + locale)
+
+        return self.processors[locale].process(request)
+    
 
+    def get_product(self, request: SentenceRequest) -> any:
+        return request.get_current_product(self)
     
-    def try_processor(self, process_index: int, request: SentenceRequest):
-        processor = self.processors[process_index]
-        alternatives = processor.process(request)
-        request.set_alternative_products(processor, alternatives)
-        for alternative in alternatives:
-            request.set_current_product(processor, alternative)
-            if process_index+1 == len(self.processors):
-                return True
-            success = self.try_processor(process_index+1, request)
-            if success:
-                return True
-        return False
```

### Comparing `richard-0.1.0/richard/entity/GrammarRule.py` & `richard-0.2.0/richard/entity/GrammarRule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 
 from richard.constants import POS_TYPE_RELATION, POS_TYPE_WORD_FORM
 from richard.entity.RuleConstituent import RuleConstituent
-from richard.type.PositionType import PositionType
 
 
 @dataclass(frozen=True)
 class GrammarRule:
     
     antecedent: RuleConstituent
     consequents: list[RuleConstituent]
@@ -26,32 +25,32 @@
                 return False
             
         return True
     
 
     def basic_form(self):
 
-        s = self.antecedent.predicate + "("
-        sep2 = ""
-        for variable in self.antecedent.arguments:
-            s += sep2 + variable
-            sep2 = ", "
-        s += ")"
+        s = self.antecedent.predicate #+ "("
+        # sep2 = ""
+        # for variable in self.antecedent.arguments:
+        #     s += sep2 + variable
+        #     sep2 = ", "
+        # s += ")"
 
         s += " -> "
 
         sep = ""
         for i in range(len(self.consequents)):
             if self.consequents[i].position_type == POS_TYPE_RELATION:
-                s += sep + self.consequents[i].predicate + "("
-                sep2 = ""
-                for variable in self.consequents[i].arguments :
-                    s += sep2 + variable
-                    sep2 = ", "
-                s += ")"
+                s += sep + self.consequents[i].predicate # + "("
+                # sep2 = ""
+                # for variable in self.consequents[i].arguments :
+                #     s += sep2 + variable
+                #     sep2 = ", "
+                # s += ")"
             elif self.consequents[i].position_type == POS_TYPE_WORD_FORM:
                 s += sep + "'" + self.consequents[i].predicate + "'"
             else:
                 s += sep + "/" + self.consequents[i].predicate + "/"
             sep = " "
 
         return s
```

### Comparing `richard-0.1.0/richard/entity/GrammarRules.py` & `richard-0.2.0/richard/entity/GrammarRules.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/entity/ParseTreeNode.py` & `richard-0.2.0/richard/entity/ParseTreeNode.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/entity/Record.py` & `richard-0.2.0/richard/store/Record.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,18 @@
                 raise ValueError("The record key '" + name + "' is not an identier")
             if not isinstance(value, float) and not isinstance(value, str) and not isinstance(value, int):
                 raise ValueError("A record must be int, float or string")
     
 
     def __str__(self):
         return self.table + " " + str(self.values)
+    
+
+    def is_empty(self) -> bool:
+        return len(self.values) == 0
 
 
     def __hash__(self) -> int:
         # see https://stackoverflow.com/a/5884123
         return hash(self.table) + hash(frozenset(self.values.items()))
```

### Comparing `richard-0.1.0/richard/entity/RecordSet.py` & `richard-0.2.0/richard/store/RecordSet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from richard.entity.Record import Record
+from richard.store.Record import Record
 
 
 class RecordSet:
     """
     A record set is a set of records: each record can appear only once 
     """
     
@@ -10,14 +10,18 @@
     _records: set[Record]
 
 
     def __init__(self) -> None:
         self._records = set()
 
 
+    def __len__(self) -> int:
+        return len(self._records)
+
+
     def add(self, record: Record):
         self._records.add(record)
 
 
     # make the set iterable
     def __iter__(self):
         for record in self._records:
```

### Comparing `richard-0.1.0/richard/entity/RuleConstituent.py` & `richard-0.2.0/richard/entity/RuleConstituent.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/entity/SentenceRequest.py` & `richard-0.2.0/richard/entity/SentenceRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,30 +7,35 @@
     This interpretation consists of one alternative interpretation per processor so far.
     """
 
     # raw text that serves as the input to the request
     text: str
 
     # each processor creates one or more products; the pipeline considers these one by one; the current product is kept here
-    current_products: dict[SomeProcessor, any] = {}
+    current_products: dict[SomeProcessor, any]
 
     # all alternative products (more than one product suggests ambiguity)
-    alternative_products: dict[SomeProcessor, list[any]] = {}
-
+    alternative_products: dict[SomeProcessor, list[any]]
+    
 
     def __init__(self, text: str) -> None:
         self.text = text
+        self.current_products = {}
+        self.alternative_products = {}
 
 
     def set_alternative_products(self, processor: SomeProcessor, alternatives: list[any]):
         self.alternative_products[processor] = alternatives
 
 
     def get_alternative_products(self, processor: SomeProcessor) -> list[any]:
-        return self.alternative_products[processor]
+        if processor in self.alternative_products:
+            return self.alternative_products[processor]
+        else:
+            return []
 
 
     def set_current_product(self, processor: SomeProcessor, alternative: any):
         self.current_products[processor] = alternative
 
 
     def get_current_product(self, processor: SomeProcessor):
```

### Comparing `richard-0.1.0/richard/interface/SomeParser.py` & `richard-0.2.0/richard/interface/SomeParser.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/interface/SomeTokenizer.py` & `richard-0.2.0/richard/interface/SomeTokenizer.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/processor/language_selector/LanguageSelector.py` & `richard-0.2.0/richard/processor/language_selector/LanguageSelector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from richard.entity.ProcessResult import ProcessResult
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.interface.SomeLanguageSelector import SomeLanguageSelector
 
 
 class LanguageSelector(SomeLanguageSelector):
     """
     Just picks one of the available locales, one by one. If processing the input with one locale fails, the next locale is tried.
@@ -11,13 +12,13 @@
     locales: list[str]
     
     def __init__(self, locales: list[str]) -> None:
         super().__init__()
         self.locales = locales
 
 
-    def process(self, request: SentenceRequest):
-        return self.locales
+    def process(self, request: SentenceRequest) -> ProcessResult:
+        return ProcessResult(self.locales, "", [])
     
 
     def get_locale(self, request: SentenceRequest) -> str:
         return request.get_current_product(self)
```

### Comparing `richard-0.1.0/richard/processor/parser/BasicParser.py` & `richard-0.2.0/richard/processor/parser/BasicParser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from richard.entity.GrammarRules import GrammarRules
 from richard.entity.ParseTreeNode import ParseTreeNode
+from richard.entity.ProcessResult import ProcessResult
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.interface.SomeParser import SomeParser
 from richard.interface.SomeTokenizer import SomeTokenizer
 from richard.processor.parser.helper.SimpleGrammarRulesParser import SimpleGrammarRulesParser
 from richard.type.SimpleGrammar import SimpleGrammar
 from .earley.EarleyParser import EarleyParser
 
@@ -20,16 +21,15 @@
         self.tokenizer = tokenizer
 
         sgrp = SimpleGrammarRulesParser()
         self.grammar = sgrp.parse(grammar)
         self.parser = EarleyParser()
             
 
-    def process(self, request: SentenceRequest):
+    def process(self, request: SentenceRequest) -> ProcessResult:
         tokens = self.tokenizer.get_tokens(request)
-        result = self.parser.parse(self.grammar, tokens)
-        return result.trees
+        return self.parser.parse(self.grammar, tokens)
     
 
     def get_tree(self, request: SentenceRequest) -> ParseTreeNode:
         return request.get_current_product(self)
```

### Comparing `richard-0.1.0/richard/processor/parser/earley/EarleyParser.py` & `richard-0.2.0/richard/processor/parser/earley/EarleyParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import re
 from richard.constants import TERMINAL, CATEGORY_PROPER_NOUN, NO_SENTENCE, NOT_UNDERSTOOD, POS_TYPE_REG_EXP, POS_TYPE_RELATION, POS_TYPE_WORD_FORM, UNKNOWN_WORD
 from richard.entity.GrammarRule import GrammarRule
 from richard.entity.GrammarRules import GrammarRules
 from richard.entity.Log import Log
-from richard.entity.ParseResult import ParseResult
+from richard.entity.ProcessResult import ProcessResult
 from richard.entity.RuleConstituent import RuleConstituent
 from richard.interface.SomeLogger import SomeLogger
 from .entity.Chart import Chart
 from .entity.ChartState import ChartState
 from .tree_extract import extract_tree_roots
 from .unknown_word import find_unknown_word
 
@@ -21,40 +21,40 @@
 
     log: SomeLogger
 
     def __init__(self, log: SomeLogger = Log(False)):
         self.log = log
 
 
-    def parse(self, grammar_rules: GrammarRules, tokens: list[str]) -> ParseResult:
+    def parse(self, grammar_rules: GrammarRules, tokens: list[str]) -> ProcessResult:
 
         chart = self.buildChart(grammar_rules, tokens, "s", ["P"])
 
         rootNodes = extract_tree_roots(chart)
         error = ""
-        errorArg = ""
+        error_args = []
 
         if len(rootNodes) == 0:
 
             nextWord = find_unknown_word(chart)
 
             if nextWord != "":
                 error = UNKNOWN_WORD
-                errorArg = nextWord
+                error_args = [nextWord]
             elif len(tokens) == 0:
                 error = NO_SENTENCE
-                errorArg = ""
+                error_args = []
             else:
                 error = NOT_UNDERSTOOD
-                errorArg = ""
+                error_args = []
 
-        return ParseResult(
-            trees=rootNodes,
-            error=error,
-            error_arg=errorArg,
+        return ProcessResult(
+            products=rootNodes,
+            error_code=error,
+            error_args=error_args,
         )
     
 
     def buildChart(self, grammar_rules: GrammarRules, words, rootCategory, rootVariables):
         """
         The body of Earley's algorithm
         """
```

### Comparing `richard-0.1.0/richard/processor/parser/earley/entity/Chart.py` & `richard-0.2.0/richard/processor/parser/earley/entity/Chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Chart:
     root_category: str
     root_variables: list[str]
     words: list[str]
     states: list[list[ChartState]]
-    # all states that were completed, by dot position
+    # all states that were completed, indexed by end word index
     completed_states: dict[int, list[ChartState]]
 
 
     def __init__(self, words: list[str], root_category: str, root_variables: list[str]) -> None:
         self.root_category = root_category
         self.words = words
         self.root_variables = root_variables
```

### Comparing `richard-0.1.0/richard/processor/parser/earley/entity/ChartState.py` & `richard-0.2.0/richard/processor/parser/earley/entity/ChartState.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/processor/parser/earley/tree_extract.py` & `richard-0.2.0/richard/processor/parser/earley/tree_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def extract_tree_roots(chart: Chart):
 
     gamma_state = chart.build_complete_gamma_state()
     if not gamma_state.end_word_index in chart.completed_states:
         return []
-
+    
     gamma_nodes = create_trees_for_state(chart, gamma_state)
     return [gamma_node.children[0] for gamma_node in gamma_nodes]
 
 
 def create_trees_for_state(chart: Chart, state: ChartState):
     trees = []
 
@@ -50,15 +50,15 @@
     """
     try to match the consequent_index'th consequent of parent_state to a new state, ending in the end_word_position
     and prepend the earlier states. this may result in multiple state sequences
     """
     sequences = []
     for state in chart.completed_states[end_word_position]:
         if state.rule.antecedent.equals(parent_state.rule.consequents[consequent_index]):
-            if consequent_index == 0:
+            if consequent_index == 0 and state.start_word_index == parent_state.start_word_index:
                 sequences.append([state])
             else:
                 # find one or more preceding sequences of this state
                 for previous_sequence in find_state_sequences(chart, parent_state, state.start_word_index, consequent_index-1):
                     sequences.append(previous_sequence + [state])
     return sequences
```

### Comparing `richard-0.1.0/richard/processor/parser/earley/unknown_word.py` & `richard-0.2.0/richard/processor/parser/earley/unknown_word.py`

 * *Files identical despite different names*

### Comparing `richard-0.1.0/richard/processor/parser/helper/SimpleGrammarRulesParser.py` & `richard-0.2.0/richard/processor/parser/helper/SimpleGrammarRulesParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class SimpleGrammarRulesParser:
     re_rule: re.Pattern
     re_space: re.Pattern
 
 
     def __init__(self) -> None:
-        self.re_rule = re.compile("\s*(\w+)\s*->((\s*[\w']+)+)")
+        self.re_rule = re.compile("\s*(\w+)\s*->((\s*[\S]+)+)")
         self.re_space = re.compile("\s+")
 
 
     def parse(self, simple_grammar: SimpleGrammar):
         rules = []
 
         for simple_rule in simple_grammar:
```

### Comparing `richard-0.1.0/richard/processor/semantic_executor/SemanticExecutor.py` & `richard-0.2.0/richard/processor/semantic_executor/SemanticExecutor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from richard.entity.ParseTreeNode import ParseTreeNode
+from richard.entity.ProcessResult import ProcessResult
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.interface.SomeProcessor import SomeProcessor
 from richard.interface.SomeSemanticComposer import SomeSemanticComposer
 
 
 class SemanticExecutor(SomeProcessor):
     """
     Executes the function that forms the meaning of the sentence, and produces its result
     """
+    
     composer: SomeSemanticComposer
 
 
     def __init__(self, composer: SomeSemanticComposer) -> None:
         super().__init__()
         self.composer = composer    
 
     
-    def process(self, request: SentenceRequest):
+    def process(self, request: SentenceRequest) -> ProcessResult:
         semantic_function = self.composer.get_semantic_function(request)
         results = [semantic_function()]
-        return results
+        return ProcessResult(results, "", [])
 
 
     def get_results(self, request: SentenceRequest) -> list:
         return request.get_current_product(self)
```

### Comparing `richard-0.1.0/richard/semantics/commands.py` & `richard-0.2.0/richard/semantics/commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     elements = nbar()
     range_count = len(elements)
 
     result = []
     for element in elements:
         for e2 in vp(element):
             result.append(element)
+
     result = list(set(result))
     result_count = len(result)
+    
     if qp(result_count, range_count):
         return result
     else:
         return []
```

### Comparing `richard-0.1.0/richard.egg-info/SOURCES.txt` & `richard-0.2.0/richard.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 LICENSE
 README.md
 setup.py
 docs/__init__.py
+richard/Domain.py
 richard/Pipeline.py
 richard/__init__.py
 richard/constants.py
 richard.egg-info/PKG-INFO
 richard.egg-info/SOURCES.txt
 richard.egg-info/dependency_links.txt
 richard.egg-info/top_level.txt
+richard/block/FindAll.py
+richard/block/FindOne.py
+richard/block/Succeed.py
+richard/block/TryFirst.py
+richard/block/__init__.py
+richard/entity/BlockResult.py
+richard/entity/ControlBlock.py
+richard/entity/Entity.py
 richard/entity/GrammarRule.py
 richard/entity/GrammarRules.py
 richard/entity/Log.py
-richard/entity/ParseResult.py
 richard/entity/ParseTreeNode.py
-richard/entity/Record.py
-richard/entity/RecordSet.py
+richard/entity/ProcessResult.py
+richard/entity/Relation.py
 richard/entity/RuleConstituent.py
 richard/entity/SentenceRequest.py
 richard/entity/__init__.py
 richard/interface/SomeLanguageSelector.py
 richard/interface/SomeLogger.py
 richard/interface/SomeParser.py
 richard/interface/SomeProcessor.py
@@ -47,17 +55,24 @@
 richard/processor/semantic_executor/SemanticExecutor.py
 richard/processor/semantic_executor/__init__.py
 richard/processor/tokenizer/BasicTokenizer.py
 richard/processor/tokenizer/__init__.py
 richard/semantics/__init__.py
 richard/semantics/commands.py
 richard/store/MemoryDb.py
+richard/store/Record.py
+richard/store/RecordSet.py
 richard/store/__init__.py
 richard/type/PositionType.py
 richard/type/SimpleGrammar.py
 richard/type/SimpleGrammarRule.py
 richard/type/__init__.py
+tests/Chat80_test.py
+tests/Composer_test.py
 tests/EarleyParser_test.py
+tests/Executor_test.py
 tests/Multilingual_test.py
 tests/Parser_test.py
+tests/Postgres_test.py
 tests/Quantifier_test.py
+tests/Tokenizer_test.py
 tests/__init__.py
```

### Comparing `richard-0.1.0/setup.py` & `richard-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='richard',
-    version='0.1.0',    
+    version='0.2.0',    
     description='A Natural Language Understanding and Execution library',
     url='https://github.com/garfix/richard',
     author='Patrick van Bergen',
     author_email='patrick.vanbergen@gmail.com',
     license='MIT',
     packages=find_packages(),
     install_requires=[],
```

### Comparing `richard-0.1.0/tests/EarleyParser_test.py` & `richard-0.2.0/tests/EarleyParser_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,13 @@
                 [RuleConstituent("john", [], POS_TYPE_WORD_FORM)],
                 lambda sem: sem
             ),
         ])
         parser = EarleyParser()
         result = parser.parse(grammarRules, ["John", "loves", "Mary"])
                     
-        self.assertEqual(len(result.trees), 4)
-        self.assertEqual(result.trees[0].inline_str(), "s(np(noun(john 'John')) verb(loves 'loves') np(noun(proper_noun(mary 'Mary'))))")
-        self.assertEqual(result.trees[1].inline_str(), "s(np(noun(proper_noun(john 'John'))) verb(loves 'loves') np(noun(proper_noun(mary 'Mary'))))")
-        self.assertEqual(result.trees[2].inline_str(), "s(np(noun(john 'John')) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
-        self.assertEqual(result.trees[3].inline_str(), "s(np(noun(proper_noun(john 'John'))) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
+        self.assertEqual(len(result.products), 4)
+        self.assertEqual(result.products[0].inline_str(), "s(np(noun(john 'John')) verb(loves 'loves') np(noun(proper_noun(mary 'Mary'))))")
+        self.assertEqual(result.products[1].inline_str(), "s(np(noun(proper_noun(john 'John'))) verb(loves 'loves') np(noun(proper_noun(mary 'Mary'))))")
+        self.assertEqual(result.products[2].inline_str(), "s(np(noun(john 'John')) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
+        self.assertEqual(result.products[3].inline_str(), "s(np(noun(proper_noun(john 'John'))) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
```

### Comparing `richard-0.1.0/tests/Multilingual_test.py` & `richard-0.2.0/tests/Multilingual_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
 from richard.Pipeline import Pipeline
+from richard.block.FindOne import FindOne
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.processor.language_selector.LanguageSelector import LanguageSelector
 from richard.processor.language_selector.Multilingual import Multilingual
 from richard.processor.parser.BasicParser import BasicParser
 from richard.processor.tokenizer.BasicTokenizer import BasicTokenizer
 
 class TestMultilingual(unittest.TestCase):
@@ -34,17 +35,17 @@
                 { "syn": "verb -> 'houdt' 'van'" },
             ], tokenizer)
         }
 
         parser = Multilingual(parsers, language_selector)
 
         pipeline = Pipeline([
-            language_selector,
-            tokenizer,
-            parser
+            FindOne(language_selector),
+            FindOne(tokenizer),
+            FindOne(parser)
         ])
 
         request = SentenceRequest("John loves Mary")
 
         pipeline.enter(request)
         tree = parser.get_product(request)
         self.assertEqual(tree.inline_str(), "s(np(noun(proper_noun(john 'John'))) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
```

### Comparing `richard-0.1.0/tests/Parser_test.py` & `richard-0.2.0/tests/Parser_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
 from richard.Pipeline import Pipeline
+from richard.block.FindOne import FindOne
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.processor.parser.BasicParser import BasicParser
 from richard.processor.tokenizer.BasicTokenizer import BasicTokenizer
 
 class TestParser(unittest.TestCase):
    
     def test_parser_process(self):
@@ -19,17 +20,31 @@
             { "syn": "verb -> 'loves'" },
         ]
 
         tokenizer = BasicTokenizer()
         parser = BasicParser(grammar, tokenizer)
 
         pipeline = Pipeline([
-            tokenizer,
-            parser
+            FindOne(tokenizer),
+            FindOne(parser)
         ])
 
         request = SentenceRequest("John loves Mary")
         pipeline.enter(request)
 
         tree = parser.get_tree(request)
         self.assertEqual(tree.inline_str(), "s(np(noun(proper_noun(john 'John'))) vp(verb(loves 'loves') np(noun(proper_noun(mary 'Mary')))))")
-    
+    
+
+    def test_syntax_error(self):
+        grammar = [
+            { "syn": "s => proper_noun verb" },
+            { "syn": "proper_noun -> 'mary'" },
+            { "syn": "verb -> 'walks'" },
+        ]
+
+        tokenizer = BasicTokenizer()
+
+        try:
+            parser = BasicParser(grammar, tokenizer)
+        except Exception as e:
+            self.assertEqual(str(e), "Could not parse 'syn' value: s => proper_noun verb")
```

### Comparing `richard-0.1.0/tests/Quantifier_test.py` & `richard-0.2.0/tests/Quantifier_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 import unittest
 
+from richard.Domain import Domain
 from richard.Pipeline import Pipeline
-from richard.entity.Record import Record
+from richard.block.FindOne import FindOne
+from richard.entity.Entity import Entity
+from richard.entity.Relation import Relation
+from richard.store.Record import Record
 from richard.entity.SentenceRequest import SentenceRequest
 from richard.processor.parser.BasicParser import BasicParser
 from richard.processor.semantic_composer.SemanticComposer import SemanticComposer
 from richard.processor.semantic_executor.SemanticExecutor import SemanticExecutor
 from richard.processor.tokenizer.BasicTokenizer import BasicTokenizer
 from richard.semantics.commands import find
 from richard.store.MemoryDb import MemoryDb
 
 
 class TestQuantifier(unittest.TestCase):
    
     def test_quantifier(self):
 
         db = MemoryDb()
-        db.assert_record(Record('has_child', {'parent': 'mary', 'child': 'lucy'}))
-        db.assert_record(Record('has_child', {'parent': 'mary', 'child': 'bonny'}))
-        db.assert_record(Record('has_child', {'parent': 'barbara', 'child': 'john'}))
-        db.assert_record(Record('has_child', {'parent': 'barbara', 'child': 'chuck'}))
-        db.assert_record(Record('has_child', {'parent': 'william', 'child': 'oswald'}))
-        db.assert_record(Record('has_child', {'parent': 'william', 'child': 'bertrand'}))
+        db.insert(Record('has_child', {'parent': 'mary', 'child': 'lucy'}))
+        db.insert(Record('has_child', {'parent': 'mary', 'child': 'bonny'}))
+        db.insert(Record('has_child', {'parent': 'barbara', 'child': 'john'}))
+        db.insert(Record('has_child', {'parent': 'barbara', 'child': 'chuck'}))
+        db.insert(Record('has_child', {'parent': 'william', 'child': 'oswald'}))
+        db.insert(Record('has_child', {'parent': 'william', 'child': 'bertrand'}))
+
+        domain = Domain([
+            Entity("parent", lambda: db.select(Record('has_child')).field('parent')),
+            Entity("child", lambda: db.select(Record('has_child')).field('child')),
+        ], [
+            Relation("has_child", ['parent', 'child'], lambda parent, child: db.select(Record('has_child', {'parent': parent, 'child': child}))),
+        ])
 
         grammar = [
             { 
                 "syn": "s -> np vp_no_sub", 
                 "sem": lambda np, vp_no_sub: lambda: find(np(), vp_no_sub) 
             },
             { 
                 "syn": "vp_no_sub -> aux qp child", 
-                "sem": lambda aux, qp, parent:
-                        lambda sub: find(
-                            (qp, parent),
-                            lambda obj: db.match(Record('has_child', {'parent': sub, 'child': obj})))
+                "sem": lambda aux, qp, child:
+                        lambda subject: find(
+                            (qp, child),
+                            lambda object: domain.relation_exists('has_child', [subject, object]))
             },
             { 
                 "syn": "np -> qp nbar", 
                 "sem": lambda qp, nbar:  lambda: (qp, nbar) 
             },
             { 
                 "syn": "qp -> det", 
@@ -50,29 +61,29 @@
             },
             { 
                 "syn": "det -> number", 
                 "sem": lambda number: lambda result, range: result == number() 
             },
             { "syn": "number -> 'two'", "sem": lambda: lambda: 2 },
             { "syn": "number -> 'three'", "sem": lambda: lambda: 3 },
-            { "syn": "noun -> 'parent'", "sem": lambda: lambda: db.match(Record('has_child')).field('parent') },
-            { "syn": "child -> 'children'", "sem": lambda: lambda: db.match(Record('has_child')).field('child') },
+            { "syn": "noun -> 'parent'", "sem": lambda: lambda: domain.get_entity_ids('parent') },
+            { "syn": "child -> 'children'", "sem": lambda: lambda: domain.get_entity_ids('child') },
             { "syn": "aux -> 'has'", "sem": lambda: lambda: None },
         ]
 
         tokenizer = BasicTokenizer()
         parser = BasicParser(grammar, tokenizer)
         composer = SemanticComposer(parser)
         executor = SemanticExecutor(composer)
 
         pipeline = Pipeline([
-            tokenizer,
-            parser,
-            composer,
-            executor
+            FindOne(tokenizer),
+            FindOne(parser),
+            FindOne(composer),
+            FindOne(executor)
         ])
 
         request = SentenceRequest("Every parent has two children")
         pipeline.enter(request)
         results = executor.get_results(request)
         self.assertEqual(len(results), 3)
```

