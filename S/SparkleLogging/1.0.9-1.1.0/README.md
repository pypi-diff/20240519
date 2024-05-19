# Comparing `tmp/SparkleLogging-1.0.9.tar.gz` & `tmp/SparkleLogging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-1.0.9.tar", last modified: Sat May 18 11:34:55 2024, max compression
+gzip compressed data, was "SparkleLogging-1.1.0.tar", last modified: Sun May 19 12:22:27 2024, max compression
```

## Comparing `SparkleLogging-1.0.9.tar` & `SparkleLogging-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.254013 SparkleLogging-1.0.9/
--rw-rw-rw-   0        0        0     3185 2024-05-18 11:34:55.251020 SparkleLogging-1.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.210128 SparkleLogging-1.0.9/SparkleLogging/
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.245036 SparkleLogging-1.0.9/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0     1160 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/HttpHander.py
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-04 07:52:07.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/excHandler.py
--rw-rw-rw-   0        0        0     1193 2024-05-18 11:31:30.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/exclogger.py
--rw-rw-rw-   0        0        0      954 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/plugins/websocketHander.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.249026 SparkleLogging-1.0.9/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-05-03 04:38:26.000000 SparkleLogging-1.0.9/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0      498 2024-05-04 03:09:16.000000 SparkleLogging-1.0.9/SparkleLogging/utils/core.py
--rw-rw-rw-   0        0        0     4700 2024-05-18 11:32:14.000000 SparkleLogging-1.0.9/SparkleLogging/utils/getLog.py
--rw-rw-rw-   0        0        0      434 2024-05-18 11:33:19.000000 SparkleLogging-1.0.9/SparkleLogging/utils/plugins_for_core.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:34:55.250022 SparkleLogging-1.0.9/SparkleLogging.egg-info/
--rw-rw-rw-   0        0        0     3185 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-05-18 11:34:54.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 11:34:53.000000 SparkleLogging-1.0.9/SparkleLogging.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 11:34:55.255010 SparkleLogging-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-05-18 11:23:59.000000 SparkleLogging-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:22:27.592154 SparkleLogging-1.1.0/
+-rw-rw-rw-   0        0        0     3374 2024-05-19 12:22:27.591159 SparkleLogging-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 12:22:27.516357 SparkleLogging-1.1.0/SparkleLogging/
+-rw-rw-rw-   0        0        0      516 2024-05-19 12:15:36.000000 SparkleLogging-1.1.0/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:22:27.583178 SparkleLogging-1.1.0/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0     1160 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/HttpHander.py
+-rw-rw-rw-   0        0        0        0 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/excHandler.py
+-rw-rw-rw-   0        0        0     1193 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/exclogger.py
+-rw-rw-rw-   0        0        0      954 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/plugins/websocketHander.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:22:27.588165 SparkleLogging-1.1.0/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0     5119 2024-05-19 12:16:04.000000 SparkleLogging-1.1.0/SparkleLogging/utils/_logger.py
+-rw-rw-rw-   0        0        0      499 2024-05-19 12:15:35.000000 SparkleLogging-1.1.0/SparkleLogging/utils/core.py
+-rw-rw-rw-   0        0        0      434 2024-05-19 12:04:01.000000 SparkleLogging-1.1.0/SparkleLogging/utils/plugins_for_core.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:22:27.589161 SparkleLogging-1.1.0/SparkleLogging.egg-info/
+-rw-rw-rw-   0        0        0     3374 2024-05-19 12:22:26.000000 SparkleLogging-1.1.0/SparkleLogging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2024-05-19 12:22:27.000000 SparkleLogging-1.1.0/SparkleLogging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:22:26.000000 SparkleLogging-1.1.0/SparkleLogging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-19 12:22:26.000000 SparkleLogging-1.1.0/SparkleLogging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-19 12:22:26.000000 SparkleLogging-1.1.0/SparkleLogging.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:22:27.592154 SparkleLogging-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-05-19 12:14:06.000000 SparkleLogging-1.1.0/setup.py
```

### Comparing `SparkleLogging-1.0.9/PKG-INFO` & `SparkleLogging-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.9
+Version: 1.1.0
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: websockets
 Requires-Dist: colorlog
 Requires-Dist: httpx
 
-
 # SparkleLogging日志库
 
 ## 描述
 
 这是一个可以支持异步记录日志,发送到HTTP,websocket服务器,同时配置简单,它还实现了识别代码异步和同步的环境
 以支持不同环境下的日志记录,当然了,理论上,这个日志如果2个模式都启用(websocket,http),那么会分别的往2个地方发送日志
 
 ### 示例用法
 
 ```python
-#from core import *
-from SparkleLogging.utils.core import LogManager
+from SparkleLogging import LogManager
 from logging import Formatter
 
 logger = LogManager.GetLogger(
     log_name='example',
     out_to_console=True,
     web_log_mode=True,
     WSpost_url='ws://localhost:8765',
     HTTPpost_url='http://localhost:8765',
     http_mode = True,
+    out_to_file=True,
     custom_fomatter=Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s',datefmt="%H:%M:%S")
 )
 
-logger.info('这是一个成功信息')
 logger.debug('这是一个调试信息')
-logger.critical('这是一个严重错误信息')
-logger.error('这是一个错误信息')
+logger.info('这是一个成功信息')
 logger.warning('这是一个警告信息')
+logger.error('这是一个错误信息')
+logger.critical('这是一个严重错误信息')
 ```
 
 ### 参数介绍
 
 - `log_name`: 指定日志记录器的名称
 - `out_to_console`: 是否输出到控制台,默认true
 - `web_log_mode`:是否启用websocket日志输出模式,默认false
