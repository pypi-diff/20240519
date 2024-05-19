# Comparing `tmp/bumpify-0.2.0.tar.gz` & `tmp/bumpify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpify-0.2.0.tar", max compression
+gzip compressed data, was "bumpify-0.3.0.tar", max compression
```

## Comparing `bumpify-0.2.0.tar` & `bumpify-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1072 2024-04-28 17:53:41.902929 bumpify-0.2.0/LICENSE
--rw-r--r--   0        0        0     4327 2024-04-28 17:53:41.902929 bumpify-0.2.0/README.md
--rw-r--r--   0        0        0       22 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/__init__.py
--rw-r--r--   0        0        0      624 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/context.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/commands.py
--rw-r--r--   0        0        0     2597 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/interface.py
--rw-r--r--   0        0        0     1744 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/presenters.py
--rw-r--r--   0        0        0     4078 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/api/providers.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/exc.py
--rw-r--r--   0        0        0      513 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/helpers.py
--rw-r--r--   0        0        0     2450 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/implementation.py
--rw-r--r--   0        0        0     1506 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/interface.py
--rw-r--r--   0        0        0     4797 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/config/objects.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/__init__.py
--rw-r--r--   0        0        0      746 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/_message_formatter.py
--rw-r--r--   0        0        0     2956 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/helpers.py
--rw-r--r--   0        0        0      660 2024-04-28 17:53:41.902929 bumpify-0.2.0/bumpify/core/console/input.py
--rw-r--r--   0        0        0     1793 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/interface.py
--rw-r--r--   0        0        0      702 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/objects.py
--rw-r--r--   0        0        0     1003 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/console/output.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/__init__.py
--rw-r--r--   0        0        0      668 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/exc.py
--rw-r--r--   0        0        0     2388 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/helpers.py
--rw-r--r--   0        0        0     4671 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/implementation.py
--rw-r--r--   0        0        0     2805 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/filesystem/interface.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/__init__.py
--rw-r--r--   0        0        0      333 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/_utils.py
--rw-r--r--   0        0        0      180 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/decorators.py
--rw-r--r--   0        0        0      696 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/exc.py
--rw-r--r--   0        0        0     3179 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/implementation.py
--rw-r--r--   0        0        0     1885 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/interface.py
--rw-r--r--   0        0        0      499 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/hook/objects.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_changelog_formatters.py
--rw-r--r--   0        0        0      680 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_constants.py
--rw-r--r--   0        0        0      744 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_hook_invokers.py
--rw-r--r--   0        0        0     3821 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_parsing.py
--rw-r--r--   0        0        0     2735 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/_version_file_updater.py
--rw-r--r--   0        0        0      964 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/exc.py
--rw-r--r--   0        0        0     1600 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/helpers.py
--rw-r--r--   0        0        0      382 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/hooks.py
--rw-r--r--   0        0        0     4626 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/implementation.py
--rw-r--r--   0        0        0     3107 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/interface.py
--rw-r--r--   0        0        0    18959 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/semver/objects.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/__init__.py
--rw-r--r--   0        0        0     1483 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/exc.py
--rw-r--r--   0        0        0     1610 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/helpers.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/__init__.py
--rw-r--r--   0        0        0     7973 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/git.py
--rw-r--r--   0        0        0     2044 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/implementation/proxy.py
--rw-r--r--   0        0        0     4049 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/interface.py
--rw-r--r--   0        0        0     1226 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/core/vcs/objects.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/__init__.py
--rw-r--r--   0        0        0     3029 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/__main__.py
--rw-r--r--   0        0        0      723 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/delivery/cli/decorators.py
--rw-r--r--   0        0        0      612 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/__init__.py
--rw-r--r--   0        0        0     1931 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/api.py
--rw-r--r--   0        0        0     1060 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/config.py
--rw-r--r--   0        0        0      485 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/console.py
--rw-r--r--   0        0        0     1079 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/filesystem.py
--rw-r--r--   0        0        0      751 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/hook.py
--rw-r--r--   0        0        0     1203 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/semver.py
--rw-r--r--   0        0        0     1212 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/di/vcs.py
--rw-r--r--   0        0        0     2921 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/exc.py
--rw-r--r--   0        0        0     5704 2024-04-28 17:53:41.906929 bumpify-0.2.0/bumpify/utils.py
--rw-r--r--   0        0        0      946 2024-04-28 17:53:41.906929 bumpify-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 bumpify-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 07:31:47.394818 bumpify-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4327 2024-05-19 07:31:47.394818 bumpify-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/__init__.py
+-rw-r--r--   0        0        0      624 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/context.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/api/__init__.py
+-rw-r--r--   0        0        0     5080 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/api/commands.py
+-rw-r--r--   0        0        0     2597 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/api/interface.py
+-rw-r--r--   0        0        0     1744 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/api/presenters.py
+-rw-r--r--   0        0        0     4134 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/api/providers.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/exc.py
+-rw-r--r--   0        0        0      513 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/helpers.py
+-rw-r--r--   0        0        0     2425 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/implementation.py
+-rw-r--r--   0        0        0     1506 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/interface.py
+-rw-r--r--   0        0        0     4847 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/config/objects.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/_message_formatter.py
+-rw-r--r--   0        0        0     2956 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/helpers.py
+-rw-r--r--   0        0        0      660 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/input.py
+-rw-r--r--   0        0        0     1793 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/interface.py
+-rw-r--r--   0        0        0      702 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/objects.py
+-rw-r--r--   0        0        0     1003 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/console/output.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/filesystem/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/filesystem/exc.py
+-rw-r--r--   0        0        0     2388 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/filesystem/helpers.py
+-rw-r--r--   0        0        0     4671 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/filesystem/implementation.py
+-rw-r--r--   0        0        0     2805 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/filesystem/interface.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/_utils.py
+-rw-r--r--   0        0        0      180 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/decorators.py
+-rw-r--r--   0        0        0      696 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/exc.py
+-rw-r--r--   0        0        0     3173 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/implementation.py
+-rw-r--r--   0        0        0     1885 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/interface.py
+-rw-r--r--   0        0        0      487 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/hook/objects.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/_changelog_formatters.py
+-rw-r--r--   0        0        0      680 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/_constants.py
+-rw-r--r--   0        0        0      744 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/_hook_invokers.py
+-rw-r--r--   0        0        0     3821 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/_parsing.py
+-rw-r--r--   0        0        0     2735 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/_version_file_updater.py
+-rw-r--r--   0        0        0      964 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/exc.py
+-rw-r--r--   0        0        0     1600 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/helpers.py
+-rw-r--r--   0        0        0      382 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/hooks.py
+-rw-r--r--   0        0        0     4616 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/implementation.py
+-rw-r--r--   0        0        0     3107 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/interface.py
+-rw-r--r--   0        0        0    18947 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/semver/objects.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/__init__.py
+-rw-r--r--   0        0        0     1483 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/exc.py
+-rw-r--r--   0        0        0     1610 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/implementation/__init__.py
+-rw-r--r--   0        0        0     7973 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/implementation/git.py
+-rw-r--r--   0        0        0     2044 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/implementation/proxy.py
+-rw-r--r--   0        0        0     4049 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/interface.py
+-rw-r--r--   0        0        0     1536 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/core/vcs/objects.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.394818 bumpify-0.3.0/bumpify/delivery/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/delivery/cli/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/delivery/cli/__main__.py
+-rw-r--r--   0        0        0      723 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/delivery/cli/decorators.py
+-rw-r--r--   0        0        0      612 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/api.py
+-rw-r--r--   0        0        0     1060 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/config.py
+-rw-r--r--   0        0        0      485 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/console.py
+-rw-r--r--   0        0        0     1079 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/filesystem.py
+-rw-r--r--   0        0        0      751 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/hook.py
+-rw-r--r--   0        0        0     1182 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/semver.py
+-rw-r--r--   0        0        0     1346 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/di/vcs.py
+-rw-r--r--   0        0        0     3488 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/exc.py
+-rw-r--r--   0        0        0     5704 2024-05-19 07:31:47.398818 bumpify-0.3.0/bumpify/utils.py
+-rw-r--r--   0        0        0      946 2024-05-19 07:31:47.398818 bumpify-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 bumpify-0.3.0/PKG-INFO
```

### Comparing `bumpify-0.2.0/LICENSE` & `bumpify-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/README.md` & `bumpify-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/context.py` & `bumpify-0.3.0/bumpify/context.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/api/commands.py` & `bumpify-0.3.0/bumpify/core/api/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bumpify import utils
 from bumpify.core.config.interface import IConfigReaderWriter
