# Comparing `tmp/nonebot_plugin_pcrjjc-0.8.0.tar.gz` & `tmp/nonebot_plugin_pcrjjc-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pcrjjc-0.8.0.tar", last modified: Tue May  7 10:34:30 2024, max compression
+gzip compressed data, was "nonebot_plugin_pcrjjc-0.8.1.tar", last modified: Sun May 19 06:08:45 2024, max compression
```

## Comparing `nonebot_plugin_pcrjjc-0.8.0.tar` & `nonebot_plugin_pcrjjc-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.582241 nonebot_plugin_pcrjjc-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.582241 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41895 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 10:34:24.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/text2img.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:34:30.586241 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 10:34:30.000000 nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:45.621100 nonebot_plugin_pcrjjc-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-19 06:08:45.617100 nonebot_plugin_pcrjjc-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 06:08:45.621100 nonebot_plugin_pcrjjc-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:45.613100 nonebot_plugin_pcrjjc-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:45.617100 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41895 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-19 06:08:35.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/text2img.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:45.617100 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-19 06:08:45.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 06:08:45.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:08:45.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-19 06:08:45.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 06:08:45.000000 nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot_plugin_pcrjjc-0.8.0/LICENSE` & `nonebot_plugin_pcrjjc-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/PKG-INFO` & `nonebot_plugin_pcrjjc-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.8.0
+Version: 0.8.1
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -66,15 +66,14 @@
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
 |        配置项        |    类型     | 是否必填  |   默认值   |           说明           |
 |:-----------------:|:---------:|:-----:|:-------:|:----------------------:|
 |    SUPERUSERS     | list[str] | True  |         | 超级用户QQ号，示例：["114514"]  |
 |   PCRJJC_GROUP    |    str    | False |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
 |       OTTO        |   bool    | False |  True   |    是否自动过验证码（不建议修改）     |
-|      VERSION      |    str    | False | "6.2.0" |         客户端版本号         |
 |      MAX_PRI      |    int    | False |    0    |         最大私聊人数         |
 |     MAX_PCRID     |    int    | False |    8    |       每人绑定的最大数量        |
 |    MAX_HISTORY    |    int    | False |   50    |        单人最多历史记录        |
 |   NOTICE_CD_MIN   |    int    | False |   10    |     上线提醒时间间隔（单位：分）     |
 |  REFRESH_SECOND   |    int    | False |    3    |      排名刷新频率（单位：秒）      |
 |  PCRJJC_ACCOUNTS  |   list    | True  |   ""    |       登录账号（模板如下）       |
 | FONT_DOWNLOAD_URL |    str    | False |    略    |        默认字体下载地址        |
```

### Comparing `nonebot_plugin_pcrjjc-0.8.0/README.md` & `nonebot_plugin_pcrjjc-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
 |        配置项        |    类型     | 是否必填  |   默认值   |           说明           |
 |:-----------------:|:---------:|:-----:|:-------:|:----------------------:|
 |    SUPERUSERS     | list[str] | True  |         | 超级用户QQ号，示例：["114514"]  |
 |   PCRJJC_GROUP    |    str    | False |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
 |       OTTO        |   bool    | False |  True   |    是否自动过验证码（不建议修改）     |
-|      VERSION      |    str    | False | "6.2.0" |         客户端版本号         |
 |      MAX_PRI      |    int    | False |    0    |         最大私聊人数         |
 |     MAX_PCRID     |    int    | False |    8    |       每人绑定的最大数量        |
 |    MAX_HISTORY    |    int    | False |   50    |        单人最多历史记录        |
 |   NOTICE_CD_MIN   |    int    | False |   10    |     上线提醒时间间隔（单位：分）     |
 |  REFRESH_SECOND   |    int    | False |    3    |      排名刷新频率（单位：秒）      |
 |  PCRJJC_ACCOUNTS  |   list    | True  |   ""    |       登录账号（模板如下）       |
 | FONT_DOWNLOAD_URL |    str    | False |    略    |        默认字体下载地址        |
```

### Comparing `nonebot_plugin_pcrjjc-0.8.0/pyproject.toml` & `nonebot_plugin_pcrjjc-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/config.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/main.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/query.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.8.0
+Version: 0.8.1
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -66,15 +66,14 @@
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
 |        配置项        |    类型     | 是否必填  |   默认值   |           说明           |
 |:-----------------:|:---------:|:-----:|:-------:|:----------------------:|
 |    SUPERUSERS     | list[str] | True  |         | 超级用户QQ号，示例：["114514"]  |
 |   PCRJJC_GROUP    |    str    | False |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
 |       OTTO        |   bool    | False |  True   |    是否自动过验证码（不建议修改）     |
-|      VERSION      |    str    | False | "6.2.0" |         客户端版本号         |
 |      MAX_PRI      |    int    | False |    0    |         最大私聊人数         |
 |     MAX_PCRID     |    int    | False |    8    |       每人绑定的最大数量        |
 |    MAX_HISTORY    |    int    | False |   50    |        单人最多历史记录        |
 |   NOTICE_CD_MIN   |    int    | False |   10    |     上线提醒时间间隔（单位：分）     |
 |  REFRESH_SECOND   |    int    | False |    3    |      排名刷新频率（单位：秒）      |
 |  PCRJJC_ACCOUNTS  |   list    | True  |   ""    |       登录账号（模板如下）       |
 | FONT_DOWNLOAD_URL |    str    | False |    略    |        默认字体下载地址        |
```

### Comparing `nonebot_plugin_pcrjjc-0.8.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot_plugin_pcrjjc-0.8.1/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

