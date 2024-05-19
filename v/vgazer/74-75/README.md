# Comparing `tmp/vgazer-74.tar.gz` & `tmp/vgazer-75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgazer-74.tar", last modified: Mon Mar 18 19:26:16 2024, max compression
+gzip compressed data, was "vgazer-75.tar", last modified: Sun May 19 12:12:32 2024, max compression
```

## Comparing `vgazer-74.tar` & `vgazer-75.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.641214 vgazer-74/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-03-18 19:26:16.641214 vgazer-74/PKG-INFO
--rw-r--r--   0 edomin    (1000) edomin    (1000)     6164 2024-03-18 16:23:11.000000 vgazer-74/README.md
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.581214 vgazer-74/libvgazer/
--rw-r--r--   0 edomin    (1000) edomin    (1000)     7350 2024-03-07 08:31:51.000000 vgazer-74/libvgazer/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1742 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/checkers_manager.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1268 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/command.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.585214 vgazer-74/libvgazer/config/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/config/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2442 2024-02-24 20:34:09.000000 vgazer-74/libvgazer/config/cmake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2119 2024-02-24 20:33:20.000000 vgazer-74/libvgazer/config/meson.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      911 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/env_vars.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2027 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/exceptions.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2479 2024-03-18 16:33:43.000000 vgazer-74/libvgazer/host_detector.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.589214 vgazer-74/libvgazer/install/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2056 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/apt.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      480 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/cmd.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      964 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.621214 vgazer-74/libvgazer/install/custom_installer/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2212 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/alsa-lib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2574 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/autoconf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1672 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/automake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1466 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/cfgpath.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2039 2024-02-24 20:27:10.000000 vgazer-74/libvgazer/install/custom_installer/cjson.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1412 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/cmake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1114 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/cmake_barebones.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2151 2024-02-24 20:27:22.000000 vgazer-74/libvgazer/install/custom_installer/cmocka.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1405 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/codecoverage.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1901 2024-03-10 14:07:36.000000 vgazer-74/libvgazer/install/custom_installer/cwalk.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1445 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/dr_wav.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1884 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/expat.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2182 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/hash_table.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     4320 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/icu.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     4172 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/icu_54_2.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2646 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/inih.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1792 2024-02-24 19:25:08.000000 vgazer-74/libvgazer/install/custom_installer/iwyu.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1479 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/ketopt.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1922 2024-02-24 20:27:36.000000 vgazer-74/libvgazer/install/custom_installer/libclipboard.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1862 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libffi.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1878 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libglvnd.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1738 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/liblzma.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1616 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libogg.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1928 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libpng.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1703 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libsir.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1415 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libtool.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1749 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libvorbis.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1882 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/libxext.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1827 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/luajit.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2729 2024-02-21 08:02:09.000000 vgazer-74/libvgazer/install/custom_installer/lwrb.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1381 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/ninja.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1465 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/nuklear.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1739 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/pthread-stubs.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2017 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/scv.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1354 2024-03-18 19:01:55.000000 vgazer-74/libvgazer/install/custom_installer/stb_image.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1360 2024-03-18 19:02:23.000000 vgazer-74/libvgazer/install/custom_installer/stb_image_write.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1358 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/stb_rect_pack.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1355 2024-03-18 19:02:51.000000 vgazer-74/libvgazer/install/custom_installer/stb_vorbis.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2263 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/tinyfiledialogs.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1973 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/wayland-scanner.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2147 2024-02-24 20:28:41.000000 vgazer-74/libvgazer/install/custom_installer/wayland.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2143 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xau.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1765 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xcb-proto.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2005 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xcb.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xlib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2210 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xmempool.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1508 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xorg-macros.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1606 2024-02-24 20:39:09.000000 vgazer-74/libvgazer/install/custom_installer/xorgproto.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2040 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/xtrans.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1873 2024-02-24 20:26:47.000000 vgazer-74/libvgazer/install/custom_installer/zip.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2600 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/custom_installer/zlib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      902 2024-02-25 15:39:40.000000 vgazer-74/libvgazer/install/pacman.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      449 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/pip3.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/install/yum.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1904 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/installers_manager.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     5424 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/licenses.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      558 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/os_release.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    14062 2024-03-18 16:34:03.000000 vgazer-74/libvgazer/platform.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.629214 vgazer-74/libvgazer/software/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      853 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/software/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    17028 2024-03-18 16:24:58.000000 vgazer-74/libvgazer/software/a_f.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     9559 2024-03-18 16:25:55.000000 vgazer-74/libvgazer/software/g_i.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     7076 2024-03-18 16:26:26.000000 vgazer-74/libvgazer/software/j_libm.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     8980 2024-03-18 16:27:05.000000 vgazer-74/libvgazer/software/libo_libz.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    10567 2024-03-18 16:28:06.000000 vgazer-74/libvgazer/software/lin_o.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    10316 2024-03-18 19:00:28.000000 vgazer-74/libvgazer/software/p_s.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    22049 2024-03-18 16:30:29.000000 vgazer-74/libvgazer/software/t_xc.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    10203 2024-03-18 16:31:20.000000 vgazer-74/libvgazer/software/xd_z.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.629214 vgazer-74/libvgazer/store/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/store/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     5847 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/store/base.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      438 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/store/home.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      439 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/store/temp.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      621 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/utils.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.633214 vgazer-74/libvgazer/version/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      843 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/apt_cache.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      822 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/custom.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.637214 vgazer-74/libvgazer/version/custom_checker/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/custom_checker/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      941 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/custom_checker/autoconf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2802 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/git.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      228 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/pacman.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      149 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/yolk3k.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/version/yum.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      676 2024-02-19 18:06:30.000000 vgazer-74/libvgazer/working_dir.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)       38 2024-03-18 19:26:16.641214 vgazer-74/setup.cfg
--rw-r--r--   0 edomin    (1000) edomin    (1000)      914 2024-03-18 19:26:09.000000 vgazer-74/setup.py
--rwxr-xr-x   0 edomin    (1000) edomin    (1000)     1349 2024-02-19 18:06:30.000000 vgazer-74/vgazer
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-03-18 19:26:16.641214 vgazer-74/vgazer.egg-info/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/PKG-INFO
--rw-r--r--   0 edomin    (1000) edomin    (1000)     3815 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/SOURCES.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/dependency_links.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/not-zip-safe
--rw-r--r--   0 edomin    (1000) edomin    (1000)       32 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/requires.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)       10 2024-03-18 19:26:16.000000 vgazer-74/vgazer.egg-info/top_level.txt
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.225622 vgazer-75/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:12:32.225622 vgazer-75/PKG-INFO
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     6182 2024-05-18 19:42:39.000000 vgazer-75/README.md
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.165622 vgazer-75/libvgazer/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     7350 2024-05-19 11:13:14.000000 vgazer-75/libvgazer/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2012 2024-05-18 20:00:03.000000 vgazer-75/libvgazer/checkers_manager.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1268 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/command.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.169622 vgazer-75/libvgazer/config/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/config/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2442 2024-02-24 20:34:09.000000 vgazer-75/libvgazer/config/cmake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2119 2024-02-24 20:33:20.000000 vgazer-75/libvgazer/config/meson.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      911 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/env_vars.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2027 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/exceptions.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2971 2024-05-19 11:12:40.000000 vgazer-75/libvgazer/host_detector.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.173622 vgazer-75/libvgazer/install/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2056 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/apt.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      480 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/cmd.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      964 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.205622 vgazer-75/libvgazer/install/custom_installer/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2212 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/alsa-lib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2574 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/autoconf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1672 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/automake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1466 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cfgpath.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2039 2024-02-24 20:27:10.000000 vgazer-75/libvgazer/install/custom_installer/cjson.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1412 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cmake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1114 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cmake_barebones.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2151 2024-02-24 20:27:22.000000 vgazer-75/libvgazer/install/custom_installer/cmocka.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1405 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/codecoverage.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1901 2024-03-10 14:07:36.000000 vgazer-75/libvgazer/install/custom_installer/cwalk.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1429 2024-05-19 11:04:00.000000 vgazer-75/libvgazer/install/custom_installer/dr_wav.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1884 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/expat.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2182 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/hash_table.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     4320 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/icu.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     4172 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/icu_54_2.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2646 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/inih.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1792 2024-02-24 19:25:08.000000 vgazer-75/libvgazer/install/custom_installer/iwyu.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1479 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/ketopt.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1922 2024-02-24 20:27:36.000000 vgazer-75/libvgazer/install/custom_installer/libclipboard.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1862 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libffi.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1878 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libglvnd.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1738 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/liblzma.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1616 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libogg.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1928 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libpng.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1703 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libsir.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1415 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libtool.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1749 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libvorbis.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1882 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libxext.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1827 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/luajit.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2729 2024-02-21 08:02:09.000000 vgazer-75/libvgazer/install/custom_installer/lwrb.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1381 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/ninja.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1465 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/nuklear.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1739 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/pthread-stubs.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2017 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/scv.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1354 2024-03-18 19:01:55.000000 vgazer-75/libvgazer/install/custom_installer/stb_image.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1360 2024-03-18 19:02:23.000000 vgazer-75/libvgazer/install/custom_installer/stb_image_write.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1358 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/stb_rect_pack.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1355 2024-03-18 19:02:51.000000 vgazer-75/libvgazer/install/custom_installer/stb_vorbis.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2263 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/tinyfiledialogs.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1973 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/wayland-scanner.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2147 2024-02-24 20:28:41.000000 vgazer-75/libvgazer/install/custom_installer/wayland.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2143 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xau.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1765 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xcb-proto.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2005 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xcb.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xlib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2210 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xmempool.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1508 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xorg-macros.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1606 2024-02-24 20:39:09.000000 vgazer-75/libvgazer/install/custom_installer/xorgproto.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2040 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xtrans.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-05-19 11:35:51.000000 vgazer-75/libvgazer/install/custom_installer/zip.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2600 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/zlib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-05-18 20:00:49.000000 vgazer-75/libvgazer/install/dnf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      902 2024-02-25 15:39:40.000000 vgazer-75/libvgazer/install/pacman.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      449 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/pip3.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/yum.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2318 2024-05-18 20:00:14.000000 vgazer-75/libvgazer/installers_manager.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     5424 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/licenses.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      558 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/os_release.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    14072 2024-05-18 19:54:42.000000 vgazer-75/libvgazer/platform.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.209622 vgazer-75/libvgazer/software/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      853 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/software/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    20324 2024-05-19 12:11:59.000000 vgazer-75/libvgazer/software/a_f.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    12117 2024-05-19 11:43:14.000000 vgazer-75/libvgazer/software/g_i.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     7222 2024-05-19 11:45:28.000000 vgazer-75/libvgazer/software/j_libm.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    10549 2024-05-19 11:49:12.000000 vgazer-75/libvgazer/software/libo_libz.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    12147 2024-05-19 11:53:58.000000 vgazer-75/libvgazer/software/lin_o.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    13177 2024-05-19 11:57:08.000000 vgazer-75/libvgazer/software/p_s.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    26795 2024-05-19 12:00:54.000000 vgazer-75/libvgazer/software/t_xc.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    11360 2024-05-19 12:10:59.000000 vgazer-75/libvgazer/software/xd_z.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.213622 vgazer-75/libvgazer/store/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     5847 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/base.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      438 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/home.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      439 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/temp.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      621 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/utils.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.217622 vgazer-75/libvgazer/version/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      843 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/apt_cache.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      822 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.221622 vgazer-75/libvgazer/version/custom_checker/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom_checker/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      941 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom_checker/autoconf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-05-18 20:00:42.000000 vgazer-75/libvgazer/version/dnf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2802 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/git.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      228 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/pacman.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      149 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/yolk3k.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/yum.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      676 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/working_dir.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       38 2024-05-19 12:12:32.225622 vgazer-75/setup.cfg
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      914 2024-05-19 12:12:11.000000 vgazer-75/setup.py
+-rwxr-xr-x   0 edomin    (1000) edomin    (1000)     1349 2024-02-19 18:06:30.000000 vgazer-75/vgazer
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.225622 vgazer-75/vgazer.egg-info/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/PKG-INFO
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     3865 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/SOURCES.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/dependency_links.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/not-zip-safe
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       32 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/requires.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       10 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/top_level.txt
```

### Comparing `vgazer-74/PKG-INFO` & `vgazer-75/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vgazer
-Version: 74
+Version: 75
 Summary: Library for checking versions and installing various software
 Home-page: https://github.com/edomin/vgazer
 Author: Vasiliy Edomin
 Author-email: Vasiliy.Edomin@gmail.com
 License: CC0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vgazer-74/README.md` & `vgazer-75/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 **hos** and **hver** - OS or Linux Distribution and version of OS or Linux
 Distribution. This is not OS and OS's version of your PC. Typically it is OS
 and OS's version of base Docker image. Currently supported:
 
 * archlinux
     * latest
