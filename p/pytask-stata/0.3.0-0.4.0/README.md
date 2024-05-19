# Comparing `tmp/pytask_stata-0.3.0.tar.gz` & `tmp/pytask_stata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytask_stata-0.3.0.tar", last modified: Mon Jan 23 10:17:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytask_stata-0.3.0.tar` & `pytask_stata-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.956615 pytask_stata-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.952615 pytask_stata-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.952615 pytask_stata-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.952615 pytask_stata-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-01-23 10:17:05.956615 pytask_stata-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-01-23 10:17:05.956615 pytask_stata-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.952615 pytask_stata-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.956615 pytask_stata-0.3.0/src/pytask_stata/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/parametrize.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-01-23 10:16:56.000000 pytask_stata-0.3.0/src/pytask_stata/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 10:17:05.956615 pytask_stata-0.3.0/src/pytask_stata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-23 10:17:05.000000 pytask_stata-0.3.0/src/pytask_stata.egg-info/top_level.txt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/_version.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/cli.py
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/collect.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/config.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/execute.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/py.typed
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/src/pytask_stata/shared.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/README.md
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 pytask_stata-0.4.0/PKG-INFO
```

### Comparing `pytask_stata-0.3.0/LICENSE` & `pytask_stata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytask_stata-0.3.0/PKG-INFO` & `pytask_stata-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pytask_stata
-Version: 0.3.0
-Summary: Execute do-files with Stata and pytask.
-Home-page: https://github.com/pytask-dev/pytask-stata
-Author: Tobias Raabe
-Author-email: raabe@posteo.de
-License: MIT
-Project-URL: Documentation, https://github.com/pytask-dev/pytask-stata
-Project-URL: Github, https://github.com/pytask-dev/pytask-stata
-Project-URL: Tracker, https://github.com/pytask-dev/pytask-stata/issues
-Project-URL: Changelog, https://github.com/pytask-dev/pytask-stata/blob/main/CHANGES.md
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pytask-stata
 
 [![PyPI](https://img.shields.io/pypi/v/pytask-stata?color=blue)](https://pypi.org/project/pytask-stata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytask-stata)](https://pypi.org/project/pytask-stata)
 [![image](https://img.shields.io/conda/vn/conda-forge/pytask-stata.svg)](https://anaconda.org/conda-forge/pytask-stata)
 [![image](https://img.shields.io/conda/pn/conda-forge/pytask-stata.svg)](https://anaconda.org/conda-forge/pytask-stata)
 [![PyPI - License](https://img.shields.io/pypi/l/pytask-stata)](https://pypi.org/project/pytask-stata)
```

### Comparing `pytask_stata-0.3.0/README.md` & `pytask_stata-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.3
+Name: pytask_stata
+Version: 0.4.0
+Summary: Execute do-files with Stata and pytask.
+Project-URL: Homepage, https://github.com/pytask-dev/pytask-stata
+Project-URL: Documentation, https://github.com/pytask-dev/pytask-stata
+Project-URL: Github, https://github.com/pytask-dev/pytask-stata
+Project-URL: Tracker, https://github.com/pytask-dev/pytask-stata/issues
+Project-URL: Changelog, https://github.com/pytask-dev/pytask-stata/blob/main/CHANGES.md
+Author-email: Tobias Raabe <raabe@posteo.de>
+License: MIT
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Requires-Dist: click
+Requires-Dist: pytask>=0.4
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-xdist; extra == 'test'
+Provides-Extra: typing
+Requires-Dist: mypy; extra == 'typing'
+Description-Content-Type: text/markdown
+
 # pytask-stata
 
 [![PyPI](https://img.shields.io/pypi/v/pytask-stata?color=blue)](https://pypi.org/project/pytask-stata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytask-stata)](https://pypi.org/project/pytask-stata)
 [![image](https://img.shields.io/conda/vn/conda-forge/pytask-stata.svg)](https://anaconda.org/conda-forge/pytask-stata)
 [![image](https://img.shields.io/conda/pn/conda-forge/pytask-stata.svg)](https://anaconda.org/conda-forge/pytask-stata)
 [![PyPI - License](https://img.shields.io/pypi/l/pytask-stata)](https://pypi.org/project/pytask-stata)
```

### Comparing `pytask_stata-0.3.0/src/pytask_stata/cli.py` & `pytask_stata-0.4.0/src/pytask_stata/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Everything related to the CLI."""
+
 from __future__ import annotations
 
 import click
 from pytask import hookimpl
 
 
 @hookimpl
```

### Comparing `pytask_stata-0.3.0/src/pytask_stata/config.py` & `pytask_stata-0.4.0/src/pytask_stata/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Configure pytask."""
+
 from __future__ import annotations
 
 import shutil
 import sys
 from typing import Any
 
 from pytask import hookimpl
+
 from pytask_stata.shared import STATA_COMMANDS
 
 
 @hookimpl
 def pytask_parse_config(config: dict[str, Any]) -> None:
     """Register the r marker."""
     config["markers"]["stata"] = "Tasks which are executed with Stata."
```

### Comparing `pytask_stata-0.3.0/src/pytask_stata/execute.py` & `pytask_stata-0.4.0/src/pytask_stata/execute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 """Execute tasks."""
+
 from __future__ import annotations
 
 import re
+from pathlib import Path
 
+from pytask import PTask
+from pytask import PTaskWithPath
+from pytask import Session
 from pytask import has_mark
 from pytask import hookimpl
-from pytask import Session
-from pytask import Task
-from pytask_stata.shared import convert_task_id_to_name_of_log_file
+
 from pytask_stata.shared import STATA_COMMANDS
 
 
 @hookimpl
-def pytask_execute_task_setup(session: Session, task: Task) -> None:
+def pytask_execute_task_setup(session: Session, task: PTask) -> None:
     """Check if Stata is found on the PATH."""
     if has_mark(task, "stata") and session.config["stata"] is None:
-        raise RuntimeError(
+        msg = (
             "Stata is needed to run do-files, but it is not found on your PATH.\n\n"
             f"We are looking for one of {STATA_COMMANDS} on your PATH. If you have a"
             "different Stata executable, please, file an issue at "
             "https://github.com/pytask-dev/pytask-stata."
         )
+        raise RuntimeError(msg)
 
 
 @hookimpl
-def pytask_execute_task_teardown(session: Session, task: Task) -> None:
+def pytask_execute_task_teardown(session: Session, task: PTask) -> None:
     """Check if the log file contains no error code.
 
     Stata has the weird behavior of always returning an exit code of 0 even if an error
     occurred. Therefore, we need to parse the real error code from the log files.
 
     Error codes have a preceding r and a number enclosed in round brackets like ``r(1)``
     or ``r(601)``.
 
     """
     if has_mark(task, "stata"):
         if session.config["platform"] == "win32":
-            log_name = convert_task_id_to_name_of_log_file(task.short_name)
-            path_to_log = task.path.with_name(log_name).with_suffix(".log")
+            log_name = task.depends_on["_log_name"].load()
+            if isinstance(task, PTaskWithPath):
+                path_to_log = task.path.with_name(log_name).with_suffix(".log")
+            else:
+                path_to_log = Path.cwd(log_name).with_name(log_name).with_suffix(".log")
         else:
-            node = task.depends_on["__script"]
+            node = task.depends_on["_script"]
             path_to_log = node.path.with_suffix(".log")
 
         n_lines = session.config["stata_check_log_lines"]
 
         log = path_to_log.read_text()
         log_tail = log.split("\n")[-n_lines:]
         for line in log_tail:
```

### Comparing `pytask_stata-0.3.0/src/pytask_stata/plugin.py` & `pytask_stata-0.4.0/src/pytask_stata/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Register hook specifications and implementations."""
+
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from _pytask.config import hookimpl
-from pluggy import PluginManager
+
 from pytask_stata import cli
 from pytask_stata import collect
 from pytask_stata import config
 from pytask_stata import execute
-from pytask_stata import parametrize
+
+if TYPE_CHECKING:
+    from pluggy import PluginManager
 
 
 @hookimpl
 def pytask_add_hooks(pm: PluginManager) -> None:
     """Register hook implementations."""
     pm.register(cli)
     pm.register(collect)
     pm.register(config)
     pm.register(execute)
-    pm.register(parametrize)
```

### Comparing `pytask_stata-0.3.0/src/pytask_stata/shared.py` & `pytask_stata-0.4.0/src/pytask_stata/shared.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """Shared functions and variables."""
+
 from __future__ import annotations
 
 import sys
-from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Iterable
 from typing import Sequence
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytask import PTask
+
 
 if sys.platform == "darwin":
     STATA_COMMANDS = [
         "Stata64MP",
         "StataMP",
         "Stata64SE",
         "StataSE",
@@ -36,30 +42,30 @@
     ]
 else:
     STATA_COMMANDS = []
 
 
 def stata(
     *,
-    script: str | Path | None = None,
+    script: str | Path,
     options: str | Iterable[str] | None = None,
 ) -> tuple[str | Path | None, str | Iterable[str] | None]:
     """Specify command line options for Stata.
 
     Parameters
     ----------
     options : str | Iterable[str] | None
         One or multiple command line options passed to Stata.
 
     """
     options = [] if options is None else list(map(str, _to_list(options)))
     return script, options
 
 
-def convert_task_id_to_name_of_log_file(id_: str) -> str:
+def convert_task_id_to_name_of_log_file(task: PTask) -> str:
     """Convert task to id to name of log file.
 
     If one passes the complete task id as the log file name, Stata would remove parent
     directories and cut the string at the double colons for parametrized task. Here is
     an example:
 
     .. code-block:: none
@@ -71,17 +77,22 @@
 
     Example
     -------
     >>> convert_task_id_to_name_of_log_file("C:/task_example.py::task_example[arg1]")
     'task_example_py_task_example[arg1]'
 
     """
-    id_without_parent_directories = id_.rsplit("/")[-1]
-    converted_id = id_without_parent_directories.replace(".", "_").replace("::", "_")
-    return converted_id
+    id_ = getattr(task, "short_name", task.name)
+    return (
+        id_.rsplit("/")[-1]
+        .replace(".", "_")
+        .replace("::", "_")
+        .replace("<", "")
+        .replace(">", "")
+    )
 
 
 def _to_list(scalar_or_iter: Any) -> list[Any]:
     """Convert scalars and iterables to list.
 
     Parameters
     ----------
```

