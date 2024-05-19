# Comparing `tmp/fastapi_cli_slim-0.0.3.tar.gz` & `tmp/fastapi_cli_slim-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cli_slim-0.0.3.tar", last modified: Tue May  7 19:03:44 2024, max compression
+gzip compressed data, was "fastapi_cli_slim-0.0.4.tar", last modified: Sun May 19 18:54:09 2024, max compression
```

## Comparing `fastapi_cli_slim-0.0.3.tar` & `fastapi_cli_slim-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1086 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/LICENSE
--rw-r--r--   0        0        0     5228 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/README.md
--rw-r--r--   0        0        0     1718 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/pdm_build.py
--rw-r--r--   0        0        0     3067 2024-05-07 19:03:44.735729 fastapi_cli_slim-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      142 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/requirements-tests.txt
--rw-r--r--   0        0        0       60 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/requirements.txt
--rwxr-xr-x   0        0        0       87 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/scripts/format.sh
--rwxr-xr-x   0        0        0      110 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/scripts/lint.sh
--rwxr-xr-x   0        0        0      124 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       70 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/scripts/test.sh
--rw-r--r--   0        0        0       22 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/__init__.py
--rw-r--r--   0        0        0       30 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/__main__.py
--rw-r--r--   0        0        0     9032 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/cli.py
--rw-r--r--   0        0        0     5285 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/discover.py
--rw-r--r--   0        0        0       47 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/exceptions.py
--rw-r--r--   0        0        0      664 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/logging.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/src/fastapi_cli/py.typed
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0       28 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/broken_package/mod/__init__.py
--rw-r--r--   0        0        0      148 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/broken_package/mod/app.py
--rw-r--r--   0        0        0       52 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/broken_package/utils.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_api/api.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app/api.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app/app.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_api/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_api/app/api.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_app/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_app/app/api.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_app/app/app.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_main/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_main/app/api.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_main/app/app.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_main/app/main.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_non_default/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_app_dir_non_default/app/nondefault.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_main/api.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_main/app.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/default_main/main.py
--rw-r--r--   0        0        0      119 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/default_files/non_default/nonstandard.py
--rw-r--r--   0        0        0       64 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/core/__init__.py
--rw-r--r--   0        0        0       55 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/core/utils.py
--rw-r--r--   0        0        0       28 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/mod/__init__.py
--rw-r--r--   0        0        0      359 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/mod/api.py
--rw-r--r--   0        0        0      447 2024-05-07 19:03:41.715746 fastapi_cli_slim-0.0.3/tests/assets/package/mod/app.py
--rw-r--r--   0        0        0      271 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/assets/package/mod/other.py
--rw-r--r--   0        0        0      371 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/assets/single_file_api.py
--rw-r--r--   0        0        0      463 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/assets/single_file_app.py
--rw-r--r--   0        0        0      279 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/assets/single_file_other.py
--rw-r--r--   0        0        0      530 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     8706 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/test_cli.py
--rw-r--r--   0        0        0     3905 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/test_utils_default_dir.py
--rw-r--r--   0        0        0     4046 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/test_utils_default_file.py
--rw-r--r--   0        0        0    20671 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/test_utils_package.py
--rw-r--r--   0        0        0     4993 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/test_utils_single_file.py
--rw-r--r--   0        0        0      325 2024-05-07 19:03:41.719746 fastapi_cli_slim-0.0.3/tests/utils.py
--rw-r--r--   0        0        0     7027 1970-01-01 00:00:00.000000 fastapi_cli_slim-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5228 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/README.md
+-rw-r--r--   0        0        0     1718 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/pdm_build.py
+-rw-r--r--   0        0        0     3028 2024-05-19 18:54:09.820773 fastapi_cli_slim-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      142 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/requirements.txt
+-rwxr-xr-x   0        0        0       87 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/scripts/format.sh
+-rwxr-xr-x   0        0        0      110 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0      124 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       70 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/scripts/test.sh
+-rw-r--r--   0        0        0       22 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/__main__.py
+-rw-r--r--   0        0        0     9278 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/cli.py
+-rw-r--r--   0        0        0     5570 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/discover.py
+-rw-r--r--   0        0        0       47 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/exceptions.py
+-rw-r--r--   0        0        0      664 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/logging.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/src/fastapi_cli/py.typed
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/broken_package/mod/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/broken_package/mod/app.py
+-rw-r--r--   0        0        0       52 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/broken_package/utils.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_api/api.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app/api.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app/app.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_api/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_api/app/api.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_app/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_app/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_app/app/app.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_main/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_main/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_main/app/app.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_main/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.232771 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_non_default/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_app_dir_non_default/app/nondefault.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_main/api.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_main/app.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/default_files/default_main/main.py
+-rw-r--r--   0        0        0      119 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/default_files/non_default/nonstandard.py
+-rw-r--r--   0        0        0       64 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/core/utils.py
+-rw-r--r--   0        0        0       28 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/mod/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/mod/api.py
+-rw-r--r--   0        0        0      447 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/mod/app.py
+-rw-r--r--   0        0        0      271 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/package/mod/other.py
+-rw-r--r--   0        0        0      371 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/single_file_api.py
+-rw-r--r--   0        0        0      463 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/single_file_app.py
+-rw-r--r--   0        0        0      279 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/assets/single_file_other.py
+-rw-r--r--   0        0        0      530 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     8706 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_cli.py
+-rw-r--r--   0        0        0     1389 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_requirements.py
+-rw-r--r--   0        0        0     3905 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_utils_default_dir.py
+-rw-r--r--   0        0        0     4046 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_utils_default_file.py
+-rw-r--r--   0        0        0    20671 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_utils_package.py
+-rw-r--r--   0        0        0     4993 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/test_utils_single_file.py
+-rw-r--r--   0        0        0      325 2024-05-19 18:54:07.236770 fastapi_cli_slim-0.0.4/tests/utils.py
+-rw-r--r--   0        0        0     7027 1970-01-01 00:00:00.000000 fastapi_cli_slim-0.0.4/PKG-INFO
```

### Comparing `fastapi_cli_slim-0.0.3/LICENSE` & `fastapi_cli_slim-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/README.md` & `fastapi_cli_slim-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/pdm_build.py` & `fastapi_cli_slim-0.0.4/pdm_build.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/pyproject.toml` & `fastapi_cli_slim-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "typer >= 0.12.3",
 ]
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 standard = [
     "fastapi",
@@ -73,19 +73,17 @@
     "scripts/",
 ]
 
 [tool.tiangolo._internal-slim-build.packages.fastapi-cli-slim.project]
 name = "fastapi-cli-slim"
 
 [tool.tiangolo._internal-slim-build.packages.fastapi-cli]