+* fedora
+    * 40
 * oraclelinux
     * 7
 
 **tarch** - architecture of device for crossplatform compiling libraries.
 Currently supported:
 
 * x86_64
```

### Comparing `vgazer-74/libvgazer/__init__.py` & `vgazer-75/libvgazer/__init__.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/checkers_manager.py` & `vgazer-75/libvgazer/checkers_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from libvgazer.exceptions        import UnknownVersionChecker
 from libvgazer.version.apt_cache import CheckAptCache
+from libvgazer.version.dnf       import CheckDnf
 from libvgazer.version.git       import CheckGit
 from libvgazer.version.pacman    import CheckPacman
 from libvgazer.version.yolk3k    import CheckYolk3k
 from libvgazer.version.yum       import CheckYum
 
 class CheckersManager:
     def __init__(self):
         self.checkFuncs = {
             "apt-cache": lambda platform, checkerData: CheckAptCache(
                 checkerData["package"],
                 platform.GetArch()
             ),
+            "dnf": lambda platform, checkerData: CheckDnf(
+                checkerData["package"],
+                checkerData["repo"] if "repo" in checkerData else None,
+                platform.GetArch()
+            ),
             "fixed": lambda platform, checkerData: checkerData["version"],
             "git": lambda platform, checkerData: CheckGit(
                 checkerData["url"],
                 checkerData["hint"] if "hint" in checkerData else None,
                 checkerData["files"] if "files" in checkerData else None
             ),
             "pacman": lambda platform, checkerData: CheckPacman(
```

### Comparing `vgazer-74/libvgazer/command.py` & `vgazer-75/libvgazer/command.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/config/cmake.py` & `vgazer-75/libvgazer/config/cmake.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/config/meson.py` & `vgazer-75/libvgazer/config/meson.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/env_vars.py` & `vgazer-75/libvgazer/env_vars.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/exceptions.py` & `vgazer-75/libvgazer/exceptions.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/host_detector.py` & `vgazer-75/libvgazer/host_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,39 @@
 class HostDetector:
     @staticmethod
     def GetLinuxOs():
         with OsRelease() as osRelease:
             try:
                 return {
                     "arch":   "archlinux",
+                    "fedora": "fedora",
                     "ol":     "oraclelinux",
                     "debian": "debian",
                 }[osRelease.GetEntry("ID")]
             except KeyError:
                 raise OsDataNotFound(
                  "Unable to find data of host OS: " + os.name)
 
     @staticmethod
+    def GetFedoraVersion():
+        with OsRelease() as osRelease:
+            try:
+                return osRelease.GetEntry("VERSION").split(" ")[0]
+            except KeyError:
+                raise ReleaseDataNotFound(
+                 "Unable to find data of Fedora version: " + os.name)
+
+    @staticmethod
     def GetOracleLinuxVersion():
         with OsRelease() as osRelease:
             try:
                 return osRelease.GetEntry("VERSION").strip("\"").split(".")[0]
             except KeyError:
                 raise ReleaseDataNotFound(
-                 "Unable to find data of Debian version: " + os.name)
+                 "Unable to find data of Oracle Linux version: " + os.name)
 
     @staticmethod
     def GetDebianVersion():
         with OsRelease() as osRelease:
             try:
                 return osRelease.GetEntry("VERSION").split("(")[1][:-2:]
             except KeyError:
@@ -44,14 +54,17 @@
         self.arch = platform.machine()
         osType = platform.system()
         if osType == "Linux":
             self.os = HostDetector.GetLinuxOs()
             if self.os == "archlinux":
                 self.osVersion = "latest"
                 self.abi = "gnu"
+            if self.os == "fedora":
+                self.osVersion = HostDetector.GetFedoraVersion()
+                self.abi = "gnu"
             if self.os == "oraclelinux":
                 self.osVersion = HostDetector.GetOracleLinuxVersion()
                 self.abi = "gnu"
             if self.os == "debian":
                 self.osVersion = HostDetector.GetDebianVersion()
                 self.abi = "gnu"
         else:
```

### Comparing `vgazer-74/libvgazer/install/apt.py` & `vgazer-75/libvgazer/install/apt.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom.py` & `vgazer-75/libvgazer/install/custom.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/alsa-lib.py` & `vgazer-75/libvgazer/install/custom_installer/alsa-lib.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/autoconf.py` & `vgazer-75/libvgazer/install/custom_installer/autoconf.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/automake.py` & `vgazer-75/libvgazer/install/custom_installer/automake.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cfgpath.py` & `vgazer-75/libvgazer/install/custom_installer/cfgpath.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cjson.py` & `vgazer-75/libvgazer/install/custom_installer/cjson.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cmake.py` & `vgazer-75/libvgazer/install/custom_installer/cmake.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cmake_barebones.py` & `vgazer-75/libvgazer/install/custom_installer/cmake_barebones.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cmocka.py` & `vgazer-75/libvgazer/install/custom_installer/cmocka.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/codecoverage.py` & `vgazer-75/libvgazer/install/custom_installer/codecoverage.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/cwalk.py` & `vgazer-75/libvgazer/install/custom_installer/cwalk.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/dr_wav.py` & `vgazer-75/libvgazer/install/custom_installer/dr_wav.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         srcDir = os.path.join(tempPath, "dr_libs")
         with WorkingDir(srcDir):
             if not os.path.exists(
              "{prefix}/include/dr_libs".format(prefix=installPrefix)):
                 RunCommand(
                  [
                   "mkdir", "-p",
-                  "{prefix}/include/dr_libs".format(prefix=installPrefix)
+                  "{prefix}/include".format(prefix=installPrefix)
                  ],
                  verbose)
             RunCommand(
              [
               "cp", "./dr_wav.h",
-              "{prefix}/include/dr_libs".format(prefix=installPrefix)
+              "{prefix}/include".format(prefix=installPrefix)
              ],
              verbose)
     except CommandError:
         print("VGAZER: Unable to install", software)
         raise InstallError(software + " not installed")
 
     print("VGAZER:", software, "installed")
```

### Comparing `vgazer-74/libvgazer/install/custom_installer/expat.py` & `vgazer-75/libvgazer/install/custom_installer/expat.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/hash_table.py` & `vgazer-75/libvgazer/install/custom_installer/hash_table.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/icu.py` & `vgazer-75/libvgazer/install/custom_installer/icu.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/icu_54_2.py` & `vgazer-75/libvgazer/install/custom_installer/icu_54_2.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/inih.py` & `vgazer-75/libvgazer/install/custom_installer/inih.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/iwyu.py` & `vgazer-75/libvgazer/install/custom_installer/iwyu.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/ketopt.py` & `vgazer-75/libvgazer/install/custom_installer/ketopt.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libclipboard.py` & `vgazer-75/libvgazer/install/custom_installer/libclipboard.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libffi.py` & `vgazer-75/libvgazer/install/custom_installer/libffi.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libglvnd.py` & `vgazer-75/libvgazer/install/custom_installer/libglvnd.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/liblzma.py` & `vgazer-75/libvgazer/install/custom_installer/liblzma.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libogg.py` & `vgazer-75/libvgazer/install/custom_installer/libogg.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libpng.py` & `vgazer-75/libvgazer/install/custom_installer/libpng.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libsir.py` & `vgazer-75/libvgazer/install/custom_installer/libsir.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libtool.py` & `vgazer-75/libvgazer/install/custom_installer/libtool.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libvorbis.py` & `vgazer-75/libvgazer/install/custom_installer/libvorbis.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/libxext.py` & `vgazer-75/libvgazer/install/custom_installer/libxext.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/luajit.py` & `vgazer-75/libvgazer/install/custom_installer/luajit.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/lwrb.py` & `vgazer-75/libvgazer/install/custom_installer/lwrb.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/ninja.py` & `vgazer-75/libvgazer/install/custom_installer/ninja.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/nuklear.py` & `vgazer-75/libvgazer/install/custom_installer/nuklear.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/pthread-stubs.py` & `vgazer-75/libvgazer/install/custom_installer/pthread-stubs.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/scv.py` & `vgazer-75/libvgazer/install/custom_installer/scv.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/stb_image.py` & `vgazer-75/libvgazer/install/custom_installer/stb_image.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/stb_image_write.py` & `vgazer-75/libvgazer/install/custom_installer/stb_image_write.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/stb_rect_pack.py` & `vgazer-75/libvgazer/install/custom_installer/stb_rect_pack.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/stb_vorbis.py` & `vgazer-75/libvgazer/install/custom_installer/stb_vorbis.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/tinyfiledialogs.py` & `vgazer-75/libvgazer/install/custom_installer/tinyfiledialogs.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/wayland-scanner.py` & `vgazer-75/libvgazer/install/custom_installer/wayland-scanner.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/wayland.py` & `vgazer-75/libvgazer/install/custom_installer/wayland.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xau.py` & `vgazer-75/libvgazer/install/custom_installer/xau.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xcb-proto.py` & `vgazer-75/libvgazer/install/custom_installer/xcb-proto.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xcb.py` & `vgazer-75/libvgazer/install/custom_installer/xcb.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xlib.py` & `vgazer-75/libvgazer/install/custom_installer/xlib.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xmempool.py` & `vgazer-75/libvgazer/install/custom_installer/xmempool.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xorg-macros.py` & `vgazer-75/libvgazer/install/custom_installer/xorg-macros.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xorgproto.py` & `vgazer-75/libvgazer/install/custom_installer/xorgproto.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/xtrans.py` & `vgazer-75/libvgazer/install/custom_installer/xtrans.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/custom_installer/zip.py` & `vgazer-75/libvgazer/install/custom_installer/zip.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,19 @@
              verbose)
             RunCommand(
              [
               "git", "checkout",
               GetLastTag("https://github.com/kuba--/zip.git")
              ],
              verbose)
