# Comparing `tmp/libsrg-5.2.1.tar.gz` & `tmp/libsrg-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg-5.2.1.tar", max compression
+gzip compressed data, was "libsrg-5.2.2.tar", max compression
```

## Comparing `libsrg-5.2.1.tar` & `libsrg-5.2.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.2.1/README.md
--rw-r--r--   0        0        0     1703 2024-05-18 01:01:00.461508 libsrg-5.2.1/libsrg/AppTemplate.py
--rw-r--r--   0        0        0    12172 2024-05-18 01:01:00.447508 libsrg-5.2.1/libsrg/Config.py
--rwxr-xr-x   0        0        0     2842 2024-05-18 01:01:00.459508 libsrg-5.2.1/libsrg/ElapsedTime.py
--rwxr-xr-x   0        0        0     9552 2024-05-18 01:11:35.933634 libsrg-5.2.1/libsrg/Info.py
--rwxr-xr-x   0        0        0     4266 2024-05-18 01:01:00.454508 libsrg-5.2.1/libsrg/LevelBanner.py
--rwxr-xr-x   0        0        0     1753 2024-05-18 01:01:00.444508 libsrg-5.2.1/libsrg/LoggerGUIProxy.py
--rwxr-xr-x   0        0        0     6374 2024-05-18 01:01:00.442508 libsrg-5.2.1/libsrg/LoggingAppBase.py
--rwxr-xr-x   0        0        0     8406 2024-05-18 01:01:00.451508 libsrg-5.2.1/libsrg/LoggingCounter.py
--rwxr-xr-x   0        0        0      832 2024-05-18 01:01:00.431508 libsrg-5.2.1/libsrg/LoggingUtils.py
--rwxr-xr-x   0        0        0     2093 2024-05-18 01:01:00.439508 libsrg-5.2.1/libsrg/LoggingWatcher.py
--rwxr-xr-x   0        0        0     3883 2024-05-18 01:01:00.435508 libsrg-5.2.1/libsrg/NagiosBase.py
--rwxr-xr-x   0        0        0     7448 2024-05-18 01:01:00.456508 libsrg-5.2.1/libsrg/Runner.py
--rwxr-xr-x   0        0        0     5142 2024-05-18 01:01:00.433508 libsrg-5.2.1/libsrg/Runner2.py
--rw-r--r--   0        0        0     4762 2024-05-18 01:01:00.503508 libsrg-5.2.1/libsrg/Statistics/ADStatsBase.py
--rw-r--r--   0        0        0     2514 2024-05-18 01:01:00.501508 libsrg-5.2.1/libsrg/Statistics/AnalogStatsBase.py
--rw-r--r--   0        0        0     1675 2024-05-18 01:01:00.498508 libsrg-5.2.1/libsrg/Statistics/AnalogStatsCumulative.py
--rw-r--r--   0        0        0     2541 2024-05-18 01:01:00.486508 libsrg-5.2.1/libsrg/Statistics/AnalogStatsFading.py
--rw-r--r--   0        0        0     1829 2024-05-18 01:01:00.496508 libsrg-5.2.1/libsrg/Statistics/AnalogStatsSlidingWindow.py
--rw-r--r--   0        0        0     2282 2024-05-19 13:20:53.883322 libsrg-5.2.1/libsrg/Statistics/DiscreteStatsBase.py
--rw-r--r--   0        0        0     1013 2024-05-18 01:01:00.492508 libsrg-5.2.1/libsrg/Statistics/DiscreteStatsCumulative.py
--rw-r--r--   0        0        0     1822 2024-05-18 01:01:00.488508 libsrg-5.2.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py
--rw-r--r--   0        0        0     2078 2024-05-18 01:01:00.511508 libsrg-5.2.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py
--rw-r--r--   0        0        0     3023 2024-05-18 01:01:00.514508 libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
--rw-r--r--   0        0        0     2583 2024-05-18 01:01:00.509508 libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
--rw-r--r--   0        0        0     4154 2024-05-18 01:01:00.507508 libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
--rw-r--r--   0        0        0     3172 2024-05-18 01:01:00.519508 libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
--rw-r--r--   0        0        0     1844 2024-05-18 01:01:00.521508 libsrg-5.2.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
--rw-r--r--   0        0        0     2846 2024-05-18 01:01:00.517508 libsrg-5.2.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
--rw-r--r--   0        0        0      239 2024-05-18 01:01:00.515508 libsrg-5.2.1/libsrg/Statistics/UnitTests/__init__.py
--rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
--rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
--rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     4177 2024-05-19 13:00:24.959786 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
--rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
--rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
--rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      239 2024-05-18 01:01:00.490508 libsrg-5.2.1/libsrg/Statistics/__init__.py
--rw-r--r--   0        0        0     7794 2024-05-19 13:00:24.980786 libsrg-5.2.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
--rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0     5520 2024-05-19 13:20:53.958321 libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
--rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
--rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
--rw-r--r--   0        0        0      172 2024-05-19 13:00:24.966786 libsrg-5.2.1/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2461 2024-05-18 01:01:00.535508 libsrg-5.2.1/libsrg/TKGUI/GuiBase.py
--rw-r--r--   0        0        0      687 2024-05-18 01:01:00.533508 libsrg-5.2.1/libsrg/TKGUI/GuiRequest.py
--rw-r--r--   0        0        0     3663 2024-05-18 01:01:00.537508 libsrg-5.2.1/libsrg/TKGUI/GuiRequestQueue.py
--rw-r--r--   0        0        0    10933 2024-05-18 01:01:00.539508 libsrg-5.2.1/libsrg/TKGUI/LoggerGUI.py
--rw-r--r--   0        0        0      239 2024-05-18 01:01:00.531508 libsrg-5.2.1/libsrg/TKGUI/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
--rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
--rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.2.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
--rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.2.1/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5737 2024-05-18 01:01:00.472508 libsrg-5.2.1/libsrg/UnitTests/Config_test.py
--rw-r--r--   0        0        0      709 2024-05-18 01:01:00.464508 libsrg-5.2.1/libsrg/UnitTests/Info_test.py
--rw-r--r--   0        0        0     1497 2024-05-18 01:01:00.468508 libsrg-5.2.1/libsrg/UnitTests/RolloverTest_filename.py
--rw-r--r--   0        0        0     1547 2024-05-18 01:01:00.466508 libsrg-5.2.1/libsrg/UnitTests/RolloverTest_logfile.py
--rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.2.1/libsrg/UnitTests/Sample.env
--rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.2.1/libsrg/UnitTests/Sample.ini
--rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.2.1/libsrg/UnitTests/Sample.json
--rw-r--r--   0        0        0      239 2024-05-18 01:01:00.470508 libsrg-5.2.1/libsrg/UnitTests/__init__.py
--rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.2.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
--rwxr-xr-x   0        0        0      353 2024-05-18 01:01:00.437508 libsrg-5.2.1/libsrg/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-19 13:25:27.224883 libsrg-5.2.1/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-02-24 22:12:03.211633 libsrg-5.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     2620 2024-05-03 23:47:01.671722 libsrg-5.2.2/README.md
+-rw-r--r--   0        0        0     1703 2024-05-18 01:01:00.461508 libsrg-5.2.2/libsrg/AppTemplate.py
+-rw-r--r--   0        0        0    12172 2024-05-18 01:01:00.447508 libsrg-5.2.2/libsrg/Config.py
+-rwxr-xr-x   0        0        0     2842 2024-05-18 01:01:00.459508 libsrg-5.2.2/libsrg/ElapsedTime.py
+-rwxr-xr-x   0        0        0     9552 2024-05-18 01:11:35.933634 libsrg-5.2.2/libsrg/Info.py
+-rwxr-xr-x   0        0        0     4266 2024-05-18 01:01:00.454508 libsrg-5.2.2/libsrg/LevelBanner.py
+-rwxr-xr-x   0        0        0     1753 2024-05-18 01:01:00.444508 libsrg-5.2.2/libsrg/LoggerGUIProxy.py
+-rwxr-xr-x   0        0        0     6374 2024-05-18 01:01:00.442508 libsrg-5.2.2/libsrg/LoggingAppBase.py
+-rwxr-xr-x   0        0        0     8406 2024-05-18 01:01:00.451508 libsrg-5.2.2/libsrg/LoggingCounter.py
+-rwxr-xr-x   0        0        0      832 2024-05-18 01:01:00.431508 libsrg-5.2.2/libsrg/LoggingUtils.py
+-rwxr-xr-x   0        0        0     2093 2024-05-18 01:01:00.439508 libsrg-5.2.2/libsrg/LoggingWatcher.py
+-rwxr-xr-x   0        0        0     3883 2024-05-18 01:01:00.435508 libsrg-5.2.2/libsrg/NagiosBase.py
+-rwxr-xr-x   0        0        0     7448 2024-05-18 01:01:00.456508 libsrg-5.2.2/libsrg/Runner.py
+-rwxr-xr-x   0        0        0     5142 2024-05-18 01:01:00.433508 libsrg-5.2.2/libsrg/Runner2.py
+-rw-r--r--   0        0        0     4762 2024-05-18 01:01:00.503508 libsrg-5.2.2/libsrg/Statistics/ADStatsBase.py
+-rw-r--r--   0        0        0     2514 2024-05-18 01:01:00.501508 libsrg-5.2.2/libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--   0        0        0     1675 2024-05-18 01:01:00.498508 libsrg-5.2.2/libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--   0        0        0     2541 2024-05-18 01:01:00.486508 libsrg-5.2.2/libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--   0        0        0     1829 2024-05-18 01:01:00.496508 libsrg-5.2.2/libsrg/Statistics/AnalogStatsSlidingWindow.py
+-rw-r--r--   0        0        0     2481 2024-05-19 14:51:24.249117 libsrg-5.2.2/libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--   0        0        0     1013 2024-05-18 01:01:00.492508 libsrg-5.2.2/libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--   0        0        0     1822 2024-05-18 01:01:00.488508 libsrg-5.2.2/libsrg/Statistics/DiscreteStatsSlidingWindow.py
+-rw-r--r--   0        0        0     2078 2024-05-18 01:01:00.511508 libsrg-5.2.2/libsrg/Statistics/UnitTests/ADStatsBase_test.py
+-rw-r--r--   0        0        0     3023 2024-05-18 01:01:00.514508 libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--   0        0        0     2583 2024-05-18 01:01:00.509508 libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--   0        0        0     4154 2024-05-18 01:01:00.507508 libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--   0        0        0     3172 2024-05-18 01:01:00.519508 libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0     1844 2024-05-18 01:01:00.521508 libsrg-5.2.2/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--   0        0        0     2846 2024-05-18 01:01:00.517508 libsrg-5.2.2/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.515508 libsrg-5.2.2/libsrg/Statistics/UnitTests/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-11 13:46:23.848269 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5015 2024-04-24 16:16:17.446580 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7026 2024-04-17 20:08:12.643029 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6891 2024-04-24 16:16:17.454580 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     5527 2024-04-11 13:56:04.579212 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     5392 2024-04-24 16:16:17.459580 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc
+-rw-r--r--   0        0        0     9207 2024-04-11 14:18:27.440094 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     9072 2024-04-24 16:16:17.471580 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc
+-rw-r--r--   0        0        0     7000 2024-04-17 20:02:03.807004 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6865 2024-04-24 16:16:17.481580 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4310 2024-04-11 13:37:57.025926 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     4177 2024-05-19 13:00:24.959786 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc
+-rw-r--r--   0        0        0     6751 2024-04-11 00:45:26.752786 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0     6616 2024-04-24 16:16:17.500579 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc
+-rw-r--r--   0        0        0     4185 2024-04-11 13:37:57.059926 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc
+-rw-r--r--   0        0        0      182 2024-04-08 17:02:46.936966 libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.490508 libsrg-5.2.2/libsrg/Statistics/__init__.py
+-rw-r--r--   0        0        0     7794 2024-05-19 13:00:24.980786 libsrg-5.2.2/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     5538 2024-04-11 13:40:23.849156 libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     3209 2024-04-08 17:03:01.079883 libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-08 17:03:01.094884 libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc
+-rw-r--r--   0        0        0     3619 2024-04-17 20:02:03.812004 libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0     5520 2024-05-19 13:20:53.958321 libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc
+-rw-r--r--   0        0        0     2252 2024-04-24 18:48:49.375379 libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc
+-rw-r--r--   0        0        0     3785 2024-04-11 13:37:57.049926 libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-05-19 13:00:24.966786 libsrg-5.2.2/libsrg/Statistics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2461 2024-05-18 01:01:00.535508 libsrg-5.2.2/libsrg/TKGUI/GuiBase.py
+-rw-r--r--   0        0        0      687 2024-05-18 01:01:00.533508 libsrg-5.2.2/libsrg/TKGUI/GuiRequest.py
+-rw-r--r--   0        0        0     3663 2024-05-18 01:01:00.537508 libsrg-5.2.2/libsrg/TKGUI/GuiRequestQueue.py
+-rw-r--r--   0        0        0    10933 2024-05-18 01:01:00.539508 libsrg-5.2.2/libsrg/TKGUI/LoggerGUI.py
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.531508 libsrg-5.2.2/libsrg/TKGUI/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-24 18:48:47.930388 libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2024-04-24 18:48:47.938388 libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc
+-rw-r--r--   0        0        0     7736 2024-04-24 18:48:47.949388 libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc
+-rw-r--r--   0        0        0    21932 2024-04-24 18:48:49.869376 libsrg-5.2.2/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-02-05 15:38:41.630152 libsrg-5.2.2/libsrg/TKGUI/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5737 2024-05-18 01:01:00.472508 libsrg-5.2.2/libsrg/UnitTests/Config_test.py
+-rw-r--r--   0        0        0      709 2024-05-18 01:01:00.464508 libsrg-5.2.2/libsrg/UnitTests/Info_test.py
+-rw-r--r--   0        0        0     1497 2024-05-18 01:01:00.468508 libsrg-5.2.2/libsrg/UnitTests/RolloverTest_filename.py
+-rw-r--r--   0        0        0     1547 2024-05-18 01:01:00.466508 libsrg-5.2.2/libsrg/UnitTests/RolloverTest_logfile.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:15:42.414708 libsrg-5.2.2/libsrg/UnitTests/Sample.env
+-rw-r--r--   0        0        0       82 2024-04-08 14:36:33.524107 libsrg-5.2.2/libsrg/UnitTests/Sample.ini
+-rw-r--r--   0        0        0       60 2024-04-09 14:56:25.134524 libsrg-5.2.2/libsrg/UnitTests/Sample.json
+-rw-r--r--   0        0        0      239 2024-05-18 01:01:00.470508 libsrg-5.2.2/libsrg/UnitTests/__init__.py
+-rw-r--r--   0        0        0    12397 2024-04-16 16:38:28.280498 libsrg-5.2.2/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc
+-rwxr-xr-x   0        0        0      353 2024-05-18 01:01:00.437508 libsrg-5.2.2/libsrg/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-19 14:51:43.004016 libsrg-5.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 libsrg-5.2.2/PKG-INFO
```

### Comparing `libsrg-5.2.1/LICENSE.txt` & `libsrg-5.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/README.md` & `libsrg-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/AppTemplate.py` & `libsrg-5.2.2/libsrg/AppTemplate.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Config.py` & `libsrg-5.2.2/libsrg/Config.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/ElapsedTime.py` & `libsrg-5.2.2/libsrg/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Info.py` & `libsrg-5.2.2/libsrg/Info.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LevelBanner.py` & `libsrg-5.2.2/libsrg/LevelBanner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LoggerGUIProxy.py` & `libsrg-5.2.2/libsrg/LoggerGUIProxy.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LoggingAppBase.py` & `libsrg-5.2.2/libsrg/LoggingAppBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LoggingCounter.py` & `libsrg-5.2.2/libsrg/LoggingCounter.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LoggingUtils.py` & `libsrg-5.2.2/libsrg/LoggingUtils.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/LoggingWatcher.py` & `libsrg-5.2.2/libsrg/LoggingWatcher.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/NagiosBase.py` & `libsrg-5.2.2/libsrg/NagiosBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Runner.py` & `libsrg-5.2.2/libsrg/Runner.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Runner2.py` & `libsrg-5.2.2/libsrg/Runner2.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/ADStatsBase.py` & `libsrg-5.2.2/libsrg/Statistics/ADStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/AnalogStatsBase.py` & `libsrg-5.2.2/libsrg/Statistics/AnalogStatsBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/AnalogStatsCumulative.py` & `libsrg-5.2.2/libsrg/Statistics/AnalogStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/AnalogStatsFading.py` & `libsrg-5.2.2/libsrg/Statistics/AnalogStatsFading.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/AnalogStatsSlidingWindow.py` & `libsrg-5.2.2/libsrg/Statistics/AnalogStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/DiscreteStatsBase.py` & `libsrg-5.2.2/libsrg/Statistics/DiscreteStatsBase.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 
     def datetimes(self) -> dict[str, datetime]:
         return self.last_time.copy()
 
     def count_for(self, value: Any) -> int:
         return self.counter[value]
 
