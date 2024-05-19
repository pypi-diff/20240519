# Comparing `tmp/vgazer-75.tar.gz` & `tmp/vgazer-76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgazer-75.tar", last modified: Sun May 19 12:12:32 2024, max compression
+gzip compressed data, was "vgazer-76.tar", last modified: Sun May 19 12:43:43 2024, max compression
```

## Comparing `vgazer-75.tar` & `vgazer-76.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.225622 vgazer-75/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:12:32.225622 vgazer-75/PKG-INFO
--rw-r--r--   0 edomin    (1000) edomin    (1000)     6182 2024-05-18 19:42:39.000000 vgazer-75/README.md
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.165622 vgazer-75/libvgazer/
--rw-r--r--   0 edomin    (1000) edomin    (1000)     7350 2024-05-19 11:13:14.000000 vgazer-75/libvgazer/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2012 2024-05-18 20:00:03.000000 vgazer-75/libvgazer/checkers_manager.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1268 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/command.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.169622 vgazer-75/libvgazer/config/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/config/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2442 2024-02-24 20:34:09.000000 vgazer-75/libvgazer/config/cmake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2119 2024-02-24 20:33:20.000000 vgazer-75/libvgazer/config/meson.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      911 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/env_vars.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2027 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/exceptions.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2971 2024-05-19 11:12:40.000000 vgazer-75/libvgazer/host_detector.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.173622 vgazer-75/libvgazer/install/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2056 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/apt.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      480 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/cmd.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      964 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.205622 vgazer-75/libvgazer/install/custom_installer/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2212 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/alsa-lib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2574 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/autoconf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1672 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/automake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1466 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cfgpath.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2039 2024-02-24 20:27:10.000000 vgazer-75/libvgazer/install/custom_installer/cjson.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1412 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cmake.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1114 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/cmake_barebones.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2151 2024-02-24 20:27:22.000000 vgazer-75/libvgazer/install/custom_installer/cmocka.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1405 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/codecoverage.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1901 2024-03-10 14:07:36.000000 vgazer-75/libvgazer/install/custom_installer/cwalk.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1429 2024-05-19 11:04:00.000000 vgazer-75/libvgazer/install/custom_installer/dr_wav.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1884 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/expat.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2182 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/hash_table.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     4320 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/icu.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     4172 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/icu_54_2.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2646 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/inih.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1792 2024-02-24 19:25:08.000000 vgazer-75/libvgazer/install/custom_installer/iwyu.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1479 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/ketopt.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1922 2024-02-24 20:27:36.000000 vgazer-75/libvgazer/install/custom_installer/libclipboard.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1862 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libffi.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1878 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libglvnd.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1738 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/liblzma.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1616 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libogg.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1928 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libpng.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1703 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libsir.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1415 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libtool.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1749 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libvorbis.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1882 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/libxext.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1827 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/luajit.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2729 2024-02-21 08:02:09.000000 vgazer-75/libvgazer/install/custom_installer/lwrb.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1381 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/ninja.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1465 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/nuklear.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1739 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/pthread-stubs.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2017 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/scv.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1354 2024-03-18 19:01:55.000000 vgazer-75/libvgazer/install/custom_installer/stb_image.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1360 2024-03-18 19:02:23.000000 vgazer-75/libvgazer/install/custom_installer/stb_image_write.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1358 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/stb_rect_pack.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1355 2024-03-18 19:02:51.000000 vgazer-75/libvgazer/install/custom_installer/stb_vorbis.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2263 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/tinyfiledialogs.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1973 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/wayland-scanner.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2147 2024-02-24 20:28:41.000000 vgazer-75/libvgazer/install/custom_installer/wayland.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2143 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xau.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1765 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xcb-proto.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2005 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xcb.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xlib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2210 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xmempool.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1508 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xorg-macros.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     1606 2024-02-24 20:39:09.000000 vgazer-75/libvgazer/install/custom_installer/xorgproto.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2040 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/xtrans.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-05-19 11:35:51.000000 vgazer-75/libvgazer/install/custom_installer/zip.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2600 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/custom_installer/zlib.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-05-18 20:00:49.000000 vgazer-75/libvgazer/install/dnf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      902 2024-02-25 15:39:40.000000 vgazer-75/libvgazer/install/pacman.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      449 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/pip3.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/install/yum.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2318 2024-05-18 20:00:14.000000 vgazer-75/libvgazer/installers_manager.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     5424 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/licenses.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      558 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/os_release.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    14072 2024-05-18 19:54:42.000000 vgazer-75/libvgazer/platform.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.209622 vgazer-75/libvgazer/software/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      853 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/software/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    20324 2024-05-19 12:11:59.000000 vgazer-75/libvgazer/software/a_f.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    12117 2024-05-19 11:43:14.000000 vgazer-75/libvgazer/software/g_i.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     7222 2024-05-19 11:45:28.000000 vgazer-75/libvgazer/software/j_libm.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    10549 2024-05-19 11:49:12.000000 vgazer-75/libvgazer/software/libo_libz.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    12147 2024-05-19 11:53:58.000000 vgazer-75/libvgazer/software/lin_o.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    13177 2024-05-19 11:57:08.000000 vgazer-75/libvgazer/software/p_s.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    26795 2024-05-19 12:00:54.000000 vgazer-75/libvgazer/software/t_xc.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)    11360 2024-05-19 12:10:59.000000 vgazer-75/libvgazer/software/xd_z.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.213622 vgazer-75/libvgazer/store/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     5847 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/base.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      438 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/home.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      439 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/store/temp.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      621 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/utils.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.217622 vgazer-75/libvgazer/version/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      843 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/apt_cache.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      822 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom.py
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.221622 vgazer-75/libvgazer/version/custom_checker/
--rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom_checker/__init__.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      941 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/custom_checker/autoconf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-05-18 20:00:42.000000 vgazer-75/libvgazer/version/dnf.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)     2802 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/git.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      228 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/pacman.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      149 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/yolk3k.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/version/yum.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)      676 2024-02-19 18:06:30.000000 vgazer-75/libvgazer/working_dir.py
--rw-r--r--   0 edomin    (1000) edomin    (1000)       38 2024-05-19 12:12:32.225622 vgazer-75/setup.cfg
--rw-r--r--   0 edomin    (1000) edomin    (1000)      914 2024-05-19 12:12:11.000000 vgazer-75/setup.py
--rwxr-xr-x   0 edomin    (1000) edomin    (1000)     1349 2024-02-19 18:06:30.000000 vgazer-75/vgazer
-drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:12:32.225622 vgazer-75/vgazer.egg-info/
--rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/PKG-INFO
--rw-r--r--   0 edomin    (1000) edomin    (1000)     3865 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/SOURCES.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/dependency_links.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/not-zip-safe
--rw-r--r--   0 edomin    (1000) edomin    (1000)       32 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/requires.txt
--rw-r--r--   0 edomin    (1000) edomin    (1000)       10 2024-05-19 12:12:31.000000 vgazer-75/vgazer.egg-info/top_level.txt
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.717609 vgazer-76/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:43:43.717609 vgazer-76/PKG-INFO
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     6182 2024-05-18 19:42:39.000000 vgazer-76/README.md
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.657609 vgazer-76/libvgazer/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     7350 2024-05-19 11:13:14.000000 vgazer-76/libvgazer/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2012 2024-05-18 20:00:03.000000 vgazer-76/libvgazer/checkers_manager.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1268 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/command.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.661609 vgazer-76/libvgazer/config/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/config/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2591 2024-05-19 12:39:42.000000 vgazer-76/libvgazer/config/cmake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2119 2024-02-24 20:33:20.000000 vgazer-76/libvgazer/config/meson.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      911 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/env_vars.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2027 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/exceptions.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2971 2024-05-19 11:12:40.000000 vgazer-76/libvgazer/host_detector.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.665609 vgazer-76/libvgazer/install/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2056 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/apt.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      480 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/cmd.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      964 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.697609 vgazer-76/libvgazer/install/custom_installer/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2212 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/alsa-lib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2574 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/autoconf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1672 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/automake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1466 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/cfgpath.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2039 2024-02-24 20:27:10.000000 vgazer-76/libvgazer/install/custom_installer/cjson.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1412 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/cmake.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1114 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/cmake_barebones.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2151 2024-02-24 20:27:22.000000 vgazer-76/libvgazer/install/custom_installer/cmocka.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1405 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/codecoverage.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1901 2024-03-10 14:07:36.000000 vgazer-76/libvgazer/install/custom_installer/cwalk.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1429 2024-05-19 11:04:00.000000 vgazer-76/libvgazer/install/custom_installer/dr_wav.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1884 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/expat.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2182 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/hash_table.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     4320 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/icu.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     4172 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/icu_54_2.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2646 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/inih.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1792 2024-02-24 19:25:08.000000 vgazer-76/libvgazer/install/custom_installer/iwyu.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1479 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/ketopt.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1922 2024-02-24 20:27:36.000000 vgazer-76/libvgazer/install/custom_installer/libclipboard.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1862 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libffi.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1878 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libglvnd.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1738 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/liblzma.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1616 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libogg.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1928 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libpng.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1703 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libsir.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1415 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libtool.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1749 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libvorbis.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1882 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/libxext.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1827 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/luajit.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2729 2024-02-21 08:02:09.000000 vgazer-76/libvgazer/install/custom_installer/lwrb.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1381 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/ninja.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1465 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/nuklear.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1739 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/pthread-stubs.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2017 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/scv.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1354 2024-03-18 19:01:55.000000 vgazer-76/libvgazer/install/custom_installer/stb_image.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1360 2024-03-18 19:02:23.000000 vgazer-76/libvgazer/install/custom_installer/stb_image_write.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1358 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/stb_rect_pack.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1355 2024-03-18 19:02:51.000000 vgazer-76/libvgazer/install/custom_installer/stb_vorbis.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2263 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/tinyfiledialogs.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1973 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/wayland-scanner.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2147 2024-02-24 20:28:41.000000 vgazer-76/libvgazer/install/custom_installer/wayland.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2143 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xau.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1765 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xcb-proto.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2005 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xcb.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xlib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2210 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xmempool.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1508 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xorg-macros.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     1606 2024-02-24 20:39:09.000000 vgazer-76/libvgazer/install/custom_installer/xorgproto.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2040 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/xtrans.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2141 2024-05-19 11:35:51.000000 vgazer-76/libvgazer/install/custom_installer/zip.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2600 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/custom_installer/zlib.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-05-18 20:00:49.000000 vgazer-76/libvgazer/install/dnf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      902 2024-02-25 15:39:40.000000 vgazer-76/libvgazer/install/pacman.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      449 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/pip3.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      872 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/install/yum.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2318 2024-05-18 20:00:14.000000 vgazer-76/libvgazer/installers_manager.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     5424 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/licenses.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      558 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/os_release.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    14072 2024-05-18 19:54:42.000000 vgazer-76/libvgazer/platform.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.705609 vgazer-76/libvgazer/software/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      853 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/software/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    20324 2024-05-19 12:11:59.000000 vgazer-76/libvgazer/software/a_f.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    12117 2024-05-19 11:43:14.000000 vgazer-76/libvgazer/software/g_i.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     7222 2024-05-19 11:45:28.000000 vgazer-76/libvgazer/software/j_libm.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    10549 2024-05-19 11:49:12.000000 vgazer-76/libvgazer/software/libo_libz.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    12147 2024-05-19 11:53:58.000000 vgazer-76/libvgazer/software/lin_o.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    13177 2024-05-19 11:57:08.000000 vgazer-76/libvgazer/software/p_s.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    26795 2024-05-19 12:00:54.000000 vgazer-76/libvgazer/software/t_xc.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)    11360 2024-05-19 12:10:59.000000 vgazer-76/libvgazer/software/xd_z.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.705609 vgazer-76/libvgazer/store/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/store/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     5847 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/store/base.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      438 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/store/home.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      439 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/store/temp.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      621 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/utils.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.713609 vgazer-76/libvgazer/version/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      843 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/apt_cache.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      822 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/custom.py
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.713609 vgazer-76/libvgazer/version/custom_checker/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        0 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/custom_checker/__init__.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      941 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/custom_checker/autoconf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-05-18 20:00:42.000000 vgazer-76/libvgazer/version/dnf.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     2802 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/git.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      228 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/pacman.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      149 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/yolk3k.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      616 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/version/yum.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      676 2024-02-19 18:06:30.000000 vgazer-76/libvgazer/working_dir.py
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       38 2024-05-19 12:43:43.717609 vgazer-76/setup.cfg
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      914 2024-05-19 12:43:33.000000 vgazer-76/setup.py
+-rwxr-xr-x   0 edomin    (1000) edomin    (1000)     1349 2024-02-19 18:06:30.000000 vgazer-76/vgazer
+drwxr-xr-x   0 edomin    (1000) edomin    (1000)        0 2024-05-19 12:43:43.717609 vgazer-76/vgazer.egg-info/
+-rw-r--r--   0 edomin    (1000) edomin    (1000)      592 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/PKG-INFO
+-rw-r--r--   0 edomin    (1000) edomin    (1000)     3865 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/SOURCES.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/dependency_links.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)        1 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/not-zip-safe
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       32 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/requires.txt
+-rw-r--r--   0 edomin    (1000) edomin    (1000)       10 2024-05-19 12:43:43.000000 vgazer-76/vgazer.egg-info/top_level.txt
```

### Comparing `vgazer-75/PKG-INFO` & `vgazer-76/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vgazer
-Version: 75
+Version: 76
 Summary: Library for checking versions and installing various software
 Home-page: https://github.com/edomin/vgazer
 Author: Vasiliy Edomin
 Author-email: Vasiliy.Edomin@gmail.com
 License: CC0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vgazer-75/README.md` & `vgazer-76/README.md`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/__init__.py` & `vgazer-76/libvgazer/__init__.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/checkers_manager.py` & `vgazer-76/libvgazer/checkers_manager.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/command.py` & `vgazer-76/libvgazer/command.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/config/cmake.py` & `vgazer-76/libvgazer/config/cmake.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from libvgazer.exceptions import FileNotFound
 from libvgazer.platform   import GetAr
 from libvgazer.platform   import GetCc
 from libvgazer.platform   import GetCxx
 from libvgazer.platform   import GetInstallPrefix
 from libvgazer.platform   import GetTriplet
 from libvgazer.platform   import Platform
 from libvgazer.store.temp import StoreTemp
@@ -16,15 +17,19 @@
 
         cmakeOs = Platform.GetGenericOs(
          platformData["target"].GetOs()).capitalize()
         prefix = GetInstallPrefix(platformData)
         targetTriplet = GetTriplet(platformData["target"])
 
         cc = GetCc(platformData["target"])
-        cxx = GetCxx(platformData["target"])
+        try:
+            cxxDef = "set(CMAKE_CXX_COMPILER {cxx})".format(cxx=GetCxx(platformData["target"]))
+        except FileNotFound:
+            cxxDef = ""
+
         ar = GetAr(platformData["target"])
 
         pkgConfigLibdirs = ("/usr/{triplet}/lib/pkgconfig"
          ":{prefix}/lib/pkgconfig:{prefix}/share/pkgconfig"
          ":/usr/lib/{triplet}/pkgconfig").format(
           prefix=prefix,
           triplet=targetTriplet
@@ -37,29 +42,29 @@
             findMode = "ONLY"
 
         storeTemp.DirectoryWriteTextFile("toolchain.cmake",
          "set(CMAKE_SYSTEM_NAME {cmakeOs})\n"
          "set(CMAKE_SYSTEM_PROCESSOR {cpu})\n"
          "set(CMAKE_C_COMPILER {cc})\n"
          "set(CMAKE_C_FLAGS {cflags})\n"
-         "set(CMAKE_CXX_COMPILER {cxx})\n"
+         "{cxxDef}\n"
          "set(CMAKE_AR {ar})\n"
          "set(CMAKE_FIND_ROOT_PATH {prefix})\n"
          "SET("
           "ENV{{PKG_CONFIG_LIBDIR}} "
           "{pkgConfigLibdirs}"
          ")\n"
          "SET(CMAKE_FIND_ROOT_PATH_MODE_PROGRAM NEVER)\n"
          "SET(CMAKE_FIND_ROOT_PATH_MODE_LIBRARY {findMode})\n"
          "SET(CMAKE_FIND_ROOT_PATH_MODE_INCLUDE {findMode})".format(
           cmakeOs=cmakeOs,
           cpu=platformData["target"].GetArch(),
           cc=cc,
           cflags=cflags if cflags is not None else "",
-          cxx=cxx,
+          cxxDef=cxxDef,
           ar=ar,
           prefix=prefix,
           pkgConfigLibdirs=pkgConfigLibdirs,
           findMode=findMode
          )
         )
```

