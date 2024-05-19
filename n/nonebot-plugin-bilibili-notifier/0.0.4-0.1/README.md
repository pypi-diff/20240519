# Comparing `tmp/nonebot-plugin-bilibili-notifier-0.0.4.tar.gz` & `tmp/nonebot-plugin-bilibili-notifier-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-bilibili-notifier-0.0.4.tar", last modified: Sun Mar 31 17:25:12 2024, max compression
+gzip compressed data, was "nonebot-plugin-bilibili-notifier-0.1.tar", last modified: Sun May 19 07:38:17 2024, max compression
```

## Comparing `nonebot-plugin-bilibili-notifier-0.0.4.tar` & `nonebot-plugin-bilibili-notifier-0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-03-31 17:25:10.145375 nonebot-plugin-bilibili-notifier-0.0.4/LICENSE
--rw-r--r--   0        0        0     3990 2024-03-31 17:25:10.145375 nonebot-plugin-bilibili-notifier-0.0.4/README.md
--rw-r--r--   0        0        0     7189 2024-03-31 17:25:10.149375 nonebot-plugin-bilibili-notifier-0.0.4/nonebot_plugin_bilibili_notifier/__init__.py
--rw-r--r--   0        0        0     1104 2024-03-31 17:25:10.149375 nonebot-plugin-bilibili-notifier-0.0.4/nonebot_plugin_bilibili_notifier/config.py
--rw-r--r--   0        0        0      740 2024-03-31 17:25:10.149375 nonebot-plugin-bilibili-notifier-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 nonebot-plugin-bilibili-notifier-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-19 07:38:15.205245 nonebot-plugin-bilibili-notifier-0.1/LICENSE
+-rw-r--r--   0        0        0     4234 2024-05-19 07:38:15.205245 nonebot-plugin-bilibili-notifier-0.1/README.md
+-rw-r--r--   0        0        0     7945 2024-05-19 07:38:15.205245 nonebot-plugin-bilibili-notifier-0.1/nonebot_plugin_bilibili_notifier/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-19 07:38:15.205245 nonebot-plugin-bilibili-notifier-0.1/nonebot_plugin_bilibili_notifier/config.py
+-rw-r--r--   0        0        0      783 2024-05-19 07:38:15.205245 nonebot-plugin-bilibili-notifier-0.1/pyproject.toml
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 nonebot-plugin-bilibili-notifier-0.1/PKG-INFO
```

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/LICENSE` & `nonebot-plugin-bilibili-notifier-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/README.md` & `nonebot-plugin-bilibili-notifier-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 </div>
 
 ## 📖 介绍
 
 B站UP的更新与开播通知机，默认每分钟爬取一次B站账号的动态与直播列表，将设置好的特定UP的更新或开播信息推送到QQ群里。
 
+理论上适配[SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere)支持的各种协议，实测了Onebot v11协议成功。
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-bilibili-notifier
@@ -87,14 +89,15 @@
 |:-----:|:----:|:----:|:----:|
 | bnotifier_cookies | 是 | 无 | 上面导出的B站cookies的文件路径 |
 | bnotifier_push_updates | 否 | {} | 设置追踪更新的UP主的ID）以及要推送的QQ群号，格式为{<BID1>: \[QQ群号1， QQ群号2, ...\], ...}。注意全部号码都应为字符串，一个例子：`{"823532": ["xxxxx", "yyyyy"]}`|
 | bnotifier_push_updates_by_group | 否 | {} | 作用同bnotifier_push_updates但格式为{QQ群: \[BID1, BID2, \]}，选择一个更适合你的方式即可 |
 | bnotifier_push_lives | 否 | {} | 同bnotifier_push_updates但这个变量控制的是开播通知 |
 | bnotifier_push_lives_by_group | 否 | {} | 格式同bnotifier_push_updates_by_group但这个变量控制的是开播通知 |
 | bnotifier_push_type_blacklist | 否 | {} | 屏蔽推送某种动态信息，格式：`{QQ群号或BID: ['DYNAMIC_TYPE_AV', 'DYNAMIC_TYPE_FORWARD', ...]}`这样会屏蔽特定群/特定up的某种动态信息。关于动态种类请参考[这个连接](https://github.com/SocialSisterYi/bilibili-API-collect/blob/master/docs/dynamic/dynamic_enum.md) |
+| bnotifier_msg_truncate | 否 | 256 | 将一条非常长的动态截短到设定的长度 |
 
 其它配置为开发调试时使用，正常使用无需调整。
 
 ### 效果图
 ![Notifier Demo](notifier-demo.png)
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # nonebot-plugin-bilibili-notifier _â¨ Bç«UPçæ´æ°ä¸å¼æ­éç¥æº â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç»
 Bç«UPçæ´æ°ä¸å¼æ­éç¥æºï¼é»è®¤æ¯åéç¬åä¸æ¬¡Bç«è´¦å·çå¨æä¸ç´æ­åè¡¨ï¼å°è®¾ç½®å¥½çç¹å®UPçæ´æ°æå¼æ­ä¿¡æ¯æ¨éå°QQç¾¤éã
-## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+çè®ºä¸éé[SAA](https://github.com/MountainDash/nonebot-plugin-send-
+anything-anywhere)æ¯æçåç§åè®®ï¼å®æµäºOnebot v11åè®®æåã ##
+ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-bilibili-notifier ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-bilibili-notifier
 pdm pdm add nonebot-plugin-bilibili-notifier poetry poetry add nonebot-plugin-
 bilibili-notifier conda conda install nonebot-plugin-bilibili-notifier æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
@@ -34,11 +36,12 @@
 bnotifier_push_lives_by_group | å¦ | {} |
 æ ¼å¼åbnotifier_push_updates_by_groupä½è¿ä¸ªåéæ§å¶çæ¯å¼æ­éç¥
 | | bnotifier_push_type_blacklist | å¦ | {} |
 å±è½æ¨éæç§å¨æä¿¡æ¯ï¼æ ¼å¼ï¼`{QQç¾¤å·æBID: ['DYNAMIC_TYPE_AV',
 'DYNAMIC_TYPE_FORWARD', ...]}`è¿æ ·ä¼å±è½ç¹å®ç¾¤/
 ç¹å®upçæç§å¨æä¿¡æ¯ãå³äºå¨æç§ç±»è¯·åè[è¿ä¸ªè¿æ¥]
 (https://github.com/SocialSisterYi/bilibili-API-collect/blob/master/docs/
-dynamic/dynamic_enum.md) |
+dynamic/dynamic_enum.md) | | bnotifier_msg_truncate | å¦ | 256 |
+å°ä¸æ¡éå¸¸é¿çå¨ææªç­å°è®¾å®çé¿åº¦ |
 å¶å®éç½®ä¸ºå¼åè°è¯æ¶ä½¿ç¨ï¼æ­£å¸¸ä½¿ç¨æ éè°æ´ã ###
 ææå¾ ![Notifier Demo](notifier-demo.png) ## å¶å®
 æé®é¢ææ°åè½éæ±ï¼è¯·æissueã
```

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/nonebot_plugin_bilibili_notifier/__init__.py` & `nonebot-plugin-bilibili-notifier-0.1/nonebot_plugin_bilibili_notifier/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from nonebot import require
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 require("nonebot_plugin_localstore")
 from nonebot_plugin_localstore import get_cache_file