-from bumpify.core.config.objects import LoadedModuleConfig
+from bumpify.core.config.objects import LoadedSection
 from bumpify.core.filesystem.interface import IFileSystemReader, IFileSystemReaderWriter
 from bumpify.core.semver.interface import ISemVerApi
 from bumpify.core.semver.objects import Changelog, ChangelogEntry, SemVerConfig, Version
 from bumpify.core.vcs.interface import IVcsReaderWriter
 
 from .interface import IBumpCommand, IInitCommand
 
@@ -25,15 +25,15 @@
         presenter.notify_done()
 
 
 class BumpCommand(IBumpCommand):
 
     def __init__(
         self,
-        semver_config: LoadedModuleConfig[SemVerConfig],
+        semver_config: LoadedSection[SemVerConfig],
         semver_api: ISemVerApi,
         filesystem_reader_writer: IFileSystemReaderWriter,
         vcs_reader_writer: IVcsReaderWriter,
     ):
         self._semver_config = semver_config
         self._semver_api = semver_api
         self._filesystem_reader_writer = filesystem_reader_writer
```

### Comparing `bumpify-0.2.0/bumpify/core/api/interface.py` & `bumpify-0.3.0/bumpify/core/api/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/api/presenters.py` & `bumpify-0.3.0/bumpify/core/api/presenters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/api/providers.py` & `bumpify-0.3.0/bumpify/core/api/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import List
 
 from bumpify.core.api.interface import IInitCommand