+            RunCommand(
+             ["sed", "-i",
+              "s/  set(CMAKE_C_FLAGS \"${CMAKE_C_FLAGS} -Wall -Wextra -Werror -pedantic\")/  set(CMAKE_C_FLAGS \"${CMAKE_C_FLAGS} -Wall -Wextra -pedantic\")/",
+              "./CMakeLists.txt"],
+             verbose)
             RunCommand(["mkdir", "build"], verbose)
         buildDir = os.path.join(tempPath, "build")
         with WorkingDir(buildDir), ConfigCmake(platformData, cflags="-std=gnu99") as conf:
             RunCommand(
              ["cmake", "..",
               "-DCMAKE_TOOLCHAIN_FILE={crossfile}".format(crossfile=conf),
               "-DCMAKE_INSTALL_PREFIX={prefix}".format(prefix=installPrefix),
```

### Comparing `vgazer-74/libvgazer/install/custom_installer/zlib.py` & `vgazer-75/libvgazer/install/custom_installer/zlib.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/pacman.py` & `vgazer-75/libvgazer/install/pacman.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/install/yum.py` & `vgazer-75/libvgazer/install/yum.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/installers_manager.py` & `vgazer-75/libvgazer/installers_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from libvgazer.exceptions     import UnknownInstaller
 from libvgazer.install.apt    import InstallApt
 from libvgazer.install.cmd    import InstallCmd
+from libvgazer.install.dnf    import InstallDnf
 from libvgazer.install.pacman import InstallPacman
 from libvgazer.install.pip3   import InstallPip3
 from libvgazer.install.yum    import InstallYum
 
 class InstallersManager:
     def __init__(self):
         self.installFuncs = {
@@ -12,14 +13,20 @@
                 InstallApt(software, installerData["package"],
                  installerData["postInstallCommands"] if "postInstallCommands"
                   in installerData else None,
                  platformData["host"],
                  verbose),
             "cmd": lambda software, platformData, installerData, verbose:
                 InstallCmd(software, installerData["cmds"], verbose),
+            "dnf": lambda software, platformData, installerData, verbose:
+                InstallDnf(software, installerData["package"],
+                 installerData["repo"] if "repo" in installerData else None,
+                 installerData["postInstallCommands"] if "postInstallCommands"
+                  in installerData else None,
+                 verbose),
             "not-needed": lambda software, platformData, installerData,
              verbose:
                 True,
             "pacman": lambda software, platformData, installerData, verbose:
                 InstallPacman(software, installerData["package"], verbose),
             "pip3": lambda software, platformData, installerData,
              verbose:
```

### Comparing `vgazer-74/libvgazer/licenses.py` & `vgazer-75/libvgazer/licenses.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/os_release.py` & `vgazer-75/libvgazer/os_release.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/platform.py` & `vgazer-75/libvgazer/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     # Platforms comparing ratings
     COMP_INCOMPATIBLE = -1000
     COMP_COMPATIBLE = 0
     COMP_EQUAL = 1
 
     @staticmethod
     def OsIsLinux(os):
-        return (os in ["linux", "archlinux", "oraclelinux", "debian"])
+        return (os in ["linux", "archlinux", "fedora", "oraclelinux", "debian"])
 
     @staticmethod
     def GetGenericOs(os):
         if Platform.OsIsLinux(os):
             return "linux"
         elif os == "windows" or os == "any":
             return os
```

### Comparing `vgazer-74/libvgazer/software/__init__.py` & `vgazer-75/libvgazer/software/__init__.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/software/a_f.py` & `vgazer-75/libvgazer/software/a_f.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,30 @@
                     "package": "alsa-lib",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "alsa-lib",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["lgpl-2.1"],
+                "changelog": "https://www.alsa-project.org/wiki/Main_Page_News",
+                "checker": {
+                    "type": "dnf",
+                    "package": "alsa-lib-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "alsa-lib-devel",
+                },
+            },
         ],
     },
     "autoconf": {
         "platform": "host",
         "projects": [
             {
                 "fallback": True,
@@ -271,14 +287,30 @@
                     "package": "cjson",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "cjson",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["mit"],
+                "changelog": "https://github.com/DaveGamble/cJSON/blob/master/CHANGELOG.md",
+                "checker": {
+                    "type": "dnf",
+                    "package": "cjson",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "cjson",
+                },
+            },
         ],
     },
     "clang": {
         "platform": "host",
         "projects": [
             {
                 "arch": ["any"],
@@ -311,14 +343,29 @@
                     "type": "pacman",
                     "package": "clang",
                 },
                 "installer": {
                     "type": "not-needed",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://clang.llvm.org/extra/ReleaseNotes.html#improvements-to-clang-tidy",
+                "checker": {
+                    "type": "dnf",
+                    "package": "clang-tools-extra",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "clang-tools-extra",
+                },
+            },
         ],
     },
     "cmake": {
         "platform": "host",
         "projects": [
             {
                 "fallback": True,
@@ -352,14 +399,29 @@
                     "package": "cmake",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "cmake",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://cmake.org/cmake/help/latest/release/index.html",
+                "checker": {
+                    "type": "dnf",
+                    "package": "cmake",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "cmake",
+                },
+            },
         ],
     },
     "cmake_barebones": {
         "platform": "host",
         "projects": [
             {
                 "fallback": True,
@@ -417,14 +479,30 @@
                     "package": "cmocka",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "cmocka",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["apache-2.0"],
+                "changelog": "https://cmocka.org/#news",
+                "checker": {
+                    "type": "dnf",
+                    "package": "libcmocka-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "libcmocka-devel",
+                },
+            },
         ],
     },
     "codecoverage": {
         "platform": "host",
         "projects": [
             {
                 "fallback": True,
@@ -492,41 +570,57 @@
                     "hint": r'v\d\.\d+\.\d+',
                 },
                 "installer": {
                     "type": "custom",
                     "name": "dr_wav",
                 },
             },
-        ],
-    },
-    "expat": {
-        "platform": "target",
-        "projects": [
             {
-                "fallback": True,
                 "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
-                "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://github.com/libexpat/libexpat/blob/master/expat/Changes",
-                "prereqs": [
-                    "{triplet}-g++",
-                    "{triplet}-gcc",
-                    "autoconf",
-                    "automake",
-                    "libtool",
-                    "make",
-                ],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["unlicense"],
+                "changelog": "https://github.com/mackron/dr_libs/blob/master/dr_wav.h#L8351",
                 "checker": {
-                    "type": "git",
-                    "url": "https://github.com/libexpat/libexpat.git",
-                    "hint": r'R_\d_\d_\d',
+                    "type": "dnf",
+                    "package": "dr_wav-devel",
                 },
                 "installer": {
-                    "type": "custom",
-                    "name": "expat",
+                    "type": "dnf",
+                    "package": "dr_wav-devel",
                 },
             },
         ],
     },
