# Comparing `tmp/xiuyutools-1.0.tar.gz` & `tmp/xiuyutools-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiuyutools-1.0.tar", last modified: Mon May  6 06:52:48 2024, max compression
+gzip compressed data, was "xiuyutools-1.1.tar", last modified: Sun May 19 14:07:01 2024, max compression
```

## Comparing `xiuyutools-1.0.tar` & `xiuyutools-1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:48.481774 xiuyutools-1.0/
--rw-rw-rw-   0        0        0      460 2024-05-06 06:52:48.480763 xiuyutools-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      128 2024-05-06 06:39:33.000000 xiuyutools-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:48.476774 xiuyutools-1.0/owntools/
--rw-rw-rw-   0        0        0     4368 2022-06-06 01:42:41.000000 xiuyutools-1.0/owntools/Common.py
--rw-rw-rw-   0        0        0     3047 2023-04-12 07:57:53.000000 xiuyutools-1.0/owntools/CrackCode.py
--rw-rw-rw-   0        0        0     6370 2023-04-12 07:57:53.000000 xiuyutools-1.0/owntools/Download.py
--rw-rw-rw-   0        0        0     1459 2021-12-27 06:01:19.000000 xiuyutools-1.0/owntools/ExtractFile.py
--rw-rw-rw-   0        0        0      948 2021-12-27 06:01:41.000000 xiuyutools-1.0/owntools/Image.py
--rw-rw-rw-   0        0        0     1169 2024-05-06 01:00:34.000000 xiuyutools-1.0/owntools/Loger.py
--rw-rw-rw-   0        0        0     2496 2022-12-13 02:02:22.000000 xiuyutools-1.0/owntools/Mysql.py
--rw-rw-rw-   0        0        0     2965 2021-12-29 01:50:41.000000 xiuyutools-1.0/owntools/Subtitles.py
--rw-rw-rw-   0        0        0     2081 2023-02-15 06:12:42.000000 xiuyutools-1.0/owntools/Time.py
--rw-rw-rw-   0        0        0     4565 2022-01-12 06:36:41.000000 xiuyutools-1.0/owntools/Translation.py
--rw-rw-rw-   0        0        0      396 2021-12-27 06:01:33.000000 xiuyutools-1.0/owntools/UncompressRAR.py
--rw-rw-rw-   0        0        0     2343 2023-02-09 00:55:34.000000 xiuyutools-1.0/owntools/_SSH.py
--rw-rw-rw-   0        0        0      398 2023-02-09 00:55:34.000000 xiuyutools-1.0/owntools/__init__.py
--rw-rw-rw-   0        0        0     2839 2022-08-25 00:51:34.000000 xiuyutools-1.0/owntools/ownEmail.py
--rw-rw-rw-   0        0        0       42 2024-05-06 06:52:48.481774 xiuyutools-1.0/setup.cfg
--rw-rw-rw-   0        0        0      495 2024-05-06 06:47:42.000000 xiuyutools-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:52:48.479766 xiuyutools-1.0/xiuyutools.egg-info/
--rw-rw-rw-   0        0        0      460 2024-05-06 06:52:48.000000 xiuyutools-1.0/xiuyutools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-05-06 06:52:48.000000 xiuyutools-1.0/xiuyutools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:52:48.000000 xiuyutools-1.0/xiuyutools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 06:52:48.000000 xiuyutools-1.0/xiuyutools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 14:07:01.692984 xiuyutools-1.1/
+-rw-rw-rw-   0        0        0      570 2024-05-19 14:07:01.692984 xiuyutools-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-19 14:05:08.000000 xiuyutools-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 14:07:01.686978 xiuyutools-1.1/owntools/
+-rw-rw-rw-   0        0        0     4368 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Common.py
+-rw-rw-rw-   0        0        0     3047 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/CrackCode.py
+-rw-rw-rw-   0        0        0     6370 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Download.py
+-rw-rw-rw-   0        0        0     1459 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/ExtractFile.py
+-rw-rw-rw-   0        0        0      948 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Image.py
+-rw-rw-rw-   0        0        0     1169 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Loger.py
+-rw-rw-rw-   0        0        0     2496 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Mysql.py
+-rw-rw-rw-   0        0        0     3074 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Subtitles.py
+-rw-rw-rw-   0        0        0     3143 2024-05-19 14:01:51.000000 xiuyutools-1.1/owntools/Time.py
+-rw-rw-rw-   0        0        0     4700 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/Translation.py
+-rw-rw-rw-   0        0        0      396 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/UncompressRAR.py
+-rw-rw-rw-   0        0        0     2343 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/_SSH.py
+-rw-rw-rw-   0        0        0      398 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/__init__.py
+-rw-rw-rw-   0        0        0     2839 2024-05-06 13:27:21.000000 xiuyutools-1.1/owntools/ownEmail.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 14:07:01.693984 xiuyutools-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      495 2024-05-19 14:05:22.000000 xiuyutools-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:07:01.691982 xiuyutools-1.1/xiuyutools.egg-info/
+-rw-rw-rw-   0        0        0      570 2024-05-19 14:07:01.000000 xiuyutools-1.1/xiuyutools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-05-19 14:07:01.000000 xiuyutools-1.1/xiuyutools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 14:07:01.000000 xiuyutools-1.1/xiuyutools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 14:07:01.000000 xiuyutools-1.1/xiuyutools.egg-info/top_level.txt
```

### Comparing `xiuyutools-1.0/owntools/Common.py` & `xiuyutools-1.1/owntools/Common.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/CrackCode.py` & `xiuyutools-1.1/owntools/CrackCode.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/Download.py` & `xiuyutools-1.1/owntools/Download.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/ExtractFile.py` & `xiuyutools-1.1/owntools/ExtractFile.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/Image.py` & `xiuyutools-1.1/owntools/Image.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/Loger.py` & `xiuyutools-1.1/owntools/Loger.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/Mysql.py` & `xiuyutools-1.1/owntools/Mysql.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/Subtitles.py` & `xiuyutools-1.1/owntools/Subtitles.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-# Imports
-import os,re
-from typing import TypedDict
-from .Common import change_path_form
-
-class SrtToVtt():
-    """Convert .srt file to .vtt file
-
-    Args:
-        inputfilename (path): the output file name based on the inputfile name, as well as the path.
-    """
-
-    def __init__(self, inputfilename):
-
-        self.inputfilename = self._getInputPath(inputfilename)
-        self.outputfilename = self._getOutputPath()
-
-    def __call__(self):
-        self.main()
-
-    def _getInputPath(self, inputfilename):
-
-        if inputfilename == None:
-            print("Please enter the name of the file to open:", end=" ")
-            inputfilename = input()
-
-        done = False
-        while done == False:
-            if os.path.isfile(inputfilename):
-                done = True
-            else:
-                print("File not found, please enter the filename:", end=" ")
-                inputfilename = input()
-
-        return inputfilename
-
-    def _getOutputPath(self):
-        """ Return the outputfilename depend on the inputfilename """
-
-        path, name = os.path.split(self.inputfilename)
-        # Get the file name with suffix
-        name = os.path.splitext(name)[0]
-        outputfilename = os.path.join(path, name+".vtt")
-        return outputfilename
-
-    def _getTransformedLine(self, line):
-        if "-->" in line:
-            return line.replace(",", ".")
-        else:
-            return line
-
-    def main(self):
-
-        # Open the file
-        inputfile = open(self.inputfilename, "rb").read().decode("utf-8-sig").splitlines()
-
-        output = open(self.outputfilename, "w")
-        output.write("WEBVTT")
-        output.write("\n\n")
-        for line in inputfile:
-            output.write(self._getTransformedLine(line))
-            output.write("\n")
-        # Close our output file
-        output.close()
-
-        print(f"Write Done : {self.outputfilename}")
-
-
-class SubFuncs():
-    """
-    Normal Subtitll functions
-    : getSubFolder()
-
-    """
-
-    def __init__(self, path: str):
-        self.path = change_path_form(path)
-
-    def getSubFolder(self):
-
-        """Get the folders video name and sub name
-
-        Returns:
-            [dict]: {'fileName': '', 'subName': ''}
-        """
-
-        Type_folderData = TypedDict("Type_folderData", fileName=str, subName=str)
-
-        videoSuffix = ['mp4', 'mkv', 'mov', 'avi']
-        subSuffix = ['srt', 'ass']
-        folderData: Type_folderData = dict()
-
-        fileList: [str] = os.listdir(self.path)
-        for file in fileList:
-            for suffix in videoSuffix:
-                if re.findall(f".{suffix}$",file):
-                    folderData["fileName"] = file
-                    break
-            for suffix in subSuffix:
-                if re.findall(f".{suffix}$", file):
-                    folderData["subName"] = file
-                    break
-
-        return folderData
-
-
-if __name__ == "__main__":
-    test = SubFuncs("E:\Videos\Friends & 老友记\S10\es1")
-
+# Imports
+import os,re
+from typing import TypedDict
+from .Common import change_path_form
+
+class SrtToVtt():
+    """Convert .srt file to .vtt file
+
+    Args:
+        inputfilename (path): the output file name based on the inputfile name, as well as the path.
+    """
+
+    def __init__(self, inputfilename):
+
+        self.inputfilename = self._getInputPath(inputfilename)
+        self.outputfilename = self._getOutputPath()
+
+    def __call__(self):
+        self.main()
+
+    def _getInputPath(self, inputfilename):
+
+        if inputfilename == None:
+            print("Please enter the name of the file to open:", end=" ")
+            inputfilename = input()
+
+        done = False
+        while done == False:
+            if os.path.isfile(inputfilename):
+                done = True
+            else:
+                print("File not found, please enter the filename:", end=" ")
+                inputfilename = input()
+
+        return inputfilename
+
+    def _getOutputPath(self):
+        """ Return the outputfilename depend on the inputfilename """
+
+        path, name = os.path.split(self.inputfilename)
+        # Get the file name with suffix
+        name = os.path.splitext(name)[0]
+        outputfilename = os.path.join(path, name+".vtt")
+        return outputfilename
+
+    def _getTransformedLine(self, line):
+        if "-->" in line:
+            return line.replace(",", ".")
+        else:
+            return line
+
+    def main(self):
+
+        # Open the file
+        inputfile = open(self.inputfilename, "rb").read().decode("utf-8-sig").splitlines()
+
+        output = open(self.outputfilename, "w")
+        output.write("WEBVTT")
+        output.write("\n\n")
+        for line in inputfile:
+            output.write(self._getTransformedLine(line))
+            output.write("\n")
+        # Close our output file
+        output.close()
+
+        print(f"Write Done : {self.outputfilename}")
+
+
+class SubFuncs():
+    """
+    Normal Subtitll functions
+    : getSubFolder()
+
+    """
+
+    def __init__(self, path: str):
+        self.path = change_path_form(path)
+
+    def getSubFolder(self):
+
+        """Get the folders video name and sub name
+
+        Returns:
+            [dict]: {'fileName': '', 'subName': ''}
+        """
+
+        Type_folderData = TypedDict("Type_folderData", fileName=str, subName=str)
+
+        videoSuffix = ['mp4', 'mkv', 'mov', 'avi']
+        subSuffix = ['srt', 'ass']
+        folderData: Type_folderData = dict()
+
+        fileList: [str] = os.listdir(self.path)
+        for file in fileList:
+            for suffix in videoSuffix:
+                if re.findall(f".{suffix}$",file):
+                    folderData["fileName"] = file
+                    break
+            for suffix in subSuffix:
+                if re.findall(f".{suffix}$", file):
+                    folderData["subName"] = file
+                    break
+
+        return folderData
+
+
+if __name__ == "__main__":
+    test = SubFuncs("E:\Videos\Friends & 老友记\S10\es1")
+
```

### Comparing `xiuyutools-1.0/owntools/Time.py` & `xiuyutools-1.1/owntools/Time.py`

 * *Files 18% similar despite different names*

```diff
@@ -84,7 +84,39 @@
             str: format
     """
 
     datetime_date = convert_datetime(date)
     result = (datetime_date + datetime.timedelta(days=num)).strftime(format)
 
     return result
+
+
+def trans_to_date(value: str | int | datetime.date| datetime.datetime, format: str = "%Y-%m-%d"):
+    """ 判断类型并转换为date对象 """
+
+    # 判断是否为数字字符串
+    if isinstance(value, str) and value.isdigit():
+        value = int(value)
+
+    if isinstance(value, datetime.date):
+        return value
+
+    elif isinstance(value, datetime.datetime):
+        return value.date()
+
+    elif isinstance(value, str):
+        try:
+            return datetime.datetime.strptime(value, format).date()
+        except ValueError:
+            raise ValueError(f"输入的字符串格式不正确,请使用<{format}>格式")
+    elif isinstance(value, int):
+        try:
+            return datetime.datetime.fromtimestamp(value).date()
+        except ValueError:
+            raise ValueError("输入的时间戳无效")
+    else:
+        raise TypeError("输入值的类型必须是字符串(str)或整数(int)")
+
+
+def trans_to_datetime(value: str | int):
+    _date = trans_to_date(value)
+    return datetime.datetime.combine(_date, datetime.time())
```

### Comparing `xiuyutools-1.0/owntools/Translation.py` & `xiuyutools-1.1/owntools/Translation.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import time
-import json
-import requests
-import re
-import httpx
-
-class Translation():
-    def __init__(self):
-        """
-        Translate Function
-        """
-        import sys
-        from importlib import reload
-        reload(sys)
-
-        self.YOUDAO_URL = 'https://openapi.youdao.com/api'
-        self.APP_KEY = '55780d0d419052ba'
-        self.APP_SECRET = 'cm9nQh6b4rrBfDBBEpWOD1i2eDTGkdCx'
-
-    def encrypt(self, signStr):
-        import hashlib
-        hash_algorithm = hashlib.sha256()
-        hash_algorithm.update(signStr.encode('utf-8'))
-        return hash_algorithm.hexdigest()
-
-    def truncate(self, q):
-        if q is None:
-            return None
-        size = len(q)
-        return q if size <= 20 else q[0:10] + str(size) + q[size - 10:size]
-
-    def do_request(self, data):
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-        return requests.post(self.YOUDAO_URL, data=data, headers=headers)
-
-    async def do_request_async(self, data):
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-        async with httpx.AsyncClient(headers=headers) as client:
-            result = await client.post(self.YOUDAO_URL, data=data)
-        return result
-
-    def trans(self, from_language, content, useby='p'):
-        """
-        from_language : ja = japan; en = english;
-        if useby = 'p' => filter bracket content
-        """
-        import uuid
-
-        if useby == 'p':
-            pattern = '\(.*?\)|（.*?）|\[.*?\]'
-            content = re.sub(pattern, '', content, 0)
-
-        if content.endswith('\\') or content.endswith("'"):
-            content = content[:-1]
-
-        data = {}
-        data['from'] = from_language
-        data['to'] = 'zh-CHS'
-        data['signType'] = 'v3'
-        curtime = str(int(time.time()))
-        data['curtime'] = curtime
-        salt = str(uuid.uuid1())
-        signStr = self.APP_KEY + self.truncate(content) + salt + curtime + self.APP_SECRET
-        sign = self.encrypt(signStr)
-        data['appKey'] = self.APP_KEY
-        data['q'] = content
-        data['salt'] = salt
-        data['sign'] = sign
-        #data['vocabId'] = "您的用户词表ID"
-
-        response = self.do_request(data)
-        #contentType = response.headers['Content-Type']
-        result = json.loads(response.content.decode())
-
-        if result['errorCode'] == '0':
-            return result['translation'][0]
-        else:
-            errorcode = result['errorCode']
-            print(f'Translation wrong Error Code : {errorcode} \n Retring...')
-
-            response = self.do_request(data)
-            result = json.loads(response.content.decode())
-
-            if result['errorCode'] == '0':
-                return result['translation'][0]
-            else:
-                errorcode = result['errorCode']
-                return f'Translation wrong Error Code : {errorcode}'
-
-    async def trans_async(self, from_language, content, useby='p'):
-        """
-        from_language : ja = japan; en = english;
-        if useby = 'p' => filter bracket content
-        """
-        import uuid
-        if useby == 'p':
-            pattern = '\(.*?\)|（.*?）|\[.*?\]'
-            content = re.sub(pattern, '', content, 0)
-
-        if content.endswith('\\') or content.endswith("'"):
-            content = content[:-1]
-
-        data = {}
-        data['from'] = from_language
-        data['to'] = 'zh-CHS'
-        data['signType'] = 'v3'
-        curtime = str(int(time.time()))
-        data['curtime'] = curtime
-        salt = str(uuid.uuid1())
-        signStr = self.APP_KEY + self.truncate(content) + salt + curtime + self.APP_SECRET
-        sign = self.encrypt(signStr)
-        data['appKey'] = self.APP_KEY
-        data['q'] = content
-        data['salt'] = salt
-        data['sign'] = sign
-        #data['vocabId'] = "您的用户词表ID"
-
-        response = await self.do_request_async(data)
-        #contentType = response.headers['Content-Type']
-        result = json.loads(response.content.decode())
-
-        if result['errorCode'] == '0':
-            return result['translation'][0]
-        else:
-            errorcode = result['errorCode']
-            print(f'Translation wrong Error Code : {errorcode} \n Retring...')
-
-            response = await self.do_request_async(data)
-            result = json.loads(response.content.decode())
-
-            if result['errorCode'] == '0':
-                return result['translation'][0]
-            else:
-                errorcode = result['errorCode']
-                return f'Translation wrong Error Code : {errorcode}'
+import time
+import json
+import requests
+import re
+import httpx
+
+class Translation():
+    def __init__(self):
+        """
+        Translate Function
+        """
+        import sys
+        from importlib import reload
+        reload(sys)
+
+        self.YOUDAO_URL = 'https://openapi.youdao.com/api'
+        self.APP_KEY = '55780d0d419052ba'
+        self.APP_SECRET = 'cm9nQh6b4rrBfDBBEpWOD1i2eDTGkdCx'
+
+    def encrypt(self, signStr):
+        import hashlib
+        hash_algorithm = hashlib.sha256()
+        hash_algorithm.update(signStr.encode('utf-8'))
+        return hash_algorithm.hexdigest()
+
+    def truncate(self, q):
+        if q is None:
+            return None
+        size = len(q)
+        return q if size <= 20 else q[0:10] + str(size) + q[size - 10:size]
+
+    def do_request(self, data):
+        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        return requests.post(self.YOUDAO_URL, data=data, headers=headers)
+
+    async def do_request_async(self, data):
+        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
+        async with httpx.AsyncClient(headers=headers) as client:
+            result = await client.post(self.YOUDAO_URL, data=data)
+        return result
+
+    def trans(self, from_language, content, useby='p'):
+        """
+        from_language : ja = japan; en = english;
+        if useby = 'p' => filter bracket content
+        """
+        import uuid
+
+        if useby == 'p':
+            pattern = '\(.*?\)|（.*?）|\[.*?\]'
+            content = re.sub(pattern, '', content, 0)
+
+        if content.endswith('\\') or content.endswith("'"):
+            content = content[:-1]
+
+        data = {}
+        data['from'] = from_language
+        data['to'] = 'zh-CHS'
+        data['signType'] = 'v3'
+        curtime = str(int(time.time()))
+        data['curtime'] = curtime
+        salt = str(uuid.uuid1())
+        signStr = self.APP_KEY + self.truncate(content) + salt + curtime + self.APP_SECRET
+        sign = self.encrypt(signStr)
+        data['appKey'] = self.APP_KEY
+        data['q'] = content
+        data['salt'] = salt
+        data['sign'] = sign
+        #data['vocabId'] = "您的用户词表ID"
+
+        response = self.do_request(data)
+        #contentType = response.headers['Content-Type']
+        result = json.loads(response.content.decode())
+
+        if result['errorCode'] == '0':
+            return result['translation'][0]
+        else:
+            errorcode = result['errorCode']
+            print(f'Translation wrong Error Code : {errorcode} \n Retring...')
+
+            response = self.do_request(data)
+            result = json.loads(response.content.decode())
+
+            if result['errorCode'] == '0':
+                return result['translation'][0]
+            else:
+                errorcode = result['errorCode']
+                return f'Translation wrong Error Code : {errorcode}'
+
+    async def trans_async(self, from_language, content, useby='p'):
+        """
+        from_language : ja = japan; en = english;
+        if useby = 'p' => filter bracket content
+        """
+        import uuid
+        if useby == 'p':
+            pattern = '\(.*?\)|（.*?）|\[.*?\]'
+            content = re.sub(pattern, '', content, 0)
+
+        if content.endswith('\\') or content.endswith("'"):
+            content = content[:-1]
+
+        data = {}
+        data['from'] = from_language
+        data['to'] = 'zh-CHS'
+        data['signType'] = 'v3'
+        curtime = str(int(time.time()))
+        data['curtime'] = curtime
+        salt = str(uuid.uuid1())
+        signStr = self.APP_KEY + self.truncate(content) + salt + curtime + self.APP_SECRET
+        sign = self.encrypt(signStr)
+        data['appKey'] = self.APP_KEY
+        data['q'] = content
+        data['salt'] = salt
+        data['sign'] = sign
+        #data['vocabId'] = "您的用户词表ID"
+
+        response = await self.do_request_async(data)
+        #contentType = response.headers['Content-Type']
+        result = json.loads(response.content.decode())
+
+        if result['errorCode'] == '0':
+            return result['translation'][0]
+        else:
+            errorcode = result['errorCode']
+            print(f'Translation wrong Error Code : {errorcode} \n Retring...')
+
+            response = await self.do_request_async(data)
+            result = json.loads(response.content.decode())
+
+            if result['errorCode'] == '0':
+                return result['translation'][0]
+            else:
+                errorcode = result['errorCode']
+                return f'Translation wrong Error Code : {errorcode}'
```

### Comparing `xiuyutools-1.0/owntools/_SSH.py` & `xiuyutools-1.1/owntools/_SSH.py`

 * *Files identical despite different names*

### Comparing `xiuyutools-1.0/owntools/ownEmail.py` & `xiuyutools-1.1/owntools/ownEmail.py`

 * *Files identical despite different names*

