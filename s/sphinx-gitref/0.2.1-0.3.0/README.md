# Comparing `tmp/sphinx-gitref-0.2.1.tar.gz` & `tmp/sphinx_gitref-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-gitref-0.2.1.tar", last modified: Sat Feb 19 07:49:13 2022, max compression
+gzip compressed data, was "sphinx_gitref-0.3.0.tar", last modified: Sun May 19 02:56:26 2024, max compression
```

## Comparing `sphinx-gitref-0.2.1.tar` & `sphinx_gitref-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 07:49:13.145672 sphinx-gitref-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-02-19 07:49:13.145672 sphinx-gitref-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4244 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-02-19 07:49:13.149672 sphinx-gitref-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 07:49:13.145672 sphinx-gitref-0.2.1/sphinx_gitref/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-02-19 07:49:05.000000 sphinx-gitref-0.2.1/sphinx_gitref/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 07:49:13.145672 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5069 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-19 07:49:13.000000 sphinx-gitref-0.2.1/sphinx_gitref.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:56:26.541679 sphinx_gitref-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-19 02:56:26.541679 sphinx_gitref-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:56:26.541679 sphinx_gitref-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:56:26.537680 sphinx_gitref-0.3.0/sphinx_gitref/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/sphinx_gitref/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:56:26.537680 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-19 02:56:26.000000 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-19 02:56:26.000000 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:56:26.000000 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 02:56:26.000000 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 02:56:26.000000 sphinx_gitref-0.3.0/sphinx_gitref.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:56:26.537680 sphinx_gitref-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-19 02:56:21.000000 sphinx_gitref-0.3.0/tests/test_role.py
```

### Comparing `sphinx-gitref-0.2.1/LICENSE` & `sphinx_gitref-0.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Sphinx-Gitref is licensed under the BSD License (BSD-3-Clause)
 ================================================================
 
-Copyright (c) 2020, Wildfish, https://wildfish.com
+Copyright (c) 2020, Richard Terry, https://radiac.net/
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are
 permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of
```

### Comparing `sphinx-gitref-0.2.1/PKG-INFO` & `sphinx_gitref-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,180 @@
-Metadata-Version: 2.1
-Name: sphinx-gitref
-Version: 0.2.1
-Summary: Link to source code and validate references in documentation
-Home-page: https://github.com/wildfish/sphinx-gitref
-Author: Wildfish
-Author-email: developers@wildfish.com
-License: BSD
-Keywords: sphinx,documentation,git,source
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-License-File: LICENSE
-
-=============
-Sphinx Gitref
-=============
+# Sphinx Gitref
 
-.. image:: https://travis-ci.org/wildfish/sphinx-gitref.svg?branch=master
-    :target: https://travis-ci.org/wildfish/sphinx-gitref
 