+    # "expat": {
+    #     "platform": "target",
+    #     "projects": [
+    #         {
+    #             "fallback": True,
+    #             "arch": ["any"],
+    #             "os": ["any"],
+    #             "osVersion": ["any"],
+    #             "abi": ["any"],
+    #             "license": ["mit"],
+    #             "changelog": "https://github.com/libexpat/libexpat/blob/master/expat/Changes",
+    #             "prereqs": [
+    #                 "{triplet}-g++",
+    #                 "{triplet}-gcc",
+    #                 "autoconf",
+    #                 "automake",
+    #                 "libtool",
+    #                 "make",
+    #             ],
+    #             "checker": {
+    #                 "type": "git",
+    #                 "url": "https://github.com/libexpat/libexpat.git",
+    #                 "hint": r'R_\d_\d_\d',
+    #             },
+    #             "installer": {
+    #                 "type": "custom",
+    #                 "name": "expat",
+    #             },
+    #         },
+    #     ],
+    # },
 }
```

### Comparing `vgazer-74/libvgazer/software/g_i.py` & `vgazer-75/libvgazer/software/libo_libz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,306 +1,331 @@
 data = {
-    "g++": {
-        "platform": "host",
+    "libogg": {
+        "platform": "target",
         "projects": [
             {
+                "fallback": True,
                 "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
-                "abi": ["any"],
-                "changelog": "https://gcc.gnu.org/",
-                "prereqs": ["gcc"],
-                "checker": {
-                    "type": "pacman",
-                    "package": "gcc",
-                },
-                "installer": {
-                    "type": "not-needed",
-                },
-            },
-            {
-                "arch": ["any"],
-                "os": ["oraclelinux"],
-                "osVersion": ["7"],
+                "os": ["any"],
+                "osVersion": ["any"],
                 "abi": ["any"],
-                "changelog": "https://gcc.gnu.org/",
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
+                "prereqs": [
+                    "{triplet}-gcc",
+                    "autoconf",
+                    "automake",
+                    "libtool",
+                    "make",
+                ],
                 "checker": {
-                    "type": "yum",
-                    "package": "gcc-c++",
+                    "type": "git",
+                    "url": "https://gitlab.xiph.org/xiph/ogg.git",
                 },
                 "installer": {
-                    "type": "yum",
-                    "package": "gcc-c++",
+                    "type": "custom",
+                    "name": "libogg",
                 },
             },
-        ],
-    },
-    "gcc": {
-        "platform": "host",
-        "projects": [
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["any"],
-                "changelog": "https://gcc.gnu.org/",
+                "abi": ["gnu"],
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
                 "checker": {
                     "type": "pacman",
-                    "package": "gcc",
+                    "package": "libogg",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "gcc",
+                    "package": "libogg",
                 },
             },
             {
                 "arch": ["any"],
-                "os": ["oraclelinux"],
-                "osVersion": ["7"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
                 "abi": ["gnu"],
-                "changelog": "https://gcc.gnu.org/",
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
                 "checker": {
-                    "type": "yum",
-                    "package": "gcc",
+                    "type": "dnf",
+                    "package": "libogg-devel",
                 },
                 "installer": {
-                    "type": "yum",
-                    "package": "gcc",
+                    "type": "dnf",
+                    "package": "libogg-devel",
                 },
             },
         ],
     },
-    "hash_table": {
+    "libpng": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://github.com/anholt/hash_table/commits/master/",
+                "license": ["libpng-2.0"],
+                "changelog": "http://www.libpng.org/pub/png/pngnews.html",
                 "prereqs": [
                     "{triplet}-gcc",
+                    "{triplet}-pkg-config",
+                    "make",
+                    "zlib",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "https://github.com/anholt/hash_table.git",
-                    "files": ["meson.build"],
-                    "hint": r'\d\.\d',
+                    "url": "git://git.code.sf.net/p/libpng/code",
+                    "hint": r'(:?v1\.6\.\d\d$)|(:?v1\.7\.\d+$)',
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "hash_table",
+                    "name": "libpng",
                 },
             },
-        ],
-    },
-    "help2man": {
-        "platform": "host",
-        "projects": [
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["any"],
-                "changelog": "https://savannah.gnu.org/news/?group=coreutils",
+                "abi": ["gnu"],
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
                 "checker": {
                     "type": "pacman",
-                    "package": "help2man",
+                    "package": "libpng",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "help2man",
+                    "package": "libpng",
                 },
             },
             {
                 "arch": ["any"],
-                "os": ["oraclelinux"],
-                "osVersion": ["7"],
-                "abi": ["any"],
-                "changelog": "https://savannah.gnu.org/news/?group=coreutils",
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
                 "checker": {
-                    "type": "yum",
-                    "repo": "ol7_optional_latest",
-                    "package": "help2man",
+                    "type": "dnf",
+                    "package": "libpng-devel",
                 },
                 "installer": {
-                    "type": "yum",
-                    "repo": "ol7_optional_latest",
-                    "package": "help2man",
+                    "type": "dnf",
+                    "package": "libpng-devel",
                 },
             },
         ],
     },
-    "icu": {
+    "libsir": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
-                "changelog": "https://github.com/unicode-org/icu/releases",
+                "license": ["mit"],
+                "changelog": "https://github.com/aremmell/libsir/releases",
                 "prereqs": [
                     "{triplet}-gcc",
-                    "{triplet}-g++",
-                    "g++",
+                    "make",
+                ],
+                "checker": {
+                    "type": "git",
+                    "url": "https://github.com/aremmell/libsir.git",
+                },
+                "installer": {
+                    "type": "custom",
+                    "name": "libsir",
+                },
+            },
+        ],
+    },
+    "libtool": {
+        "platform": "host",
+        "projects": [
+            {
+                "arch": ["any"],
+                "os": ["any"],
+                "osVersion": ["any"],
+                "abi": ["any"],
+                "changelog": "https://savannah.gnu.org/news/?group=libtool",
+                "prereqs": [
+                    "autoconf",
+                    "automake",
                     "gcc",
+                    "help2man",
                     "make",
+                    "makeinfo",
+                    "xz",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "https://github.com/unicode-org/icu.git",
-                    "hint": r'release-\d+-\d$',
+                    "url": "git://git.savannah.gnu.org/libtool.git",
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "icu",
+                    "name": "libtool",
                 },
             },
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["gnu"],
-                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
-                "changelog": "https://github.com/unicode-org/icu/releases",
+                "abi": ["any"],
+                "changelog": "https://savannah.gnu.org/news/?group=libtool",
                 "checker": {
                     "type": "pacman",
-                    "package": "icu",
+                    "package": "libtool",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "icu",
+                    "package": "libtool",
                 },
             },
             {
-                "fallback": True,
                 "arch": ["any"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
-                "abi": ["gnu"],
-                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
-                "changelog": "https://github.com/unicode-org/icu/releases",
+                "abi": ["any"],
+                "changelog": "https://savannah.gnu.org/news/?group=libtool",
                 "prereqs": [
-                    "{triplet}-gcc",
-                    "{triplet}-g++",
-                    "g++",
+                    "autoconf",
+                    "automake",
                     "gcc",
+                    "help2man",
                     "make",
+                    "makeinfo",
+                    "patch",
+                    "xz",
                 ],
                 "checker": {
-                    "type": "fixed",
-                    "version": "67.1",
+                    "type": "git",
+                    "url": "git://git.savannah.gnu.org/libtool.git",
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "icu-67",
+                    "name": "libtool",
                 },
             },
         ],
     },
-    "icu-54.2": {
+    "libvorbis": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
-                "changelog": "https://github.com/unicode-org/icu/releases",
+                "license": ["bsd-3"],
+                "changelog": "https://xiph.org/press/",
                 "prereqs": [
                     "{triplet}-gcc",
-                    "{triplet}-g++",
-                    "g++",
-                    "gcc",
+                    "{triplet}-pkg-config",
+                    "autoconf",
+                    "automake",
+                    "libogg",
+                    "libtool",
                     "make",
                 ],
                 "checker": {
-                    "type": "fixed",
-                    "version": "54.2",
+                    "type": "git",
+                    "url": "https://gitlab.xiph.org/xiph/vorbis.git",
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "icu_54_2",
+                    "name": "libvorbis",
                 },
             },
-        ],
-    },
-    "inih": {
-        "platform": "target",
-        "projects": [
             {
-                "fallback": True,
                 "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
-                "abi": ["any"],
+                "os": ["archlinux"],
+                "osVersion": ["latest"],
+                "abi": ["gnu"],
                 "license": ["bsd-3"],
-                "changelog": "https://github.com/benhoyt/inih/releases",
-                "prereqs": [
-                    "{triplet}-gcc",
-                ],
+                "changelog": "https://xiph.org/press/",
                 "checker": {
-                    "type": "git",
-                    "url": "https://github.com/benhoyt/inih.git",
+                    "type": "pacman",
+                    "package": "libvorbis",
                 },
                 "installer": {
-                    "type": "custom",
-                    "name": "inih",
+                    "type": "pacman",
+                    "package": "libvorbis",
                 },
             },
             {
                 "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
                 "abi": ["gnu"],
                 "license": ["bsd-3"],
-                "changelog": "https://github.com/benhoyt/inih/releases",
+                "changelog": "https://xiph.org/press/",
                 "checker": {
-                    "type": "pacman",
-                    "package": "libinih",
+                    "type": "dnf",
+                    "package": "libvorbis-devel",
                 },
                 "installer": {
-                    "type": "pacman",
-                    "package": "libinih",
+                    "type": "dnf",
+                    "package": "libvorbis-devel",
                 },
             },
         ],
     },
