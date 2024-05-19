# Comparing `tmp/easy_ernie-1.0.0.tar.gz` & `tmp/easy_ernie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ernie-1.0.0.tar", last modified: Thu May  9 13:06:08 2024, max compression
+gzip compressed data, was "easy_ernie-1.0.1.tar", last modified: Sun May 19 13:19:13 2024, max compression
```

## Comparing `easy_ernie-1.0.0.tar` & `easy_ernie-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/easy_ernie/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/ernie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/fast_ernie.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/easy_ernie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:19:13.524518 easy_ernie-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-19 13:19:13.524518 easy_ernie-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:19:13.528518 easy_ernie-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:19:13.524518 easy_ernie-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:19:13.524518 easy_ernie-1.0.1/src/easy_ernie/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/src/easy_ernie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/src/easy_ernie/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/src/easy_ernie/ernie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/src/easy_ernie/fast_ernie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-19 13:18:59.000000 easy_ernie-1.0.1/src/easy_ernie/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:19:13.524518 easy_ernie-1.0.1/src/easy_ernie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-19 13:19:13.000000 easy_ernie-1.0.1/src/easy_ernie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 13:19:13.000000 easy_ernie-1.0.1/src/easy_ernie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:19:13.000000 easy_ernie-1.0.1/src/easy_ernie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 13:19:13.000000 easy_ernie-1.0.1/src/easy_ernie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 13:19:13.000000 easy_ernie-1.0.1/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy_ernie-1.0.0/LICENSE` & `easy_ernie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ernie-1.0.0/PKG-INFO` & `easy_ernie-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 1.0.0
+Version: 1.0.1
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 
 ## Easy-Ernie原仓库误删,新建的
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/1)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-1.0.0-blue)
+![Release](https://img.shields.io/badge/Release-1.0.1-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI.
 ## 需求
 1. 语言: Python3.8+.
 2. 其他: 文心一言账户.
 ## 安装
@@ -48,24 +48,24 @@
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionName = '你好'
     response1 = ernie.ask('你好', sessionName=sessionName)
     print(response1.answer)
-    response2 = ernie.ask('我给你发的上一个消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
+    response2 = ernie.ask('我给你发的上一条消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
     print(response2.answer)
     ernie.deleteSession(response1.sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好').answer)
-    print(fastErnie.ask('我给你发的上一个消息是什么').answer)
+    print(fastErnie.ask('我给你发的上一条消息是什么').answer)
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy_ernie-1.0.0/README.md` & `easy_ernie-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Easy-Ernie原仓库误删,新建的
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/1)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-1.0.0-blue)
+![Release](https://img.shields.io/badge/Release-1.0.1-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI.
 ## 需求
 1. 语言: Python3.8+.
 2. 其他: 文心一言账户.
 ## 安装
@@ -28,24 +28,24 @@
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionName = '你好'
     response1 = ernie.ask('你好', sessionName=sessionName)
     print(response1.answer)
-    response2 = ernie.ask('我给你发的上一个消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
+    response2 = ernie.ask('我给你发的上一条消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
     print(response2.answer)
     ernie.deleteSession(response1.sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好').answer)
-    print(fastErnie.ask('我给你发的上一个消息是什么').answer)
+    print(fastErnie.ask('我给你发的上一条消息是什么').answer)
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy_ernie-1.0.0/setup.py` & `easy_ernie-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as file:
     readMe = file.read()
 
 setup(
     name='easy-ernie',
-    version='1.0.0',
+    version='1.0.1',
     description='简洁的调用文心一言的WebAPI',
     long_description=readMe,
     long_description_content_type='text/markdown',
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
```

### Comparing `easy_ernie-1.0.0/src/easy_ernie/ernie.py` & `easy_ernie-1.0.1/src/easy_ernie/ernie.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from typing import Generator, Optional
+from typing import Generator, Optional, BinaryIO
 from . import auxiliary, model
 import requests
-import re
 import json
+import baidubce.bce_client_configuration
+import baidubce.auth.bce_credentials
+import baidubce.services.bos.bos_client
+import io
+import hashlib
+import base64
 
 class Ernie:
     def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.BAIDUID = BAIDUID
         self.session = requests.Session()
-        self.session.headers = {
+        self.postHeaders = {
             'Accept': '*/*',
             'Accept-Encoding': 'gzip, deflate, br, zstd',
             'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
             'Connection': 'keep-alive',
             'Content-Length': '0',
             'Content-Type': 'application/json',
             'Cookie': f'BDUSS_BFESS={BDUSS_BFESS};',
@@ -36,27 +41,26 @@
             data = json.loads(data)
         except:
             raise Exception('请求失败,响应格式错误')
 
         if data['code'] != 0:
             raise Exception(f'请求失败,{data["msg"]}')
 
-    def request(self, method: str, url: str, data: Optional[dict]=None, stream: bool=False, check: bool=True) -> requests.Response:
-        if method == 'get':
-            self.response = self.session.get(url, params=data, stream=stream)
-        else:
-            self.session.headers['Content-Length'] = str(len(data))
-            self.response = self.session.request(method, url, data=json.dumps(data), stream=stream)
+    def request(self, method: str, url: str, data: Optional[dict]=None, headers: Optional[dict]=None, stream: bool=False, check: bool=True) -> requests.Response:
+        if method == 'post':
+            headers = headers or self.postHeaders.copy()
+            headers['Content-Length'] = str(len(data))
+            response = self.session.request(method, url, data=json.dumps(data), headers=headers, stream=stream)
 
         if not stream and check:
-            self.checkJson(self.response.text)
-        return self.response
+            self.checkJson(response.text)
+        return response
 
-    def post(self, url: str, data: dict, stream: bool=False, check: bool=True) -> requests.Response:
-        return self.request('post', url, data, stream=stream, check=check)
+    def post(self, url: str, data: dict, headers: Optional[dict]=None, stream: bool=False, check: bool=True) -> requests.Response:
+        return self.request('post', url, data, headers=headers, stream=stream, check=check)
 
     def getSession(self) -> model.Session:
         top = self.post(
             'https://yiyan.baidu.com/eb/session/top/list',
             {
                 'deviceType': 'pc',
                 'timestamp': auxiliary.getTimestamp(ms=True)
@@ -72,15 +76,15 @@
         ).json()
         originalTops = top['data']['sessions']
         originalNormals = normal['data']['sessions'] or []
 
         resultTops = []
         resultNormals = []
         for session in originalTops + originalNormals:
-            conversation = model.SessionBase(sessionId=session['sessionId'], name=session['sessionName'], botModel=session['model'], creationTimestamp=auxiliary.timeToTimestamp(session['createTime']))
+            conversation = model.SessionBase(sessionId=session['sessionId'], name=session['sessionName'], pluginIds=session['pluginIds'].split(','), botModel=session['model'], creationTimestamp=auxiliary.timeToTimestamp(session['createTime']))
             if session in originalTops:
                 resultTops.append(conversation)
             else:
                 resultNormals.append(conversation)
         return model.Session(tops=resultTops, normals=resultNormals)
 
     def renameSession(self, sessionId: str, name: str) -> bool:
@@ -169,46 +173,109 @@
         histories = []
         chats = sorted(chats.values(), key=lambda data: data['createTime'])
         for chat in chats:
             histories.append(model.SessionDetailHistory(chatId=chat['id'], role=chat['role'], text=chat['message'][0]['content'], creationTimestamp=auxiliary.timeToTimestamp(chat['createTime'])))
         currentChatId = history['data']['currentChatId']
         return model.SessionDetail(base=base, histories=histories, currentChatId=str(currentChatId))
 
-    def askStream(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0', botModel: model.BotModel=model.BotModel.EB3_5) -> Generator[model.AskStreamResponse, None, None]:
+    def getPlugin(self) -> list[model.Plugin]:
+        data = self.post(
+            'https://yiyan.baidu.com/plugin/store/user/query/install/plugin/detail',
+            {
+                'deviceType': 'pc',
+                'timestamp': auxiliary.getTimestamp(ms=True)
+            }
+        ).json()
+        plugins = []
+        for plugin in data['data']['pluginInfoVoList']:
+            plugins.append(model.Plugin(id=plugin['id'], name=plugin['pluginNameForHuman'], description=plugin['descriptionForHuman'], fileTypes=plugin['uploadTypeList'], raw=plugin))
+        return plugins
+
+    def uploadFile(self, file: BinaryIO, extension: model.FileExtension, sessionId: str='') -> model.File:
+        timestamp = auxiliary.getTimestamp(ms=True)
+        fileName = f'{timestamp}.{extension.name}'
+        yiyan = self.post(
+            'https://yiyan.baidu.com/eb/file/upload/acl',
+            {
+                'bucketName': None,
+                'deviceType': 'pc',
+                'fileName': fileName,
+                'sessionId': sessionId,
+                'timestamp': timestamp
+            }
+        ).json()
+        yiyanData = yiyan['data']
+
+        bceCnfig = baidubce.bce_client_configuration.BceClientConfiguration(credentials=baidubce.auth.bce_credentials.BceCredentials(yiyanData['ak'], yiyanData['sk']), endpoint=yiyanData['bceUrl'].split('//')[1], security_token=yiyanData['token'])
+        bce = baidubce.services.bos.bos_client.BosClient(config=bceCnfig)
+        file.seek(0, io.SEEK_END)
+        fileSize = file.tell()
+        file.seek(0, io.SEEK_SET)
+        contentMD5 = base64.b64encode(hashlib.md5(file.read()).digest()).decode()
+        file.seek(0, io.SEEK_SET)
+        bce.put_object(yiyanData['bucketName'], yiyanData['fileKey'], file, fileSize, contentMD5)
+
+        if extension.value == 'image':
+            self.post(
+                'https://yiyan.baidu.com/eb/file/image/risk',
+                {
+                    'deviceType': 'pc',
+                    'fileKey': yiyanData['fileKey'],
+                    'fileUrl': yiyanData['bosUrl'],
+                    'timestamp': auxiliary.getTimestamp(ms=True)
+                }
+            )
+        return model.File(name=fileName, type_=extension.value, size=fileSize, url=yiyanData["bosUrl"])
+
+    def askStream(self, question: str, files: Optional[list[model.File]]=None, plugins: Optional[list[model.Plugin]]=None, sessionId: str='', sessionName: str='', parentChatId: str='0', botModel: model.BotModel=model.BotModel.EB3_5) -> Generator[model.AskStreamResponse, None, None]:
         acsToken = self.getAcsToken()
-        self.session.headers['Accept'] = 'text/event-stream, application/json'
-        self.session.headers['Acs-Token'] = acsToken
-        response = self.post(
-            'https://yiyan.baidu.com/eb/chat/conversation/v2',
-            {
-                'code': 0,
-                'deviceType': 'pc',
-                'file_ids': [],
-                'jt': '',
-                'model': botModel.value,
-                'msg': '',
-                'newAppSessionId': '',
-                'parentChatId': parentChatId,  # 官方上新会话时为数字0(但为了方便统一,初始为字符串0),之后官方是字符串
-                'pluginInfo': [],
-                'plugins': [],
-                'sessionId': sessionId,
-                'sessionName': sessionName or question,
-                'sign': acsToken,
-                'text': question,
-                'timestamp': auxiliary.getTimestamp(ms=True),
-                'type': 10
-            },
-            stream=True,
-            check=False
-        )
+        headers = self.postHeaders.copy()
+        headers['Accept'] = 'text/event-stream, application/json'
+        headers['Acs-Token'] = acsToken
+        askData = {
+            'code': 0,
+            'deviceType': 'pc',
+            'file_ids': [],
+            'jt': '',
+            'model': botModel.value,
+            'msg': '',
+            'newAppSessionId': '',
+            'parentChatId': parentChatId,  # 官方上新会话时为数字0(但为了方便统一,初始为字符串0),之后官方是字符串
+            'pluginInfo': [],
+            'plugins': [],
+            'sessionId': sessionId,
+            'sessionName': sessionName or question,
+            'sign': acsToken,
+            'text': question,
+            'timestamp': auxiliary.getTimestamp(ms=True),
+            'type': 10
+        }
+        if files:
+            askData['files'] = []
+            fileIndex = 1
+            for file in files:
+                askData['files'].append({
+                    'fId': f'file_{fileIndex}',
+                    'name': file.name,
+                    'size': file.size,
+                    'type': file.type_,
+                    'url': file.url
+                })
+                fileIndex += 1
+        if plugins:
+            for plugin in plugins:
+                askData['pluginInfo'].append(plugin.raw)
+                askData['plugins'].append({
+                    'plugin_id': plugin.id,
+                })
+        response = self.post('https://yiyan.baidu.com/eb/chat/conversation/v2', askData, headers=headers, stream=True, check=False)
 
         if 'application/json' in response.headers.get('Content-Type'):
             self.checkJson(response.text)
 
-        imageUrlPattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
         for line in response.iter_lines(decode_unicode=True):
             if not line:
                 continue
 
             if line.startswith('event:'):
                 event = line[6:]
                 continue
@@ -223,23 +290,19 @@
             if event == 'major':
                 sessionId = dataD['createSessionResponseVoCommonResult']['data']['sessionId']
                 botChatId = dataD['createChatResponseVoCommonResult']['data']['botChat']['id']
             elif event == 'message':
                 done = dataD['is_end']
                 if done == 0:
                     answer = dataD['content']
-                    urls = re.findall(imageUrlPattern, answer)
-                    answer = re.sub(imageUrlPattern, '', answer)
                     answer = answer.replace('<br>', '\n')
-                    yield model.AskStreamResponse(answer=answer, urls=urls, sessionId=sessionId, botChatId=botChatId, done=False)
+                    yield model.AskStreamResponse(answer=answer, sessionId=sessionId, botChatId=botChatId, done=False)
                 else:
                     answer = dataD['tokens_all']
-                    urls = re.findall(imageUrlPattern, answer)
-                    answer = re.sub(imageUrlPattern, '', answer)
                     answer = answer.replace('<br>', '\n')
                     answer = answer.strip()
-                    yield model.AskStreamResponse(answer=answer, urls=urls, sessionId=sessionId, botChatId=botChatId, done=True)
+                    yield model.AskStreamResponse(answer=answer, sessionId=sessionId, botChatId=botChatId, done=True)
 
     def ask(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0', botModel: model.BotModel=model.BotModel.EB3_5) -> model.AskResponse:
         data = list(self.askStream(question, sessionId=sessionId, sessionName=sessionName, parentChatId=parentChatId, botModel=botModel))
         doneData = data[-1]
-        return model.AskResponse(answer=doneData.answer, urls=doneData.urls, sessionId=doneData.sessionId, botChatId=doneData.botChatId)
+        return model.AskResponse(answer=doneData.answer, sessionId=doneData.sessionId, botChatId=doneData.botChatId)
```

### Comparing `easy_ernie-1.0.0/src/easy_ernie/fast_ernie.py` & `easy_ernie-1.0.1/src/easy_ernie/fast_ernie.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             yield data
         self.sessionId = data.sessionId
         self.parentChatId = data.botChatId
 
     def ask(self, question: str, botModel: model.BotModel=model.BotModel.EB3_5) -> model.AskResponse:
         data = list(self.askStream(question, botModel=botModel))
         doneData = data[-1]
-        return model.AskResponse(answer=doneData.answer, urls=doneData.urls, sessionId=doneData.sessionId, botChatId=doneData.botChatId)
+        return model.AskResponse(answer=doneData.answer, sessionId=doneData.sessionId, botChatId=doneData.botChatId)
 
     def close(self) -> bool:
         if self.ernie.deleteSession(self.sessionId):
             self.sessionId = ''
             self.sessionName = ''
             self.parentChatId = '0'
             return True
```

### Comparing `easy_ernie-1.0.0/src/easy_ernie.egg-info/PKG-INFO` & `easy_ernie-1.0.1/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 1.0.0
+Version: 1.0.1
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 
 ## Easy-Ernie原仓库误删,新建的
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/1)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-1.0.0-blue)
+![Release](https://img.shields.io/badge/Release-1.0.1-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI.
 ## 需求
 1. 语言: Python3.8+.
 2. 其他: 文心一言账户.
 ## 安装
@@ -48,24 +48,24 @@
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionName = '你好'
     response1 = ernie.ask('你好', sessionName=sessionName)
     print(response1.answer)
-    response2 = ernie.ask('我给你发的上一个消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
+    response2 = ernie.ask('我给你发的上一条消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
     print(response2.answer)
     ernie.deleteSession(response1.sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
     print(fastErnie.ask('你好').answer)
-    print(fastErnie.ask('我给你发的上一个消息是什么').answer)
+    print(fastErnie.ask('我给你发的上一条消息是什么').answer)
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