-include-optional-dependencies = [
-    "standard",
-]
+include-optional-dependencies = []
 
-[tool.tiangolo._internal-slim-build.packages.fastapi-cli.project.optional-dependencies]
+[tool.tiangolo._internal-slim-build.packages.fastapi-cli.project]
 
 [tool.pytest.ini_options]
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 xfail_strict = true
```

### Comparing `fastapi_cli_slim-0.0.3/src/fastapi_cli/cli.py` & `fastapi_cli_slim-0.0.4/src/fastapi_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Union
 
 import typer
-import uvicorn
 from rich import print
 from rich.padding import Padding
 from rich.panel import Panel
 from typing_extensions import Annotated
 
 from fastapi_cli.discover import get_import_string
 from fastapi_cli.exceptions import FastAPICLIException
@@ -16,14 +15,19 @@
 from .logging import setup_logging
 
 app = typer.Typer(rich_markup_mode="rich")
 
 setup_logging()
 logger = getLogger(__name__)
 
+try:
+    import uvicorn
+except ImportError:  # pragma: no cover
+    uvicorn = None  # type: ignore[assignment]
+
 
 def version_callback(value: bool) -> None:
     if value:
         print(f"FastAPI CLI version: [green]{__version__}[/green]")
         raise typer.Exit()
 
 