-    "iwyu": {
-        "platform": "host",
+    "libxext": {
+        "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["bsd-3"],
-                "changelog": "https://include-what-you-use.org/",
+                "license": ["mit", "x11", "hpnd", "hpnd-sv", "smlnj"],
+                "changelog": "https://gitlab.freedesktop.org/xorg/lib/libxext/-/tags",
                 "prereqs": [
-                    "clang",
-                    "cmake",
-                    "g++",
-                    "llvm",
+                    "{triplet}-gcc",
+                    "{triplet}-pkg-config",
+                    "autoconf",
+                    "libtool",
                     "make",
+                    "xlib",
+                    "xorg-macros",
+                    "xorgproto",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "https://github.com/include-what-you-use/include-what-you-use.git",
-                    "hint": r'\d.\d+',
+                    "url": "https://gitlab.freedesktop.org/xorg/lib/libxext.git",
+                    "hint": r'libXext-\d\.\d(\.\d+(\.\d)?)?$',
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "iwyu",
+                    "name": "libxext",
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["archlinux"],
+                "osVersion": ["latest"],
+                "abi": ["gnu"],
+                "license": ["mit", "x11", "hpnd", "hpnd-sv", "smlnj"],
+                "changelog": "https://gitlab.freedesktop.org/xorg/lib/libxext/-/tags",
+                "checker": {
+                    "type": "pacman",
+                    "package": "libxext",
+                },
+                "installer": {
+                    "type": "pacman",
+                    "package": "libxext",
                 },
             },
         ],
     },
 }
```

### Comparing `vgazer-74/libvgazer/software/j_libm.py` & `vgazer-75/libvgazer/software/j_libm.py`

 * *Files 22% similar despite different names*

```diff
@@ -141,81 +141,81 @@
                 "installer": {
                     "type": "custom",
                     "name": "libintl-lite",
                 },
             },
         ],
     },
-    "liblzma": {
-        "platform": "target",
-        "projects": [
-            {
-                "arch": ["any"],
-                "os": ["linux"],
-                "osVersion": ["any"],
-                "abi": ["any"],
-                "license": ["pd"],
-                "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
-                "prereqs": [
-                    "{triplet}-gcc",
-                    "autoconf",
-                    "automake",
-                    "autopoint",
-                    "libtool",
-                    "make",
-                ],
-                "checker": {
-                    "type": "git",
-                    "url": "https://github.com/tukaani-project/xz.git",
-                    "hint": r'v\d\.\d.\d+$',
-                },
-                "installer": {
-                    "type": "custom",
-                    "name": "liblzma",
-                },
-            },
-            {
-                "arch": ["any"],
-                "os": ["windows"],
-                "osVersion": ["any"],
-                "abi": ["any"],
-                "license": ["pd"],
-                "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
-                "prereqs": [
-                    "{triplet}-gcc",
-                    "autoconf",
-                    "automake",
-                    "autopoint",
-                    "libtool",
-                    "make",
-                    # "libintl",
-                ],
-                "checker": {
-                    "type": "sourceforge",
-                    "project": "lzmautils",
-                },
-                "installer": {
-                    "type": "custom",
-                    "name": "liblzma",
-                },
-            },
-            {
-                "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
-                "abi": ["gnu"],
-                "license": ["pd"],
-                "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
-                "prereqs": [
-                    "xz",
-                ],
-                "checker": {
-                    "type": "pacman",
-                    "package": "xz",
-                },
-                "installer": {
-                    "type": "not-needed",
-                },
-            },
-        ],
-    },
+    # "liblzma": {
+    #     "platform": "target",
+    #     "projects": [
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["linux"],
+    #             "osVersion": ["any"],
+    #             "abi": ["any"],
+    #             "license": ["pd"],
+    #             "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
+    #             "prereqs": [
+    #                 "{triplet}-gcc",
+    #                 "autoconf",
+    #                 "automake",
+    #                 "autopoint",
+    #                 "libtool",
+    #                 "make",
+    #             ],
+    #             "checker": {
+    #                 "type": "git",
+    #                 "url": "https://github.com/tukaani-project/xz.git",
+    #                 "hint": r'v\d\.\d.\d+$',
+    #             },
+    #             "installer": {
+    #                 "type": "custom",
+    #                 "name": "liblzma",
+    #             },
+    #         },
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["windows"],
+    #             "osVersion": ["any"],
+    #             "abi": ["any"],
+    #             "license": ["pd"],
+    #             "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
+    #             "prereqs": [
+    #                 "{triplet}-gcc",
+    #                 "autoconf",
+    #                 "automake",
+    #                 "autopoint",
+    #                 "libtool",
+    #                 "make",
+    #                 # "libintl",
+    #             ],
+    #             "checker": {
+    #                 "type": "sourceforge",
+    #                 "project": "lzmautils",
+    #             },
+    #             "installer": {
+    #                 "type": "custom",
+    #                 "name": "liblzma",
+    #             },
+    #         },
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["archlinux"],
+    #             "osVersion": ["latest"],
+    #             "abi": ["gnu"],
+    #             "license": ["pd"],
+    #             "changelog": "https://github.com/tukaani-project/xz/blob/master/NEWS",
+    #             "prereqs": [
+    #                 "xz",
+    #             ],
+    #             "checker": {
+    #                 "type": "pacman",
+    #                 "package": "xz",
+    #             },
+    #             "installer": {
+    #                 "type": "not-needed",
+    #             },
+    #         },
+    #     ],
+    # },
 }
