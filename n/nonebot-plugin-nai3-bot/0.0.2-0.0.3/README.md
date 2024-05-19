# Comparing `tmp/nonebot_plugin_nai3_bot-0.0.2.tar.gz` & `tmp/nonebot_plugin_nai3_bot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3_bot-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3_bot-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_nai3_bot-0.0.2.tar` & `nonebot_plugin_nai3_bot-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2716 2024-05-18 18:12:40.986423 nonebot_plugin_nai3_bot-0.0.2/README.md
--rw-r--r--   0        0        0     6148 2024-05-18 18:12:40.996971 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/.DS_Store
--rw-r--r--   0        0        0    11728 2024-05-18 18:12:40.997303 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/__init__.py
--rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/config.py
--rw-r--r--   0        0        0      639 2024-05-18 18:13:46.377339 nonebot_plugin_nai3_bot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.2/setup.py
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2723 2024-05-18 18:20:33.483820 nonebot_plugin_nai3_bot-0.0.3/README.md
+-rw-r--r--   0        0        0    11728 2024-05-18 18:12:40.997303 nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/__init__.py
+-rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/config.py
+-rw-r--r--   0        0        0      660 2024-05-18 18:21:10.165223 nonebot_plugin_nai3_bot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.3/setup.py
+-rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_nai3_bot-0.0.2/README.md` & `nonebot_plugin_nai3_bot-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
-- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。
+- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。
 
 # TODO
 - [ ] 添加用户自定义人格功能
 - [ ] 代理支持
-- [ ] 支持绘图排队(NAI3只支持一次出一张图)
+- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -21,10 +21,10 @@
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
 è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
 - æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
-æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã
 # TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
-æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
+æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

### Comparing `nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/__init__.py` & `nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.2/nonebot_plugin_nai3_bot/config.py` & `nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.2/pyproject.toml` & `nonebot_plugin_nai3_bot-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3-bot"
-version = "0.0.2"
+version = "0.0.3"
 description = "基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc3"
 nonebot-adapter-onebot = "^2.2.1"
 openai = "^1.30.1"
 Pillow = "^9.1.0"
+requests = "^2.27.1"
 
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

### Comparing `nonebot_plugin_nai3_bot-0.0.2/setup.py` & `nonebot_plugin_nai3_bot-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.1.0,<10.0.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
- 'openai>=1.30.1,<2.0.0']
+ 'openai>=1.30.1,<2.0.0',
+ 'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-nai3-bot',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队(NAI3只支持一次出一张图)\n',
+    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_nai3_bot'] package_data = \ {'': ['*']} install_requires = \
 ['Pillow>=9.1.0,<10.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