-from nonebot import  get_plugin_config, get_bot
+require("nonebot_plugin_saa")
+from nonebot_plugin_saa import TargetQQGroup, MessageFactory, enable_auto_select_bot
+from nonebot import  get_plugin_config
 from nonebot.log import logger
 from .config import Config
 import json
 import time
 import datetime
 
 from bilibili_api import Credential
 from bilibili_api.dynamic import get_live_users
 from bilibili_api.utils.utils import get_api
 from bilibili_api.utils.network import Api
 from bilibili_api import settings
 
 API = get_api("dynamic")
+enable_auto_select_bot()
 
 async def get_dynamic_page_info(
     credential: Credential,
     features: str = "itemOpusStyle",
     pn: int = 1,
 ):
     api = API["info"]["dynamic_page_info"]
@@ -86,17 +89,14 @@
 
 # 获得验证信息信息
 def get_credential(file: str):
     cookies = fetch_cookies(file=file)
     # 生成一个 Credential 对象
     return Credential(**cookies)
 
-# 获取当前时刻（只发布当前时刻之后更新的动态）
-def get_last_update():
-    return int(time.time()) - config.bnotifier_timeshift
 
 # 把{qq: [mid]}的形式转化为{mid: [qq]}
 def convert_by_group(by_group: dict, normal: dict):
     for k, v in by_group.items():
         for ups in v:
             if ups in normal:
                 normal[ups].append(k)
