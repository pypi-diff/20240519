# Comparing `tmp/actionlint_py-1.6.27.13.tar.gz` & `tmp/actionlint_py-1.7.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.27.13.tar", last modified: Sat Apr  6 06:49:50 2024, max compression
+gzip compressed data, was "actionlint_py-1.7.0.14.tar", last modified: Sun May 19 07:23:12 2024, max compression
```

## Comparing `actionlint_py-1.6.27.13.tar` & `actionlint_py-1.7.0.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_ACTIONLINT.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_BUILD_SYSTEM.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/VERSION_DEV.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/auto_update_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/checksums.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/bdist_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/fetch_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/commands/install_actionlint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.805586 actionlint_py-1.6.27.13/_custom_build/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/utils/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/_custom_build/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/actionlint_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 06:49:50.000000 actionlint_py-1.6.27.13/actionlint_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-06 06:49:40.000000 actionlint_py-1.6.27.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:49:50.809586 actionlint_py-1.6.27.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.152948 actionlint_py-1.7.0.14/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_ACTIONLINT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_BUILD_SYSTEM.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_DEV.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/auto_update_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/checksums.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/bdist_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/fetch_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/install_actionlint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/actionlint_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:23:12.152948 actionlint_py-1.7.0.14/setup.cfg
```

### Comparing `actionlint_py-1.6.27.13/LICENSE` & `actionlint_py-1.7.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/PKG-INFO` & `actionlint_py-1.7.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.27.13
+Version: 1.7.0.14
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -75,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.13
+  rev: v1.7.0.14
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -95,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.13]
+      #additional_dependencies: [actionlint-py==1.7.0.14]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -117,15 +117,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.6.27
+  rev: v1.7.0
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.6.27.13/README.md` & `actionlint_py-1.7.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.13
+  rev: v1.7.0.14
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -48,17 +48,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.13]
+      #additional_dependencies: [actionlint-py==1.7.0.14]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -70,15 +70,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.6.27
+  rev: v1.7.0
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.6.27.13/_custom_build/auto_update_main.py` & `actionlint_py-1.7.0.14/_custom_build/auto_update_main.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/_custom_build/checksums.cfg` & `actionlint_py-1.7.0.14/_custom_build/checksums.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [linux-x86_64]
-file_name = actionlint_1.6.27_linux_amd64.tar.gz
-checksum = 5c9b6e5418f688b7f7c7e3d40c13d9e41b1ca45fb6a2c35788b0580e34b7300f
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_linux_amd64.tar.gz
+file_name = actionlint_1.7.0_linux_amd64.tar.gz
+checksum = 8aae9148f61952d11a97651852fdc7dffd2b762ed3cdd28b3c2232ae5f55d4db
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_linux_amd64.tar.gz
 
 [linux-arm64]
-file_name = actionlint_1.6.27_linux_arm64.tar.gz
-checksum = 03ffe5891da7800ec39533543667697b5c292d0ff8b906397b43c58374ec052a
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_linux_arm64.tar.gz
+file_name = actionlint_1.7.0_linux_arm64.tar.gz
+checksum = 8181452246e7e6310b988f83762fc982e03f27eeb53dd4ad33fa4a5f4276b383
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_linux_arm64.tar.gz
 
 [darwin-x86_64]
-file_name = actionlint_1.6.27_darwin_amd64.tar.gz
-checksum = 1459f1ec2182162c85beddacff9b05d1cb921bfb2656a6fd9151e9cd84cd63e9
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_darwin_amd64.tar.gz
+file_name = actionlint_1.7.0_darwin_amd64.tar.gz
+checksum = 138aff674f31bd218030d4b00b3024bf0c721b75a7ec8e90b743763f81e3128e
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_darwin_amd64.tar.gz
 
 [darwin-arm64]
-file_name = actionlint_1.6.27_darwin_arm64.tar.gz
-checksum = 4b8eff986643b8d9918c4fd3ada9c0eee7e59230a53a46a9bd9686521dcad170
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_darwin_arm64.tar.gz
+file_name = actionlint_1.7.0_darwin_arm64.tar.gz
+checksum = 806e73fbafe54b7324d9478798534c5195fb71ea171633d9035b3fca237addd3
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_darwin_arm64.tar.gz
 
 [win32-AMD64]
-file_name = actionlint_1.6.27_windows_amd64.zip
-checksum = 2040aeb2530a80abbb923493f6947443203b7e60e829cb7bad1c8cde1483c376
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_windows_amd64.zip
+file_name = actionlint_1.7.0_windows_amd64.zip
+checksum = 2ecb1b4d3b54ee4503a0edeb29bdc910c5ef8826358698078905f485e0bab675
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_amd64.zip
 
 [win32-ARM64]
-file_name = actionlint_1.6.27_windows_arm64.zip
-checksum = bc082f32a036a86dad364bc46e2d707c4da5615598e2d50da2cb840cff97731d
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_windows_arm64.zip
+file_name = actionlint_1.7.0_windows_arm64.zip
+checksum = c2d9d30c7fdb4808a99a0800b768425b14132d4968ab01926f1bafa44b0f230a
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_arm64.zip
 
 [cygwin-x86_64]
-file_name = actionlint_1.6.27_windows_amd64.zip
-checksum = 2040aeb2530a80abbb923493f6947443203b7e60e829cb7bad1c8cde1483c376
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.27/actionlint_1.6.27_windows_amd64.zip
+file_name = actionlint_1.7.0_windows_amd64.zip
+checksum = 2ecb1b4d3b54ee4503a0edeb29bdc910c5ef8826358698078905f485e0bab675
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_amd64.zip
```

### Comparing `actionlint_py-1.6.27.13/_custom_build/commands/fetch_binaries.py` & `actionlint_py-1.7.0.14/_custom_build/commands/fetch_binaries.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/_custom_build/commands/install_actionlint.py` & `actionlint_py-1.7.0.14/_custom_build/commands/install_actionlint.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/_custom_build/utils/file_ops.py` & `actionlint_py-1.7.0.14/_custom_build/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/_custom_build/version.py` & `actionlint_py-1.7.0.14/_custom_build/version.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.7.0.14/actionlint_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.27.13
+Version: 1.7.0.14
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -75,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.27.13
+  rev: v1.7.0.14
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -95,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.27.13]
+      #additional_dependencies: [actionlint-py==1.7.0.14]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.6.27" but "1.6.27.13" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -117,15 +117,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.6.27
+  rev: v1.7.0
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.6.27.13/actionlint_py.egg-info/SOURCES.txt` & `actionlint_py-1.7.0.14/actionlint_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.27.13/pyproject.toml` & `actionlint_py-1.7.0.14/pyproject.toml`

 * *Files identical despite different names*

