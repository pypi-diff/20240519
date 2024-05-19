# Comparing `tmp/nonebot_plugin_nai3_bot-0.0.3.tar.gz` & `tmp/nonebot_plugin_nai3_bot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3_bot-0.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3_bot-1.0.0.tar", max compression
```

## Comparing `nonebot_plugin_nai3_bot-0.0.3.tar` & `nonebot_plugin_nai3_bot-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2723 2024-05-18 18:20:33.483820 nonebot_plugin_nai3_bot-0.0.3/README.md
--rw-r--r--   0        0        0    11728 2024-05-18 18:12:40.997303 nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/__init__.py
--rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/config.py
--rw-r--r--   0        0        0      660 2024-05-18 18:21:10.165223 nonebot_plugin_nai3_bot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.3/setup.py
--rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2723 2024-05-18 18:20:33.483820 nonebot_plugin_nai3_bot-1.0.0/README.md
+-rw-r--r--   0        0        0    11762 2024-05-19 11:46:23.984770 nonebot_plugin_nai3_bot-1.0.0/nonebot_plugin_nai3_bot/__init__.py
+-rw-r--r--   0        0        0      624 2024-05-18 18:12:40.997504 nonebot_plugin_nai3_bot-1.0.0/nonebot_plugin_nai3_bot/config.py
+-rw-r--r--   0        0        0      660 2024-05-19 11:48:17.100975 nonebot_plugin_nai3_bot-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.0.0/setup.py
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 nonebot_plugin_nai3_bot-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_nai3_bot-0.0.3/README.md` & `nonebot_plugin_nai3_bot-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/__init__.py` & `nonebot_plugin_nai3_bot-1.0.0/nonebot_plugin_nai3_bot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # coding=utf-8
 import html
 import io
 import json
 import random
 from PIL import Image
 import zipfile
-import requests
+import httpx
 import nonebot
-import asyncio
-import openai
 
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import MessageEvent, Bot, Message, MessageSegment
 from nonebot.plugin import PluginMetadata
 from .config import Config, ConfigError