-from bumpify.core.config.objects import Config, VCSConfig
+from bumpify.core.config.objects import Config
 from bumpify.core.console.helpers import prompt_confirm, prompt_enum, prompt_string
 from bumpify.core.console.interface import IConsoleInput
 from bumpify.core.semver.objects import SemVerConfig, VersionComponent
+from bumpify.core.vcs.objects import VCSConfig
 
 
 class InitProvider(IInitCommand.IInitProvider):
 
     def __init__(self, cin: IConsoleInput):
         self._cin = cin
 
     def provide_config(self) -> Config:
-        config = Config(vcs=self._VCSConfigProvider(self._cin).provide())
+        config = Config()
+        config.save_section(self._VCSConfigProvider(self._cin).provide())
         if prompt_confirm(self._cin, "Create semantic versioning configuration?", default=True):
-            config.save_module_config(self._SemVerConfigProvider(self._cin).provide())
+            config.save_section(self._SemVerConfigProvider(self._cin).provide())
         return config
 
     class _SemVerConfigProvider:
 
         def __init__(self, cin: IConsoleInput):
             self._cin = cin
```

### Comparing `bumpify-0.2.0/bumpify/core/config/exc.py` & `bumpify-0.3.0/bumpify/core/config/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/config/helpers.py` & `bumpify-0.3.0/bumpify/core/config/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/config/implementation.py` & `bumpify-0.3.0/bumpify/core/config/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,18 @@
         try:
             data = tomlkit.loads(data)
         except tomlkit.exceptions.ParseError as e:
             raise ConfigParseError(self.abspath(), str(e), original_exc=e)
         try:
             return LoadedConfig(
                 config_file_abspath=self.abspath(),
-                config=Config(**data),
+                config=Config(data=data),
             )
         except pydantic.ValidationError as e:
             raise ConfigValidationError(self.abspath(), exc.ValidationError(e))
 
     def save(self, config: Config):
-        data = config.model_dump()
-        data = utils.json_dict(data, exclude_none=True)
+        data = utils.json_dict(config.data, exclude_none=True)
         data = tomlkit.dumps(data)
         self._filesystem_reader_writer.write(
             self._config_file_path, data.encode(self._config_file_encoding)
         )
