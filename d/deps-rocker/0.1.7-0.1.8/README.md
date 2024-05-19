# Comparing `tmp/deps_rocker-0.1.7.tar.gz` & `tmp/deps_rocker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.7.tar` & `deps_rocker-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     7139 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/__init__.py
--rw-r--r--   0        0        0     1097 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/command_layer.py
--rw-r--r--   0        0        0      128 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/dep_rocker_cli.py
--rw-r--r--   0        0        0     7392 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      226 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0     2292 2024-05-17 16:39:34.480766 deps_rocker-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 deps_rocker-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     7095 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/__init__.py
+-rw-r--r--   0        0        0     1097 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/command_layer.py
+-rw-r--r--   0        0        0      128 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/dep_rocker_cli.py
+-rw-r--r--   0        0        0     7367 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      226 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0     2292 2024-05-18 11:51:08.128986 deps_rocker-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7957 1970-01-01 00:00:00.000000 deps_rocker-0.1.8/PKG-INFO
```

### Comparing `deps_rocker-0.1.7/README.md` & `deps_rocker-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: deps_rocker
+Version: 0.1.8
+Summary: A rocker plugin to help installing apt and pip dependencies
+Author-email: Austin Gregg-Smith <blooop@gmail.com>
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Requires-Dist: rocker
+Requires-Dist: pyyaml
+Requires-Dist: off-your-rocker
+Requires-Dist: toml
+Requires-Dist: black>=23,<=24.4.2 ; extra == "test"
+Requires-Dist: pylint>=2.16,<=3.2.0 ; extra == "test"
+Requires-Dist: pytest-cov>=4.1,<=5.0.0 ; extra == "test"
+Requires-Dist: pytest>=7.4,<=8.2.0 ; extra == "test"
+Requires-Dist: hypothesis>=6.82,<=6.102.4 ; extra == "test"
+Requires-Dist: ruff>=0.0.280,<=0.4.4 ; extra == "test"
+Requires-Dist: coverage>=7.2.7,<=7.5.1 ; extra == "test"
+Project-URL: Home, https://github.com/blooop/deps_rocker
+Project-URL: Source, https://github.com/blooop/deps_rocker
+Provides-Extra: test
+
 # deps_rocker
 
 ## Continuous Integration Status
 
 [![Ci](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/blooop/deps_rocker/actions/workflows/ci.yml?query=branch%3Amain)
 [![Codecov](https://codecov.io/gh/blooop/deps_rocker/branch/main/graph/badge.svg?token=Y212GW1PG6)](https://codecov.io/gh/blooop/deps_rocker)
 [![GitHub issues](https://img.shields.io/github/issues/blooop/deps_rocker.svg)](https://GitHub.com/blooop/deps_rocker/issues/)
@@ -15,20 +37,15 @@
 ```
 pip install deps-rocker
 ```
 
 ## Usage
 
 ```
-rocker --deps ubuntu:22.04
-#or
-rocker --deps "specific_pkg.deps.yaml" ubuntu:22.04
-#or
-rocker --deps "*.deps.yaml" ubuntu:22.04
-
+rocker --deps ubuntu:22.04  #recursivly search for *.deps.yaml
 ```
 
 ## Motivation
 
 Docker enables easy isolation of dependencies from the host system, but it is not easy to dynamically combine docker files from separate projects into a single unified environment.
 
 
@@ -39,112 +56,112 @@
 For example:
 
 pkg a requires git, make and ffmpeg and pkg_b requires git-lfs and pip.  Their deps.yaml files would look something like: 
 
 pkg_a.deps.yaml:
 
 ```
-apt_tools:
+apt_sources:
   - git
 
 apt_language-toolchain:
   - make
   - gcc
 
 apt:
   - ffmpeg
 ```
 pkg_b.deps.yaml
 
 ```
-apt_tools:
+apt_sources:
   - git
   - git-lfs
 
 apt_language-toolchain:
   - python3-pip
 ```
 
 If you wanted a container that had the dependencies of both installed deps-rocker would combine the dependencies to produce a file like:
 
 ```
-apt_tools:
+apt_sources:
   - git
   - git-lfs
 
 apt_language-toolchain:
   - make
   - gcc
   - python3-pip
 
 apt:
   - ffmpeg
 ```
 
 Each heading in the yaml file produces a docker layer based on the command and the label.  The format of the labels is {command_name}_{command-label}.  The layer names are delimited by _ so layer names should use - eg: language-toolchain. 
 
-This makes it easy to define the dependencies for a single project, but enable reuse of common dependencies across multiple projects. However, deps rocker does not restrict what is defined in each layer and so relies on a common convention for multiple packages to play nicely with eachother.  If one package adds "make" to apt_tools and other package adds "make" to apt_langage_toolchain, the deps-rocker will not complain and will not deduplicate that install step.   
+This makes it easy to define the dependencies for a single project, but enable reuse of common dependencies across multiple projects. However, deps rocker does not restrict what is defined in each layer and so relies on a common convention for multiple packages to play nicely with eachother.  If one package adds "make" to apt_sources and other package adds "make" to apt_langage_toolchain, the deps-rocker will not complain and will not deduplicate that install step.   
 
 ## Methodology:
 
 The algorithm works by splitting each entry in the yaml file into a command and a layer.  The entries from all the deps.yaml files are grouped by the command and layer into a list of entries for that command.  The order of the commands is defined by the order they appear in the deps.yaml file.  As long as all the files follow the same order of commands then a dependency tree of commands can be created and executed in a deterministic order.  However if two files define conflicting orders deps-rocker will not be able to produce a deterministic set of commands and fail.  e.g:
 
 pkg_a.deps.yaml:
 
 ```
-apt_tools:
+apt_sources:
   - git
 
 apt_language-toolchain:
   - make
   - gcc
 ```
 pkg_b.deps.yaml
 
 ```
 apt_language-toolchain:
   - python3-pip
 
-apt_tools:
+apt_sources:
   - git
   - git-lfs
 ```
 
-pkg_a says that apt_langage-toolchain comes before apt_tools, and pkg_b says that apt_tools comes before apt_language-toolchain, which is a conflict. 
+pkg_a says that apt_langage-toolchain comes before apt_sources, and pkg_b says that apt_sources comes before apt_language-toolchain, which is a conflict. 
 
 The pseudocode for the deps-rocker algorithm is as follows:
 ```
 dependencies_dictionary
 for file in glob(*.deps.yaml):
   for entry in file.entries:
     add 
 ```
 
 If two packages have unqiue layers that depend on a common layer
 
 pkg_a.deps.yaml:
 
 ```
-apt_tools:
+apt_sources:
   - git
 
 apt_pkg_a_custom:
   - custom1
 ```
 pkg_b.deps.yaml
 
 ```
-apt_tools:
+apt_sources:
   - git-lfs
 
 apt_pkg_b_custom:
   - custom1
 ```
 
-Here apt_pkg_b_custom and apt_pkg_a_custom both need to be run after apt_tools.  They will be run run in alphabetical order (to ensure determinism)
+Here apt_pkg_b_custom and apt_pkg_a_custom both need to be run after apt_sources.  They will be run run in alphabetical order (to ensure determinism)
 
 
 ## Commands
 
 Commands are defined in templates/commandname_snippet.Dockerfile.
 
 They use the [empy](https://pypi.org/project/empy/) templating langage that is used by [rocker](https://github.com/tfoote/rocker).  deps-rocker has some basic commands already implemented but adding a new command is as simple as adding a _snippet.Dockerfile.  
@@ -225,7 +242,8 @@
 
 ```
 
 ## limitations/TODO
 
 This has only been tested on the ubuntu base image. It assumes you have access to apt-get.
 
+
```

### Comparing `deps_rocker-0.1.7/deps_rocker/command_layer.py` & `deps_rocker-0.1.8/deps_rocker/command_layer.py`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.7/deps_rocker/dependencies.py` & `deps_rocker-0.1.8/deps_rocker/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,23 +172,22 @@
     def get_user_snippet(self, cliargs):
         """Get a dockerfile snippet to be executed after switchingto the expected USER."""
         self.setup_deps(cliargs)
         return "\n".join([lay.to_snippet() for lay in self.layers_user.values()])
 
     @staticmethod
     def register_arguments(parser, defaults=None):
-        # parser.add_argument("--deps", action="store_true", help="install all deps.yaml ")
-        parser.add_argument(
-            "--deps",
-            type=str,
-            nargs="?",
-            const="*.deps.yaml",
-            help="A filter to select deps.yaml files. Defaults to *.deps.yaml",
-            # default="*.deps.yaml",
-        )
+        parser.add_argument("--deps", action="store_true", help="install all deps.yaml ")
+        # parser.add_argument(
+        #     "--deps",
+        #     type=str,
+        #     nargs="?",
+        #     const="*.deps.yaml",
+        #     help="A filter to select deps.yaml files. Defaults to *.deps.yaml",
+        # )
 
 
 if __name__ == "__main__":
     deps = Dependencies()
     # print(deps)
 
     # scr= deps
```

### Comparing `deps_rocker-0.1.7/pyproject.toml` & `deps_rocker-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deps_rocker"
-version = "0.1.7"
+version = "0.1.8"
 license = { text = "MIT" }
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A rocker plugin to help installing apt and pip dependencies"
 readme = "README.md"
 
 requires-python = ">=3.10"
```