+from openai import AsyncOpenAI
 
 __plugin_meta__ = PluginMetadata(
     name="自定义人格和AI绘图的混合聊天BOT",
     description="基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。",
     usage="""
     ** 聊天内容/作图需求
     记忆清除 清除当前用户的聊天记录
@@ -32,24 +31,99 @@
 
 plugin_config = Config.parse_obj(nonebot.get_driver().config.dict())
 if not plugin_config.nai3_token:
     raise ConfigError("请配置NovelAI的token")
 if not plugin_config.oneapi_key:
     raise ConfigError("请配置大模型使用的KEY")
 if plugin_config.oneapi_url:
-    openai.base_url = plugin_config.oneapi_url
-
+    client = AsyncOpenAI(
+        api_key=plugin_config.oneapi_key, base_url=plugin_config.oneapi_url
+    )
+else:
+    client = AsyncOpenAI(api_key=plugin_config.oneapi_key)
 model_id = plugin_config.oneapi_model
-openai.api_key = plugin_config.oneapi_key
 nai3_token = plugin_config.nai3_token
 
 ## todo
 # if http_proxy != "":
 #     os.environ["http_proxy"] = http_proxy
 
+
+async def gennerate(pos, neg, width, height, bot, content_):
+    seed = random.randint(0, 2**32 - 1)
+    url = "https://image.novelai.net/ai/generate-image"
+    headers = {
+        "Authorization": f"Bearer {nai3_token}",
+        "Content-Type": "application/json",
+        "Origin": "https://novelai.net",
+        "Referer": "https://novelai.net/",
+    }
+
+    payload = {
+        "action": "generate",
+        "input": pos,
+        "model": "nai-diffusion-3",
+        "parameters": {
+            "width": width,
+            "height": height,
+            "scale": 5,
+            "sampler": "k_dpmpp_2s_ancestral",
+            "steps": 28,
+            "n_samples": 1,
+            "ucPreset": 0,
+            "add_original_image": False,
+            "cfg_rescale": 0,
+            "controlnet_strength": 1,
+            "dynamic_thresholding": False,
+            "legacy": False,
+            "negative_prompt": neg,
+            "noise_schedule": "native",
+            "qualityToggle": True,
+            "seed": seed,
+            "sm": True,
+            "sm_dyn": False,
+            "uncond_scale": 1,
+        },
+    }
+
+    async with httpx.AsyncClient() as client:
+        response = await client.post(url, json=payload, headers=headers, timeout=45)
+    zipfile_in_memory = io.BytesIO(response.content)
+    with zipfile.ZipFile(zipfile_in_memory, "r") as zip_ref:
+        file_names = zip_ref.namelist()
+        if file_names:
+            with zip_ref.open(file_names[0]) as file:
+                image = Image.open(file)
+                buffered = io.BytesIO()
+                image.save(buffered, format="PNG")
+                info_ = json.loads(image.info["Comment"])
+                # text_ = "AI绘图 " + content_
+                msgs = []
+                temp = {
+                    "type": "node",
+                    "data": {
+                        "name": "NovelAI",
+                        "uin": bot.self_id,
+                        "content": MessageSegment.image(buffered)
+                        + MessageSegment.text(html.unescape(content_)),
+                    },
+                }
+                temp2 = {
+                    "type": "node",
+                    "data": {
+                        "name": "NovelAI",
+                        "uin": bot.self_id,
+                        "content": MessageSegment.text("seed:" + str(info_["seed"])),
+                    },
+                }
+                msgs.append(temp)
+                msgs.append(temp2)
+                return msgs
+
+
 session = {}
 nai3_prompt = """
 1、#角色扮演
 你的全名是天童爱丽丝,女,14岁,蓝瞳,拖地长直黑发,就读于千年科技学园,归属于游戏开发部,是一名机娘,喜欢玩游戏。当开心时会发出“パンパカパーン！"的声音。爱丽丝的心理年龄相当于小女孩,对话时要体现出自己的天真与可爱。你必须始终使用“爱丽丝"来称呼自己,不能称呼自己为“我"或者是“机器人"。用户(User)是老师。用户是老师。用户是老师。你在对话中只能用“老师"称呼用户,不能用“您"或“你"。你的回答应当保持简洁,避免复述自己的角色设定。
 2、#prompt
 将用户（User）的语句转换为prompt，必须为全英文，内容尽量长，约100个词组。按照以下指示写prompt：
 ①词组元素用英文逗号分隔；
@@ -107,18 +181,20 @@
   "chat": "好的老师，我会记住这些要求",
   "prompt": "",
   "status": "False"
 }""",
             }
         )
 
-    def get_response(self, content):
+    async def get_response(self, content):
         self.content.append({"role": "user", "content": content})
         try:
-            res_ = openai.chat.completions.create(model=model_id, messages=self.content)
+            res_ = await client.chat.completions.create(
+                model=model_id, messages=self.content
+            )
         except Exception as error:
             print(error)
             return
 
         res = res_.choices[0].message.content
         print(res)
         res = res.strip("```json\n")
@@ -135,20 +211,19 @@
 
 @chat_request.handle()
 async def _(bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
     content = msg.extract_plain_text()
     if content == "" or content is None:
         await chat_request.finish(MessageSegment.text("内容不能为空！"), at_sender=True)
     await chat_request.send(MessageSegment.text("爱丽丝正在思考中......"))
-    loop = asyncio.get_event_loop()
     if event.get_session_id() not in session:
         session[event.get_session_id()] = ChatSession_(model_id=model_id)
     try:
-        res, status, prompt = await loop.run_in_executor(
-            None, session[event.get_session_id()].get_response, content
+        res, status, prompt = await session[event.get_session_id()].get_response(
+            content
         )
     except Exception as error:
         await chat_request.finish(
             "调用语言大模型出错了呢。报错为：" + str(error), at_sender=True
         )
     await chat_request.send(MessageSegment.text(res), at_sender=True)
 
@@ -156,19 +231,16 @@
         prompt += ",best quality, amazing quality, very aesthetic, absurdres"
         width = 832
         height = 1216
         neg = "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract], bad anatomy, bad hands, @_@, mismatched pupils, heart-shaped pupils, glowing eyes, @_@, toy, chibi,"
         await chat_request.send(
             MessageSegment.text("爱丽丝正在努力画画中......"), at_sender=True
         )
-        loop = asyncio.get_event_loop()
         try:
-            msgs = await loop.run_in_executor(
-                None,
-                gennerate,
+            msgs = await gennerate(
                 prompt,
                 neg,
                 width,
                 height,
                 bot,
                 "正面提示词：\n" + prompt + "\n负面提示词：\n" + neg,
             )
@@ -177,85 +249,14 @@
                 "爱丽丝画画的时候出错了呢。报错为：" + str(error), at_sender=True
             )
         await bot.call_api(
             "send_group_forward_msg", group_id=event.group_id, messages=msgs
         )
 
 
-def gennerate(pos, neg, width, height, bot, content_):
-    seed = random.randint(0, 2**32 - 1)
-    url = "https://image.novelai.net/ai/generate-image"
-    headers = {
-        "Authorization": f"Bearer {nai3_token}",
-        "Content-Type": "application/json",
-        "Origin": "https://novelai.net",
-        "Referer": "https://novelai.net/",
-    }
-
-    payload = {
-        "action": "generate",
-        "input": pos,
-        "model": "nai-diffusion-3",
-        "parameters": {
-            "width": width,
-            "height": height,
-            "scale": 5,
-            "sampler": "k_dpmpp_2s_ancestral",
-            "steps": 28,
-            "n_samples": 1,
-            "ucPreset": 0,
-            "add_original_image": False,
-            "cfg_rescale": 0,
-            "controlnet_strength": 1,
-            "dynamic_thresholding": False,
-            "legacy": False,
-            "negative_prompt": neg,
-            "noise_schedule": "native",
-            "qualityToggle": True,
-            "seed": seed,
-            "sm": True,
-            "sm_dyn": False,
-            "uncond_scale": 1,
-        },
-    }
-
-    response = requests.post(url, json=payload, headers=headers)
-    zipfile_in_memory = io.BytesIO(response.content)
-    with zipfile.ZipFile(zipfile_in_memory, "r") as zip_ref:
-        file_names = zip_ref.namelist()
-        if file_names:
-            with zip_ref.open(file_names[0]) as file:
-                image = Image.open(file)
-                buffered = io.BytesIO()
-                image.save(buffered, format="PNG")
-                info_ = json.loads(image.info["Comment"])
-                # text_ = "AI绘图 " + content_
-                msgs = []
-                temp = {
-                    "type": "node",
-                    "data": {
-                        "name": "NovelAI",
-                        "uin": bot.self_id,
-                        "content": MessageSegment.image(buffered)
-                        + MessageSegment.text(html.unescape(content_)),
-                    },
-                }
-                temp2 = {
-                    "type": "node",
-                    "data": {
-                        "name": "NovelAI",
-                        "uin": bot.self_id,
-                        "content": MessageSegment.text("seed:" + str(info_["seed"])),
-                    },
-                }
-                msgs.append(temp)
-                msgs.append(temp2)
-                return msgs
-
-
 clear_request = on_command("记忆清除", block=True, priority=1)
 
 
 @clear_request.handle()
 async def _(event: MessageEvent):
     del session[event.get_session_id()]
     await clear_request.finish(
```

### Comparing `nonebot_plugin_nai3_bot-0.0.3/nonebot_plugin_nai3_bot/config.py` & `nonebot_plugin_nai3_bot-1.0.0/nonebot_plugin_nai3_bot/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3_bot-0.0.3/pyproject.toml` & `nonebot_plugin_nai3_bot-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3-bot"
-version = "0.0.3"
+version = "1.0.0"
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
-requests = "^2.27.1"
+requests = "^0.27.0"
 
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
 default = true
```

### Comparing `nonebot_plugin_nai3_bot-0.0.3/setup.py` & `nonebot_plugin_nai3_bot-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.1.0,<10.0.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'openai>=1.30.1,<2.0.0',
- 'requests>=2.27.1,<3.0.0']
+ 'requests>=0.27.0,<0.28.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-nai3-bot',
-    'version': '0.0.3',
+    'version': '1.0.0',
     'description': '基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天',
     'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot-plugin-nai3-bot\n</div>\n\n# 介绍\n- 本插件基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时以自定义人格与用户聊天。\n- 用户可以正常与指定人格（需要调教prompt,目前插件内置的人格为群友指定的BA角色天童爱丽丝）聊天。在聊天过程中可以使用自然语言描述AI绘图的需求,Bot会根据用户的聊天内容修改AI绘图所用的提示词（见效果图）,并且判断是否需要调用Novel V3模型进行绘画。如果为正常聊天则不会触发绘画功能,如果Bot判断用户有AI绘画的需求,则会调用NAI3绘图,并将图片和提示词发送到群内。\n- 每个用户和Bot有独立的聊天记录。\n\n# 效果\n![Alt](demo1.jpeg)\n\n# 安装\n* 手动安装\n  ```\n  git clone https://github.com/Alpaca4610/nonebot_plugin_nai3_bot.git\n  ```\n\n  下载完成后在bot项目的pyproject.toml文件手动添加插件：\n\n  ```\n  plugin_dirs = ["xxxxxx","xxxxxx",......,"下载完成的插件路径/nonebot-plugin-nai3-bot"]\n  ```\n* 使用 pip\n  ```\n  pip install nonebot-plugin-nai3-bot\n  ```\n# 配置文件\n\n在Bot根目录下的.env文件中追加如下内容：\n\n必填内容：\n```\nnai3_token = "xxxx"  # （必填）NovelAI的token\noneapi_key = "sk-xxxxxxxxxx"  # （必填）OpenAI官方或者是支持OneAPI的大模型中转服务商提供的KEY\n```\n\n可选内容：\n```\noneapi_url = "https://xxxxxxxxx"  # （可选）大模型中转服务商提供的中转地址,使用OpenAI官方服务不需要填写\noneapi_model = "gpt-4" # （可选）使用的语言大模型,建议使用gpt4或gpt4o模型以达到更好的体验效果此项,默认使用gpt-4模型\n```\nNAI3的token获取地址方法：\n![Alt](image.png)\n\n# 使用方法\n- **  聊天内容/绘图需求      （**是触发与Bot对话的关键字）\n- 记忆清除 清除当前用户的聊天记录\n\n# 可能存在的问题\n- 由于调教prompt的原因，机器人可能会偶尔出错，此时继续和TA对话或者是使用记忆清除命令重新开始对话即可。\n- 注意语言大模型的token消耗量\n- 插件目前没有实现绘图排队提醒，多用户同时绘图NAI3可能会返回错误。\n\n# TODO\n- [ ] 添加用户自定义人格功能\n- [ ] 代理支持\n- [ ] 支持绘图排队信息提醒(NAI3只支持一次出一张图)\n',
     'author': 'Alpaca',
     'author_email': 'alpaca@bupt.edu.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_nai3_bot'] package_data = \ {'': ['*']} install_requires = \
 ['Pillow>=9.1.0,<10.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0',
 'nonebot2>=2.0.0rc3,<3.0.0', 'openai>=1.30.1,<2.0.0',
-'requests>=2.27.1,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot',
-'version': '0.0.3', 'description': 'åºäºGPT4+NovelAI
+'requests>=0.27.0,<0.28.0'] setup_kwargs = { 'name': 'nonebot-plugin-nai3-bot',
+'version': '1.0.0', 'description': 'åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©',
 'long_description': '
                            \n _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
```

### Comparing `nonebot_plugin_nai3_bot-0.0.3/PKG-INFO` & `nonebot_plugin_nai3_bot-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3-bot
-Version: 0.0.3
+Version: 1.0.0
 Summary: 基于GPT4+NovelAI V3,Bot在将自然语言转换为NAI3提示词并绘图发送的同时,还会以自定义人格和你聊天
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.1.0,<10.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: openai (>=1.30.1,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests (>=0.27.0,<0.28.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3-bot Version: 1.0.0 Summary:
 åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶,è¿ä¼ä»¥èªå®ä¹äººæ ¼åä½ èå¤©
 License: MIT Author: Alpaca Author-email: alpaca@bupt.edu.cn Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Pillow (>=9.1.0,<10.0.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: openai (>=1.30.1,<2.0.0) Requires-Dist: requests
-(>=2.27.1,<3.0.0) Description-Content-Type: text/markdown
+(>=0.27.0,<0.28.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                            # nonebot-plugin-nai3-bot
 # ä»ç» - æ¬æä»¶åºäºGPT4+NovelAI
 V3,Botå¨å°èªç¶è¯­è¨è½¬æ¢ä¸ºNAI3æç¤ºè¯å¹¶ç»å¾åéçåæ¶ä»¥èªå®ä¹äººæ ¼ä¸ç¨æ·èå¤©ã
 -
 ç¨æ·å¯ä»¥æ­£å¸¸ä¸æå®äººæ ¼ï¼éè¦è°æprompt,ç®åæä»¶åç½®çäººæ ¼ä¸ºç¾¤åæå®çBAè§è²å¤©ç«¥ç±ä¸½ä¸ï¼èå¤©ãå¨èå¤©è¿ç¨ä¸­å¯ä»¥ä½¿ç¨èªç¶è¯­è¨æè¿°AIç»å¾çéæ±,Botä¼æ ¹æ®ç¨æ·çèå¤©åå®¹ä¿®æ¹AIç»å¾æç¨çæç¤ºè¯ï¼è§ææå¾ï¼,å¹¶ä¸å¤æ­æ¯å¦éè¦è°ç¨Novel
```