-.. image:: https://codecov.io/gh/wildfish/sphinx-gitref/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/wildfish/sphinx-gitref
+[![PyPI](https://img.shields.io/pypi/v/sphinx-gitref.svg)](https://pypi.org/project/sphinx-gitref/)
+[![Tests](https://github.com/radiac/sphinx-gitref/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/sphinx-gitref/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/radiac/sphinx-gitref/branch/main/graph/badge.svg?token=Q9AKPHRJF5)](https://codecov.io/gh/radiac/sphinx-gitref)
 
-Adds a ``:gitref:`..``` role to sphinx to link to your code on GitHub, GitLab or
+Adds a `` :gitref:`..` `` role to sphinx to link to your code on GitHub, GitLab or
 Bitbucket, and to make sure the references in your docs match the code.
 
 Key features:
 
 * Check code references are up to date
 * Link to source code on github
 * Incorporate into tests or git hooks
 
-Supports Python 3.6+
+Supports Python 3.7+
 
 
-Installation
-============
+## Installation
 
 Install::
 
     pip install sphinx-gitref
 
 
-Modify your Sphinx ``conf.py``:
+In your Sphinx ``conf.py``, add ``sphinx_gitref`` to the ``extensions`` list:
 
-#. Add ``sphinx_gitref`` to the ``extensions`` list in your Sphinx ``conf.py``::
+   ```python
+   extensions = [
+       ...
+       'sphinx_gitref',
+   ]
+   ```
 
-      extensions = [
-          ...
-          'sphinx_gitref',
-      ]
+Gitref should now work for most projects, but see "Configuration" below to customise its
+defaults.
 
-#. Optional: Explicitly specify the remote URL.
 
-   Gitref will try to detect your remote origin URL from the ``.git`` dir in your docs'
-   parent dir. If it can't find it, or detects the wrong remote, you can set or override
-   the remote URL explicitly with::
+## Usage
 
-      gitref_remote_url = "https://github.com/username/repository.git"
+The `` :gitref:`..` `` role supports the following features:
 
-#. Optional: Explicitly specify the branch to link to.
-
-   Gitref will try to detect your current branch from the ``.git`` dir in your docs'
-   parent dir. If it can't find it, or you'd like it to use a different branch, you can
-   set or override it explicitly with::
-
-      gitref_branch = "master"
-
-#. Optional: Change the link label format when a coderef is provided without an
-   explicit label, eg ``:gitref:`filename.py::coderef```
-
-   Gitref defaults to using showing the coderef and dropping the filename. This can be
-   overridden by setting a format string::
-
-        gitref_label_format = "{filename} {coderef}"
-
-
-Usage
-=====
-
-The ``:gitref:`..``` role supports the following features:
-
-* ``:gitref:`path/to/filename```
-* ``:gitref:`path/to/filename.py::coderef```
+* `` :gitref:`path/to/filename` ``
+* `` :gitref:`path/to/filename.py::coderef` ``
 
 You can optionally use them with a text label:
 
-* ``:gitref:`text <path/to/filename>```
-* ``:gitref:`text <path/to/filename.py::coderef>```
+* `` :gitref:`text <path/to/filename>` ``
+* `` :gitref:`text <path/to/filename.py::coderef>` ``
 
 where ``coderef`` is a Python class, function or variable. You can also refer to class
 attributes as you would in python, eg ``MyClass.attribute``.
 
 These will be replaced by a link to the code.
 
 If you do not provide a ``coderef``, gitref will just check that the file exists.
 
 Where you provide a ``coderef``, gitref will check that an object with that name exists
 in the code, and will add its line number to the link.
 
 
-Examples
---------
+### Examples
 
 Link to a file on gitref::
 
-    This file is :gitref:`README.rst`
-    For more information, see the :gitref:`project README <README.rst>`
+```
+This file is :gitref:`README.rst`
+For more information, see the :gitref:`project README <README.rst>`
+```
 
 Link to a variable, function or class in a python file::
 
-    The method which turns a reference into a line number
-    is :gitref:`sphinx_python/parse.py::python_to_lineno` -
-    this will raise a warning if the reference is not found.
-
-    Reference class attributes as you would in Python, such
-    as :gitref:`sphinx_python/git.py::Repo.path`.
-
+```
+The method which turns a reference into a line number
+is :gitref:`sphinx_python/parse.py::python_to_lineno` -
+this will raise a warning if the reference is not found.
+
+Reference class attributes as you would in Python, such
+as :gitref:`sphinx_python/git.py::Repo.path`.
+```
 
-Using in tests
---------------
+### Using in tests
 
 Because ``sphinx-gitref`` integrates into Sphinx, you can test the references are valid
 by performing a test build of your documentation.
 
 
-Custom remotes
---------------
+### Custom remotes
 
 If your code is stored somewhere other than one of the supported platforms, you can add
 a custom remote by subclassing ``sphinx_github.remotes.Remote`` in your Sphinx
 ``conf.py``; for example::
 
-    from sphinx_github.remotes import Remote
-    class Gitea(Remote):
-        remote_match = re.compile(r"^git@gitea.example.com:(?P<repo>.+?)\.git$")
-        url_pattern = "https://gitea.example.com/{repo}/blob/{branch}/{filename}{line}"
-        url_pattern_line = "#L{line}"
+```python
+from sphinx_github.remotes import Remote
+class Gitea(Remote):
+    remote_match = re.compile(r"^git@gitea.example.com:(?P<repo>.+?)\.git$")
+    url_pattern = "https://gitea.example.com/{repo}/blob/{branch}/{filename}{line}"
+    url_pattern_line = "#L{line}"
+```
+
+
+## Configuration
+
+Define the following variables in Sphinx ``conf.py``.
+
+
+### ``gitref_relative_project_root``
+
+Explicitly specify the relative path to the project root form your docs' source dir.
+
+The project root is the root directory of your git repository.
+
+Gitref will walk up the directory tree from your documentation source, looking for the
+first directory with a ``.git`` dir. It will use this as the project root.
+
+If it mis-detects the path, you can configure it with a relative path. For example, if
+your docs are in ``docs/``, you can specify one parent up as:
+
+```python
+gitref_relative_project_root = ".."
+```
+
+
+### ``gitref_remote_url``
+
+Explicitly specify the remote URL.
+
+Gitref will try to detect your remote origin URL from the ``.git`` dir in your project
+root. If it can't find it, or detects the wrong remote, you can set or override the
+remote URL explicitly with:
+
+```python
+gitref_remote_url = "https://github.com/username/repository.git"
+```
+
+
+### ``gitref_branch``
 
+Explicitly specify the branch to link to.
 
-Contributing
-============
+Gitref will try to detect your current branch from the ``.git`` dir in your project
+root. If it can't find it, or you'd like it to use a different branch, you can set or
+override it explicitly with::
 
-Contributions are welcome by pull request.
+```python
+gitref_branch = "master"
+```
 
-They will be merged more quickly if they are provided with unit tests; to run tests
-locally with tox::
+### ``gitref_label_format``
 
-    pip install tox
-    tox
+Change the link label format when a coderef is provided without an explicit label, eg
+`` :gitref:`filename.py::coderef` ``
 
+Gitref defaults to using showing the coderef and dropping the filename. This can be
+overridden by setting a format string::
 
-Changelog
-=========
+```python
+gitref_label_format = "{filename} {coderef}"
+```
 
-======= ====
-0.1.0   Initial release
 
-0.2.0   Add custom label formatting with ``gitref_label_format``
 
-        Fix bug when node target has no id
+## Changelog
 
-        Improve branch detection to support a recently detached ``HEAD``
+0.3.0 - 2024-05-19
+* Better project root detection with override support (fixes #12)
+* Support latest Sphinx
 
-0.2.1   Improve repository pattern matching
-======= ====
+0.2.1 - 2022-02-19
+* Improve repository pattern matching
 
+0.2.0 - 2022-02-13
+* Add custom label formatting with ``gitref_label_format``
+* Fix bug when node target has no id
+* Improve branch detection to support a recently detached ``HEAD``
 
+0.1.0 - 2020-04-18
+* Initial release
```

### Comparing `sphinx-gitref-0.2.1/sphinx_gitref/git.py` & `sphinx_gitref-0.3.0/sphinx_gitref/git.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,15 +56,20 @@
         config_src = "\n".join(
             [line.strip() for line in config_path.read_text().splitlines()]
         )
         config_io = StringIO(config_src)
 
         # Read the config - intentionally don't catch exceptions, we need those reported
         config = RawConfigParser(allow_no_value=True)
-        config.readfp(config_io)
+        if hasattr(config, "read_fp"):
+            # sphinx 4
+            config.read_fp(config_io)
+        else:
+            # sphinx 5
+            config.read_file(config_io)
 
         try:
             url = config.get(f'remote "{self.remote_name}"', "url")
         except NoSectionError:
             return None
 
         return url
```

### Comparing `sphinx-gitref-0.2.1/sphinx_gitref/parser.py` & `sphinx_gitref-0.3.0/sphinx_gitref/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-gitref-0.2.1/sphinx_gitref/remote.py` & `sphinx_gitref-0.3.0/sphinx_gitref/remote.py`

 * *Files identical despite different names*

### Comparing `sphinx-gitref-0.2.1/sphinx_gitref/setup.py` & `sphinx_gitref-0.3.0/sphinx_gitref/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     """
     # Pick up config defaults from current repo
     doc_root = Path(app.confdir)
     git_root = doc_root.parent / ".git"
     repo = Repo(git_root)
 
     # Add config variables
+    app.add_config_value("gitref_relative_project_root", default=None, rebuild="html")
     app.add_config_value("gitref_remote_url", repo.get_remote_url(), "html")
     app.add_config_value("gitref_branch", repo.get_local_branch(), "html")
     app.add_config_value("gitref_label_format", DEFAULT_LABEL_FORMAT, "html")
 
     # Listen for config initialised
     app.connect("config-inited", lookup_remote)
```

