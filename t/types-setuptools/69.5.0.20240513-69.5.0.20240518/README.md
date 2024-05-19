# Comparing `tmp/types-setuptools-69.5.0.20240513.tar.gz` & `tmp/types-setuptools-69.5.0.20240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-69.5.0.20240513.tar", last modified: Mon May 13 02:23:30 2024, max compression
+gzip compressed data, was "types-setuptools-69.5.0.20240518.tar", last modified: Sat May 18 02:21:11 2024, max compression
```

## Comparing `types-setuptools-69.5.0.20240513.tar` & `types-setuptools-69.5.0.20240518.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/
--rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.178083 types-setuptools-69.5.0.20240513/distutils-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/distutils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.178083 types-setuptools-69.5.0.20240513/distutils-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.178083 types-setuptools-69.5.0.20240513/distutils-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/distutils-stubs/compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/distutils-stubs/util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.178083 types-setuptools-69.5.0.20240513/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    20037 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.182083 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/requirements.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.182083 types-setuptools-69.5.0.20240513/pkg_resources-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/pkg_resources-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.186083 types-setuptools-69.5.0.20240513/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.186083 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/_modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/ccompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.186083 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/bdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/upload.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.186083 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/compat/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/sysconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.190083 types-setuptools-69.5.0.20240513/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/bdist_egg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/bdist_rpm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/editable_wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/command/upload_docs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.190083 types-setuptools-69.5.0.20240513/setuptools-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/compat/py310.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/compat/py311.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/compat/py39.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/setuptools-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/config/expand.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/config/pyprojecttoml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/config/setupcfg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/modified.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:28.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 02:23:18.000000 types-setuptools-69.5.0.20240513/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 02:23:30.194083 types-setuptools-69.5.0.20240513/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-13 02:23:30.000000 types-setuptools-69.5.0.20240513/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-13 02:23:30.000000 types-setuptools-69.5.0.20240513/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 02:23:30.000000 types-setuptools-69.5.0.20240513/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 02:23:30.000000 types-setuptools-69.5.0.20240513/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/
+-rw-r--r--   0 runner    (1001) docker     (127)    17882 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.489235 types-setuptools-69.5.0.20240518/distutils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/distutils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.493235 types-setuptools-69.5.0.20240518/distutils-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.493235 types-setuptools-69.5.0.20240518/distutils-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/distutils-stubs/compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/distutils-stubs/util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.493235 types-setuptools-69.5.0.20240518/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    20037 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.493235 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/requirements.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/specifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.493235 types-setuptools-69.5.0.20240518/pkg_resources-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/pkg_resources-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.497235 types-setuptools-69.5.0.20240518/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.497235 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/_modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/ccompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.501235 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/bdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/upload.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.501235 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/sysconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/bdist_egg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/bdist_rpm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/editable_wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/command/upload_docs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/setuptools-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/compat/py310.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/compat/py311.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/compat/py39.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/setuptools-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/config/expand.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/config/pyprojecttoml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/config/setupcfg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/modified.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:09.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 02:20:52.000000 types-setuptools-69.5.0.20240518/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:21:11.505235 types-setuptools-69.5.0.20240518/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-18 02:21:11.000000 types-setuptools-69.5.0.20240518/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-18 02:21:11.000000 types-setuptools-69.5.0.20240518/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 02:21:11.000000 types-setuptools-69.5.0.20240518/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-18 02:21:11.000000 types-setuptools-69.5.0.20240518/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-69.5.0.20240513/CHANGELOG.md` & `types-setuptools-69.5.0.20240518/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 69.5.0.20240518 (2024-05-18)
+
+`distutils`: improve boolean parameters with int defaults (#11928)
+
 ## 69.5.0.20240513 (2024-05-13)
 
 Avoid using new `_typeshed` protocol in `pkg_resources` for now (#11909)
 
 Use protocols instead of `importlib.abc.Loader/MetaPathFinder/PathEntryFinder` (#11890)
 
 ## 69.5.0.20240423 (2024-04-23)
```

### Comparing `types-setuptools-69.5.0.20240513/PKG-INFO` & `types-setuptools-69.5.0.20240518/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240513
+Version: 69.5.0.20240518
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `459c3288da6245c9687e51aa65caf6ecfef68ea0` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240513/pkg_resources-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240518/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/markers.pyi` & `types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/markers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/specifiers.pyi` & `types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/specifiers.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/pkg_resources-stubs/_vendored_packaging/version.pyi` & `types-setuptools-69.5.0.20240518/pkg_resources-stubs/_vendored_packaging/version.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/pkg_resources-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240518/pkg_resources-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setup.py` & `types-setuptools-69.5.0.20240518/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `459c3288da6245c9687e51aa65caf6ecfef68ea0` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="69.5.0.20240513",
+      version="69.5.0.20240518",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['setuptools-stubs', 'distutils-stubs', 'pkg_resources-stubs'],
-      package_data={'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed'], 'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed']},
+      packages=['pkg_resources-stubs', 'distutils-stubs', 'setuptools-stubs'],
+      package_data={'pkg_resources-stubs': ['__init__.pyi', '_vendored_packaging/__init__.pyi', '_vendored_packaging/markers.pyi', '_vendored_packaging/requirements.pyi', '_vendored_packaging/specifiers.pyi', '_vendored_packaging/version.pyi', 'extern/__init__.pyi', 'METADATA.toml', 'py.typed'], 'distutils-stubs': ['_modified.pyi', 'archive_util.pyi', 'ccompiler.pyi', 'cmd.pyi', 'command/bdist.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/install.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/sdist.pyi', 'command/upload.pyi', 'compat/__init__.pyi', 'config.pyi', 'dep_util.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'filelist.pyi', 'sysconfig.pyi', 'util.pyi', 'METADATA.toml', 'compat/py.typed'], 'setuptools-stubs': ['__init__.pyi', '_distutils/_modified.pyi', '_distutils/archive_util.pyi', '_distutils/ccompiler.pyi', '_distutils/cmd.pyi', '_distutils/command/bdist.pyi', '_distutils/command/bdist_rpm.pyi', '_distutils/command/build.pyi', '_distutils/command/build_clib.pyi', '_distutils/command/build_ext.pyi', '_distutils/command/build_py.pyi', '_distutils/command/install.pyi', '_distutils/command/install_lib.pyi', '_distutils/command/install_scripts.pyi', '_distutils/command/register.pyi', '_distutils/command/sdist.pyi', '_distutils/command/upload.pyi', '_distutils/compat/__init__.pyi', '_distutils/config.pyi', '_distutils/dep_util.pyi', '_distutils/dist.pyi', '_distutils/errors.pyi', '_distutils/extension.pyi', '_distutils/filelist.pyi', '_distutils/sysconfig.pyi', '_distutils/util.pyi', 'archive_util.pyi', 'build_meta.pyi', 'command/__init__.pyi', 'command/alias.pyi', 'command/bdist_egg.pyi', 'command/bdist_rpm.pyi', 'command/build.pyi', 'command/build_clib.pyi', 'command/build_ext.pyi', 'command/build_py.pyi', 'command/develop.pyi', 'command/dist_info.pyi', 'command/easy_install.pyi', 'command/editable_wheel.pyi', 'command/egg_info.pyi', 'command/install.pyi', 'command/install_egg_info.pyi', 'command/install_lib.pyi', 'command/install_scripts.pyi', 'command/register.pyi', 'command/rotate.pyi', 'command/saveopts.pyi', 'command/sdist.pyi', 'command/setopt.pyi', 'command/test.pyi', 'command/upload.pyi', 'command/upload_docs.pyi', 'compat/__init__.pyi', 'compat/py310.pyi', 'compat/py311.pyi', 'compat/py39.pyi', 'config/__init__.pyi', 'config/expand.pyi', 'config/pyprojecttoml.pyi', 'config/setupcfg.pyi', 'dep_util.pyi', 'depends.pyi', 'discovery.pyi', 'dist.pyi', 'errors.pyi', 'extension.pyi', 'extern/__init__.pyi', 'glob.pyi', 'installer.pyi', 'launch.pyi', 'logging.pyi', 'modified.pyi', 'monkey.pyi', 'msvc.pyi', 'namespaces.pyi', 'package_index.pyi', 'sandbox.pyi', 'unicode_utils.pyi', 'version.pyi', 'warnings.pyi', 'wheel.pyi', 'windows_support.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/__init__.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from _typeshed import StrPath
 from abc import abstractmethod
 from collections.abc import Iterable, Mapping, Sequence
-from typing import Any
+from typing import Any, Literal
 
 from ._distutils.cmd import Command as _Command
 from .depends import Require as Require
 from .dist import Distribution as Distribution
 from .extension import Extension as Extension
 from .warnings import SetuptoolsDeprecationWarning as SetuptoolsDeprecationWarning
 
@@ -72,15 +72,17 @@
 ) -> Distribution: ...
 
 class Command(_Command):
     command_consumes_arguments: bool
     distribution: Distribution
     def __init__(self, dist: Distribution, **kw: Any) -> None: ...
     def ensure_string_list(self, option: str | list[str]) -> None: ...
-    def reinitialize_command(self, command: _Command | str, reinit_subcommands: int = 0, **kw: Any) -> _Command: ...
+    def reinitialize_command(
+        self, command: _Command | str, reinit_subcommands: bool | Literal[0, 1] = 0, **kw: Any
+    ) -> _Command: ...
     @abstractmethod
     def initialize_options(self) -> None: ...
     @abstractmethod
     def finalize_options(self) -> None: ...
     @abstractmethod
     def run(self) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/archive_util.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/archive_util.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from typing import Literal
+
 def make_archive(
     base_name: str,
     format: str,
     root_dir: str | None = ...,
     base_dir: str | None = ...,
-    verbose: int = ...,
-    dry_run: int = ...,
+    verbose: bool | Literal[0, 1] = 0,
+    dry_run: bool | Literal[0, 1] = 0,
     owner: str | None = ...,
     group: str | None = ...,
 ) -> str: ...
 def make_tarball(
     base_name: str,
     base_dir: str,
     compress: str | None = ...,
-    verbose: int = ...,
-    dry_run: int = ...,
+    verbose: bool | Literal[0, 1] = 0,
+    dry_run: bool | Literal[0, 1] = 0,
     owner: str | None = ...,
     group: str | None = ...,
 ) -> str: ...
-def make_zipfile(base_name: str, base_dir: str, verbose: int = ..., dry_run: int = ...) -> str: ...
+def make_zipfile(base_name: str, base_dir: str, verbose: bool | Literal[0, 1] = 0, dry_run: bool | Literal[0, 1] = 0) -> str: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/ccompiler.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/ccompiler.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from collections.abc import Callable
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Literal
 from typing_extensions import TypeAlias
 
 _Macro: TypeAlias = tuple[str] | tuple[str, str | None]
 
 def gen_lib_options(
     compiler: CCompiler, library_dirs: list[str], runtime_library_dirs: list[str], libraries: list[str]
 ) -> list[str]: ...
 def gen_preprocess_options(macros: list[_Macro], include_dirs: list[str]) -> list[str]: ...
 def get_default_compiler(osname: str | None = ..., platform: str | None = ...) -> str: ...
 def new_compiler(
-    plat: str | None = ..., compiler: str | None = ..., verbose: int = ..., dry_run: int = ..., force: int = ...
+    plat: str | None = ...,
+    compiler: str | None = ...,
+    verbose: bool | Literal[0, 1] = 0,
+    dry_run: bool | Literal[0, 1] = 0,
+    force: bool | Literal[0, 1] = 0,
 ) -> CCompiler: ...
 def show_compilers() -> None: ...
 
 class CCompiler:
     src_extensions: ClassVar[list[str] | None]
     obj_extension: ClassVar[str | None]
     static_lib_extension: ClassVar[str | None]
@@ -30,29 +34,31 @@
     output_dir: str | None
     macros: list[_Macro]
     include_dirs: list[str]
     libraries: list[str]
     library_dirs: list[str]
     runtime_library_dirs: list[str]
     objects: list[str]
-    def __init__(self, verbose: int = ..., dry_run: int = ..., force: int = ...) -> None: ...
+    def __init__(
+        self, verbose: bool | Literal[0, 1] = 0, dry_run: bool | Literal[0, 1] = 0, force: bool | Literal[0, 1] = 0
+    ) -> None: ...
     def add_include_dir(self, dir: str) -> None: ...
     def set_include_dirs(self, dirs: list[str]) -> None: ...
     def add_library(self, libname: str) -> None: ...
     def set_libraries(self, libnames: list[str]) -> None: ...
     def add_library_dir(self, dir: str) -> None: ...
     def set_library_dirs(self, dirs: list[str]) -> None: ...
     def add_runtime_library_dir(self, dir: str) -> None: ...
     def set_runtime_library_dirs(self, dirs: list[str]) -> None: ...
     def define_macro(self, name: str, value: str | None = ...) -> None: ...
     def undefine_macro(self, name: str) -> None: ...
     def add_link_object(self, object: str) -> None: ...
     def set_link_objects(self, objects: list[str]) -> None: ...
     def detect_language(self, sources: str | list[str]) -> str | None: ...
-    def find_library_file(self, dirs: list[str], lib: str, debug: bool = ...) -> str | None: ...
+    def find_library_file(self, dirs: list[str], lib: str, debug: bool | Literal[0, 1] = 0) -> str | None: ...
     def has_function(
         self,
         funcname: str,
         includes: list[str] | None = ...,
         include_dirs: list[str] | None = ...,
         libraries: list[str] | None = ...,
         library_dirs: list[str] | None = ...,
@@ -63,99 +69,103 @@
     def set_executables(self, **args: str) -> None: ...
     def compile(
         self,
         sources: list[str],
         output_dir: str | None = ...,
         macros: list[_Macro] | None = ...,
         include_dirs: list[str] | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
         depends: list[str] | None = ...,
     ) -> list[str]: ...
     def create_static_lib(
         self,
         objects: list[str],
         output_libname: str,
         output_dir: str | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         target_lang: str | None = ...,
     ) -> None: ...
     def link(
         self,
         target_desc: str,
         objects: list[str],
         output_filename: str,
         output_dir: str | None = ...,
         libraries: list[str] | None = ...,
         library_dirs: list[str] | None = ...,
         runtime_library_dirs: list[str] | None = ...,
         export_symbols: list[str] | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
         build_temp: str | None = ...,
         target_lang: str | None = ...,
     ) -> None: ...
     def link_executable(
         self,
         objects: list[str],
         output_progname: str,
         output_dir: str | None = ...,
         libraries: list[str] | None = ...,
         library_dirs: list[str] | None = ...,
         runtime_library_dirs: list[str] | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
         target_lang: str | None = ...,
     ) -> None: ...
     def link_shared_lib(
         self,
         objects: list[str],
         output_libname: str,
         output_dir: str | None = ...,
         libraries: list[str] | None = ...,
         library_dirs: list[str] | None = ...,
         runtime_library_dirs: list[str] | None = ...,
         export_symbols: list[str] | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
         build_temp: str | None = ...,
         target_lang: str | None = ...,
     ) -> None: ...
     def link_shared_object(
         self,
         objects: list[str],
         output_filename: str,
         output_dir: str | None = ...,
         libraries: list[str] | None = ...,
         library_dirs: list[str] | None = ...,
         runtime_library_dirs: list[str] | None = ...,
         export_symbols: list[str] | None = ...,
-        debug: bool = ...,
+        debug: bool | Literal[0, 1] = 0,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
         build_temp: str | None = ...,
         target_lang: str | None = ...,
     ) -> None: ...
     def preprocess(
         self,
         source: str,
         output_file: str | None = ...,
         macros: list[_Macro] | None = ...,
         include_dirs: list[str] | None = ...,
         extra_preargs: list[str] | None = ...,
         extra_postargs: list[str] | None = ...,
     ) -> None: ...
-    def executable_filename(self, basename: str, strip_dir: int = ..., output_dir: str = ...) -> str: ...
-    def library_filename(self, libname: str, lib_type: str = "static", strip_dir: int = 0, output_dir: str = "") -> str: ...
-    def object_filenames(self, source_filenames: list[str], strip_dir: int = ..., output_dir: str = ...) -> list[str]: ...
-    def shared_object_filename(self, basename: str, strip_dir: int = ..., output_dir: str = ...) -> str: ...
+    def executable_filename(self, basename: str, strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...) -> str: ...
+    def library_filename(
+        self, libname: str, lib_type: str = "static", strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ""
+    ) -> str: ...
+    def object_filenames(
+        self, source_filenames: list[str], strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...
+    ) -> list[str]: ...
+    def shared_object_filename(self, basename: str, strip_dir: bool | Literal[0, 1] = 0, output_dir: str = ...) -> str: ...
     def execute(self, func: Callable[..., object], args: tuple[Any, ...], msg: str | None = ..., level: int = ...) -> None: ...
     def spawn(self, cmd: list[str]) -> None: ...
     def mkpath(self, name: str, mode: int = ...) -> None: ...
     def move_file(self, src: str, dst: str) -> str: ...
     def announce(self, msg: str, level: int = ...) -> None: ...
     def warn(self, msg: str) -> None: ...
     def debug_print(self, msg: str) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/bdist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/bdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/bdist_rpm.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/bdist_rpm.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from typing import Literal
 
 from ..cmd import Command
 
 class build_py(Command):
     description: str
     user_options: Incomplete
     boolean_options: Incomplete
@@ -27,12 +28,12 @@
     def check_package(self, package, package_dir): ...
     def check_module(self, module, module_file): ...
     def find_package_modules(self, package, package_dir): ...
     def find_modules(self): ...
     def find_all_modules(self): ...
     def get_source_files(self): ...
     def get_module_outfile(self, build_dir, package, module): ...
-    def get_outputs(self, include_bytecode: int = ...): ...
+    def get_outputs(self, include_bytecode: bool | Literal[0, 1] = 1): ...
     def build_module(self, module, module_file, package): ...
     def build_modules(self) -> None: ...
     def build_packages(self) -> None: ...
     def byte_compile(self, files) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/command/upload.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/command/upload.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/filelist.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -13,25 +13,33 @@
     def append(self, item: str) -> None: ...
     def extend(self, items: Iterable[str]) -> None: ...
     def sort(self) -> None: ...
     def remove_duplicates(self) -> None: ...
     def process_template_line(self, line: str) -> None: ...
     @overload
     def include_pattern(
-        self, pattern: str, anchor: bool | Literal[0, 1] = ..., prefix: str | None = ..., is_regex: Literal[0, False] = ...
+        self, pattern: str, anchor: bool | Literal[0, 1] = 1, prefix: str | None = ..., is_regex: Literal[0, False] = 0
     ) -> bool: ...
     @overload
-    def include_pattern(self, pattern: str | Pattern[str], *, is_regex: Literal[True, 1] = ...) -> bool: ...
+    def include_pattern(self, pattern: str | Pattern[str], *, is_regex: Literal[True, 1]) -> bool: ...
     @overload
     def include_pattern(
-        self, pattern: str | Pattern[str], anchor: bool | Literal[0, 1] = ..., prefix: str | None = ..., is_regex: int = ...
+        self,
+        pattern: str | Pattern[str],
+        anchor: bool | Literal[0, 1] = 1,
+        prefix: str | None = ...,
+        is_regex: bool | Literal[0, 1] = 0,
     ) -> bool: ...
     @overload
     def exclude_pattern(
-        self, pattern: str, anchor: bool | Literal[0, 1] = ..., prefix: str | None = ..., is_regex: Literal[0, False] = ...
+        self, pattern: str, anchor: bool | Literal[0, 1] = 1, prefix: str | None = ..., is_regex: Literal[0, False] = 0
     ) -> bool: ...
     @overload
-    def exclude_pattern(self, pattern: str | Pattern[str], *, is_regex: Literal[True, 1] = ...) -> bool: ...
+    def exclude_pattern(self, pattern: str | Pattern[str], *, is_regex: Literal[True, 1]) -> bool: ...
     @overload
     def exclude_pattern(
-        self, pattern: str | Pattern[str], anchor: bool | Literal[0, 1] = ..., prefix: str | None = ..., is_regex: int = ...
+        self,
+        pattern: str | Pattern[str],
+        anchor: bool | Literal[0, 1] = 1,
+        prefix: str | None = ...,
+        is_regex: bool | Literal[0, 1] = 0,
     ) -> bool: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/sysconfig.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/sysconfig.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -13,10 +13,12 @@
 def get_config_var(name: str) -> int | str | None: ...
 @overload
 def get_config_vars() -> dict[str, str | int]: ...
 @overload
 def get_config_vars(arg: str, /, *args: str) -> list[str | int]: ...
 def get_config_h_filename() -> str: ...
 def get_makefile_filename() -> str: ...
-def get_python_inc(plat_specific: bool = ..., prefix: str | None = ...) -> str: ...
-def get_python_lib(plat_specific: bool = ..., standard_lib: bool = ..., prefix: str | None = ...) -> str: ...
+def get_python_inc(plat_specific: bool | Literal[0, 1] = 0, prefix: str | None = ...) -> str: ...
+def get_python_lib(
+    plat_specific: bool | Literal[0, 1] = 0, standard_lib: bool | Literal[0, 1] = 0, prefix: str | None = ...
+) -> str: ...
 def customize_compiler(compiler: CCompiler) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/_distutils/util.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/_distutils/util.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 def convert_path(pathname: str) -> str: ...
 def change_root(new_root: str, pathname: str) -> str: ...
 def check_environ() -> None: ...
 def subst_vars(s: str, local_vars: Mapping[str, str]) -> None: ...
 def grok_environment_error(exc: object, prefix: str = ...) -> str: ...
 def split_quoted(s: str) -> list[str]: ...
 def execute(
-    func: Callable[..., object], args: tuple[Any, ...], msg: str | None = ..., verbose: bool = ..., dry_run: bool = ...
+    func: Callable[..., object],
+    args: tuple[Any, ...],
+    msg: str | None = ...,
+    verbose: bool | Literal[0, 1] = 0,
+    dry_run: bool | Literal[0, 1] = 0,
 ) -> None: ...
 def strtobool(val: str) -> Literal[0, 1]: ...
 def byte_compile(
     py_files: list[str],
     optimize: int = ...,
-    force: bool = ...,
+    force: bool | Literal[0, 1] = 0,
     prefix: str | None = ...,
     base_dir: str | None = ...,
-    verbose: bool = ...,
-    dry_run: bool = ...,
+    verbose: bool | Literal[0, 1] = 1,
+    dry_run: bool | Literal[0, 1] = 0,
     direct: bool | None = ...,
 ) -> None: ...
 def rfc822_escape(header: str) -> str: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/archive_util.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/build_meta.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/bdist_egg.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/bdist_egg.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _typeshed import Incomplete
 from collections.abc import Generator
+from typing import Literal
 
 from .. import Command
 
 def strip_module(filename): ...
 def sorted_walk(dir) -> Generator[Incomplete, None, None]: ...
 def write_stub(resource, pyfile) -> None: ...
 
@@ -42,8 +43,15 @@
 
 def scan_module(egg_dir, base, name, stubs): ...
 def iter_symbols(code) -> Generator[Incomplete, None, None]: ...
 def can_scan(): ...
 
 INSTALL_DIRECTORY_ATTRS: Incomplete
 
-def make_zipfile(zip_filename, base_dir, verbose: int = 0, dry_run: int = 0, compress: bool = True, mode: str = "w"): ...
+def make_zipfile(
+    zip_filename,
+    base_dir,
+    verbose: bool | Literal[0, 1] = 0,
+    dry_run: bool | Literal[0, 1] = 0,
+    compress: bool = True,
+    mode: str = "w",
+): ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/build_ext.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Literal
 
 from .._distutils.command.build_ext import build_ext as _build_ext
 
 have_rtld: bool
 use_stubs: bool
 libtype: str
 
@@ -36,13 +36,13 @@
     objects,
     output_libname,
     output_dir: Incomplete | None = None,
     libraries: Incomplete | None = None,
     library_dirs: Incomplete | None = None,
     runtime_library_dirs: Incomplete | None = None,
     export_symbols: Incomplete | None = None,
-    debug: int = 0,
+    debug: bool | Literal[0, 1] = 0,
     extra_preargs: Incomplete | None = None,
     extra_postargs: Incomplete | None = None,
     build_temp: Incomplete | None = None,
     target_lang: Incomplete | None = None,
 ) -> None: ...
```

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/build_py.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/develop.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/editable_wheel.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/editable_wheel.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/sdist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/setopt.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/test.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/config/expand.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/config/expand.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/config/pyprojecttoml.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/config/pyprojecttoml.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/config/setupcfg.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/config/setupcfg.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/depends.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/discovery.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/dist.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/errors.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/extension.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/msvc.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/package_index.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/setuptools-stubs/sandbox.pyi` & `types-setuptools-69.5.0.20240518/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-69.5.0.20240513/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-69.5.0.20240518/types_setuptools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 69.5.0.20240513
+Version: 69.5.0.20240518
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-setuptools` aims to provide accurate annotations
 for `setuptools==69.5.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0382803c4c228229295ae601dc431e452980fbd2` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `459c3288da6245c9687e51aa65caf6ecfef68ea0` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-setuptools-69.5.0.20240513/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-69.5.0.20240518/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