@@ -55,17 +54,22 @@
 - `HTTPpost_url`: 如果启用http模式,则传入post_url,否则不管,默认None
 - `http_mode`: 是否启用http日志输出模式,默认false
 - `setConsoleLevel`: 设置控制台日志输出级别,默认DEBUG
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
+- `out_to_file`: 设置是否输出到文件,默认为True
 
 ## 更新日志
 
+# 2024/5/19 20:20
+
+添加了out_to_file参数,改善了代码,现在可以用 from SparkleLogging import logger 来直接导入使用!
+
 # 2024/5/18 19:24
 
 更新了不同的堆栈格式和方便使用的装饰器
 
 # 2024/2/20 1:01
 
 更新了自定义格式功能,修复了少量bug
```

### Comparing `SparkleLogging-1.0.9/SparkleLogging/plugins/HttpHander.py` & `SparkleLogging-1.1.0/SparkleLogging/plugins/HttpHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.9/SparkleLogging/plugins/excHandler.py` & `SparkleLogging-1.1.0/SparkleLogging/plugins/excHandler.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.9/SparkleLogging/plugins/exclogger.py` & `SparkleLogging-1.1.0/SparkleLogging/plugins/exclogger.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.9/SparkleLogging/plugins/websocketHander.py` & `SparkleLogging-1.1.0/SparkleLogging/plugins/websocketHander.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-1.0.9/SparkleLogging/utils/getLog.py` & `SparkleLogging-1.1.0/SparkleLogging/utils/_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from SparkleLogging.utils.plugins_for_core import *
 
 # 建议不要改这个地方
 DEFAUIT_FOMATTER = logging.Formatter(
-    fmt='[%(asctime)s.%(msecs)03d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d]: %(message)s',
+    fmt='%(asctime)s.%(msecs)03d| %(levelname)-8s |%(threadName)s|%(name)s.%(funcName)s|%(filename)s:%(lineno)d - %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 class LogManager:
     public_formatter = DEFAUIT_FOMATTER
 
     @classmethod
@@ -16,17 +16,22 @@
                   setWebsocketLevel: int = logging.INFO,
                   setHTTPLevel: int = logging.INFO,
                   out_to_console: bool = True,
                   web_log_mode: bool = False,
                   WSpost_url: str = "",
                   HTTPpost_url: str = "",
                   http_mode: bool = False,
-                  custom_formatter: logging.Formatter = DEFAUIT_FOMATTER
+                  custom_formatter: logging.Formatter = DEFAUIT_FOMATTER,
+                  out_to_file: bool = True
         ):
         # 确保日志名称有效
+        # 判断out_to_console和out_to_file的值
+        if (out_to_console == False and out_to_file == False and web_log_mode == False and http_mode == False):
+            raise AssertionError(f"emm,请问,你这4个模式都不启用,那你获取这个logger对象的意义在哪?🤔")
+        
         log_name = log_name if log_name else "default"
         if out_to_console:
             log_folder = f'./logs/{log_name}'
             if not os.path.exists(log_folder):
                 os.makedirs(log_folder, exist_ok=True)
 
         logger = logging.getLogger(log_name)
@@ -55,31 +60,31 @@
             if isinstance(console_handler, logging.StreamHandler):
                 console_formatter = colorlog.ColoredFormatter(fmt=f"%(log_color)s {console_formatter._fmt} %(reset)s",datefmt=console_formatter.datefmt, log_colors=log_color_config)
                 console_handler.setFormatter(console_formatter)
 
             logger.setLevel(setConsoleLevel)
             logger.addHandler(console_handler)
 
