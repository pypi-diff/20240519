# Comparing `tmp/embykeeper-3.2.8.tar.gz` & `tmp/embykeeper-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-3.2.8.tar", last modified: Wed Feb 14 18:24:37 2024, max compression
+gzip compressed data, was "embykeeper-3.2.9.tar", last modified: Fri Mar 15 17:25:48 2024, max compression
```

## Comparing `embykeeper-3.2.8.tar` & `embykeeper-3.2.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.889555 embykeeper-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-14 18:24:29.000000 embykeeper-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-14 18:24:29.000000 embykeeper-3.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-02-14 18:24:37.889555 embykeeper-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-14 18:24:29.000000 embykeeper-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.873555 embykeeper-3.2.8/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.873555 embykeeper-3.2.8/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.877555 embykeeper-3.2.8/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.881555 embykeeper-3.2.8/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27162 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/jms_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/judog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/ljyy_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/lyrebird.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/misty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/temby.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/terminus_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/bots/zhipian.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.881555 embykeeper-3.2.8/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/messager/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/follow.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/infinity_fly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/judog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_dragon_rain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_nohp.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (127)    26702 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeper/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.889555 embykeeper-3.2.8/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-14 18:24:37.000000 embykeeper-3.2.8/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.869555 embykeeper-3.2.8/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.869555 embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (127)   202097 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80372 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.885555 embykeeper-3.2.8/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.869555 embykeeper-3.2.8/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.889555 embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.889555 embykeeper-3.2.8/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-02-14 18:24:29.000000 embykeeper-3.2.8/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-14 18:24:29.000000 embykeeper-3.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-14 18:24:29.000000 embykeeper-3.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 18:24:37.889555 embykeeper-3.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 18:24:37.889555 embykeeper-3.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-14 18:24:29.000000 embykeeper-3.2.8/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-15 17:25:43.000000 embykeeper-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-15 17:25:43.000000 embykeeper-3.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-03-15 17:25:48.132820 embykeeper-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-03-15 17:25:43.000000 embykeeper-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.120820 embykeeper-3.2.9/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.120820 embykeeper-3.2.9/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.120820 embykeeper-3.2.9/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.124820 embykeeper-3.2.9/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27162 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/jms_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/judog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/ljyy_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/lyrebird.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/misty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/temby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/terminus_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/bots/zhipian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.128820 embykeeper-3.2.9/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/messager/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.128820 embykeeper-3.2.9/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/follow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/infinity_fly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/judog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_dragon_rain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_nohp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26702 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeper/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 17:25:47.000000 embykeeper-3.2.9/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-15 17:25:48.000000 embykeeper-3.2.9/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.128820 embykeeper-3.2.9/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.128820 embykeeper-3.2.9/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.116820 embykeeper-3.2.9/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.116820 embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   202097 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80372 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.116820 embykeeper-3.2.9/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-15 17:25:43.000000 embykeeper-3.2.9/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-15 17:25:43.000000 embykeeper-3.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-15 17:25:43.000000 embykeeper-3.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 17:25:48.132820 embykeeper-3.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 17:25:48.132820 embykeeper-3.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-15 17:25:43.000000 embykeeper-3.2.9/tests/test_cli.py
```

### Comparing `embykeeper-3.2.8/LICENSE` & `embykeeper-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/PKG-INFO` & `embykeeper-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 3.2.8
+Version: 3.2.9
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -123,15 +123,15 @@
 
 Embykeeper 支持 Docker 或 PyPI 安装 (Linux / Windows), 也支持云部署, 请点击下方按钮开始安装:
 
 [![Setup Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 
 若您没有服务器, 您可以通过免费的 Render 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/embykeeper-render-tutorial)
 
 若您有服务器, 我们推荐使用 [Docker 部署](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-%E9%83%A8%E7%BD%B2):
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 3.2.8 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 3.2.9 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -123,16 +123,16 @@
 embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/
 embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 è¥æ¨æ²¡ææå¡å¨, æ¨å¯ä»¥éè¿åè´¹ç Render
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-
 render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/
 embykeeper/tree/stable)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/
