# Comparing `tmp/types-antlr4-python3-runtime-4.13.0.20240331.tar.gz` & `tmp/types-antlr4-python3-runtime-4.13.0.20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-antlr4-python3-runtime-4.13.0.20240331.tar", last modified: Sun Mar 31 02:18:04 2024, max compression
+gzip compressed data, was "types-antlr4-python3-runtime-4.13.0.20240519.tar", last modified: Sun May 19 02:23:38 2024, max compression
```

## Comparing `types-antlr4-python3-runtime-4.13.0.20240331.tar` & `types-antlr4-python3-runtime-4.13.0.20240519.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.607502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/BufferedTokenStream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/CommonTokenFactory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/CommonTokenStream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/FileStream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/InputStream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/IntervalSet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/LL1Analyzer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Lexer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ListTokenSource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Parser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ParserInterpreter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ParserRuleContext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/PredictionContext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Recognizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/RuleContext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/StdinStream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/TokenStreamRewriter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/_pygrun.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATN.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNConfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNConfigSet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNDeserializationOptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNDeserializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNSimulator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNState.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNType.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerATNSimulator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerAction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerActionExecutor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ParserATNSimulator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/PredictionMode.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/SemanticContext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/Transition.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFA.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFASerializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFAState.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/DiagnosticErrorListener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/ErrorListener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/ErrorStrategy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/Errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/Chunk.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreeMatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreePattern.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreePatternMatcher.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/RuleTagToken.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/TokenTagToken.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/Tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/Trees.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/XPath.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/XPathLexer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:04.611502 types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-31 02:18:04.000000 types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.142804 types-antlr4-python3-runtime-4.13.0.20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-19 02:23:35.000000 types-antlr4-python3-runtime-4.13.0.20240519/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:23:35.000000 types-antlr4-python3-runtime-4.13.0.20240519/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-19 02:23:38.142804 types-antlr4-python3-runtime-4.13.0.20240519/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.134804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/BufferedTokenStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/CommonTokenFactory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/CommonTokenStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/FileStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/InputStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/IntervalSet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/LL1Analyzer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Lexer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ListTokenSource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 02:23:35.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ParserInterpreter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ParserRuleContext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/PredictionContext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Recognizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/RuleContext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/StdinStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/TokenStreamRewriter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/_pygrun.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.138804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATN.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNConfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNConfigSet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNDeserializationOptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNDeserializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNSimulator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNState.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNType.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerATNSimulator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerAction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerActionExecutor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ParserATNSimulator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/PredictionMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/SemanticContext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/Transition.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.138804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFA.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFASerializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFAState.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.138804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/DiagnosticErrorListener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/ErrorListener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/ErrorStrategy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/Errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:35.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.138804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/Chunk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreeMatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreePattern.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreePatternMatcher.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/RuleTagToken.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/TokenTagToken.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/Tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/Trees.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.138804 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/XPath.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/XPathLexer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:23:38.142804 types-antlr4-python3-runtime-4.13.0.20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-19 02:23:35.000000 types-antlr4-python3-runtime-4.13.0.20240519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:38.142804 types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-19 02:23:38.000000 types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-19 02:23:38.000000 types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:23:38.000000 types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 02:23:38.000000 types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/top_level.txt
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/PKG-INFO` & `types-antlr4-python3-runtime-4.13.0.20240519/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-antlr4-python3-runtime
-Version: 4.13.0.20240331
+Version: 4.13.0.20240519
 Summary: Typing stubs for antlr4-python3-runtime
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/antlr4-python3-runtime.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-antlr4-python3-runtime` aims to provide accurate annotations
 for `antlr4-python3-runtime==4.13.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/antlr4-python3-runtime. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/BufferedTokenStream.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/BufferedTokenStream.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/CommonTokenStream.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/CommonTokenStream.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/InputStream.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/InputStream.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/IntervalSet.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/IntervalSet.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/LL1Analyzer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/LL1Analyzer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Lexer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Lexer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ListTokenSource.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ListTokenSource.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Parser.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Parser.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ParserInterpreter.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ParserInterpreter.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/ParserRuleContext.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/ParserRuleContext.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/PredictionContext.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/PredictionContext.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Recognizer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Recognizer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/RuleContext.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/RuleContext.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/Token.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/Token.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/TokenStreamRewriter.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/TokenStreamRewriter.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/__init__.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATN.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATN.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNConfig.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNConfig.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNConfigSet.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNConfigSet.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNDeserializer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNDeserializer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNSimulator.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNSimulator.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ATNState.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ATNState.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerATNSimulator.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerATNSimulator.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerAction.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerAction.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from _typeshed import Incomplete
 from enum import IntEnum
 
 Lexer: Incomplete
 
 class LexerActionType(IntEnum):