```

### Comparing `bumpify-0.2.0/bumpify/core/config/interface.py` & `bumpify-0.3.0/bumpify/core/config/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/_message_formatter.py` & `bumpify-0.3.0/bumpify/core/console/_message_formatter.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/helpers.py` & `bumpify-0.3.0/bumpify/core/console/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/input.py` & `bumpify-0.3.0/bumpify/core/console/input.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/interface.py` & `bumpify-0.3.0/bumpify/core/console/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/objects.py` & `bumpify-0.3.0/bumpify/core/console/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/console/output.py` & `bumpify-0.3.0/bumpify/core/console/output.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/filesystem/exc.py` & `bumpify-0.3.0/bumpify/core/filesystem/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/filesystem/helpers.py` & `bumpify-0.3.0/bumpify/core/filesystem/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/filesystem/implementation.py` & `bumpify-0.3.0/bumpify/core/filesystem/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/filesystem/interface.py` & `bumpify-0.3.0/bumpify/core/filesystem/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/hook/exc.py` & `bumpify-0.3.0/bumpify/core/hook/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/hook/implementation.py` & `bumpify-0.3.0/bumpify/core/hook/implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
 
     def __init__(self, loaded_config: LoadedConfig, filesystem_reader: IFileSystemReader):
         self._loaded_config = loaded_config
         self._filesystem_reader = filesystem_reader
 
     def load(self) -> IHookApi:
-        hook_config = self._loaded_config.config.load_module_config(HookConfig)
+        hook_config = self._loaded_config.config.load_section(HookConfig)
         if not hook_config:
             return self._HookApi({})
         all_hook_functions = {}
         for path in hook_config.paths:
             hook_payload = self._filesystem_reader.read(path)
             try:
                 g = globals()
```

### Comparing `bumpify-0.2.0/bumpify/core/hook/interface.py` & `bumpify-0.3.0/bumpify/core/hook/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/_changelog_formatters.py` & `bumpify-0.3.0/bumpify/core/semver/_changelog_formatters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/_constants.py` & `bumpify-0.3.0/bumpify/core/semver/_constants.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/_hook_invokers.py` & `bumpify-0.3.0/bumpify/core/semver/_hook_invokers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/_parsing.py` & `bumpify-0.3.0/bumpify/core/semver/_parsing.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/_version_file_updater.py` & `bumpify-0.3.0/bumpify/core/semver/_version_file_updater.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/exc.py` & `bumpify-0.3.0/bumpify/core/semver/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/helpers.py` & `bumpify-0.3.0/bumpify/core/semver/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/implementation.py` & `bumpify-0.3.0/bumpify/core/semver/implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 from typing import List, Optional
 