-26/embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
+embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/
+embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-
 %E9%83%A8%E7%BD%B2): ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨ä¹å¯ä»¥ä½¿ç¨ [Docker Compose é¨ç½²]
 (https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-Compose-
 %E9%83%A8%E7%BD%B2). é¤æ­¤ä¹å¤, æ¨è¿å¯ä»¥éè¿ [PyPI å®è£](https://
 github.com/embykeeper/embykeeper/wiki/Linux-%E4%BB%8E-PyPI-%E5%AE%89%E8%A3%85)
 æ [æºç æå»º](https://github.com/embykeeper/embykeeper/wiki/Linux-
```

### Comparing `embykeeper-3.2.8/README.md` & `embykeeper-3.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 Embykeeper 支持 Docker 或 PyPI 安装 (Linux / Windows), 也支持云部署, 请点击下方按钮开始安装:
 
 [![Setup Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 
 若您没有服务器, 您可以通过免费的 Render 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/embykeeper-render-tutorial)
 
 若您有服务器, 我们推荐使用 [Docker 部署](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-%E9%83%A8%E7%BD%B2):
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
```

#### html2text {}

```diff
@@ -102,16 +102,16 @@
 embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/
 embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 è¥æ¨æ²¡ææå¡å¨, æ¨å¯ä»¥éè¿åè´¹ç Render
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-
 render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/
 embykeeper/tree/stable)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/
-26/embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
+embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/
+embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-
 %E9%83%A8%E7%BD%B2): ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨ä¹å¯ä»¥ä½¿ç¨ [Docker Compose é¨ç½²]
 (https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-Compose-
 %E9%83%A8%E7%BD%B2). é¤æ­¤ä¹å¤, æ¨è¿å¯ä»¥éè¿ [PyPI å®è£](https://
 github.com/embykeeper/embykeeper/wiki/Linux-%E4%BB%8E-PyPI-%E5%AE%89%E8%A3%85)
 æ [æºç æå»º](https://github.com/embykeeper/embykeeper/wiki/Linux-
```

### Comparing `embykeeper-3.2.8/embykeeper/cli.py` & `embykeeper-3.2.9/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/data.py` & `embykeeper-3.2.9/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/embywatcher/emby.py` & `embykeeper-3.2.9/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/embywatcher/main.py` & `embykeeper-3.2.9/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/log.py` & `embykeeper-3.2.9/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/settings.py` & `embykeeper-3.2.9/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/base.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/charon.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/jms.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/jms_old.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/jms_old.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/judog.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/judog.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/ljyy_old.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/ljyy_old.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/lyrebird.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/lyrebird.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/magic.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/magic.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/misty.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/misty.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,26 +35,23 @@
                     msg = await wr("🛎每日签到")
                     if any(w in (msg.text or msg.caption) for w in ("上次签到", "验证码")):
                         break
                 else:
                     msg: Message = await wr("/cancel")
                     if "选择您要使用的功能" in (msg.caption or msg.text):
                         await asyncio.sleep(random.uniform(2, 4))
-                        msg = await wr("🌏切换服务器")
-                    if "选择您要使用的服务器" in (msg.text or msg.caption):
-                        await asyncio.sleep(random.uniform(2, 4))
-                        msg = await wr("✨Misty")
-                    if "选择您要使用的功能" in (msg.caption or msg.text):
-                        await asyncio.sleep(random.uniform(2, 4))
                         msg = await wr("🎲更多功能")
                     if "请选择功能" in msg.text or msg.caption:
                         await asyncio.sleep(random.uniform(2, 4))
                         msg = await wr("🛎每日签到")
                         if any(w in (msg.text or msg.caption) for w in ("上次签到", "验证码")):
                             break
+                        elif "获取账号失败" in (msg.text or msg.caption):
+                            self.log.warning(f"签到失败: 未注册账号.")
+                            return await self.fail()
             except asyncio.TimeoutError:
                 pass
         else:
             self.log.warning(f"签到失败: 无法进入签到页面.")
             await self.fail()
 
     async def cleanup(self):
```

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/nebula.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/peach.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/singularity.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/bots/terminus.py` & `embykeeper-3.2.9/embykeeper/telechecker/bots/terminus.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     name = "终点站"
     bot_username = "EmbyPublicBot"
     bot_checkin_cmd = ["/cancel", "/checkin"]
     bot_text_ignore = ["会话已取消", "没有活跃的会话"]
     bot_checked_keywords = ["今天已签到"]
     additional_auth = ["visual"]
     max_retries = 1
+    bot_use_history = 3
 
     async def on_photo(self, message: Message):
         """分析分析传入的验证码图片并返回验证码."""
         if message.reply_markup:
             clean = lambda o: emoji.replace_emoji(o, "").replace(" ", "")
             keys = [k for r in message.reply_markup.inline_keyboard for k in r]
             options = [k.text for k in keys]
@@ -29,12 +30,15 @@
             for i in range(3):
                 result, by = await Link(self.client).visual(message.photo.file_id, options_cleaned)
                 if result:
                     self.log.debug(f"已通过远端 ({by}) 解析答案: {result}.")
                     break
                 else:
                     self.log.warning(f"远端解析失败, 正在重试解析 ({i + 1}/3).")
+            else:
+                self.log.warning(f"签到失败: 验证码识别错误.")
+                return await self.fail()
             result = options[options_cleaned.index(result)]
             try:
                 await message.click(result)
             except RPCError:
                 self.log.warning("按钮点击失败.")
```

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/debug.py` & `embykeeper-3.2.9/embykeeper/telechecker/debug.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/link.py` & `embykeeper-3.2.9/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/log.py` & `embykeeper-3.2.9/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/main.py` & `embykeeper-3.2.9/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/messager/base.py` & `embykeeper-3.2.9/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/messager/pornemby.py` & `embykeeper-3.2.9/embykeeper/telechecker/messager/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/base.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import asyncio
-from logging import handlers
 import random
 import re
 from contextlib import asynccontextmanager
 import string
 from typing import Awaitable, Callable, Iterable, List, Optional, Sized, Union
 
 from loguru import logger
```

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/follow.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/follow.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/infinity_fly.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/infinity_fly.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/judog.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/judog.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/misty.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/polo.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_alert.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_alert.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_answer.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_answer.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_double.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_double.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_dragon_rain.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_dragon_rain.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_nohp.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_nohp.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/pornemby_register.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/pornemby_register.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/test.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/monitor/viper.py` & `embykeeper-3.2.9/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/telechecker/tele.py` & `embykeeper-3.2.9/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/utils.py` & `embykeeper-3.2.9/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper/windows.py` & `embykeeper-3.2.9/embykeeper/windows.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeper.egg-info/PKG-INFO` & `embykeeper-3.2.9/embykeeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 3.2.8
+Version: 3.2.9
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -123,15 +123,15 @@
 
 Embykeeper 支持 Docker 或 PyPI 安装 (Linux / Windows), 也支持云部署, 请点击下方按钮开始安装:
 
 [![Setup Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 
 若您没有服务器, 您可以通过免费的 Render 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+[![Deploy to Render](https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/embykeeper-render-tutorial)
 
 若您有服务器, 我们推荐使用 [Docker 部署](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-%E9%83%A8%E7%BD%B2):
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 3.2.8 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 3.2.9 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -123,16 +123,16 @@
 embykeeper/embykeeper/raw/main/images/setup-button.svg)](https://github.com/
 embykeeper/embykeeper/wiki/%E5%AE%89%E8%A3%85%E6%8C%87%E5%8D%97)
 è¥æ¨æ²¡ææå¡å¨, æ¨å¯ä»¥éè¿åè´¹ç Render
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
 (https://github.com/embykeeper/embykeeper/raw/main/images/deploy-to-
 render.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/
 embykeeper/tree/stable)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/
-26/embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
+embykeeper/raw/main/images/render-tutorial.svg)](https://zetx.tech/2023/06/26/
+embykeeper-render-tutorial) è¥æ¨ææå¡å¨, æä»¬æ¨èä½¿ç¨ [Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-
 %E9%83%A8%E7%BD%B2): ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
 net=host embykeeper/embykeeper ``` æ¨ä¹å¯ä»¥ä½¿ç¨ [Docker Compose é¨ç½²]
 (https://github.com/embykeeper/embykeeper/wiki/Linux-Docker-Compose-
 %E9%83%A8%E7%BD%B2). é¤æ­¤ä¹å¤, æ¨è¿å¯ä»¥éè¿ [PyPI å®è£](https://
 github.com/embykeeper/embykeeper/wiki/Linux-%E4%BB%8E-PyPI-%E5%AE%89%E8%A3%85)
 æ [æºç æå»º](https://github.com/embykeeper/embykeeper/wiki/Linux-
```

### Comparing `embykeeper-3.2.8/embykeeper.egg-info/SOURCES.txt` & `embykeeper-3.2.9/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/app.py` & `embykeeper-3.2.9/embykeeperweb/app.py`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/404.html` & `embykeeper-3.2.9/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-3.2.9/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-3.2.9/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-3.2.9/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-3.2.9/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/js/console.js` & `embykeeper-3.2.9/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/assets/js/script.js` & `embykeeper-3.2.9/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/console.html` & `embykeeper-3.2.9/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/embykeeperweb/templates/login.html` & `embykeeper-3.2.9/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-3.2.8/pyproject.toml` & `embykeeper-3.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "3.2.8"
+version = "3.2.9"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-3.2.8/tests/test_cli.py` & `embykeeper-3.2.9/tests/test_cli.py`

 * *Files identical despite different names*