@@ -119,80 +119,97 @@
 try:
     with open(tmp_save, 'r') as f:
         last_update = json.load(f)['last_update']
     dt = datetime.datetime.fromtimestamp(last_update)
     logger.info(f'加载上次更新时间{dt}({last_update})')
 except:
     logger.warning('未找到上次更新时间，使用当前时间')
-    last_update = get_last_update()
+    last_update = int(time.time())
     
 last_live = None
 # 设置延时
 settings.timeout = config.bnotifier_api_timeout
 # 将by group的配置转化为标准配置
 convert_by_group(config.bnotifier_push_updates_by_group, config.bnotifier_push_updates)
 convert_by_group(config.bnotifier_push_lives_by_group, config.bnotifier_push_lives)
 logger.info(f'推送更新消息的用户：群：{config.bnotifier_push_updates}' )
 logger.info(f'推送直播消息的用户：群：{config.bnotifier_push_lives}' )
 logger.info(f'屏蔽的消息/群：{config.bnotifier_push_type_blacklist}' )
 
-@scheduler.scheduled_job('cron', second='0', misfire_grace_time=60) # = UTC+8 1445
+def clean_url(u: str) -> str:
+    # 叔叔现在开始往链接里塞奇怪的东西了
+    return u.split('?')[0]
+
+def shorten(u: str) -> str:
+    l = config.bnotifier_msg_truncate
+    if len(u) > l:
+        return u[:l] + '\n...点击链接查看全文'
+    return u
+
+@scheduler.scheduled_job('cron', second='0', misfire_grace_time=20)
 async def fetch_bilibili_updates():
     global last_update
     if len(config.bnotifier_push_updates) == 0:
         return
     logger.debug('获取B站动态更新')
     dyna = await get_dynamic_page_info(credential)
     logger.debug(f'更新到{len(dyna)}条动态')
-    bot = get_bot()
     dyna_names = []
+    dyna_times = []
     for i, d in enumerate(dyna):
         logger.debug(f'处理第{i + 1}条动态')
         # logger.debug(d)
         res = parse_dynamic(d)
         logger.debug(res)
         dyna_names.append(res['name'])
         logger.debug(f'Time: {datetime.datetime.fromtimestamp(res["time"])}({res["time"]}) vs {last_update}')
         if (key:=str(res['mid'])) in config.bnotifier_push_updates and res['time'] > last_update:
             dtype = res['mid']
             if is_in_blacklist(key, dtype):
                 continue
-            msg = f"{res['name']} {res['text']}\n{res['url']}"
+            msg = f"{res['name']} {shorten(res['text'])}\n{clean_url(res['url'])}"
             for gid in config.bnotifier_push_updates[key]:
                 if is_in_blacklist(gid, dtype):
                     continue
                 logger.info(f'将{key}的更新推送到{gid}\n{msg}')
-                await bot.send_group_msg(group_id=gid, message=msg)
-    last_update = get_last_update()
-    with open(tmp_save, 'w') as f:
-        json.dump({'last_update': last_update}, f)
+                await MessageFactory(msg).send_to(TargetQQGroup(group_id=int(gid)))
+        dyna_times.append(res["time"])
+    if (t:= max(dyna_times)) != last_update: # 使用最后一条动态的时间
+        last_update = t
+        with open(tmp_save, 'w') as f:
+            json.dump({'last_update': t}, f)
+        logger.debug(f'刷新动态更新时间为{t}({last_update})')
     logger.debug(f'成功刷新{len(dyna)}条动态：' + ', '.join(dyna_names))
 
     
-@scheduler.scheduled_job('cron', second='0', misfire_grace_time=60) # = UTC+8 1445
+@scheduler.scheduled_job('cron', second='0', misfire_grace_time=20)
 async def fetch_bilibili_live_info():
     global last_live
     if len(config.bnotifier_push_lives) == 0:
         return
     logger.debug('获取直播状态')
     live = await get_live_users(credential=credential, size=50)
