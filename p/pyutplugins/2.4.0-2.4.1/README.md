# Comparing `tmp/pyutplugins-2.4.0.tar.gz` & `tmp/pyutplugins-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutplugins-2.4.0.tar", last modified: Sat May 11 20:27:17 2024, max compression
+gzip compressed data, was "pyutplugins-2.4.1.tar", last modified: Sat May 18 23:00:04 2024, max compression
```

## Comparing `pyutplugins-2.4.0.tar` & `pyutplugins-2.4.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.758022 pyutplugins-2.4.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-26 20:44:48.000000 pyutplugins-2.4.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-11 20:27:17.757816 pyutplugins-2.4.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1856 2023-09-21 21:54:41.000000 pyutplugins-2.4.0/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1092 2024-05-10 18:22:45.000000 pyutplugins-2.4.0/pyproject.toml
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-11 20:27:17.758064 pyutplugins-2.4.0/setup.cfg
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.730224 pyutplugins-2.4.0/src/
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.733845 pyutplugins-2.4.0/src/pyutplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8405 2024-05-09 19:12:08.000000 pyutplugins-2.4.0/src/pyutplugins/ExternalTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3913 2024-05-09 18:28:12.000000 pyutplugins-2.4.0/src/pyutplugins/IPluginAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9462 2024-05-11 19:54:18.000000 pyutplugins-2.4.0/src/pyutplugins/PluginManager.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-11 20:27:12.000000 pyutplugins-2.4.0/src/pyutplugins/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.735502 pyutplugins-2.4.0/src/pyutplugins/common/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1133 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ElementTreeData.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2373 2024-04-28 17:55:59.000000 pyutplugins-2.4.0/src/pyutplugins/common/LinkMakerMixin.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      471 2024-01-27 20:56:43.000000 pyutplugins-2.4.0/src/pyutplugins/common/PluginTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.735922 pyutplugins-2.4.0/src/pyutplugins/common/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/BaseEditDialog.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.736409 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5182 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/common/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.737331 pyutplugins-2.4.0/src/pyutplugins/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/InvalidPluginExtensionException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/InvalidPluginNameException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/exceptions/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.739409 pyutplugins-2.4.0/src/pyutplugins/ioplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4236 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOAscii.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IODTD.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOGML.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOJava.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3260 2024-05-11 19:29:41.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOMermaid.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6403 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPdf.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9664 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOWxImage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8278 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOXml.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.740157 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDAttribute.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDElementTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10417 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.740630 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8649 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/GMLExporter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/UnsupportedOperation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.741357 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28064 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaReader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11176 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.741946 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13434 2024-05-11 19:55:08.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.742652 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12933 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.743641 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PythonParseException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12478 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PyutToPython.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10232 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.745333 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    54703 2024-02-05 14:09:02.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17041 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   541896 2024-02-05 14:09:03.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    35740 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.746447 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2892 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1592 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3974 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20411 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-05 02:43:00.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.747112 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4852 2024-05-01 01:58:53.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/WxImageFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.748074 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11800 2024-03-07 18:41:20.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/BasePluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/IOPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1364 2024-03-08 21:53:51.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/ToolPluginInterface.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.749715 pyutplugins-2.4.0/src/pyutplugins/plugintypes/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/ExportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/ImportDirectoryResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/InputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/MultipleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/OutputFormat.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/PluginDataTypes.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/SingleFileRequestResponse.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/plugintypes/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.750158 pyutplugins-2.4.0/src/pyutplugins/preferences/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7286 2024-01-17 21:40:45.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/PluginPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/preferences/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.752332 pyutplugins-2.4.0/src/pyutplugins/toolplugins/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1729 2024-04-25 17:28:09.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolArrangeLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5225 2024-03-11 01:31:01.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4534 2024-04-28 19:32:22.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolLoadLayout.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2024-03-08 05:03:28.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2427 2024-05-06 22:41:41.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalRouting.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4012 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSaveLayout.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2024-05-02 19:47:25.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolTransforms.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.753363 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8287 2024-03-09 15:59:30.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2069 2024-03-08 21:45:45.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-03-09 19:18:23.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-07 17:58:31.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.754240 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2001 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.755154 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9817 2024-05-10 19:24:31.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3467 2024-05-10 19:47:03.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6852 2024-05-10 19:05:00.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 21:22:45.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.755458 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      903 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/Layout.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 17:19:08.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.757383 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3560 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28457 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-11 20:27:17.757514 pyutplugins-2.4.0/src/pyutplugins.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6791 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      267 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-05-11 20:27:17.000000 pyutplugins-2.4.0/src/pyutplugins.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.038772 pyutplugins-2.4.1/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2024-04-26 20:44:48.000000 pyutplugins-2.4.1/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-18 23:00:04.038585 pyutplugins-2.4.1/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1856 2023-09-21 21:54:41.000000 pyutplugins-2.4.1/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1092 2024-05-10 18:22:45.000000 pyutplugins-2.4.1/pyproject.toml
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2024-05-18 23:00:04.038812 pyutplugins-2.4.1/setup.cfg
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.010269 pyutplugins-2.4.1/src/
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.013687 pyutplugins-2.4.1/src/pyutplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8405 2024-05-09 19:12:08.000000 pyutplugins-2.4.1/src/pyutplugins/ExternalTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3913 2024-05-09 18:28:12.000000 pyutplugins-2.4.1/src/pyutplugins/IPluginAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9462 2024-05-11 19:54:18.000000 pyutplugins-2.4.1/src/pyutplugins/PluginManager.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       45 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2024-05-13 19:09:47.000000 pyutplugins-2.4.1/src/pyutplugins/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.015334 pyutplugins-2.4.1/src/pyutplugins/common/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1133 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ElementTreeData.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2373 2024-04-28 17:55:59.000000 pyutplugins-2.4.1/src/pyutplugins/common/LinkMakerMixin.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      471 2024-01-27 20:56:43.000000 pyutplugins-2.4.1/src/pyutplugins/common/PluginTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.015799 pyutplugins-2.4.1/src/pyutplugins/common/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2224 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/BaseEditDialog.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.016315 pyutplugins-2.4.1/src/pyutplugins/common/ui/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5182 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/common/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.017330 pyutplugins-2.4.1/src/pyutplugins/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       66 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/exceptions/AbstractMethodNotImplementedException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       60 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/exceptions/InvalidPluginExtensionException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/exceptions/InvalidPluginNameException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/exceptions/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/exceptions/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.019344 pyutplugins-2.4.1/src/pyutplugins/ioplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4236 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOAscii.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2893 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IODTD.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2849 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOGML.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4134 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOJava.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3260 2024-05-11 19:29:41.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOMermaid.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6403 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOPdf.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9664 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4078 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOWxImage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8278 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOXml.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.020123 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      326 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/DTDAttribute.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      430 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/DTDElementTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10417 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/DTDParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.020764 pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8649 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/GMLExporter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/UnsupportedOperation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.021539 pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28064 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/JavaReader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11176 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/JavaWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.022317 pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      994 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13434 2024-05-11 19:55:08.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.023082 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/ImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      554 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/ImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12933 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.024227 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6135 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/PythonParseException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12478 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/PyutToPython.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10232 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.026267 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    54703 2024-02-05 14:09:02.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    17041 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)   541896 2024-02-05 14:09:03.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      543 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    35740 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.027412 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2892 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1592 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3974 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5181 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    20411 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-02-05 02:43:00.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.028042 pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4852 2024-05-01 01:58:53.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      929 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/WxImageFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.029141 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    11800 2024-03-07 18:41:20.000000 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/BasePluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5202 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/IOPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1364 2024-03-08 21:53:51.000000 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/ToolPluginInterface.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.030761 pyutplugins-2.4.1/src/pyutplugins/plugintypes/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2131 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/BaseFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      112 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/BaseRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      225 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/ExportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      205 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/ImportDirectoryResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      532 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/InputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/MultipleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      533 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/OutputFormat.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1766 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/PluginDataTypes.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      202 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/SingleFileRequestResponse.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       52 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/plugintypes/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.031278 pyutplugins-2.4.1/src/pyutplugins/preferences/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7286 2024-01-17 21:40:45.000000 pyutplugins-2.4.1/src/pyutplugins/preferences/PluginPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/preferences/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/preferences/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.033339 pyutplugins-2.4.1/src/pyutplugins/toolplugins/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1729 2024-04-25 17:28:09.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolArrangeLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5225 2024-03-11 01:31:01.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4534 2024-04-28 19:32:22.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolLoadLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4402 2024-03-08 05:03:28.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2427 2024-05-06 22:41:41.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolOrthogonalRouting.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4012 2024-04-28 17:19:08.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolSaveLayout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3159 2024-05-02 19:47:25.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolSugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1989 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolTransforms.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.034470 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8287 2024-03-09 15:59:30.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2069 2024-03-08 21:45:45.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1245 2024-03-09 19:18:23.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-03-07 17:58:31.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.035294 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2001 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5230 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       55 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapterException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.035952 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9817 2024-05-18 22:45:09.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3467 2024-05-10 19:47:03.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6892 2024-05-18 22:44:28.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 21:22:45.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.036190 pyutplugins-2.4.1/src/pyutplugins/toolplugins/savelayout/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      903 2024-04-28 17:19:08.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/savelayout/Layout.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-04-28 17:19:08.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/savelayout/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.038214 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3560 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1025 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3262 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    28457 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      263 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2108 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3228 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14778 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1387 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-12-17 01:57:34.000000 pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2024-05-18 23:00:04.038349 pyutplugins-2.4.1/src/pyutplugins.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2744 2024-05-18 23:00:04.000000 pyutplugins-2.4.1/src/pyutplugins.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6791 2024-05-18 23:00:04.000000 pyutplugins-2.4.1/src/pyutplugins.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2024-05-18 23:00:04.000000 pyutplugins-2.4.1/src/pyutplugins.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      267 2024-05-18 23:00:04.000000 pyutplugins-2.4.1/src/pyutplugins.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2024-05-18 23:00:04.000000 pyutplugins-2.4.1/src/pyutplugins.egg-info/top_level.txt
```

### Comparing `pyutplugins-2.4.0/LICENSE` & `pyutplugins-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/PKG-INFO` & `pyutplugins-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 2.4.0
+Version: 2.4.1
 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutplugins
 Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.0 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.1 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutplugins Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 codeallybasic>=1.3.1 Requires-Dist: codeallyadvanced>=1.3.1 Requires-Dist:
 pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.32 Requires-Dist:
```

### Comparing `pyutplugins-2.4.0/README.md` & `pyutplugins-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/pyproject.toml` & `pyutplugins-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ExternalTypes.py` & `pyutplugins-2.4.1/src/pyutplugins/ExternalTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/IPluginAdapter.py` & `pyutplugins-2.4.1/src/pyutplugins/IPluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/PluginManager.py` & `pyutplugins-2.4.1/src/pyutplugins/PluginManager.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/common/ElementTreeData.py` & `pyutplugins-2.4.1/src/pyutplugins/common/ElementTreeData.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/common/LinkMakerMixin.py` & `pyutplugins-2.4.1/src/pyutplugins/common/LinkMakerMixin.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/common/ui/BaseEditDialog.py` & `pyutplugins-2.4.1/src/pyutplugins/common/ui/BaseEditDialog.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py` & `pyutplugins-2.4.1/src/pyutplugins/common/ui/preferences/PluginPreferencesPage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOAscii.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOAscii.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IODTD.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IODTD.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOGML.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOGML.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOJava.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOJava.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOMermaid.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOMermaid.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPdf.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOPdf.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOPython.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOWxImage.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOWxImage.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/IOXml.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/IOXml.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/dtd/DTDParser.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/dtd/DTDParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/gml/GMLExporter.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/gml/GMLExporter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaReader.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/JavaReader.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/java/JavaWriter.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/java/JavaWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/MermaidDirection.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/mermaid/MermaidWriter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/ImageOptions.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/ImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/pdf/PyUmlDefinitionAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/DlgSelectMultiplePackages.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/PyutToPython.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/PyutToPython.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/ReverseEngineerPythonV3.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexer.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonLexerBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParser.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonParserBase.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/pythonpegparser/PythonPegParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/ParentsDictionaryHandler.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/ParserTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutBaseVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegClassVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/python/visitor/PyutPythonPegVisitor.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/DlgWxImageOptions.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/ioplugins/wximage/WxImageFormat.py` & `pyutplugins-2.4.1/src/pyutplugins/ioplugins/wximage/WxImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/BasePluginInterface.py` & `pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/BasePluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/IOPluginInterface.py` & `pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/IOPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugininterfaces/ToolPluginInterface.py` & `pyutplugins-2.4.1/src/pyutplugins/plugininterfaces/ToolPluginInterface.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugintypes/BaseFormat.py` & `pyutplugins-2.4.1/src/pyutplugins/plugintypes/BaseFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugintypes/InputFormat.py` & `pyutplugins-2.4.1/src/pyutplugins/plugintypes/InputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugintypes/OutputFormat.py` & `pyutplugins-2.4.1/src/pyutplugins/plugintypes/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/plugintypes/PluginDataTypes.py` & `pyutplugins-2.4.1/src/pyutplugins/plugintypes/PluginDataTypes.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/preferences/PluginPreferences.py` & `pyutplugins-2.4.1/src/pyutplugins/preferences/PluginPreferences.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolArrangeLinks.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolArrangeLinks.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolForceDirectedLayout.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolLoadLayout.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolLoadLayout.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolOrthogonalLayoutV2.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolOrthogonalRouting.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolOrthogonalRouting.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSaveLayout.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolSaveLayout.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolSugiyama.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolSugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/ToolTransforms.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/ToolTransforms.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/ConfigurationPanel.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/DlgConfiguration.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/forcedirectedlayout/OglNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/DlgLayoutSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/LayoutAreaSize.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonal/OrthogonalAdapter.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/DlgConfiguration.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/LabelledSlider.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/orthogonalrouting/OrthogonalConnectorAdapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         sourceSide, destinationSide = self._determineAttachmentSide(oglLink=oglLink)
 
         sourceRect:      Rect = self._shapeToRect(oglLink.sourceShape)
         destinationRect: Rect = self._shapeToRect(oglLink.destinationShape)
 
         sourceConnectorPoint:      ConnectorPoint = ConnectorPoint(shape=sourceRect,      side=sourceSide,      distance=self._configuration.sourceEdgeDistance)
