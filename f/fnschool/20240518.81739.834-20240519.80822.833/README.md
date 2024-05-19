# Comparing `tmp/fnschool-20240518.81739.834.tar.gz` & `tmp/fnschool-20240519.80822.833.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240518.81739.834.tar", last modified: Sat May 18 09:39:38 2024, max compression
+gzip compressed data, was "fnschool-20240519.80822.833.tar", last modified: Sun May 19 00:22:36 2024, max compression
```

## Comparing `fnschool-20240518.81739.834.tar` & `fnschool-20240519.80822.833.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.688960 fnschool-20240518.81739.834/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-18 09:39:38.687960 fnschool-20240518.81739.834/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-18 09:39:38.688960 fnschool-20240518.81739.834/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.671960 fnschool-20240518.81739.834/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.676960 fnschool-20240518.81739.834/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3116 2024-05-17 17:07:47.000000 fnschool-20240518.81739.834/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.681960 fnschool-20240518.81739.834/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240518.81739.834/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-17 16:08:29.000000 fnschool-20240518.81739.834/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240518.81739.834/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      949 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.682960 fnschool-20240518.81739.834/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240518.81739.834/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240518.81739.834/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240518.81739.834/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240518.81739.834/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240518.81739.834/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-17 16:33:52.000000 fnschool-20240518.81739.834/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.685960 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-17 16:02:00.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2282 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4492 2024-05-17 16:33:53.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-17 16:33:56.000000 fnschool-20240518.81739.834/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240518.81739.834/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.686960 fnschool-20240518.81739.834/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240518.81739.834/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-17 16:08:56.000000 fnschool-20240518.81739.834/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.673960 fnschool-20240518.81739.834/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.671960 fnschool-20240518.81739.834/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.686960 fnschool-20240518.81739.834/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.672960 fnschool-20240518.81739.834/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.686960 fnschool-20240518.81739.834/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    18082 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.672960 fnschool-20240518.81739.834/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.686960 fnschool-20240518.81739.834/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.672960 fnschool-20240518.81739.834/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.687960 fnschool-20240518.81739.834/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.673960 fnschool-20240518.81739.834/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.687960 fnschool-20240518.81739.834/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-18 09:39:34.000000 fnschool-20240518.81739.834/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-17 16:00:10.000000 fnschool-20240518.81739.834/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240518.81739.834/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-18 09:39:38.687960 fnschool-20240518.81739.834/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-18 09:39:38.000000 fnschool-20240518.81739.834/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.419926 fnschool-20240519.80822.833/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-19 00:22:36.419926 fnschool-20240519.80822.833/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-19 00:22:36.419926 fnschool-20240519.80822.833/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.396926 fnschool-20240519.80822.833/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.401926 fnschool-20240519.80822.833/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      380 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3153 2024-05-19 00:18:53.000000 fnschool-20240519.80822.833/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.410926 fnschool-20240519.80822.833/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-12 17:09:24.000000 fnschool-20240519.80822.833/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-17 16:08:29.000000 fnschool-20240519.80822.833/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-08 00:15:03.000000 fnschool-20240519.80822.833/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      949 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.411926 fnschool-20240519.80822.833/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-12 21:10:58.000000 fnschool-20240519.80822.833/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-12 19:17:55.000000 fnschool-20240519.80822.833/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-12 09:54:45.000000 fnschool-20240519.80822.833/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:28.000000 fnschool-20240519.80822.833/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:50:32.000000 fnschool-20240519.80822.833/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1236 2024-05-17 16:33:52.000000 fnschool-20240519.80822.833/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.416926 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4075 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-17 16:02:00.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9302 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8254 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10827 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9734 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2282 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4492 2024-05-17 16:33:53.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-12 18:18:03.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-17 16:33:56.000000 fnschool-20240519.80822.833/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-01 14:48:23.000000 fnschool-20240519.80822.833/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.417926 fnschool-20240519.80822.833/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-04-27 16:06:09.000000 fnschool-20240519.80822.833/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-17 16:08:56.000000 fnschool-20240519.80822.833/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.398926 fnschool-20240519.80822.833/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.397926 fnschool-20240519.80822.833/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.417926 fnschool-20240519.80822.833/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.397926 fnschool-20240519.80822.833/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.417926 fnschool-20240519.80822.833/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18082 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.397926 fnschool-20240519.80822.833/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.418926 fnschool-20240519.80822.833/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.398926 fnschool-20240519.80822.833/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.418926 fnschool-20240519.80822.833/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.398926 fnschool-20240519.80822.833/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.418926 fnschool-20240519.80822.833/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-19 00:22:33.000000 fnschool-20240519.80822.833/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-17 16:00:10.000000 fnschool-20240519.80822.833/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-12 04:59:07.000000 fnschool-20240519.80822.833/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-19 00:22:36.418926 fnschool-20240519.80822.833/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-19 00:22:36.000000 fnschool-20240519.80822.833/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240518.81739.834/LICENSE` & `fnschool-20240519.80822.833/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/PKG-INFO` & `fnschool-20240519.80822.833/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240518.81739.834
+Version: 20240519.80822.833
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240518.81739.834/README.md` & `fnschool-20240519.80822.833/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/pyproject.toml` & `fnschool-20240519.80822.833/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/app.py` & `fnschool-20240519.80822.833/src/fnschool/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 app_name = "fnschool"
 app_author = "larryw3i"
 app_version = None
 
 
 def get_app_version():