```

### Comparing `vgazer-74/libvgazer/software/libo_libz.py` & `vgazer-75/libvgazer/software/g_i.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,283 +1,384 @@
 data = {
-    "libogg": {
-        "platform": "target",
+    "g++": {
+        "platform": "host",
         "projects": [
             {
-                "fallback": True,
                 "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
+                "os": ["archlinux"],
+                "osVersion": ["latest"],
                 "abi": ["any"],
-                "license": ["bsd-3"],
-                "changelog": "https://xiph.org/press/",
-                "prereqs": [
-                    "{triplet}-gcc",
-                    "autoconf",
-                    "automake",
-                    "libtool",
-                    "make",
-                ],
+                "changelog": "https://gcc.gnu.org/",
+                "prereqs": ["gcc"],
                 "checker": {
-                    "type": "git",
-                    "url": "https://gitlab.xiph.org/xiph/ogg.git",
+                    "type": "pacman",
+                    "package": "gcc",
                 },
                 "installer": {
-                    "type": "custom",
-                    "name": "libogg",
+                    "type": "not-needed",
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://gcc.gnu.org/",
+                "checker": {
+                    "type": "dnf",
+                    "package": "gcc-c++",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "gcc-c++",
                 },
             },
             {
                 "arch": ["any"],
+                "os": ["oraclelinux"],
+                "osVersion": ["7"],
+                "abi": ["any"],
+                "changelog": "https://gcc.gnu.org/",
+                "checker": {
+                    "type": "yum",
+                    "package": "gcc-c++",
+                },
+                "installer": {
+                    "type": "yum",
+                    "package": "gcc-c++",
+                },
+            },
+        ],
+    },
+    "gcc": {
+        "platform": "host",
+        "projects": [
+            {
+                "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["gnu"],
-                "license": ["bsd-3"],
-                "changelog": "https://xiph.org/press/",
+                "abi": ["any"],
+                "changelog": "https://gcc.gnu.org/",
                 "checker": {
                     "type": "pacman",
-                    "package": "libogg",
+                    "package": "gcc",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "libogg",
+                    "package": "gcc",
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "changelog": "https://gcc.gnu.org/",
+                "checker": {
+                    "type": "dnf",
+                    "package": "gcc",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "gcc",
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["oraclelinux"],
+                "osVersion": ["7"],
+                "abi": ["gnu"],
+                "changelog": "https://gcc.gnu.org/",
+                "checker": {
+                    "type": "yum",
+                    "package": "gcc",
+                },
+                "installer": {
+                    "type": "yum",
+                    "package": "gcc",
                 },
             },
         ],
     },
-    "libpng": {
+    "hash_table": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["libpng-2.0"],
-                "changelog": "http://www.libpng.org/pub/png/pngnews.html",
+                "license": ["mit"],
+                "changelog": "https://github.com/anholt/hash_table/commits/master/",
                 "prereqs": [
                     "{triplet}-gcc",
-                    "{triplet}-pkg-config",
-                    "make",
-                    "zlib",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "git://git.code.sf.net/p/libpng/code",
-                    "hint": r'(:?v1\.6\.\d\d$)|(:?v1\.7\.\d+$)',
+                    "url": "https://github.com/anholt/hash_table.git",
+                    "files": ["meson.build"],
+                    "hint": r'\d\.\d',
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "libpng",
+                    "name": "hash_table",
                 },
             },
+        ],
+    },
+    "help2man": {
+        "platform": "host",
+        "projects": [
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["gnu"],
-                "license": ["bsd-3"],
-                "changelog": "https://xiph.org/press/",
+                "abi": ["any"],
+                "changelog": "https://savannah.gnu.org/news/?group=coreutils",
                 "checker": {
                     "type": "pacman",
-                    "package": "libpng",
+                    "package": "help2man",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "libpng",
+                    "package": "help2man",
                 },
             },
-        ],
-    },
-    "libsir": {
-        "platform": "target",
-        "projects": [
             {
-                "fallback": True,
                 "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
+                "os": ["oraclelinux"],
+                "osVersion": ["7"],
                 "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://github.com/aremmell/libsir/releases",
-                "prereqs": [
-                    "{triplet}-gcc",
-                    "make",
-                ],
+                "changelog": "https://savannah.gnu.org/news/?group=coreutils",
                 "checker": {
-                    "type": "git",
-                    "url": "https://github.com/aremmell/libsir.git",
+                    "type": "yum",
+                    "repo": "ol7_optional_latest",
+                    "package": "help2man",
                 },
                 "installer": {
-                    "type": "custom",
-                    "name": "libsir",
+                    "type": "yum",
+                    "repo": "ol7_optional_latest",
+                    "package": "help2man",
                 },
             },
         ],
     },
-    "libtool": {
-        "platform": "host",
+    "icu": {
+        "platform": "target",
         "projects": [
             {
+                "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "changelog": "https://savannah.gnu.org/news/?group=libtool",
+                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
+                "changelog": "https://github.com/unicode-org/icu/releases",
                 "prereqs": [
-                    "autoconf",
-                    "automake",
+                    "{triplet}-gcc",
+                    "{triplet}-g++",
+                    "g++",
                     "gcc",
-                    "help2man",
                     "make",
-                    "makeinfo",
-                    "xz",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "git://git.savannah.gnu.org/libtool.git",
+                    "url": "https://github.com/unicode-org/icu.git",
+                    "hint": r'release-\d+-\d$',
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "libtool",
+                    "name": "icu",
                 },
             },
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
-                "abi": ["any"],
-                "changelog": "https://savannah.gnu.org/news/?group=libtool",
+                "abi": ["gnu"],
+                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
+                "changelog": "https://github.com/unicode-org/icu/releases",
                 "checker": {
                     "type": "pacman",
-                    "package": "libtool",
+                    "package": "icu",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "libtool",
+                    "package": "icu",
                 },
             },
             {
                 "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
+                "changelog": "https://github.com/unicode-org/icu/releases",
+                "checker": {
+                    "type": "dnf",
+                    "package": "libicu-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "libicu-devel",
+                },
+            },
+            {
+                "fallback": True,
+                "arch": ["any"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
+                "abi": ["gnu"],
+                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
+                "changelog": "https://github.com/unicode-org/icu/releases",
+                "prereqs": [
+                    "{triplet}-gcc",
+                    "{triplet}-g++",
+                    "g++",
+                    "gcc",
+                    "make",
+                ],
+                "checker": {
+                    "type": "fixed",
+                    "version": "67.1",
+                },
+                "installer": {
+                    "type": "custom",
+                    "name": "icu-67",
+                },
+            },
+        ],
+    },
+    "icu-54.2": {
+        "platform": "target",
+        "projects": [
+            {
+                "fallback": True,
+                "arch": ["any"],
+                "os": ["any"],
+                "osVersion": ["any"],
                 "abi": ["any"],
-                "changelog": "https://savannah.gnu.org/news/?group=libtool",
+                "license": ["unicode", "icu", "bsd-3", "naist", "bsd-2"],
+                "changelog": "https://github.com/unicode-org/icu/releases",
                 "prereqs": [
-                    "autoconf",
-                    "automake",
+                    "{triplet}-gcc",
+                    "{triplet}-g++",
+                    "g++",
                     "gcc",
-                    "help2man",
                     "make",
-                    "makeinfo",
-                    "patch",
-                    "xz",
                 ],
                 "checker": {
-                    "type": "git",
-                    "url": "git://git.savannah.gnu.org/libtool.git",
+                    "type": "fixed",
+                    "version": "54.2",
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "libtool",
+                    "name": "icu_54_2",
                 },
             },
         ],
     },
-    "libvorbis": {
+    "inih": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
                 "license": ["bsd-3"],
-                "changelog": "https://xiph.org/press/",
+                "changelog": "https://github.com/benhoyt/inih/releases",
                 "prereqs": [
                     "{triplet}-gcc",
-                    "{triplet}-pkg-config",
-                    "autoconf",
-                    "automake",
-                    "libogg",
-                    "libtool",
-                    "make",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "https://gitlab.xiph.org/xiph/vorbis.git",
+                    "url": "https://github.com/benhoyt/inih.git",
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "libvorbis",
+                    "name": "inih",
                 },
             },
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
                 "abi": ["gnu"],
                 "license": ["bsd-3"],
-                "changelog": "https://xiph.org/press/",
+                "changelog": "https://github.com/benhoyt/inih/releases",
                 "checker": {
                     "type": "pacman",
-                    "package": "libvorbis",
+                    "package": "libinih",
                 },
                 "installer": {
                     "type": "pacman",
-                    "package": "libvorbis",
+                    "package": "libinih",
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["bsd-3"],
+                "changelog": "https://github.com/benhoyt/inih/releases",
+                "checker": {
+                    "type": "dnf",
+                    "package": "inih-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "inih-devel",
                 },
             },
         ],
     },
-    "libxext": {
-        "platform": "target",
+    "iwyu": {
+        "platform": "host",
         "projects": [
             {
                 "fallback": True,
                 "arch": ["any"],
                 "os": ["any"],
                 "osVersion": ["any"],
                 "abi": ["any"],
-                "license": ["mit", "x11", "hpnd", "hpnd-sv", "smlnj"],
-                "changelog": "https://gitlab.freedesktop.org/xorg/lib/libxext/-/tags",
+                "license": ["bsd-3"],
+                "changelog": "https://include-what-you-use.org/",
                 "prereqs": [
-                    "{triplet}-gcc",
-                    "{triplet}-pkg-config",
-                    "autoconf",
-                    "libtool",
+                    "clang",
+                    "cmake",
+                    "g++",
+                    "llvm",
                     "make",
-                    "xlib",
-                    "xorg-macros",
-                    "xorgproto",
                 ],
                 "checker": {
                     "type": "git",
-                    "url": "https://gitlab.freedesktop.org/xorg/lib/libxext.git",
-                    "hint": r'libXext-\d\.\d(\.\d+(\.\d)?)?$',
+                    "url": "https://github.com/include-what-you-use/include-what-you-use.git",
+                    "hint": r'\d.\d+',
                 },
                 "installer": {
                     "type": "custom",
-                    "name": "libxext",
+                    "name": "iwyu",
                 },
             },
             {
                 "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
-                "abi": ["gnu"],
-                "license": ["mit", "x11", "hpnd", "hpnd-sv", "smlnj"],
-                "changelog": "https://gitlab.freedesktop.org/xorg/lib/libxext/-/tags",
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "license": ["bsd-3"],
+                "changelog": "https://include-what-you-use.org/",
                 "checker": {
-                    "type": "pacman",
-                    "package": "libxext",
+                    "type": "dnf",
+                    "package": "iwyu",
                 },
                 "installer": {
-                    "type": "pacman",
-                    "package": "libxext",
+                    "type": "dnf",
+                    "package": "iwyu",
                 },
             },
         ],
     },
 }
```

### Comparing `vgazer-74/libvgazer/software/lin_o.py` & `vgazer-75/libvgazer/software/lin_o.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,14 +56,30 @@
                     "package": "luajit",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "luajit",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["mit"],
+                "changelog": "http://luajit.org/status.html",
+                "checker": {
+                    "type": "dnf",
+                    "package": "luajit-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "luajit-devel",
+                },
+            },
         ],
     },
     "lwrb": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
@@ -139,14 +155,29 @@
                 "installer": {
                     "type": "pacman",
                     "package": "make",
                 },
             },
             {
                 "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://savannah.gnu.org/news/?group=make",
+                "checker": {
+                    "type": "dnf",
+                    "package": "make",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "make",
+                },
+            },
+            {
+                "arch": ["any"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
                 "abi": ["any"],
                 "changelog": "https://savannah.gnu.org/news/?group=make",
                 "checker": {
                     "type": "yum",
                     "package": "make",
@@ -331,10 +362,26 @@
                     "package": "libglvnd",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "libglvnd",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["mit", "bsd-1", "bsd-3"],
+                "changelog": "https://gitlab.freedesktop.org/glvnd/libglvnd/-/tags",
+                "checker": {
+                    "type": "dnf",
+                    "package": "libglvnd-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "libglvnd-devel",
+                },
+            },
         ],
     },
 }
```

### Comparing `vgazer-74/libvgazer/software/p_s.py` & `vgazer-75/libvgazer/software/p_s.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,14 +75,29 @@
                 "installer": {
                     "type": "pacman",
                     "package": "pkgconf",
                 },
             },
             {
                 "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://gitlab.freedesktop.org/pkg-config/pkg-config/-/blob/master/NEWS?ref_type=heads",
+                "checker": {
+                    "type": "dnf",
+                    "package": "pkgconf-pkg-config",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "pkgconf-pkg-config",
+                },
+            },
+            {
+                "arch": ["any"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
                 "abi": ["any"],
                 "changelog": "https://gitlab.freedesktop.org/pkg-config/pkg-config/-/blob/master/NEWS?ref_type=heads",
                 "checker": {
                     "type": "yum",
                     "package": "pkgconfig",
@@ -187,14 +202,30 @@
                     "package": "stb",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "stb",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "license": ["unlicense"],
+                "changelog": "https://github.com/nothings/stb/blob/master/stb_image.h#L51",
+                "checker": {
+                    "type": "dnf",
+                    "package": "stb_image-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "stb_image-devel",
+                },
+            },
         ],
     },
     "stb_image_write": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
@@ -227,14 +258,30 @@
                     "package": "stb",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "stb",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "license": ["unlicense"],