-'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=1.30.1,<2.0.0'] setup_kwargs = { 'name':
-'nonebot-plugin-nai3-bot', 'version': '0.0.2', 'description':
-'åºäºGPT4+NovelAI
+'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=1.30.1,<2.0.0',
+'requests>=2.27.1,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot',
+'version': '0.0.3', 'description': 'åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©',
 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
@@ -32,14 +32,14 @@
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å\n```\nNAI3çtokenè·åå°åæ¹æ³ï¼\n![Alt](image.png)\n\n#
 ä½¿ç¨æ¹æ³\n- ** èå¤©åå®¹/ç»å¾éæ±
 ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼\n- è®°å¿æ¸é¤
 æ¸é¤å½åç¨æ·çèå¤©è®°å½\n\n# å¯è½å­å¨çé®é¢\n-
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã\n-
 æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé\n-
-æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã\n\n#
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã\n\n#
 TODO\n- [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½\n- [ ] ä»£çæ¯æ\n- [ ]
-æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)\n', 'author': 'Alpaca',
-'author_email': 'alpaca@bupt.edu.cn', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)\n', 'author':
+'Alpaca', 'author_email': 'alpaca@bupt.edu.cn', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_nai3_bot-0.0.2/PKG-INFO` & `nonebot_plugin_nai3_bot-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: 基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.1.0,<10.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: openai (>=1.30.1,<2.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -73,14 +74,14 @@
 # 使用方法
 - **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）
 - 记忆清除 清除当前用户的聊天记录
 
 # 可能存在的问题
 - 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。
 - 注意语言大模型的token消耗量
-- 插件目前没有实现绘图排队功能，所以请避免较多用户同时使用绘图功能。
+- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。
 
 # TODO
 - [ ] 添加用户自定义人格功能
 - [ ] 代理支持
-- [ ] 支持绘图排队(NAI3只支持一次出一张图)
+- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 0.0.3 Summary:
 åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©
 License: MIT Author: Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Pillow (>=9.1.0,<10.0.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
-Requires-Dist: openai (>=1.30.1,<2.0.0) Description-Content-Type: text/markdown
+Requires-Dist: openai (>=1.30.1,<2.0.0) Requires-Dist: requests
+(>=2.27.1,<3.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                            # nonebot-plugin-nai3-bot
 # ä»ç» - æ¬æä»¶åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶ä»¥èªå®ä¹äººæ ¼ä¸ç¨æ·èå¤©ã
 -
 ç¨æ·å¯ä»¥æ­£å¸¸ä¸æå®äººæ ¼ï¼éè¦è°æprompt,ç®åæä»¶åç½®çäººæ ¼ä¸ºç¾¤åæå®çBAè§è²å¤©ç«¥ç±ä¸½ä¸ï¼èå¤©ãå¨èå¤©è¿ç¨ä¸­å¯ä»¥ä½¿ç¨èªç¶è¯­è¨æè¿°AIç»å¾çéæ±,Botä¼æ ¹æ®ç¨æ·çèå¤©åå®¹ä¿®æ¹AIç»å¾æç¨çæç¤ºè¯ï¼è§ææå¾ï¼,å¹¶ä¸å¤æ­æ¯å¦éè¦è°ç¨Novel
@@ -32,10 +33,10 @@
 oneapi_model = "gpt-4" #
 ï¼å¯éï¼ä½¿ç¨çè¯­è¨å¤§æ¨¡å,å»ºè®®ä½¿ç¨gpt4ægpt4oæ¨¡åä»¥è¾¾å°æ´å¥½çä½éªæææ­¤é¡¹,é»è®¤ä½¿ç¨gpt-
 4æ¨¡å ``` NAI3çtokenè·åå°åæ¹æ³ï¼ ![Alt](image.png) # ä½¿ç¨æ¹æ³
 - ** èå¤©åå®¹/ç»å¾éæ± ï¼**æ¯è§¦åä¸Botå¯¹è¯çå³é®å­ï¼ -
 è®°å¿æ¸é¤ æ¸é¤å½åç¨æ·çèå¤©è®°å½ # å¯è½å­å¨çé®é¢ -
 ç±äºè°æpromptçåå ï¼æºå¨äººå¯è½ä¼å¶å°åºéï¼æ­¤æ¶ç»§ç»­åTAå¯¹è¯æèæ¯ä½¿ç¨è®°å¿æ¸é¤å½ä»¤éæ°å¼å§å¯¹è¯å³å¯ã
 - æ³¨æè¯­è¨å¤§æ¨¡åçtokenæ¶èé -
-æä»¶ç®åæ²¡æå®ç°ç»å¾æéåè½ï¼æä»¥è¯·é¿åè¾å¤ç¨æ·åæ¶ä½¿ç¨ç»å¾åè½ã
+æä»¶ç®åæ²¡æå®ç°ç»å¾æéæéï¼å¤ç¨æ·åæ¶ç»å¾NAI3å¯è½ä¼è¿åéè¯¯ã
 # TODO - [ ] æ·»å ç¨æ·èªå®ä¹äººæ ¼åè½ - [ ] ä»£çæ¯æ - [ ]
-æ¯æç»å¾æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
+æ¯æç»å¾æéä¿¡æ¯æé(NAI3åªæ¯æä¸æ¬¡åºä¸å¼ å¾)
```