### Comparing `vgazer-75/libvgazer/config/meson.py` & `vgazer-76/libvgazer/config/meson.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/env_vars.py` & `vgazer-76/libvgazer/env_vars.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/exceptions.py` & `vgazer-76/libvgazer/exceptions.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/host_detector.py` & `vgazer-76/libvgazer/host_detector.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/apt.py` & `vgazer-76/libvgazer/install/apt.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom.py` & `vgazer-76/libvgazer/install/custom.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/alsa-lib.py` & `vgazer-76/libvgazer/install/custom_installer/alsa-lib.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/autoconf.py` & `vgazer-76/libvgazer/install/custom_installer/autoconf.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/automake.py` & `vgazer-76/libvgazer/install/custom_installer/automake.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cfgpath.py` & `vgazer-76/libvgazer/install/custom_installer/cfgpath.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cjson.py` & `vgazer-76/libvgazer/install/custom_installer/cjson.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cmake.py` & `vgazer-76/libvgazer/install/custom_installer/cmake.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cmake_barebones.py` & `vgazer-76/libvgazer/install/custom_installer/cmake_barebones.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cmocka.py` & `vgazer-76/libvgazer/install/custom_installer/cmocka.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/codecoverage.py` & `vgazer-76/libvgazer/install/custom_installer/codecoverage.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/cwalk.py` & `vgazer-76/libvgazer/install/custom_installer/cwalk.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/dr_wav.py` & `vgazer-76/libvgazer/install/custom_installer/dr_wav.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/expat.py` & `vgazer-76/libvgazer/install/custom_installer/expat.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/hash_table.py` & `vgazer-76/libvgazer/install/custom_installer/hash_table.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/icu.py` & `vgazer-76/libvgazer/install/custom_installer/icu.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/icu_54_2.py` & `vgazer-76/libvgazer/install/custom_installer/icu_54_2.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/inih.py` & `vgazer-76/libvgazer/install/custom_installer/inih.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/iwyu.py` & `vgazer-76/libvgazer/install/custom_installer/iwyu.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/ketopt.py` & `vgazer-76/libvgazer/install/custom_installer/ketopt.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libclipboard.py` & `vgazer-76/libvgazer/install/custom_installer/libclipboard.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libffi.py` & `vgazer-76/libvgazer/install/custom_installer/libffi.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libglvnd.py` & `vgazer-76/libvgazer/install/custom_installer/libglvnd.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/liblzma.py` & `vgazer-76/libvgazer/install/custom_installer/liblzma.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libogg.py` & `vgazer-76/libvgazer/install/custom_installer/libogg.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libpng.py` & `vgazer-76/libvgazer/install/custom_installer/libpng.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libsir.py` & `vgazer-76/libvgazer/install/custom_installer/libsir.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libtool.py` & `vgazer-76/libvgazer/install/custom_installer/libtool.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libvorbis.py` & `vgazer-76/libvgazer/install/custom_installer/libvorbis.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/libxext.py` & `vgazer-76/libvgazer/install/custom_installer/libxext.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/luajit.py` & `vgazer-76/libvgazer/install/custom_installer/luajit.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/lwrb.py` & `vgazer-76/libvgazer/install/custom_installer/lwrb.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/ninja.py` & `vgazer-76/libvgazer/install/custom_installer/ninja.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/nuklear.py` & `vgazer-76/libvgazer/install/custom_installer/nuklear.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/pthread-stubs.py` & `vgazer-76/libvgazer/install/custom_installer/pthread-stubs.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/scv.py` & `vgazer-76/libvgazer/install/custom_installer/scv.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/stb_image.py` & `vgazer-76/libvgazer/install/custom_installer/stb_image.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/stb_image_write.py` & `vgazer-76/libvgazer/install/custom_installer/stb_image_write.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/stb_rect_pack.py` & `vgazer-76/libvgazer/install/custom_installer/stb_rect_pack.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/stb_vorbis.py` & `vgazer-76/libvgazer/install/custom_installer/stb_vorbis.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/tinyfiledialogs.py` & `vgazer-76/libvgazer/install/custom_installer/tinyfiledialogs.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/wayland-scanner.py` & `vgazer-76/libvgazer/install/custom_installer/wayland-scanner.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/wayland.py` & `vgazer-76/libvgazer/install/custom_installer/wayland.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xau.py` & `vgazer-76/libvgazer/install/custom_installer/xau.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xcb-proto.py` & `vgazer-76/libvgazer/install/custom_installer/xcb-proto.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xcb.py` & `vgazer-76/libvgazer/install/custom_installer/xcb.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xlib.py` & `vgazer-76/libvgazer/install/custom_installer/xlib.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xmempool.py` & `vgazer-76/libvgazer/install/custom_installer/xmempool.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xorg-macros.py` & `vgazer-76/libvgazer/install/custom_installer/xorg-macros.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xorgproto.py` & `vgazer-76/libvgazer/install/custom_installer/xorgproto.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/xtrans.py` & `vgazer-76/libvgazer/install/custom_installer/xtrans.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/zip.py` & `vgazer-76/libvgazer/install/custom_installer/zip.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/custom_installer/zlib.py` & `vgazer-76/libvgazer/install/custom_installer/zlib.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/dnf.py` & `vgazer-76/libvgazer/install/dnf.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/pacman.py` & `vgazer-76/libvgazer/install/pacman.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/install/yum.py` & `vgazer-76/libvgazer/install/yum.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/installers_manager.py` & `vgazer-76/libvgazer/installers_manager.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/licenses.py` & `vgazer-76/libvgazer/licenses.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/os_release.py` & `vgazer-76/libvgazer/os_release.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/platform.py` & `vgazer-76/libvgazer/platform.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/__init__.py` & `vgazer-76/libvgazer/software/__init__.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/a_f.py` & `vgazer-76/libvgazer/software/a_f.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/g_i.py` & `vgazer-76/libvgazer/software/g_i.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/j_libm.py` & `vgazer-76/libvgazer/software/j_libm.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/libo_libz.py` & `vgazer-76/libvgazer/software/libo_libz.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/lin_o.py` & `vgazer-76/libvgazer/software/lin_o.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/p_s.py` & `vgazer-76/libvgazer/software/p_s.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/t_xc.py` & `vgazer-76/libvgazer/software/t_xc.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/software/xd_z.py` & `vgazer-76/libvgazer/software/xd_z.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/store/base.py` & `vgazer-76/libvgazer/store/base.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/utils.py` & `vgazer-76/libvgazer/utils.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/apt_cache.py` & `vgazer-76/libvgazer/version/apt_cache.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/custom.py` & `vgazer-76/libvgazer/version/custom.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/custom_checker/autoconf.py` & `vgazer-76/libvgazer/version/custom_checker/autoconf.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/dnf.py` & `vgazer-76/libvgazer/version/dnf.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/git.py` & `vgazer-76/libvgazer/version/git.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/version/yum.py` & `vgazer-76/libvgazer/version/yum.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/libvgazer/working_dir.py` & `vgazer-76/libvgazer/working_dir.py`

 * *Files identical despite different names*

### Comparing `vgazer-75/setup.py` & `vgazer-76/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vgazer",
-    version="75",
+    version="76",
     url="https://github.com/edomin/vgazer",
     license="CC0",
     author="Vasiliy Edomin",
     author_email="Vasiliy.Edomin@gmail.com",
     description="Library for checking versions and installing various software",
     packages=find_packages(),
     scripts=["vgazer"],
```

### Comparing `vgazer-75/vgazer` & `vgazer-76/vgazer`

 * *Files identical despite different names*

### Comparing `vgazer-75/vgazer.egg-info/PKG-INFO` & `vgazer-76/vgazer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vgazer
-Version: 75
+Version: 76
 Summary: Library for checking versions and installing various software
 Home-page: https://github.com/edomin/vgazer
 Author: Vasiliy Edomin
 Author-email: Vasiliy.Edomin@gmail.com
 License: CC0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vgazer-75/vgazer.egg-info/SOURCES.txt` & `vgazer-76/vgazer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