-        destinationConnectorPoint: ConnectorPoint = ConnectorPoint(shape=destinationRect, side=destinationSide, distance=0.5)
+        destinationConnectorPoint: ConnectorPoint = ConnectorPoint(shape=destinationRect, side=destinationSide, distance=self._configuration.destinationEdgeDistance)
 
         options: OrthogonalConnectorOptions = OrthogonalConnectorOptions()
         options.pointA = sourceConnectorPoint
         options.pointB = destinationConnectorPoint
 
         options.shapeMargin        = self._configuration.shapeMargin
         options.globalBoundsMargin = self._configuration.globalBoundsMargin
```

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/savelayout/Layout.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/savelayout/Layout.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/ALayoutLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/ALayoutNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/RealSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/Sugiyama.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaGlobals.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaLink.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/SugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py` & `pyutplugins-2.4.1/src/pyutplugins/toolplugins/sugiyama/VirtualSugiyamaNode.py`

 * *Files identical despite different names*

### Comparing `pyutplugins-2.4.0/src/pyutplugins.egg-info/PKG-INFO` & `pyutplugins-2.4.1/src/pyutplugins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutplugins
-Version: 2.4.0
+Version: 2.4.1
 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 Maintainer-email: "Humberto A. Sanchez II" <Humbert.A.Sanchez.II@gmail.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Project-URL: Repository, https://github.com/hasii2011/pyutplugins
 Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.0 Summary: Pyut Plugins
+Metadata-Version: 2.1 Name: pyutplugins Version: 2.4.1 Summary: Pyut Plugins
 Author-email: "Humberto A. Sanchez II"
 gmail.com> Maintainer-email: "Humberto A. Sanchez II"
 gmail.com> License: GNU AFFERO GENERAL PUBLIC LICENSE Project-URL: Repository,
 https://github.com/hasii2011/pyutplugins Keywords: pyut,python,plugin
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 codeallybasic>=1.3.1 Requires-Dist: codeallyadvanced>=1.3.1 Requires-Dist:
 pyutmodelv2>=2.1.5 Requires-Dist: ogl>=2.1.32 Requires-Dist:
```

### Comparing `pyutplugins-2.4.0/src/pyutplugins.egg-info/SOURCES.txt` & `pyutplugins-2.4.1/src/pyutplugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