-    from fnschool import __version__
 
     global app_version
-    app_version = __version__
+    if not app_version:
+        from fnschool import __version__
+        app_version = __version__
     return app_version
 
 
 def print_app():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
@@ -33,19 +34,19 @@
         r"||_|   |_| \_|____/ \____|_| |_|\___/ \___/|_____||",
         r"|                                                 |",
         r"```````````````````````````````````````````````````",
         r"",
     ]
     app_name2 = [
         "",
-        "  ▄▄                ▗▖             ▗▄▖",
-        " ▐▛▀                ▐▌             ▝▜▌",
-        "▐███ ▐▙██▖▗▟██▖ ▟██▖▐▙██▖ ▟█▙  ▟█▙  ▐▌",
-        " ▐▌  ▐▛ ▐▌▐▙▄▖▘▐▛  ▘▐▛ ▐▌▐▛ ▜▌▐▛ ▜▌ ▐▌",
-        " ▐▌  ▐▌ ▐▌ ▀▀█▖▐▌   ▐▌ ▐▌▐▌ ▐▌▐▌ ▐▌ ▐▌",
+        "  ▄▄                ▗▖             ▗▄▖ ",
+        " ▐▛▀                ▐▌             ▝▜▌ ",
+        "▐███ ▐▙██▖▗▟██▖ ▟██▖▐▙██▖ ▟█▙  ▟█▙  ▐▌ ",
+        " ▐▌  ▐▛ ▐▌▐▙▄▖▘▐▛  ▘▐▛ ▐▌▐▛ ▜▌▐▛ ▜▌ ▐▌ ",
+        " ▐▌  ▐▌ ▐▌ ▀▀█▖▐▌   ▐▌ ▐▌▐▌ ▐▌▐▌ ▐▌ ▐▌ ",
         " ▐▌  ▐▌ ▐▌▐▄▄▟▌▝█▄▄▌▐▌ ▐▌▝█▄█▘▝█▄█▘ ▐▙▄",
         " ▝▘  ▝▘ ▝▘ ▀▀▀  ▝▀▀ ▝▘ ▝▘ ▝▀▘  ▝▀▘   ▀▀",
         "",
     ]
     app_name3 = [
         " _______________________________________",
         "|  ▄▄                ▗▖             ▗▄▖ |",
```

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/bill.cp.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/bill.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/canteen.toml` & `fnschool-20240519.80822.833/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/config.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/consuming.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240519.80822.833/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240519.80822.833/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240519.80822.833/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/food.cp.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/food.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/food_classes.toml` & `fnschool-20240519.80822.833/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/operator.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/path.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/profile.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/test.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/canteen/workbook.py` & `fnschool-20240519.80822.833/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/entry.py` & `fnschool-20240519.80822.833/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/external.py` & `fnschool-20240519.80822.833/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/fnprint.py` & `fnschool-20240519.80822.833/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/language.py` & `fnschool-20240519.80822.833/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240519.80822.833/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/path.py` & `fnschool-20240519.80822.833/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool/test.py` & `fnschool-20240519.80822.833/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240518.81739.834/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240519.80822.833/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240518.81739.834
+Version: 20240519.80822.833
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240518.81739.834/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240519.80822.833/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

