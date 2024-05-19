# Comparing `tmp/nonebot_plugin_bf1marneserverlist-0.1.7.tar.gz` & `tmp/nonebot_plugin_bf1marneserverlist-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bf1marneserverlist-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_bf1marneserverlist-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_bf1marneserverlist-0.1.7.tar` & `nonebot_plugin_bf1marneserverlist-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2591 2024-02-18 08:20:09.032954 nonebot_plugin_bf1marneserverlist-0.1.7/README.md
--rw-r--r--   0        0        0     5602 2024-02-18 08:20:09.032954 nonebot_plugin_bf1marneserverlist-0.1.7/plugins/bf1marneserverlist/__init__.py
--rw-r--r--   0        0        0      203 2024-02-18 08:20:09.032954 nonebot_plugin_bf1marneserverlist-0.1.7/plugins/bf1marneserverlist/config.py
--rw-r--r--   0        0        0      410 2024-02-18 08:20:09.032954 nonebot_plugin_bf1marneserverlist-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 nonebot_plugin_bf1marneserverlist-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5602 2024-02-18 07:49:22.280926 nonebot_plugin_bf1marneserverlist-0.1.8/nonebot_plugin_bf1marneserverlist/__init__.py
+-rw-r--r--   0        0        0      203 2024-02-18 06:16:54.510012 nonebot_plugin_bf1marneserverlist-0.1.8/nonebot_plugin_bf1marneserverlist/config.py
+-rw-r--r--   0        0        0      392 2024-02-18 08:33:58.095086 nonebot_plugin_bf1marneserverlist-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2674 2024-02-18 04:37:21.020017 nonebot_plugin_bf1marneserverlist-0.1.8/README.md
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 nonebot_plugin_bf1marneserverlist-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_bf1marneserverlist-0.1.7/README.md` & `nonebot_plugin_bf1marneserverlist-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-bf1marneserverlist
+Version: 0.1.8
+Summary: nonebot-plugin-bf1marneserverlist
+Author: safeluren
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Description-Content-Type: text/markdown
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -77,8 +94,8 @@
 | marne_data_dir | 是 | './marne_data/' | 存储绑定数据的目录，目前是以群号为命名的.json文件，里面保存的是通过API返回到数据 |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | marne bind {服务器ID} | 主人、群主、管理员 | 否 | 群聊 | 服务器ID需要你自己寻找~ |
-| marne | 群员 | 否 | 群聊 | 无 |
+| marne | 群员 | 否 | 群聊 | 无 |
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-bf1marneserverlist Version: 0.1.8
+Summary: nonebot-plugin-bf1marneserverlist Author: safeluren Requires-Python:
+>=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.2.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-bf1marneserverlist _â¨ æ¥è¯¢BF1-MarneServeræå¡å¨ä¿¡æ¯
                           â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» æ¥è¯¢BF1çMarneServeræå¡å¨ä¿¡æ¯ ## ð¿ å®è£ ä½¿ç¨ nb-
 cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-
```

### Comparing `nonebot_plugin_bf1marneserverlist-0.1.7/plugins/bf1marneserverlist/__init__.py` & `nonebot_plugin_bf1marneserverlist-0.1.8/nonebot_plugin_bf1marneserverlist/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bf1marneserverlist-0.1.7/PKG-INFO` & `nonebot_plugin_bf1marneserverlist-0.1.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,84 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-bf1marneserverlist
-Version: 0.1.7
-Summary: nonebot-plugin-bf1marneserverlist
-Author: safeluren
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
-Description-Content-Type: text/markdown
-
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-bf1marneserverlist
-
-_✨ 查询BF1-MarneServer服务器信息 ✨_
-
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/safeluren/nonebot-plugin-bf1marneserverlist.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-bf1marneserverlist">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-bf1marneserverlist.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-查询BF1的MarneServer服务器信息
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-bf1marneserverlist
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-bf1marneserverlist
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-bf1marneserverlist
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-bf1marneserverlist
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-bf1marneserverlist
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_bf1marneserverlist"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| marne_url | 是 | 无 | 自行寻找相关URL，需要以/结尾 |
-| marne_plugin_enabled | 是 | True | 是否启用插件 |
-| marne_data_dir | 是 | './marne_data/' | 存储绑定数据的目录，目前是以群号为命名的.json文件，里面保存的是通过API返回到数据 |
-
-## 🎉 使用
-### 指令表
-| 指令 | 权限 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|:----:|
-| marne bind {服务器ID} | 主人、群主、管理员 | 否 | 群聊 | 服务器ID需要你自己寻找~ |
-| marne | 群员 | 否 | 群聊 | 无 |
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-bf1marneserverlist
+
+_✨ 查询BF1-MarneServer服务器信息 ✨_
+
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/safeluren/nonebot-plugin-bf1marneserverlist.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-bf1marneserverlist">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-bf1marneserverlist.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+查询BF1的MarneServer服务器信息
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-bf1marneserverlist
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-bf1marneserverlist
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-bf1marneserverlist
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-bf1marneserverlist
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-bf1marneserverlist
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_bf1marneserverlist"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| marne_url | 是 | 无 | 自行寻找相关URL，需要以/结尾 |
+| marne_plugin_enabled | 是 | True | 是否启用插件 |
+| marne_data_dir | 是 | './marne_data/' | 存储绑定数据的目录，目前是以群号为命名的.json文件，里面保存的是通过API返回到数据 |
+
+## 🎉 使用
+### 指令表
+| 指令 | 权限 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|:----:|
+| marne bind {服务器ID} | 主人、群主、管理员 | 否 | 群聊 | 服务器ID需要你自己寻找~ |
+| marne | 群员 | 否 | 群聊 | 无 |
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bf1marneserverlist Version: 0.1.7
-Summary: nonebot-plugin-bf1marneserverlist Author: safeluren Requires-Python:
->=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: nonebot-
-adapter-onebot (>=2.2.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
-Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-bf1marneserverlist _â¨ æ¥è¯¢BF1-MarneServeræå¡å¨ä¿¡æ¯
                           â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» æ¥è¯¢BF1çMarneServeræå¡å¨ä¿¡æ¯ ## ð¿ å®è£ ä½¿ç¨ nb-
 cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-
```