@@ -77,14 +81,18 @@
             f"{serving_str}\n\n[dim]Running in production mode, for development use:[/dim] \n\n[b]fastapi dev[/b]",
             title="FastAPI CLI - Production mode",
             expand=False,
             padding=(1, 2),
             style="green",
         )
     print(Padding(panel, 1))
+    if not uvicorn:
+        raise FastAPICLIException(
+            "Could not import Uvicorn, try running 'pip install uvicorn'"
+        ) from None
     uvicorn.run(
         app=use_uvicorn_app,
         host=host,
         port=port,
         reload=reload,
         workers=workers,
         root_path=root_path,
```

### Comparing `fastapi_cli_slim-0.0.3/src/fastapi_cli/discover.py` & `fastapi_cli_slim-0.0.4/src/fastapi_cli/discover.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import importlib
 import sys
 from dataclasses import dataclass
 from logging import getLogger
 from pathlib import Path
 from typing import Union
 
-from fastapi import FastAPI
 from rich import print
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.syntax import Syntax
 from rich.tree import Tree
 
 from fastapi_cli.exceptions import FastAPICLIException
 
 logger = getLogger(__name__)
 
+try:
+    from fastapi import FastAPI
+except ImportError:  # pragma: no cover
+    FastAPI = None  # type: ignore[misc, assignment]
+
 
 def get_default_path() -> Path:
     path = Path("main.py")
     if path.is_file():
         return path
     path = Path("app.py")
     if path.is_file():
@@ -103,14 +107,18 @@
         mod = importlib.import_module(mod_data.module_import_str)
     except (ImportError, ValueError) as e:
         logger.error(f"Import error: {e}")
         logger.warning(
             "Ensure all the package directories have an [blue]__init__.py[/blue] file"
         )
         raise
+    if not FastAPI:  # type: ignore[truthy-function]
+        raise FastAPICLIException(
+            "Could not import FastAPI, try running 'pip install fastapi'"
+        ) from None
     object_names = dir(mod)
     object_names_set = set(object_names)
     if app_name:
         if app_name not in object_names_set:
             raise FastAPICLIException(
                 f"Could not find app name {app_name} in {mod_data.module_import_str}"
             )
```

### Comparing `fastapi_cli_slim-0.0.3/src/fastapi_cli/logging.py` & `fastapi_cli_slim-0.0.4/src/fastapi_cli/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/conftest.py` & `fastapi_cli_slim-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/test_cli.py` & `fastapi_cli_slim-0.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/test_utils_default_dir.py` & `fastapi_cli_slim-0.0.4/tests/test_utils_default_dir.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/test_utils_default_file.py` & `fastapi_cli_slim-0.0.4/tests/test_utils_default_file.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/test_utils_package.py` & `fastapi_cli_slim-0.0.4/tests/test_utils_package.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/tests/test_utils_single_file.py` & `fastapi_cli_slim-0.0.4/tests/test_utils_single_file.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli_slim-0.0.3/PKG-INFO` & `fastapi_cli_slim-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cli-slim
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run and manage FastAPI apps from the command line with FastAPI CLI. 🚀
 Home-page: https://github.com/tiangolo/fastapi-cli
 Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?= <tiangolo@gmail.com>
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cli-slim Version: 0.0.3 Summary: Run and
+Metadata-Version: 2.1 Name: fastapi-cli-slim Version: 0.0.4 Summary: Run and
 manage FastAPI apps from the command line with FastAPI CLI. ð Home-page:
 https://github.com/tiangolo/fastapi-cli Author-Email: =?utf-
 8?q?Sebasti=C3=A1n_Ram=C3=ADrez?=
 gmail.com> License: MIT Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python Classifier: Topic :: Software
```

