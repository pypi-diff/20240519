# Comparing `tmp/RiskQuantLib-0.3.7.tar.gz` & `tmp/riskquantlib-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskQuantLib-0.3.7.tar", last modified: Mon Dec 18 12:34:35 2023, max compression
+gzip compressed data, was "riskquantlib-0.3.8.tar", last modified: Sun May 19 13:57:25 2024, max compression
```

## Comparing `RiskQuantLib-0.3.7.tar` & `riskquantlib-0.3.8.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.155195 RiskQuantLib-0.3.7/
--rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 RiskQuantLib-0.3.7/LICENSE
--rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 RiskQuantLib-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1221 2023-12-18 12:34:35.155195 RiskQuantLib-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 RiskQuantLib-0.3.7/README.md
--rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 RiskQuantLib-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-18 12:34:35.159200 RiskQuantLib-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-12-18 12:29:18.000000 RiskQuantLib-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.080356 RiskQuantLib-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.084860 RiskQuantLib-0.3.7/src/RiskQuantLib/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.108910 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/Instrument/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/Instrument/__init__.py
--rw-rw-rw-   0        0        0      388 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/InstrumentList/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0      409 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Auto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
--rw-rw-rw-   0        0        0      351 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
--rw-rw-rw-   0        0        0      355 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
--rw-rw-rw-   0        0        0      402 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
--rw-rw-rw-   0        0        0      369 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.110341 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
--rw-rw-rw-   0        0        0     1474 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
--rw-rw-rw-   0        0        0     2151 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
--rw-rw-rw-   0        0        0     1515 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
--rw-rw-rw-   0        0        0     1101 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/__init__.py
--rw-rw-rw-   0        0        0    14083 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/macro.pyt
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/__init__.py
--rw-rw-rw-   0        0        0    47031 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/builder.py
--rw-rw-rw-   0        0        0     8192 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/controller.py
--rw-rw-rw-   0        0        0     9325 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/debugger.py
--rw-rw-rw-   0        0        0     1637 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/render.py
--rw-rw-rw-   0        0        0     8835 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/router.py
--rw-rw-rw-   0        0        0     6073 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Build/tree.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.119346 RiskQuantLib-0.3.7/src/RiskQuantLib/Instrument/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Instrument/__init__.py
--rw-rw-rw-   0        0        0      935 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Instrument/instrument.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.120265 RiskQuantLib-0.3.7/src/RiskQuantLib/InstrumentList/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/InstrumentList/__init__.py
--rw-rw-rw-   0        0        0     1470 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/InstrumentList/instrumentList.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.120265 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.120265 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/Copula/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/Copula/__init__.py
--rw-rw-rw-   0        0        0     1207 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/Copula/copula.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.120265 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/KMV/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/KMV/__init__.py
--rw-rw-rw-   0        0        0     2181 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/KMV/kmv.py
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/__init__.py
--rw-rw-rw-   0        0        0      274 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Model/model.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.122770 RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/iloc.py
--rw-rw-rw-   0        0        0     1107 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/loc.py
--rw-rw-rw-   0        0        0    66940 2023-12-18 12:20:10.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/operation.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.122770 RiskQuantLib-0.3.7/src/RiskQuantLib/Property/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Property/__init__.py
--rw-rw-rw-   0        0        0     1106 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Property/property.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.132687 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/
--rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/__init__.py
--rw-rw-rw-   0        0        0     6514 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/codeBuilderTool.py
--rw-rw-rw-   0        0        0    10785 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/databaseTool.py
--rw-rw-rw-   0        0        0      672 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/decoratorTool.py
--rw-rw-rw-   0        0        0     1593 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/excelTool.py
--rw-rw-rw-   0        0        0    19765 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/fileTool.py
--rw-rw-rw-   0        0        0     4862 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/githubTool.py
--rw-rw-rw-   0        0        0     4368 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/guiTool.py
--rw-rw-rw-   0        0        0     2817 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/mathTool.py
--rw-rw-rw-   0        0        0     1158 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/multiThreadTool.py
--rw-rw-rw-   0        0        0     4705 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/outlookTool.py
--rw-rw-rw-   0        0        0     4487 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/plotTool.py
--rw-rw-rw-   0        0        0     9707 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/pptTool.py
--rw-rw-rw-   0        0        0     9605 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/strTool.py
--rw-rw-rw-   0        0        0     6111 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/wordTool.py
--rw-rw-rw-   0        0        0    39083 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/__init__.py
--rw-rw-rw-   0        0        0      665 2023-12-18 12:13:16.000000 RiskQuantLib-0.3.7/src/RiskQuantLib/module.py
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.155195 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/
--rw-rw-rw-   0        0        0     1221 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3049 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      619 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-12-18 12:34:35.000000 RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-18 12:34:35.155195 RiskQuantLib-0.3.7/src/TestCode/
--rw-rw-rw-   0        0        0     8746 2023-04-12 02:11:42.000000 RiskQuantLib-0.3.7/src/TestCode/Test.py
--rw-rw-rw-   0        0        0        0 2021-04-28 07:07:13.000000 RiskQuantLib-0.3.7/src/TestCode/__init__.py
--rw-rw-rw-   0        0        0      119 2022-10-11 12:38:30.000000 RiskQuantLib-0.3.7/src/TestCode/a.py
--rw-rw-rw-   0        0        0     3989 2021-06-03 09:15:00.000000 RiskQuantLib-0.3.7/src/TestCode/bond.py
--rw-rw-rw-   0        0        0     2310 2021-07-07 08:09:00.000000 RiskQuantLib-0.3.7/src/TestCode/newProject.py
--rw-rw-rw-   0        0        0     4766 2021-06-25 09:35:46.000000 RiskQuantLib-0.3.7/src/TestCode/pathObj.py
--rw-rw-rw-   0        0        0      477 2021-07-02 09:23:16.000000 RiskQuantLib-0.3.7/src/TestCode/shitBond.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.218504 riskquantlib-0.3.8/
+-rw-rw-rw-   0        0        0     1091 2021-03-25 06:21:56.000000 riskquantlib-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-01-06 05:45:25.000000 riskquantlib-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1221 2024-05-19 13:57:25.218504 riskquantlib-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2021-09-05 04:59:33.000000 riskquantlib-0.3.8/README.md
+-rw-rw-rw-   0        0        0      179 2022-06-23 07:53:24.000000 riskquantlib-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 13:57:25.218504 riskquantlib-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2024-05-19 13:56:28.000000 riskquantlib-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.906361 riskquantlib-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.935711 riskquantlib-0.3.8/src/RiskQuantLib/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.951290 riskquantlib-0.3.8/src/RiskQuantLib/Auto/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.951290 riskquantlib-0.3.8/src/RiskQuantLib/Auto/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Auto/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      388 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Auto/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.951290 riskquantlib-0.3.8/src/RiskQuantLib/Auto/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Auto/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Auto/InstrumentList/instrumentList.py
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Auto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.998195 riskquantlib-0.3.8/src/RiskQuantLib/Build/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:24.998195 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.029541 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt
+-rw-rw-rw-   0        0        0      351 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/module.pyt
+-rw-rw-rw-   0        0        0      355 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttribute.pyt
+-rw-rw-rw-   0        0        0      402 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/setAttributeList.pyt
+-rw-rw-rw-   0        0        0      369 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/sourceCodeDebugger.pyt
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.060776 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt
+-rw-rw-rw-   0        0        0     1474 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt
+-rw-rw-rw-   0        0        0     2151 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt
+-rw-rw-rw-   0        0        0     1515 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt
+-rw-rw-rw-   0        0        0     1101 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/__init__.py
+-rw-rw-rw-   0        0        0    14083 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/macro.pyt
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/__init__.py
+-rw-rw-rw-   0        0        0    47031 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/builder.py
+-rw-rw-rw-   0        0        0     8473 2024-05-19 13:30:40.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/controller.py
+-rw-rw-rw-   0        0        0     9325 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/debugger.py
+-rw-rw-rw-   0        0        0     1637 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/render.py
+-rw-rw-rw-   0        0        0     8835 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/router.py
+-rw-rw-rw-   0        0        0     6073 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Build/tree.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.060776 riskquantlib-0.3.8/src/RiskQuantLib/Instrument/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Instrument/__init__.py
+-rw-rw-rw-   0        0        0      935 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Instrument/instrument.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.060776 riskquantlib-0.3.8/src/RiskQuantLib/InstrumentList/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/InstrumentList/__init__.py
+-rw-rw-rw-   0        0        0     1470 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/InstrumentList/instrumentList.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.060776 riskquantlib-0.3.8/src/RiskQuantLib/Model/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.076413 riskquantlib-0.3.8/src/RiskQuantLib/Model/Copula/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/Copula/__init__.py
+-rw-rw-rw-   0        0        0     1207 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/Copula/copula.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.076413 riskquantlib-0.3.8/src/RiskQuantLib/Model/KMV/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/KMV/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/KMV/kmv.py
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/__init__.py
+-rw-rw-rw-   0        0        0      274 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.092795 riskquantlib-0.3.8/src/RiskQuantLib/Operation/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Operation/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Operation/iloc.py
+-rw-rw-rw-   0        0        0     1107 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Operation/loc.py
+-rw-rw-rw-   0        0        0    69812 2024-05-19 13:50:19.000000 riskquantlib-0.3.8/src/RiskQuantLib/Operation/operation.py
+-rw-rw-rw-   0        0        0     1415 2024-05-19 13:51:49.000000 riskquantlib-0.3.8/src/RiskQuantLib/Operation/vectorization.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.092795 riskquantlib-0.3.8/src/RiskQuantLib/Property/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Property/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Property/property.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.189727 riskquantlib-0.3.8/src/RiskQuantLib/Tool/
+-rw-rw-rw-   0        0        0        0 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/codeBuilderTool.py
+-rw-rw-rw-   0        0        0    10785 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/databaseTool.py
+-rw-rw-rw-   0        0        0      672 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/decoratorTool.py
+-rw-rw-rw-   0        0        0     1593 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/excelTool.py
+-rw-rw-rw-   0        0        0    21495 2024-05-19 13:30:40.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/fileTool.py
+-rw-rw-rw-   0        0        0     4862 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/githubTool.py
+-rw-rw-rw-   0        0        0     4368 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/guiTool.py
+-rw-rw-rw-   0        0        0     2817 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/mathTool.py
+-rw-rw-rw-   0        0        0     1158 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/multiThreadTool.py
+-rw-rw-rw-   0        0        0     4705 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/outlookTool.py
+-rw-rw-rw-   0        0        0     4487 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/plotTool.py
+-rw-rw-rw-   0        0        0     9707 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/pptTool.py
+-rw-rw-rw-   0        0        0     9605 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/strTool.py
+-rw-rw-rw-   0        0        0     6111 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/Tool/wordTool.py
+-rw-rw-rw-   0        0        0    39083 2023-12-18 12:13:16.000000 riskquantlib-0.3.8/src/RiskQuantLib/__init__.py
+-rw-rw-rw-   0        0        0      749 2024-05-19 13:30:40.000000 riskquantlib-0.3.8/src/RiskQuantLib/module.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.218504 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/
+-rw-rw-rw-   0        0        0     1221 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3093 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      619 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-19 13:57:24.000000 riskquantlib-0.3.8/src/RiskQuantLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 13:57:25.218504 riskquantlib-0.3.8/src/TestCode/
+-rw-rw-rw-   0        0        0     8746 2023-04-12 02:11:42.000000 riskquantlib-0.3.8/src/TestCode/Test.py
+-rw-rw-rw-   0        0        0        0 2021-04-28 07:07:13.000000 riskquantlib-0.3.8/src/TestCode/__init__.py
+-rw-rw-rw-   0        0        0      119 2022-10-11 12:38:30.000000 riskquantlib-0.3.8/src/TestCode/a.py
+-rw-rw-rw-   0        0        0     3989 2021-06-03 09:15:00.000000 riskquantlib-0.3.8/src/TestCode/bond.py
+-rw-rw-rw-   0        0        0     2310 2021-07-07 08:09:00.000000 riskquantlib-0.3.8/src/TestCode/newProject.py
+-rw-rw-rw-   0        0        0     4766 2021-06-25 09:35:46.000000 riskquantlib-0.3.8/src/TestCode/pathObj.py
+-rw-rw-rw-   0        0        0      477 2021-07-02 09:23:16.000000 riskquantlib-0.3.8/src/TestCode/shitBond.py
```

### Comparing `RiskQuantLib-0.3.7/LICENSE` & `riskquantlib-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/PKG-INFO` & `riskquantlib-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.3.7
+Version: 0.3.8
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.3.7/README.md` & `riskquantlib-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/setup.py` & `riskquantlib-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RiskQuantLib",
-    version="0.3.7",
+    version="0.3.8",
     author="Syuya_Murakami",
     author_email="wxy135@mail.ustc.edu.cn",
     description="RiskQuantLib is a QuantLib derivative to evaluate risk.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://riskquantlib-doc.readthedocs.io/en/latest/index.html",
     project_urls={
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/ContentGenerator/filePath.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrument.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentList.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/instrumentListAuto.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/FileInitiator/property.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/Component/macro.pyt` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/Component/macro.pyt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/builder.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/builder.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/controller.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def linkController(linkToBuilder, controlSyntaxList:list):
         """
         Given original builder, create a new builder, this new builder will copy all build path of original builder, but use
         additional build information declared by declaration content to modify itself. Then the new builder will trigger a
         build action. This function will return the new builder as a mimic one of original builder.
         """
         from RiskQuantLib.Build.builder import validateBuilder,builder
-        [linkToBuilder.mimicBuilder.bindContent("", bindType=bt, persist=False) for bt in linkToBuilder.mimicBuilder.bindType] if hasattr(linkToBuilder,'mimicBuilder') and isinstance(linkToBuilder.mimicBuilder,builder) else None
+        [linkToBuilder.mimicBuilder.bindContent("", bindType=bt, persist=False) for bt in linkToBuilder.mimicBuilder.bindType] if hasattr(linkToBuilder,'mimicBuilder') and isinstance(linkToBuilder.mimicBuilder,builder) and (linkToBuilder.buildFromPath, linkToBuilder.projectPath, linkToBuilder.targetPath, linkToBuilder.templatePath) == (linkToBuilder.mimicBuilder.buildFromPath, linkToBuilder.mimicBuilder.projectPath, linkToBuilder.mimicBuilder.targetPath, linkToBuilder.mimicBuilder.templatePath) else None
         mimicBuilder = validateBuilder()
         mimicBuilder.projectPath = linkToBuilder.projectPath
         mimicBuilder.targetPath = linkToBuilder.targetPath
         mimicBuilder.buildFromPath = linkToBuilder.buildFromPath
         mimicBuilder.templatePath = linkToBuilder.templatePath
         mimicBuilder.instrumentTree = linkToBuilder.instrumentTree.copy()
         mimicBuilder.propertyTree = linkToBuilder.propertyTree.copy()
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/debugger.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/debugger.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/render.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/render.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/router.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/router.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Build/tree.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Build/tree.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Instrument/instrument.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Instrument/instrument.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/InstrumentList/instrumentList.py` & `riskquantlib-0.3.8/src/RiskQuantLib/InstrumentList/instrumentList.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Model/Copula/copula.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Model/Copula/copula.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Model/KMV/kmv.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Model/KMV/kmv.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/iloc.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Operation/iloc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/loc.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Operation/loc.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Operation/operation.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Operation/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
 #coding = utf-8
 import numpy as np
 import copy
 from collections.abc import Iterable
 import pandas as pd
 from RiskQuantLib.Operation.loc import loc
+from RiskQuantLib.Operation.vectorization import vectorization
 from RiskQuantLib.Tool.strTool import changeSecurityListToStr
 #<import>
 #</import>
 
 class operation(object):
     """
     operation() is the function class that makes all RiskQuantLib list object functional.
@@ -341,16 +342,14 @@
             result = self.new()
             result.setAll([[j for j in self.all if getattr(j,attrNameString) == i][keepIndex] for i in propertyValueList])
             return result
 
     def apply(self,applyFunction,*args):
         """
         This function will apply the given function to each element of RiskQuantLib list.
-        Default settings will leave any change to element out. Your change to elements won't
-        be kept. Only the result of applyFunction is returned.
         """
         result = [applyFunction(i,*args) for i in self.all]
         tmp = operation()
         tmp.setAll(result)
         return tmp
 
     def groupBy(self, attrName:str, useObj = True, inplace = True):
@@ -560,14 +559,72 @@
             tmp.setAll(result)
             self._paraQueue = []
             return tmp
         except Exception as e:
             print('Parallel Failed:', e)
             pass
 
+    def vecApply(self, lambdaFunction=lambda x: None):
+        """
+        This function is like operation.apply, it will apply the given function to each 
+        element of RiskQuantLib list. The passed function should be one-parameter function,
+        whose parameter represents the element of current RiskQuantLib list.
+
+        The difference is this function will try to vectorize the calculation to speed up.
+        It will convert the attribute to np.array and operate mathematical calculation.
+
+        Notice: Only Pure Mathematic Function can be vectorized, this is to say, any logic key word
+        of python, like 'in', 'if', 'for', etc, can Not be used in passed function. If must be pure
+        math formula. Luckily, all numpy function can be used. If you want to do some logistic calculation,
+        you should make sure you write function as logic-matrix-like.
+
+        Returns
+        -------
+        operation
+        """
+        allElement = self.all
+        if len(allElement) != 0:
+            dynamicClass = type('tmp', (vectorization,), {'lambdaFuncName': lambdaFunction})
+            dynamicObj = dynamicClass(allElement)
+            result = super(vectorization, dynamicObj).__getattribute__('lambdaFuncName')()
+            del dynamicObj, dynamicClass
+            return self if result is None else result
+        else:
+            return self
+
+    def vecFunc(self, functionName, *args, **kwargs):
+        """
+        This function is like operation.execFunc, it will call the given function of each 
+        element of RiskQuantLib list. The passed function should be the attribute function 
+        of element of current RiskQuantLib List.
+
+        The difference is this function will try to vectorize the calculation to speed up.
+        It will convert the attribute to np.array and operate mathematical calculation.
+
+        Notice: Only Pure Mathematic Function can be vectorized, this is to say, any logic key word
+        of python, like 'in', 'if', 'for', etc, can Not be used in passed function. If must be pure
+        math formula. Luckily, all numpy function can be used. If you want to do some logistic calculation,
+        you should make sure you write function as logic-matrix-like.
+
+        Returns
+        -------
+        operation
+        """
+        allElement = self.all
+        if len(allElement) != 0:
+            functionObj = getattr(type(allElement[0]), functionName, lambda *argsSub, **kwargsSub: None)
+            functionObjName = functionName + 'Attribute'
+            dynamicClass = type(functionName, (vectorization,), {functionObjName: functionObj})
+            dynamicObj = dynamicClass(allElement)
+            result = super(vectorization, dynamicObj).__getattribute__(functionObjName)(*args, **kwargs)
+            del dynamicObj, dynamicClass
+            return self if result is None else result
+        else:
+            return self
+
     def copy(self,deep = True):
         """
         Get a copy of present RiskQuantLib list object.
         """
         if deep:
             tmp = copy.deepcopy(self)
             tmp.__init_get_item__()
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Property/property.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Property/property.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/codeBuilderTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/codeBuilderTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/databaseTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/databaseTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/decoratorTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/decoratorTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/excelTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/excelTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/fileTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/fileTool.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,51 @@
 def loadVariable(filePath:str):
     """
     Use python module pickle to load variable.
     """
     import pickle as pkl
     return pkl.load(open(filePath,"rb"))
 
+def loadCsv(filePath:str, index_col=0):
+    """
+    Use pandas.read_csv to load csv file, default set the first column as index.
+    """
+    return pd.read_csv(filePath, index_col=index_col)
+
+def loadCsvTimeSeries(filePath:str, index_col=0, converters={0:pd.Timestamp}):
+    """
+    Use pandas.read_csv to load csv file, default set the first column as index, and set its datatype as pandas.Timestamp.
+    """
+    return pd.read_csv(filePath, index_col=index_col, converters=converters)
+
+def loadCsvDict(dirPath:str, index_col=0):
+    """
+    Read all csv file in the target directory, return a dict whose keys are file names and values are pandas.DataFrames.
+    """
+    return {i:loadCsv(dirPath+os.sep+i, index_col=index_col) for i in os.listdir(dirPath) if os.path.splitext(i)[-1] == '.csv'}
+
+def loadCsvTimeSeriesDict(dirPath:str, index_col=0, converters={0:pd.Timestamp}):
+    """
+    Read all csv file in the target directory, return a dict whose keys are file names and values are pandas.DataFrames.
+    Default set the first column of each file as index, and set its datatype as pandas.Timestamp.
+    """
+    return {i:loadCsvTimeSeries(dirPath+os.sep+i, index_col=index_col, converters=converters) for i in os.listdir(dirPath) if os.path.splitext(i)[-1] == '.csv'}
+
+def loadExcel(filePath:str):
+    """
+    Use pandas.read_excel to load csv file.
+    """
+    return pd.read_excel(filePath)
+
+def loadExcelDict(dirPath:str):
+    """
+    Read all excel file in the target directory, return a dict whose keys are file names and values are pandas.DataFrames.
+    """
+    return {i:loadExcel(dirPath+os.sep+i) for i in os.listdir(dirPath) if os.path.splitext(i)[-1] in {'.xlsx', '.xls'}}
+
 def dumpDictToJson(dictVariable:dict,filePath:str):
     """
     Dump dict to json file.
     """
     import json
     json.dump(dictVariable,open(filePath,"w",encoding='UTF-8'),ensure_ascii=False)
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/githubTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/githubTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/guiTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/guiTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/mathTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/mathTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/multiThreadTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/multiThreadTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/outlookTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/outlookTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/plotTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/plotTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/pptTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/pptTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/strTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/strTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/Tool/wordTool.py` & `riskquantlib-0.3.8/src/RiskQuantLib/Tool/wordTool.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/__init__.py` & `riskquantlib-0.3.8/src/RiskQuantLib/__init__.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib/module.py` & `riskquantlib-0.3.8/src/RiskQuantLib/module.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #<import>
 #</import>
 
 from RiskQuantLib.Tool import mathTool
 from RiskQuantLib.Tool import fileTool
 from RiskQuantLib.Tool import plotTool
 from RiskQuantLib.Tool import strTool
-from RiskQuantLib.Tool.fileTool import loadVariable,dumpVariable
+from RiskQuantLib.Tool.fileTool import loadVariable,dumpVariable,loadExcel,loadExcelDict,loadCsv,loadCsvTimeSeries,loadCsvDict,loadCsvTimeSeriesDict
 
 from RiskQuantLib.Build.builder import *
 from RiskQuantLib.Build.router import *
 from RiskQuantLib.Build.render import *
 from RiskQuantLib.Build.tree import *
 
 # build module, contents below will be automatically built and replaced, self-defined functions shouldn't be written here
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/PKG-INFO` & `riskquantlib-0.3.8/src/RiskQuantLib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskQuantLib
-Version: 0.3.7
+Version: 0.3.8
 Summary: RiskQuantLib is a QuantLib derivative to evaluate risk.
 Home-page: https://riskquantlib-doc.readthedocs.io/en/latest/index.html
 Author: Syuya_Murakami
 Author-email: wxy135@mail.ustc.edu.cn
 Project-URL: Bug Tracker, https://github.com/SyuyaMurakami/RiskQuantLib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/SOURCES.txt` & `riskquantlib-0.3.8/src/RiskQuantLib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 src/RiskQuantLib/Model/Copula/copula.py
 src/RiskQuantLib/Model/KMV/__init__.py
 src/RiskQuantLib/Model/KMV/kmv.py
 src/RiskQuantLib/Operation/__init__.py
 src/RiskQuantLib/Operation/iloc.py
 src/RiskQuantLib/Operation/loc.py
 src/RiskQuantLib/Operation/operation.py
+src/RiskQuantLib/Operation/vectorization.py
 src/RiskQuantLib/Property/__init__.py
 src/RiskQuantLib/Property/property.py
 src/RiskQuantLib/Tool/GUITool.py
 src/RiskQuantLib/Tool/__init__.py
 src/RiskQuantLib/Tool/codeBuilderTool.py
 src/RiskQuantLib/Tool/databaseTool.py
 src/RiskQuantLib/Tool/decoratorTool.py
```

### Comparing `RiskQuantLib-0.3.7/src/RiskQuantLib.egg-info/entry_points.txt` & `riskquantlib-0.3.8/src/RiskQuantLib.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/TestCode/Test.py` & `riskquantlib-0.3.8/src/TestCode/Test.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/TestCode/bond.py` & `riskquantlib-0.3.8/src/TestCode/bond.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/TestCode/newProject.py` & `riskquantlib-0.3.8/src/TestCode/newProject.py`

 * *Files identical despite different names*

### Comparing `RiskQuantLib-0.3.7/src/TestCode/pathObj.py` & `riskquantlib-0.3.8/src/TestCode/pathObj.py`

 * *Files identical despite different names*