+                "changelog": "https://github.com/nothings/stb/blob/master/stb_image_write.h#L1630",
+                "checker": {
+                    "type": "dnf",
+                    "package": "stb_image_write-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "stb_image_write-devel",
+                },
+            },
         ],
     },
     "stb_rect_pack": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
@@ -267,14 +314,30 @@
                     "package": "stb",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "stb",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "license": ["unlicense"],
+                "changelog": "https://github.com/nothings/stb/blob/master/stb_rect_pack.h#L42",
+                "checker": {
+                    "type": "dnf",
+                    "package": "stb_rect_pack-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "stb_rect_pack-devel",
+                },
+            },
         ],
     },
     "stb_vorbis": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
@@ -307,10 +370,26 @@
                     "package": "stb",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "stb",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "license": ["unlicense"],
+                "changelog": "https://github.com/nothings/stb/blob/master/stb_vorbis.c#L39",
+                "checker": {
+                    "type": "dnf",
+                    "package": "stb_vorbis-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "stb_vorbis-devel",
+                },
+            },
         ],
     },
 }
```

### Comparing `vgazer-74/libvgazer/software/t_xc.py` & `vgazer-75/libvgazer/software/t_xc.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,34 +23,34 @@
                 "installer": {
                     "type": "custom",
                     "name": "tinyfiledialogs",
                 },
             },
         ],
     },
-    "unzip": {
-        "platform": "host",
-        "projects": [
-            {
-                "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
-                "abi": ["any"],
-                "changelog": "https://infozip.sourceforge.net/UnZip.html#Release",
-                "checker": {
-                    "type": "pacman",
-                    "package": "unzip",
-                },
-                "installer": {
-                    "type": "pacman",
-                    "package": "unzip",
-                },
-            },
-        ],
-    },
+    # "unzip": {
+    #     "platform": "host",
+    #     "projects": [
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["archlinux"],
+    #             "osVersion": ["latest"],
+    #             "abi": ["any"],
+    #             "changelog": "https://infozip.sourceforge.net/UnZip.html#Release",
+    #             "checker": {
+    #                 "type": "pacman",
+    #                 "package": "unzip",
+    #             },
+    #             "installer": {
+    #                 "type": "pacman",
+    #                 "package": "unzip",
+    #             },
+    #         },
+    #     ],
+    # },
     "valgrind": {
         "platform": "host",
         "projects": [
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
@@ -61,110 +61,125 @@
                     "package": "valgrind",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": ["valgrind", "debuginfod"],
                 },
             },