-    CHANNEL: int
-    CUSTOM: int
-    MODE: int
-    MORE: int
-    POP_MODE: int
-    PUSH_MODE: int
-    SKIP: int
-    TYPE: int
+    CHANNEL = 0
+    CUSTOM = 1
+    MODE = 2
+    MORE = 3
+    POP_MODE = 4
+    PUSH_MODE = 5
+    SKIP = 6
+    TYPE = 7
 
 class LexerAction:
     actionType: Incomplete
     isPositionDependent: bool
     def __init__(self, action: LexerActionType) -> None: ...
     def __hash__(self): ...
     def __eq__(self, other): ...
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/LexerActionExecutor.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/LexerActionExecutor.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/ParserATNSimulator.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/ParserATNSimulator.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/PredictionMode.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/PredictionMode.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from antlr4.atn.ATN import ATN as ATN
 from antlr4.atn.ATNConfig import ATNConfig as ATNConfig
 from antlr4.atn.ATNConfigSet import ATNConfigSet as ATNConfigSet
 from antlr4.atn.ATNState import RuleStopState as RuleStopState
 from antlr4.atn.SemanticContext import SemanticContext as SemanticContext
 
 class PredictionMode(Enum):
-    SLL: int
-    LL: int
-    LL_EXACT_AMBIG_DETECTION: int
+    SLL = 0
+    LL = 1
+    LL_EXACT_AMBIG_DETECTION = 2
     @classmethod
     def hasSLLConflictTerminatingPrediction(cls, mode: PredictionMode, configs: ATNConfigSet): ...
     @classmethod
     def hasConfigInRuleStopState(cls, configs: ATNConfigSet): ...
     @classmethod
     def allConfigsInRuleStopStates(cls, configs: ATNConfigSet): ...
     @classmethod
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/SemanticContext.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/SemanticContext.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/atn/Transition.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/atn/Transition.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFA.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFA.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFASerializer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFASerializer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/dfa/DFAState.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/dfa/DFAState.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/DiagnosticErrorListener.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/DiagnosticErrorListener.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/ErrorListener.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/ErrorListener.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/ErrorStrategy.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/ErrorStrategy.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/error/Errors.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/error/Errors.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreeMatch.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreeMatch.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreePattern.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreePattern.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/ParseTreePatternMatcher.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/ParseTreePatternMatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/Tree.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/Tree.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/tree/Trees.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/tree/Trees.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/XPath.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/XPath.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/antlr4-stubs/xpath/XPathLexer.pyi` & `types-antlr4-python3-runtime-4.13.0.20240519/antlr4-stubs/xpath/XPathLexer.pyi`

 * *Files identical despite different names*

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/setup.py` & `types-antlr4-python3-runtime-4.13.0.20240519/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-antlr4-python3-runtime` aims to provide accurate annotations
 for `antlr4-python3-runtime==4.13.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/antlr4-python3-runtime. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="4.13.0.20240331",
+      version="4.13.0.20240519",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/antlr4-python3-runtime.md",
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/PKG-INFO` & `types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-antlr4-python3-runtime
-Version: 4.13.0.20240331
+Version: 4.13.0.20240519
 Summary: Typing stubs for antlr4-python3-runtime
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/antlr4-python3-runtime.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-antlr4-python3-runtime` aims to provide accurate annotations
 for `antlr4-python3-runtime==4.13.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/antlr4-python3-runtime. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-antlr4-python3-runtime-4.13.0.20240331/types_antlr4_python3_runtime.egg-info/SOURCES.txt` & `types-antlr4-python3-runtime-4.13.0.20240519/types_antlr4_python3_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