-from bumpify.core.config.objects import LoadedModuleConfig
+from bumpify.core.config.objects import LoadedSection
 from bumpify.core.filesystem.interface import IFileSystemReaderWriter
 from bumpify.core.hook.interface import IHookApi
 from bumpify.core.semver.objects import (
     Changelog,
     ChangelogEntry,
     ChangelogEntryData,
     ConventionalCommit,
@@ -21,15 +21,15 @@
 
 
 class SemVerApi(ISemVerApi):
     """Default implementation of the semantic versioning API."""
 
     def __init__(
         self,
-        semver_config: LoadedModuleConfig[SemVerConfig],
+        semver_config: LoadedSection[SemVerConfig],
         filesystem_reader_writer: IFileSystemReaderWriter,
         vcs_reader_writer: IVcsReaderWriter,
         hook_api: IHookApi,
     ):
         self._semver_config = semver_config
         self._filesystem_reader_writer = filesystem_reader_writer
         self._vcs_reader_writer = vcs_reader_writer
```

### Comparing `bumpify-0.2.0/bumpify/core/semver/interface.py` & `bumpify-0.3.0/bumpify/core/semver/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/semver/objects.py` & `bumpify-0.3.0/bumpify/core/semver/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import datetime
 import enum
 import re
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel
 
-from bumpify.core.config.objects import register_module_config
+from bumpify.core.config.objects import register_section
 from bumpify.core.vcs.objects import Commit, Tag
 
 from . import _constants, _parsing
 
 
 class VersionComponent(enum.Enum):
     """Enumeration with version component names."""
 
     # TODO: Add comparator: major > minor > patch
     MAJOR = "major"
     MINOR = "minor"
     PATCH = "patch"
 
 
-@register_module_config("semver")
+@register_section("semver")
 class SemVerConfig(BaseModel):
     """Model to store semantic versioning configuration."""
 
     class VersionFile(BaseModel):
         """Version file configuration model."""
 
         #: Path to a version file.
```

### Comparing `bumpify-0.2.0/bumpify/core/vcs/exc.py` & `bumpify-0.3.0/bumpify/core/vcs/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/vcs/helpers.py` & `bumpify-0.3.0/bumpify/core/vcs/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/vcs/implementation/git.py` & `bumpify-0.3.0/bumpify/core/vcs/implementation/git.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/vcs/implementation/proxy.py` & `bumpify-0.3.0/bumpify/core/vcs/implementation/proxy.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/vcs/interface.py` & `bumpify-0.3.0/bumpify/core/vcs/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/core/vcs/objects.py` & `bumpify-0.3.0/bumpify/core/vcs/objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 import datetime
 import typing
+import enum
 
 from pydantic import BaseModel, field_validator
 
+from bumpify.core.config.objects import register_section
+
+
+@register_section("vcs")
+class VCSConfig(BaseModel):
+    """VCS repository configuration model."""
+
+    class Type(enum.Enum):
+        """Supported VCS types."""
+
+        AUTO = "auto"
+        GIT = "git"
+
+    #: VCS type.
+    type: Type
+
 
 class Commit(BaseModel):
     """Model representing information parsed from a single commit."""
 
     #: Commit's revision.
     #:
     #: This uniquely identifies a commit within entire repository. For example,
```

### Comparing `bumpify-0.2.0/bumpify/delivery/cli/__main__.py` & `bumpify-0.3.0/bumpify/delivery/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/delivery/cli/decorators.py` & `bumpify-0.3.0/bumpify/delivery/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/di/__init__.py` & `bumpify-0.3.0/bumpify/di/__init__.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/di/api.py` & `bumpify-0.3.0/bumpify/di/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from bumpify import utils
 from bumpify.core.api.commands import BumpCommand, InitCommand
 from bumpify.core.api.interface import IBumpCommand, IInitCommand
 from bumpify.core.api.presenters import BumpCommandPresenter, InitPresenter
 from bumpify.core.api.providers import InitProvider
 from bumpify.core.config.interface import IConfigReaderWriter
-from bumpify.core.config.objects import LoadedModuleConfig
+from bumpify.core.config.objects import LoadedSection
 from bumpify.core.console.interface import IConsoleInput, IConsoleOutput
 from bumpify.core.filesystem.interface import IFileSystemReaderWriter
 from bumpify.core.semver.interface import ISemVerApi
 from bumpify.core.semver.objects import SemVerConfig
 from bumpify.core.vcs.interface import IVcsReaderWriter
 
 provider = Provider()
@@ -32,15 +32,15 @@
 def make_init_presenter(injector):
     cout = utils.inject_type(injector, IConsoleOutput)
     return InitPresenter(cout)
 
 
 @provider.provides(IBumpCommand)
 def make_bump_command(injector):
-    semver_config = utils.inject_type(injector, LoadedModuleConfig[SemVerConfig])
+    semver_config = utils.inject_type(injector, LoadedSection[SemVerConfig])
     semver_api = utils.inject_type(injector, ISemVerApi)
     filesystem_reader_writer = utils.inject_type(injector, IFileSystemReaderWriter)
     vcs_reader_writer = utils.inject_type(injector, IVcsReaderWriter)
     return BumpCommand(semver_config, semver_api, filesystem_reader_writer, vcs_reader_writer)
 
 
 @provider.provides(IBumpCommand.IBumpPresenter)
```

### Comparing `bumpify-0.2.0/bumpify/di/config.py` & `bumpify-0.3.0/bumpify/di/config.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/di/filesystem.py` & `bumpify-0.3.0/bumpify/di/filesystem.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/di/hook.py` & `bumpify-0.3.0/bumpify/di/hook.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/bumpify/di/semver.py` & `bumpify-0.3.0/bumpify/di/semver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pydio.api import Provider
 
 from bumpify import utils
-from bumpify.core.config.objects import LoadedConfig, LoadedModuleConfig
+from bumpify.core.config.objects import LoadedConfig, LoadedSection
 from bumpify.core.filesystem.interface import IFileSystemReaderWriter
 from bumpify.core.hook.interface import IHookApi
 from bumpify.core.semver.implementation import SemVerApi
 from bumpify.core.semver.interface import ISemVerApi
 from bumpify.core.semver.objects import SemVerConfig
 from bumpify.core.vcs.interface import IVcsReaderWriter
 
 provider = Provider()
 
 
 @provider.provides(ISemVerApi)
 def make_semver_api(injector):
-    semver_config = utils.inject_type(injector, LoadedModuleConfig[SemVerConfig])
+    semver_config = utils.inject_type(injector, LoadedSection[SemVerConfig])
     filesystem_reader_writer = utils.inject_type(injector, IFileSystemReaderWriter)
     vcs_reader_writer = utils.inject_type(injector, IVcsReaderWriter)
     hook_api = utils.inject_type(injector, IHookApi)
     return SemVerApi(semver_config, filesystem_reader_writer, vcs_reader_writer, hook_api)
 
 
-@provider.provides(LoadedModuleConfig[SemVerConfig])
+@provider.provides(LoadedSection[SemVerConfig])
 def make_loaded_semver_config(injector):
     loaded_config = utils.inject_type(injector, LoadedConfig)
-    loaded_semver_config = loaded_config.require_module_config(SemVerConfig)
+    loaded_semver_config = loaded_config.require_section(SemVerConfig)
     return loaded_semver_config
```

### Comparing `bumpify-0.2.0/bumpify/exc.py` & `bumpify-0.3.0/bumpify/exc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import dataclasses
 import textwrap
 import typing
+import dataclasses
 
 import pydantic
 
 
 class BumpifyError(Exception):
     """Common base class for all Bumpify specific exceptions."""
 
@@ -68,36 +68,52 @@
     @property
     def stderr_str(self) -> str:
         """Command's STDERR decoded to string."""
         return self.stderr.decode()
 
 
 class ValidationError(BumpifyError):
-    """Generic exception for wrapping Pydantic validation error behind Bumpify
-    specific exception class."""
+    """Generic model validation error class.
+
+    This is mostly used for wrapping 3rd party validation errors behind
+    Bumpify-specific exception interface, allowing those to be handled in user
+    friendly way.
+    """
 
+    @dataclasses.dataclass
     class ErrorItem:
-        """Wraps single error."""
+        """Object containing information about single error."""
 
-        def __init__(self, error: dict):
-            self._error = error
+        #: Error location in a model that failed validation.
+        loc: tuple
 
-        @property
-        def loc_str(self) -> str:
-            return ".".join(str(x) for x in self._error["loc"])
+        #: Error message text.
+        msg: str
 
         @property
-        def msg(self) -> str:
-            return self._error["msg"]
+        def loc_str(self) -> str:
+            """Error location formatted as string."""
+            return ".".join(str(x) for x in self.loc)
 
     #: List of validation errors.
     errors: typing.List[ErrorItem]
 
-    #: Original Pydantic's validation error.
-    original_exc: pydantic.ValidationError
-
-    def __init__(self, original_exc: pydantic.ValidationError):
+    def __init__(self, errors: typing.List[ErrorItem], original_exc: Exception=None):
         super().__init__(original_exc)
-        self.errors = [self.ErrorItem(e) for e in original_exc.errors()]
+        self.errors = errors
+
+    def find_msg_by_loc(self, *loc) -> typing.Optional[str]:
+        """Return message for error location given via positional args.
+
+        If given location does not exist in error list, then ``None`` is
+        returned.
+        """
+        for item in self.errors:
+            if item.loc == loc:
+                return item.msg
 
     def __str__(self):
-        return str(self.original_exc)
+        rows = []
+        for e in self.errors:
+            rows.append(textwrap.indent(e.loc_str, " "*2))
+            rows.append(textwrap.indent(e.msg, " "*4))
+        return "\n" + "\n".join(rows)
```

### Comparing `bumpify-0.2.0/bumpify/utils.py` & `bumpify-0.3.0/bumpify/utils.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.2.0/pyproject.toml` & `bumpify-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bumpify"
-version = "0.2.0"
+version = "0.3.0"
 description = "Semantic versioning automation tool for software projects"
 authors = ["Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mwiatrzyk/bumpify"
 keywords = ["semantic", "versioning", "cli", "tool"]
 classifiers = [
```

### Comparing `bumpify-0.2.0/PKG-INFO` & `bumpify-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpify
-Version: 0.2.0
+Version: 0.3.0
 Summary: Semantic versioning automation tool for software projects
 Home-page: https://github.com/mwiatrzyk/bumpify
 License: MIT
 Keywords: semantic,versioning,cli,tool
 Author: Maciej Wiatrzyk
 Author-email: maciej.wiatrzyk@gmail.com
 Requires-Python: >=3.8,<4.0
```