-    def most_common(self, n: int) -> list[tuple[Any, int]]:
-        return self.counter.most_common(n)
+    def most_common(self, n: int) -> list[tuple[Any, int,str]]:
+        if time_format is None:
+            time_format="%Y-%m-%d %H:%M:%S %Z"
+        mc = self.counter.most_common(n)
+        mct = [(key,val,self.last_time[key].astimezone().strftime(time_format)) for key,val in mc]
+        return mct
 
     def most_common_as_str(self, n: int,time_format:str=None) -> str:
         if time_format is None:
             time_format="%Y-%m-%d %H:%M:%S %Z"
         mc = self.counter.most_common(n)
         mct = [(key,val,self.last_time[key].astimezone().strftime(time_format)) for key,val in mc]
         return str(mct)
```

### Comparing `libsrg-5.2.1/libsrg/Statistics/DiscreteStatsCumulative.py` & `libsrg-5.2.2/libsrg/Statistics/DiscreteStatsCumulative.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/DiscreteStatsSlidingWindow.py` & `libsrg-5.2.2/libsrg/Statistics/DiscreteStatsSlidingWindow.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/ADStatsBase_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/ADStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsFading_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/AnalogStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/DiscteteStatsSlidingWindow_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/ADStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsCumulative_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsFading_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/AnalogStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsBase_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/DiscteteStatsSlidingWindow_test.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/Statistics/UnitTests/__pycache__/RunStatsBase_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/ADStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsFading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/AnalogStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsCumulative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc` & `libsrg-5.2.2/libsrg/Statistics/__pycache__/DiscreteStatsSlidingWindow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/GuiBase.py` & `libsrg-5.2.2/libsrg/TKGUI/GuiBase.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/GuiRequest.py` & `libsrg-5.2.2/libsrg/TKGUI/GuiRequest.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/GuiRequestQueue.py` & `libsrg-5.2.2/libsrg/TKGUI/GuiRequestQueue.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/LoggerGUI.py` & `libsrg-5.2.2/libsrg/TKGUI/LoggerGUI.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc` & `libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiBase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc` & `libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiRequest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc` & `libsrg-5.2.2/libsrg/TKGUI/__pycache__/GuiRequestQueue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc` & `libsrg-5.2.2/libsrg/TKGUI/__pycache__/LoggerGUI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/UnitTests/Config_test.py` & `libsrg-5.2.2/libsrg/UnitTests/Config_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/UnitTests/Info_test.py` & `libsrg-5.2.2/libsrg/UnitTests/Info_test.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/UnitTests/RolloverTest_filename.py` & `libsrg-5.2.2/libsrg/UnitTests/RolloverTest_filename.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/UnitTests/RolloverTest_logfile.py` & `libsrg-5.2.2/libsrg/UnitTests/RolloverTest_logfile.py`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc` & `libsrg-5.2.2/libsrg/UnitTests/__pycache__/Config_test.cpython-311-pytest-7.2.0.pyc`

 * *Files identical despite different names*

### Comparing `libsrg-5.2.1/pyproject.toml` & `libsrg-5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg"
-version = "5.2.1"
+version = "5.2.2"
 description = "Utility lib logging, statistics, subprocesses"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
```

### Comparing `libsrg-5.2.1/PKG-INFO` & `libsrg-5.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 5.2.1
+Version: 5.2.2
 Summary: Utility lib logging, statistics, subprocesses
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