-        ],
-    },
-    "wayland-libs": {
-        "platform": "target",
-        "projects": [
-            {
-                "fallback": True,
-                "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
-                "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://wayland.freedesktop.org/releases.html",
-                "prereqs": [
-                    "{triplet}-g++",
-                    "{triplet}-gcc",
-                    "{triplet}-pkg-config",
-                    "libffi",
-                    "meson",
-                    "ninja",
-                    "wayland-scanner",
-                ],
-                "checker": {
-                    "type": "git",
-                    "url": "https://gitlab.freedesktop.org/wayland/wayland.git",
-                    "hint": r'1\.\d\d.\d+',
-                },
-                "installer": {
-                    "type": "custom",
-                    "name": "wayland",
-                },
-            },
-            {
-                "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
-                "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://wayland.freedesktop.org/releases.html",
-                "checker": {
-                    "type": "pacman",
-                    "package": "wayland",
-                },
-                "installer": {
-                    "type": "pacman",
-                    "package": "wayland",
-                },
-            },
-        ],
-    },
-    "wayland-scanner": {
-        "platform": "host",
-        "projects": [
-            {
-                "fallback": True,
-                "arch": ["any"],
-                "os": ["any"],
-                "osVersion": ["any"],
-                "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://wayland.freedesktop.org/releases.html",
-                "prereqs": [
-                    "expat",
-                    "gcc",
-                    "meson",
-                    "ninja",
-                    "pkg-config",
-                ],
-                "checker": {
-                    "type": "git",
-                    "url": "https://gitlab.freedesktop.org/wayland/wayland.git",
-                    "hint": r'1\.\d\d.\d+',
-                },
-                "installer": {
-                    "type": "custom",
-                    "name": "wayland-scanner",
-                },
-            },
             {
                 "arch": ["any"],
-                "os": ["archlinux"],
-                "osVersion": ["latest"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
                 "abi": ["any"],
-                "license": ["mit"],
-                "changelog": "https://wayland.freedesktop.org/releases.html",
+                "changelog": "https://valgrind.org/docs/manual/dist.news.html",
                 "checker": {
-                    "type": "pacman",
-                    "package": "wayland",
+                    "type": "dnf",
+                    "package": "valgrind",
                 },
                 "installer": {
-                    "type": "pacman",
-                    "package": "wayland",
+                    "type": "dnf",
+                    "package": "valgrind",
                 },
             },
         ],
     },
+    # "wayland-libs": {
+    #     "platform": "target",
+    #     "projects": [
+    #         {
+    #             "fallback": True,
+    #             "arch": ["any"],
+    #             "os": ["any"],
+    #             "osVersion": ["any"],
+    #             "abi": ["any"],
+    #             "license": ["mit"],
+    #             "changelog": "https://wayland.freedesktop.org/releases.html",
+    #             "prereqs": [
+    #                 "{triplet}-g++",
+    #                 "{triplet}-gcc",
+    #                 "{triplet}-pkg-config",
+    #                 "libffi",
+    #                 "meson",
+    #                 "ninja",
+    #                 "wayland-scanner",
+    #             ],
+    #             "checker": {
+    #                 "type": "git",
+    #                 "url": "https://gitlab.freedesktop.org/wayland/wayland.git",
+    #                 "hint": r'1\.\d\d.\d+',
+    #             },
+    #             "installer": {
+    #                 "type": "custom",
+    #                 "name": "wayland",
+    #             },
+    #         },
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["archlinux"],
+    #             "osVersion": ["latest"],
+    #             "abi": ["any"],
+    #             "license": ["mit"],
+    #             "changelog": "https://wayland.freedesktop.org/releases.html",
+    #             "checker": {
+    #                 "type": "pacman",
+    #                 "package": "wayland",
+    #             },
+    #             "installer": {
+    #                 "type": "pacman",
+    #                 "package": "wayland",
+    #             },
+    #         },
+    #     ],
+    # },
+    # "wayland-scanner": {
+    #     "platform": "host",
+    #     "projects": [
+    #         {
+    #             "fallback": True,
+    #             "arch": ["any"],
+    #             "os": ["any"],
+    #             "osVersion": ["any"],
+    #             "abi": ["any"],
+    #             "license": ["mit"],
+    #             "changelog": "https://wayland.freedesktop.org/releases.html",
+    #             "prereqs": [
+    #                 "expat",
+    #                 "gcc",
+    #                 "meson",
+    #                 "ninja",
+    #                 "pkg-config",
+    #             ],
+    #             "checker": {
+    #                 "type": "git",
+    #                 "url": "https://gitlab.freedesktop.org/wayland/wayland.git",
+    #                 "hint": r'1\.\d\d.\d+',
+    #             },
+    #             "installer": {
+    #                 "type": "custom",
+    #                 "name": "wayland-scanner",
+    #             },
+    #         },
+    #         {
+    #             "arch": ["any"],
+    #             "os": ["archlinux"],
+    #             "osVersion": ["latest"],
+    #             "abi": ["any"],
+    #             "license": ["mit"],
+    #             "changelog": "https://wayland.freedesktop.org/releases.html",
+    #             "checker": {
+    #                 "type": "pacman",
+    #                 "package": "wayland",
+    #             },
+    #             "installer": {
+    #                 "type": "pacman",
+    #                 "package": "wayland",
+    #             },
+    #         },
+    #     ],
+    # },
     "wget": {
         "platform": "host",
         "projects": [
             {
                 "arch": ["any"],
                 "os": ["archlinux"],
                 "osVersion": ["latest"],
@@ -192,60 +207,82 @@
                 "installer": {
                     "type": "yum",
                     "package": "wget",
                 },
             },
         ],
     },
-    "x86_64-linux-gnu-binutils": {
+    # "x86_64-linux-gnu-binutils": {
+    #     "platform": "host",
+    #     "projects": [
+    #         {
+    #             "arch": ["x86_64"],
+    #             "os": ["oraclelinux"],
+    #             "osVersion": ["7"],
+    #             "abi": ["any"],
+    #             "changelog": "https://fossies.org/linux/binutils/binutils/NEWS",
+    #             "checker": {
+    #                 "type": "yum",
+    #                 "package": "binutils",
+    #             },
+    #             "installer": {
+    #                 "type": "cmd",
+    #                 "cmds": [
+    #                     ["mkdir", "-p", "/usr/local/bin"],
+    #                     [
+    #                         "ln", "-s", "/usr/bin/ar",
+    #                         "/usr/local/bin/x86_64-linux-gnu-ar"
+    #                     ],
+    #                     [
+    #                         "ln", "-s", "/usr/bin/strip",
+    #                         "/usr/local/bin/x86_64-linux-gnu-strip"
+    #                     ],
+    #                 ]
+    #             },
+    #         },
+    #     ],
+    # },
+    "x86_64-linux-gnu-g++": {
         "platform": "host",
         "projects": [
             {
                 "arch": ["x86_64"],
-                "os": ["oraclelinux"],
-                "osVersion": ["7"],
+                "os": ["archlinux"],
+                "osVersion": ["any"],
                 "abi": ["any"],
-                "changelog": "https://fossies.org/linux/binutils/binutils/NEWS",
+                "changelog": "https://gcc.gnu.org/",
+                "prereqs": ["g++"],
                 "checker": {
-                    "type": "yum",
-                    "package": "binutils",
+                    "type": "pacman",
+                    "package": "gcc",
                 },
                 "installer": {
-                    "type": "cmd",
-                    "cmds": [
-                        ["mkdir", "-p", "/usr/local/bin"],
-                        [
-                            "ln", "-s", "/usr/bin/ar",
-                            "/usr/local/bin/x86_64-linux-gnu-ar"
-                        ],
-                        [
-                            "ln", "-s", "/usr/bin/strip",
-                            "/usr/local/bin/x86_64-linux-gnu-strip"
-                        ],
-                    ]
+                    "type": "not-needed",
                 },
             },
-        ],
-    },
-    "x86_64-linux-gnu-g++": {
-        "platform": "host",
-        "projects": [
             {
                 "arch": ["x86_64"],
-                "os": ["archlinux"],
-                "osVersion": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
                 "abi": ["any"],
                 "changelog": "https://gcc.gnu.org/",
                 "prereqs": ["g++"],
                 "checker": {
-                    "type": "pacman",
-                    "package": "gcc",
+                    "type": "dnf",
+                    "package": "gcc-c++",
                 },
                 "installer": {
-                    "type": "not-needed",
+                    "type": "cmd",
+                    "cmds": [
+                        ["mkdir", "-p", "/usr/local/bin"],
+                        [
+                            "ln", "-s", "/usr/bin/g++",
+                            "/usr/local/bin/x86_64-linux-gnu-g++"
+                        ],
+                    ]
                 },
             },
             {
                 "arch": ["x86_64"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
                 "abi": ["any"],
@@ -284,14 +321,52 @@
                 },
                 "installer": {
                     "type": "not-needed",
                 },
             },
             {
                 "arch": ["x86_64"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["any"],
+                "changelog": "https://gcc.gnu.org/",
+                "prereqs": ["gcc"],
+                "checker": {
+                    "type": "dnf",
+                    "package": "gcc",
+                },
+                "installer": {
+                    "type": "cmd",
+                    "cmds": [
+                        ["mkdir", "-p", "/usr/local/bin"],
+                        [
+                            "ln", "-s", "/usr/bin/gcc",
+                            "/usr/local/bin/x86_64-linux-gnu-gcc"
+                        ],
+                        [
+                            "ln", "-s", "/usr/bin/gcc-ar",
+                            "/usr/local/bin/x86_64-linux-gnu-gcc-ar"
+                        ],
+                        [
+                            "ln", "-s", "/usr/bin/gcc-nm",
+                            "/usr/local/bin/x86_64-linux-gnu-gcc-nm"
+                        ],
+                        [
+                            "ln", "-s", "/usr/bin/gcc-ranlib",
+                            "/usr/local/bin/x86_64-linux-gnu-gcc-ranlib"
+                        ],
+                        [
+                            "ln", "-s", "/usr/bin/gcov",
+                            "/usr/local/bin/x86_64-linux-gnu-gcov"
+                        ],
+                    ]
+                },
+            },
+            {
+                "arch": ["x86_64"],
                 "os": ["oraclelinux"],
                 "osVersion": ["7"],
                 "abi": ["any"],
                 "changelog": "https://gcc.gnu.org/",
                 "prereqs": ["gcc"],
                 "checker": {
                     "type": "yum",
@@ -344,14 +419,53 @@
                 },
                 "installer": {
                     "type": "cmd",
                     "cmds": [
                         ["mkdir", "-p", "/usr/local/bin/"],
                         ["sh", "-c", "echo "
                             "'#!/bin/sh\n"
+                            "export PKG_CONFIG_DIR=\n"
+                            "export PKG_CONFIG_PATH="
+                                "/usr/local/x86_64-linux-gnu/lib/pkgconfig:"
+                                "/usr/local/x86_64-linux-gnu/share/pkgconfig"
+                                "\n"
+                            "export PKG_CONFIG_LIBDIR="
+                                "/usr/local/x86_64-linux-gnu/lib/pkgconfig:"
+                                "/usr/local/x86_64-linux-gnu/share/pkgconfig"
+                                "\n"
+                            "export PKG_CONFIG_SYSROOT_DIR=/\n"
+                            "exec pkg-config \"$@\"' "
+                            "> /usr/local/bin/x86_64-linux-gnu-pkg-config",
+                        ],
+                        [
+                            "chmod", "+x",
+                            "/usr/local/bin/x86_64-linux-gnu-pkg-config",
+                        ],
+                    ],
+                },
+            },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "changelog": "https://gitlab.freedesktop.org/pkg-config/pkg-config/-/blob/master/NEWS?ref_type=heads",
+                "prereqs": [
+                    "pkg-config",
+                ],
+                "checker": {
+                    "type": "dnf",
+                    "package": "pkgconf-pkg-config",
+                },
+                "installer": {
+                    "type": "cmd",
+                    "cmds": [
+                        ["mkdir", "-p", "/usr/local/bin/"],
+                        ["sh", "-c", "echo "
+                            "'#!/bin/sh\n"
                             "export PKG_CONFIG_DIR=\n"
                             "export PKG_CONFIG_PATH="
                                 "/usr/local/x86_64-linux-gnu/lib/pkgconfig:"
                                 "/usr/local/x86_64-linux-gnu/share/pkgconfig"
                                 "\n"
                             "export PKG_CONFIG_LIBDIR="
                                 "/usr/local/x86_64-linux-gnu/lib/pkgconfig:"
```

### Comparing `vgazer-74/libvgazer/software/xd_z.py` & `vgazer-75/libvgazer/software/xd_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,30 @@
                     "package": "libx11",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "libx11",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["mit", "x11", "hpnd-sv", "smlnj", "hpnd", "bsd-1"],
+                "changelog": "https://gitlab.freedesktop.org/xorg/lib/libx11#release-187",
+                "checker": {
+                    "type": "dnf",
+                    "package": "libX11-devel",
+                },
+                "installer": {
+                    "type": "dnf",
+                    "package": "libX11-devel",
+                },
+            },
         ],
     },
     "xmempool": {
         "platform": "target",
         "projects": [
             {
                 "fallback": True,
@@ -305,10 +321,26 @@
                     "package": "zlib",
                 },
                 "installer": {
                     "type": "pacman",
                     "package": "zlib",
                 },
             },
+            {
+                "arch": ["any"],
+                "os": ["fedora"],
+                "osVersion": ["40"],
+                "abi": ["gnu"],
+                "license": ["zlib"],
+                "changelog": "https://github.com/zlib-ng/zlib-ng/releases",
+                "checker": {
+                    "type": "dnf",
+                    "package": "zlib-ng-compat-devel",
+                },
+                "installer": {
+                    "type": "pacman",
+                    "package": "zlib-ng-compat-devel",
+                },
+            },
         ],
     },
 }
```

### Comparing `vgazer-74/libvgazer/store/base.py` & `vgazer-75/libvgazer/store/base.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/utils.py` & `vgazer-75/libvgazer/utils.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/version/apt_cache.py` & `vgazer-75/libvgazer/version/apt_cache.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/version/custom.py` & `vgazer-75/libvgazer/version/custom.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/version/custom_checker/autoconf.py` & `vgazer-75/libvgazer/version/custom_checker/autoconf.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/version/git.py` & `vgazer-75/libvgazer/version/git.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/version/yum.py` & `vgazer-75/libvgazer/version/yum.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/libvgazer/working_dir.py` & `vgazer-75/libvgazer/working_dir.py`

 * *Files identical despite different names*

### Comparing `vgazer-74/setup.py` & `vgazer-75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vgazer",
-    version="74",
+    version="75",
     url="https://github.com/edomin/vgazer",
     license="CC0",
     author="Vasiliy Edomin",
     author_email="Vasiliy.Edomin@gmail.com",
     description="Library for checking versions and installing various software",
     packages=find_packages(),
     scripts=["vgazer"],
```

### Comparing `vgazer-74/vgazer` & `vgazer-75/vgazer`

 * *Files identical despite different names*

### Comparing `vgazer-74/vgazer.egg-info/PKG-INFO` & `vgazer-75/vgazer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vgazer
-Version: 74
+Version: 75
 Summary: Library for checking versions and installing various software
 Home-page: https://github.com/edomin/vgazer
 Author: Vasiliy Edomin
 Author-email: Vasiliy.Edomin@gmail.com
 License: CC0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vgazer-74/vgazer.egg-info/SOURCES.txt` & `vgazer-75/vgazer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 libvgazer/config/__init__.py
 libvgazer/config/cmake.py
 libvgazer/config/meson.py
 libvgazer/install/__init__.py
 libvgazer/install/apt.py
 libvgazer/install/cmd.py
 libvgazer/install/custom.py
+libvgazer/install/dnf.py
 libvgazer/install/pacman.py
 libvgazer/install/pip3.py
 libvgazer/install/yum.py
 libvgazer/install/custom_installer/__init__.py
 libvgazer/install/custom_installer/alsa-lib.py
 libvgazer/install/custom_installer/autoconf.py
 libvgazer/install/custom_installer/automake.py
@@ -87,14 +88,15 @@
 libvgazer/store/__init__.py
 libvgazer/store/base.py
 libvgazer/store/home.py
 libvgazer/store/temp.py
 libvgazer/version/__init__.py
 libvgazer/version/apt_cache.py
 libvgazer/version/custom.py
+libvgazer/version/dnf.py
 libvgazer/version/git.py
 libvgazer/version/pacman.py
 libvgazer/version/yolk3k.py
 libvgazer/version/yum.py
 libvgazer/version/custom_checker/__init__.py
 libvgazer/version/custom_checker/autoconf.py
 vgazer.egg-info/PKG-INFO
```