-        
-        file_handler = TimedRotatingFileHandler(f'./logs/{log_name}/{log_name}.log',encoding="utf-8", when='midnight', interval=1, backupCount=7)
-        file_handler.setLevel(setFileLevel)
-        file_handler.setFormatter(cls.public_formatter)
-
-        if custom_formatter:
-            file_handler.setFormatter(custom_formatter)
-
-        # 检查代码是否在异步环境中运行
-        if asyncio.iscoroutinefunction(logging.Handler.emit):
-            queue = asyncio.Queue()
-            queue_handler = QueueHandler(queue)
-            queue_listener = QueueListener(queue, file_handler)
-            logger.addHandler(queue_handler)
-            asyncio.ensure_future(queue_listener.start())
-        else:
-            logger.addHandler(file_handler)
+        if out_to_file:
+            file_handler = TimedRotatingFileHandler(f'./logs/{log_name}/{log_name}.log',encoding="utf-8", when='midnight', interval=1, backupCount=7)
+            file_handler.setLevel(setFileLevel)
+            file_handler.setFormatter(cls.public_formatter)
+
+            if custom_formatter:
+                file_handler.setFormatter(custom_formatter)
+
+            # 检查代码是否在异步环境中运行
+            if asyncio.iscoroutinefunction(logging.Handler.emit):
+                queue = asyncio.Queue()
+                queue_handler = QueueHandler(queue)
+                queue_listener = QueueListener(queue, file_handler)
+                logger.addHandler(queue_handler)
+                asyncio.ensure_future(queue_listener.start())
+            else:
+                logger.addHandler(file_handler)
 
         if web_log_mode and WSpost_url:
             websocket_handler = WebsocketHandler(WSpost_url)
             websocket_handler.setLevel(setWebsocketLevel)
             formatter = cls.public_formatter
             if custom_formatter:
                 formatter = custom_formatter
```

### Comparing `SparkleLogging-1.0.9/SparkleLogging.egg-info/PKG-INFO` & `SparkleLogging-1.1.0/SparkleLogging.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: SparkleLogging
-Version: 1.0.9
+Version: 1.1.0
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/SparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: websockets
 Requires-Dist: colorlog
 Requires-Dist: httpx
 
-
 # SparkleLogging日志库
 
 ## 描述
 
 这是一个可以支持异步记录日志,发送到HTTP,websocket服务器,同时配置简单,它还实现了识别代码异步和同步的环境
 以支持不同环境下的日志记录,当然了,理论上,这个日志如果2个模式都启用(websocket,http),那么会分别的往2个地方发送日志
 
 ### 示例用法
 
 ```python
-#from core import *
-from SparkleLogging.utils.core import LogManager
+from SparkleLogging import LogManager
 from logging import Formatter
 
 logger = LogManager.GetLogger(
     log_name='example',
     out_to_console=True,
     web_log_mode=True,
     WSpost_url='ws://localhost:8765',
     HTTPpost_url='http://localhost:8765',
     http_mode = True,
+    out_to_file=True,
     custom_fomatter=Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s',datefmt="%H:%M:%S")
 )
 
-logger.info('这是一个成功信息')
 logger.debug('这是一个调试信息')
-logger.critical('这是一个严重错误信息')
-logger.error('这是一个错误信息')
+logger.info('这是一个成功信息')
 logger.warning('这是一个警告信息')
+logger.error('这是一个错误信息')
+logger.critical('这是一个严重错误信息')
 ```
 
 ### 参数介绍
 
 - `log_name`: 指定日志记录器的名称
 - `out_to_console`: 是否输出到控制台,默认true
 - `web_log_mode`:是否启用websocket日志输出模式,默认false
@@ -55,17 +54,22 @@
 - `HTTPpost_url`: 如果启用http模式,则传入post_url,否则不管,默认None
 - `http_mode`: 是否启用http日志输出模式,默认false
 - `setConsoleLevel`: 设置控制台日志输出级别,默认DEBUG
 - `setFileLevel`: 设置文件日志输出级别,默认INFO
 - `setWebLevel`: 设置websocket日志输出级别,默认INFO
 - `setHttpLevel`: 设置http日志输出级别,默认INFO
 - `custom_fomatter`: 自定义格式化函数,默认None
+- `out_to_file`: 设置是否输出到文件,默认为True
 
 ## 更新日志
 
+# 2024/5/19 20:20
+
+添加了out_to_file参数,改善了代码,现在可以用 from SparkleLogging import logger 来直接导入使用!
+
 # 2024/5/18 19:24
 
 更新了不同的堆栈格式和方便使用的装饰器
 
 # 2024/2/20 1:01
 
 更新了自定义格式功能,修复了少量bug
```

### Comparing `SparkleLogging-1.0.9/SparkleLogging.egg-info/SOURCES.txt` & `SparkleLogging-1.1.0/SparkleLogging.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 SparkleLogging/plugins/DecoratorsTools.py
 SparkleLogging/plugins/HttpHander.py
 SparkleLogging/plugins/__init__.py
 SparkleLogging/plugins/excHandler.py
 SparkleLogging/plugins/exclogger.py
 SparkleLogging/plugins/websocketHander.py
 SparkleLogging/utils/__init__.py
+SparkleLogging/utils/_logger.py
 SparkleLogging/utils/core.py
-SparkleLogging/utils/getLog.py
 SparkleLogging/utils/plugins_for_core.py
```

### Comparing `SparkleLogging-1.0.9/setup.py` & `SparkleLogging-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SparkleLogging',
-    version='1.0.9',
+    version='1.1.0',
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/SparkleLogging',
```