-    if live['count'] == 0:
-        last_live = set()
+    if live['count'] == 0 or 'items' not in live:
+        # 应对有时奇怪的网络错误
         return
     on_live = []
     on_live_names = []
-    bot = get_bot()
     for i, d in enumerate(live['items']):
         # logger.debug(f'处理第{i + 1}个直播用户')
         key = str(d['uid'])
         on_live.append(key)
         on_live_names.append(d['uname'])
         if key in config.bnotifier_push_lives and last_live is not None:
             # 已经在直播就不通知了
             if key in last_live:
                 continue
-            msg = f"{d['uname']}开始直播了：{d['title']}\n地址：{d['link']}"
+            # 现在title全都是空了，不知道为什么
+            msg = f"{d['uname']}开始直播了：{d['title']}\n地址：{clean_url(d['link'])}"
             for gid in config.bnotifier_push_lives[key]:
                 logger.info(f'将{key}的直播消息推送到{gid}')
-                await bot.send_group_msg(group_id=gid, message=msg)
+                await MessageFactory(msg).send_to(TargetQQGroup(group_id=int(gid)))
     last_live = set(on_live)
-    logger.debug(f'正在直播的有：{", ".join(on_live_names)}')
+    logger.debug(f'{live["count"]}用户正在直播：{", ".join(on_live_names)}')
+    # if live['count'] >= 10:
+    #     with open('live.log', '+a') as f:
+    #        f.write(f'{datetime.datetime.now()} | {live["count"]}用户正在直播：{", ".join(on_live_names)}\n')
+
```

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/nonebot_plugin_bilibili_notifier/config.py` & `nonebot-plugin-bilibili-notifier-0.1/nonebot_plugin_bilibili_notifier/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     {
         qq群：['DYNAMIC_TYPE_AV'],   不在群里推送视频投稿信息
         UP: ['DYNAMIC_TYPE_FORWARD'] 不推送这个up的转发信息
     }
     """
     bnotifier_api_timeout: float = 20
     """
-    dev用，API访问超时设置，不用管
+    dev用，API访问超时设置，如果网络不稳定可以酌情加大
     """
-    bnotifier_timeshift: int = 45
-    """
-    dev用，允许稍微靠前一点时间的动态，不用管
+    bnotifier_msg_truncate: int = 256
     """
+    截断一条超长的动态
+    """
```

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/pyproject.toml` & `nonebot-plugin-bilibili-notifier-0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "nonebot-plugin-bilibili-notifier"
-version = "0.0.4"
+version = "0.1"
 description = "NoneBot2 plugin for Bilibili update and live notifications"
 authors = [
     { name = "Variante", email = "382086919@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
     "nonebot-plugin-apscheduler>=0.2.0",
     "bilibili-api-python>=16.2.0",
     "nonebot_plugin_localstore",
+    "nonebot-plugin-send-anything-anywhere",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot-plugin-bilibili-notifier-0.0.4/PKG-INFO` & `nonebot-plugin-bilibili-notifier-0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilibili-notifier
-Version: 0.0.4
+Version: 0.1
 Summary: NoneBot2 plugin for Bilibili update and live notifications
 License: MIT
 Author-email: Variante <382086919@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/Variante/nonebot-plugin-bilibili-notifier
 Project-URL: Repository, https://github.com/Variante/nonebot-plugin-bilibili-notifier
 Description-Content-Type: text/markdown
@@ -32,14 +32,16 @@
 
 </div>
 
 ## 📖 介绍
 
 B站UP的更新与开播通知机，默认每分钟爬取一次B站账号的动态与直播列表，将设置好的特定UP的更新或开播信息推送到QQ群里。
 
+理论上适配[SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere)支持的各种协议，实测了Onebot v11协议成功。
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-bilibili-notifier
@@ -98,14 +100,15 @@
 |:-----:|:----:|:----:|:----:|
 | bnotifier_cookies | 是 | 无 | 上面导出的B站cookies的文件路径 |
 | bnotifier_push_updates | 否 | {} | 设置追踪更新的UP主的ID）以及要推送的QQ群号，格式为{<BID1>: \[QQ群号1， QQ群号2, ...\], ...}。注意全部号码都应为字符串，一个例子：`{"823532": ["xxxxx", "yyyyy"]}`|
 | bnotifier_push_updates_by_group | 否 | {} | 作用同bnotifier_push_updates但格式为{QQ群: \[BID1, BID2, \]}，选择一个更适合你的方式即可 |
 | bnotifier_push_lives | 否 | {} | 同bnotifier_push_updates但这个变量控制的是开播通知 |
 | bnotifier_push_lives_by_group | 否 | {} | 格式同bnotifier_push_updates_by_group但这个变量控制的是开播通知 |
 | bnotifier_push_type_blacklist | 否 | {} | 屏蔽推送某种动态信息，格式：`{QQ群号或BID: ['DYNAMIC_TYPE_AV', 'DYNAMIC_TYPE_FORWARD', ...]}`这样会屏蔽特定群/特定up的某种动态信息。关于动态种类请参考[这个连接](https://github.com/SocialSisterYi/bilibili-API-collect/blob/master/docs/dynamic/dynamic_enum.md) |
+| bnotifier_msg_truncate | 否 | 256 | 将一条非常长的动态截短到设定的长度 |
 
 其它配置为开发调试时使用，正常使用无需调整。
 
 ### 效果图
 ![Notifier Demo](notifier-demo.png)
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilibili-notifier Version: 0.0.4
+Metadata-Version: 2.1 Name: nonebot-plugin-bilibili-notifier Version: 0.1
 Summary: NoneBot2 plugin for Bilibili update and live notifications License:
 MIT Author-email: Variante <382086919@qq.com> Requires-Python: >=3.8 Project-
 URL: Homepage, https://github.com/Variante/nonebot-plugin-bilibili-notifier
 Project-URL: Repository, https://github.com/Variante/nonebot-plugin-bilibili-
 notifier Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # nonebot-plugin-bilibili-notifier _â¨ Bç«UPçæ´æ°ä¸å¼æ­éç¥æº â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç»
 Bç«UPçæ´æ°ä¸å¼æ­éç¥æºï¼é»è®¤æ¯åéç¬åä¸æ¬¡Bç«è´¦å·çå¨æä¸ç´æ­åè¡¨ï¼å°è®¾ç½®å¥½çç¹å®UPçæ´æ°æå¼æ­ä¿¡æ¯æ¨éå°QQç¾¤éã
-## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+çè®ºä¸éé[SAA](https://github.com/MountainDash/nonebot-plugin-send-
+anything-anywhere)æ¯æçåç§åè®®ï¼å®æµäºOnebot v11åè®®æåã ##
+ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-bilibili-notifier ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-bilibili-notifier
 pdm pdm add nonebot-plugin-bilibili-notifier poetry poetry add nonebot-plugin-
 bilibili-notifier conda conda install nonebot-plugin-bilibili-notifier æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
@@ -40,11 +42,12 @@
 bnotifier_push_lives_by_group | å¦ | {} |
 æ ¼å¼åbnotifier_push_updates_by_groupä½è¿ä¸ªåéæ§å¶çæ¯å¼æ­éç¥
 | | bnotifier_push_type_blacklist | å¦ | {} |
 å±è½æ¨éæç§å¨æä¿¡æ¯ï¼æ ¼å¼ï¼`{QQç¾¤å·æBID: ['DYNAMIC_TYPE_AV',
 'DYNAMIC_TYPE_FORWARD', ...]}`è¿æ ·ä¼å±è½ç¹å®ç¾¤/
 ç¹å®upçæç§å¨æä¿¡æ¯ãå³äºå¨æç§ç±»è¯·åè[è¿ä¸ªè¿æ¥]
 (https://github.com/SocialSisterYi/bilibili-API-collect/blob/master/docs/
-dynamic/dynamic_enum.md) |
+dynamic/dynamic_enum.md) | | bnotifier_msg_truncate | å¦ | 256 |
+å°ä¸æ¡éå¸¸é¿çå¨ææªç­å°è®¾å®çé¿åº¦ |
 å¶å®éç½®ä¸ºå¼åè°è¯æ¶ä½¿ç¨ï¼æ­£å¸¸ä½¿ç¨æ éè°æ´ã ###
 ææå¾ ![Notifier Demo](notifier-demo.png) ## å¶å®
 æé®é¢ææ°åè½éæ±ï¼è¯·æissueã
```

