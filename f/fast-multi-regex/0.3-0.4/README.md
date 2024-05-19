# Comparing `tmp/fast_multi_regex-0.3.tar.gz` & `tmp/fast_multi_regex-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_multi_regex-0.3.tar", last modified: Sun May 19 10:48:46 2024, max compression
+gzip compressed data, was "fast_multi_regex-0.4.tar", last modified: Sun May 19 11:43:28 2024, max compression
```

## Comparing `fast_multi_regex-0.3.tar` & `fast_multi_regex-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:48:46.557851 fast_multi_regex-0.3/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.3/LICENSE
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:48:46.557851 fast_multi_regex-0.3/PKG-INFO
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:48:46.542851 fast_multi_regex-0.3/fast_multi_regex/
--rwxrwxrwx   0     1024 users      (100)      510 2024-05-19 09:13:52.000000 fast_multi_regex-0.3/fast_multi_regex/__init__.py
--rwxrwxrwx   0     1024 users      (100)     6126 2024-05-19 10:09:51.000000 fast_multi_regex-0.3/fast_multi_regex/api.py
--rwxrwxrwx   0     1024 users      (100)     3087 2024-05-19 07:13:16.000000 fast_multi_regex-0.3/fast_multi_regex/api_types.py
--rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.3/fast_multi_regex/matcher.py
--rwxrwxrwx   0     1024 users      (100)     3236 2024-05-19 10:48:24.000000 fast_multi_regex-0.3/fast_multi_regex/server.py
--rwxrwxrwx   0     1024 users      (100)    11361 2024-05-19 10:45:38.000000 fast_multi_regex-0.3/fast_multi_regex/utils.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:48:46.554851 fast_multi_regex-0.3/fast_multi_regex.egg-info/
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       73 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 10:48:46.000000 fast_multi_regex-0.3/fast_multi_regex.egg-info/top_level.txt
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 10:48:46.558851 fast_multi_regex-0.3/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1234 2024-05-19 10:48:32.000000 fast_multi_regex-0.3/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.899294 fast_multi_regex-0.4/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.4/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:43:28.898294 fast_multi_regex-0.4/PKG-INFO
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.882294 fast_multi_regex-0.4/fast_multi_regex/
+-rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.4/fast_multi_regex/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     6199 2024-05-19 11:41:53.000000 fast_multi_regex-0.4/fast_multi_regex/api.py
+-rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.4/fast_multi_regex/api_types.py
+-rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.4/fast_multi_regex/matcher.py
+-rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.4/fast_multi_regex/server.py
+-rwxrwxrwx   0     1024 users      (100)    11517 2024-05-19 11:31:04.000000 fast_multi_regex-0.4/fast_multi_regex/utils.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.896294 fast_multi_regex-0.4/fast_multi_regex.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       73 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/top_level.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 11:43:28.899294 fast_multi_regex-0.4/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1234 2024-05-19 11:33:04.000000 fast_multi_regex-0.4/setup.py
```

### Comparing `fast_multi_regex-0.3/LICENSE` & `fast_multi_regex-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.3/PKG-INFO` & `fast_multi_regex-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_multi_regex
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,35 +20,14 @@
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
 
-访问 `http://127.0.0.1:8000/docs` 查看接口文档，接口访问例子：
-```shell
-curl -X 'POST' \
-  'http://127.0.0.1:8000/match' \
-  -H 'accept: application/json' \
-  -H 'Authorization: Bearer test' \
-  -H 'Content-Type: application/json' \
-  -d '{
-  "qs": [
-    {
-      "query": "test",
-      "db": "default",
-      "method": "strict",
-      "is_sort": true,
-      "detailed_level": 2,
-      "match_top_n": 0
-    }
-  ]
-}'
-```
-
 构建正则库，matchers_config_folder 内 json 文件例子：
 ```json
 {
     "cache_size": 128,
     "targets": [
         {
             "mark": "test",
@@ -65,14 +44,35 @@
             "bool_expr": "",
             "priority": 1
         }
     ]
 }
 ```
 
+访问 `http://127.0.0.1:8000/docs` 查看接口文档，接口访问例子：
+```shell
+curl -X 'POST' \
+  'http://127.0.0.1:8000/match' \
+  -H 'accept: application/json' \
+  -H 'Authorization: Bearer test' \
+  -H 'Content-Type: application/json' \
+  -d '{
+  "qs": [
+    {
+      "query": "test",
+      "db": "default",
+      "method": "strict",
+      "is_sort": true,
+      "detailed_level": 2,
+      "match_top_n": 0
+    }
+  ]
+}'
+```
+
 直接调包使用：
 ```python
 from fast_multi_regex import MultiRegexMatcher
 mr = MultiRegexMatcher()
 targets = [
     {
         "mark": "test",
```

### Comparing `fast_multi_regex-0.3/fast_multi_regex/api.py` & `fast_multi_regex-0.4/fast_multi_regex/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 
 def file_processor(
     path: str, 
     opt: Literal['modified', 'created', 'deleted'],
     context: dict,
 ):
+    if not (path.endswith('.pkl') and path[-1] != '.'):
+        return
     matchers_folder: str = context['matchers_folder']
     matchers: dict[str, MultiRegexMatcher] = context['matchers']
     name = os.path.splitext(os.path.relpath(path, matchers_folder))[0]
     if opt == 'modified' or opt == 'created':
         with open(path, 'rb') as f:
             matchers[name] = pickle.load(f)
     elif opt == 'deleted':
@@ -92,46 +94,46 @@
     start = time.time()
     result = []
     qs = body.qs if isinstance(body.qs, list) else [body.qs]
     
     for i, q in enumerate(qs):
         if q.db not in global_matchers:
             return RespMatch(message=f"qs{i}: db '{q.db}' not found", status=1)
-        one_result: list[OneMatchMark] = []
+        one_result: list[dict] = []  # list[OneMatchMark]
+                        
+        if q.method == 'first':
+            match = global_matchers[q.db].match_first(q.query)
+            if match:
+                one_result.append({'mark': match[0], 'matches': [match[1]], 'match_count': 1})
         
-        if q.method == 'all':
+        elif q.method == 'all':
             matches = global_matchers[q.db].match_all(q.query, q.is_sort, q.detailed_level, q.match_top_n)
             if isinstance(matches, list):
-                one_result += [OneMatchMark(mark=m) for m in matches]
+                one_result += [{'mark': m} for m in matches]
             else:
                 for mark, v in matches.items():
                     if isinstance(v, int):
-                        one_result.append(OneMatchMark(mark=mark, match_count=v))
+                        one_result.append({'mark': mark, 'match_count': v})
                     else:
-                        one_result.append(OneMatchMark(mark=mark, matches=v, match_count=len(v)))
-                        
-        elif q.method == 'first':
-            match = global_matchers[q.db].match_first(q.query)
-            if match:
-                one_result.append(OneMatchMark(mark=match[0], matches=[OneMatch(**match[1])]))
+                        one_result.append({'mark': mark, 'matches': v, 'match_count': len(v)})
                 
         elif q.method == 'strict':
             matches = global_matchers[q.db].match_strict(q.query, q.is_sort)
             for mark, v in matches.items():
-                one_result.append(OneMatchMark(mark=mark, matches=v, match_count=len(v)))
+                one_result.append({'mark': mark, 'matches': v, 'match_count': len(v)})
                 
         else:
             return RespMatch(message=f"qs{i}: method '{q.method}' not found", status=1)
         
         for om in one_result:
             if q.detailed_level == 1:
-                om.matches = None
-                om.match_count = None
+                om['matches'] = None
+                om['match_count'] = None
             elif q.detailed_level == 2:
-                om.matches = None
+                om['matches'] = None
         result.append(one_result)
     return RespMatch(result=result, milliseconds=(time.time() - start) * 1000)
 
 
 @app.get(
     "/info",
     response_model=RespInfo,
```

### Comparing `fast_multi_regex-0.3/fast_multi_regex/api_types.py` & `fast_multi_regex-0.4/fast_multi_regex/api_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     match_no: int = Field(..., ge=0, description='总共第几次匹配到的，从0开始')
     mark_regex_no: int = Field(..., ge=0, description='OneTarget.regexs 中的第几个正则匹配到的，从0开始')
 
 
 class OneMatchMark(BaseModel):
     mark: str = Field(..., description='匹配到的正则组')
     matches: Optional[list[OneMatch]] = Field(None, description='匹配到具体正则的详细信息')
-    match_count: Optional[int] = Field(None, description='匹配到的正则次数')
+    match_count: Optional[int] = Field(None, description='停止匹配前匹配到的正则次数')
 
 
 class OneQuery(BaseModel):
     query: str = Field(..., description='待匹配的字符串')
-    db: str = Field('default', description='匹配的正则库 name')
+    db: str = Field('default', description='匹配的正则库 name，一般是相对于 matchers_folder 的pkl路径(无后缀名)')
     method: Literal['first', 'all', 'strict'] = Field('strict', description='匹配方法，first: 只返回第一个匹配，all: 返回所有匹配，strict: 严格匹配')
     is_sort: bool = Field(True, description='是否按照正则库中出现顺序返回，适用于 method=all/strict')
     detailed_level: Literal[1, 2, 3] = Field(2, description='1: 只返回 mark, 2: 返回 mark 和出现次数, 3: 返回详细 OneMatch')
     match_top_n: int = Field(0, description='匹配元素次数限制, 小于等于 0 代表不限制，适用于 method=all')
 
 
 class RespGeneral(BaseModel):
```

### Comparing `fast_multi_regex-0.3/fast_multi_regex/matcher.py` & `fast_multi_regex-0.4/fast_multi_regex/matcher.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.3/fast_multi_regex/server.py` & `fast_multi_regex-0.4/fast_multi_regex/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 import os
 import uvicorn
 import multiprocessing
-# from fast_multi_regex import update_matchers_folder
 from .utils import update_matchers_folder
 
 
 log_config = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
@@ -34,15 +33,15 @@
             "propagate": False,
             "qualname": "uvicorn",
         },
     },
 }
 
 
-def main():
+def app_server():
     parser = argparse.ArgumentParser(
         description="fast_multi_regex server",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--api_tokens", type=str, default="test", help="API token，多个用英文逗号分隔")
     parser.add_argument("--port", type=int, default=8000, help="端口")
     parser.add_argument("--host", type=str, default="0.0.0.0", help="主机")
@@ -74,8 +73,8 @@
         workers=args.workers,
         log_level=args.log_level,
         log_config=args.log_config or log_config,
     )
 
 
 if __name__ == "__main__":
-    main()
+    app_server()
```

### Comparing `fast_multi_regex-0.3/fast_multi_regex/utils.py` & `fast_multi_regex-0.4/fast_multi_regex/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,30 +122,35 @@
             matchers_folder (str): matcher 文件夹路径
             matchers_config_folder (str): matcher 配置文件夹路径
             matchers (dict[str, MultiRegexMatcher]): matcher 字典
 
     Returns:
         str: 输出信息
     """
+    if not (path.endswith('.json') and path[-1] != '.'):
+        return
     matchers_folder: str = context['matchers_folder']
     matchers_config_folder: str = context['matchers_config_folder']
     matchers: dict[str, MultiRegexMatcher] = context['matchers']
     name = os.path.splitext(os.path.relpath(path, matchers_config_folder))[0]
     pkl_path = os.path.join(matchers_folder, f'{name}.pkl')
     success = False
     if opt == 'modified' or opt == 'created':
         with open(path, 'r', encoding='utf-8') as f:
-            config = json.load(f)
+            config: dict = json.load(f)
+        if not config.get('targets'):
+            return None
+        cache_size = config.get('cache_size')
         if name in matchers:
             success |= matchers[name].compile(config['targets'])
-            if config['cache_size'] != matchers[name].info.cache_size:
-                matchers[name].reset_cache(config['cache_size'])
+            if cache_size != matchers[name].info.cache_size:
+                matchers[name].reset_cache(cache_size)
                 success = True
         else:
-            matchers[name] = MultiRegexMatcher(config['cache_size'])
+            matchers[name] = MultiRegexMatcher(cache_size)
             matchers[name].compile(config['targets'])
             success = True
         if success:
             os.makedirs(os.path.dirname(pkl_path), exist_ok=True)
             with open(pkl_path, 'wb') as f:
                 pickle.dump(matchers[name], f)
     elif opt == 'deleted':
```

### Comparing `fast_multi_regex-0.3/fast_multi_regex.egg-info/PKG-INFO` & `fast_multi_regex-0.4/fast_multi_regex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-multi-regex
-Version: 0.3
+Version: 0.4
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -20,35 +20,14 @@
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
 
-访问 `http://127.0.0.1:8000/docs` 查看接口文档，接口访问例子：
-```shell
-curl -X 'POST' \
-  'http://127.0.0.1:8000/match' \
-  -H 'accept: application/json' \
-  -H 'Authorization: Bearer test' \
-  -H 'Content-Type: application/json' \
-  -d '{
-  "qs": [
-    {
-      "query": "test",
-      "db": "default",
-      "method": "strict",
-      "is_sort": true,
-      "detailed_level": 2,
-      "match_top_n": 0
-    }
-  ]
-}'
-```
-
 构建正则库，matchers_config_folder 内 json 文件例子：
 ```json
 {
     "cache_size": 128,
     "targets": [
         {
             "mark": "test",
@@ -65,14 +44,35 @@
             "bool_expr": "",
             "priority": 1
         }
     ]
 }
 ```
 
+访问 `http://127.0.0.1:8000/docs` 查看接口文档，接口访问例子：
+```shell
+curl -X 'POST' \
+  'http://127.0.0.1:8000/match' \
+  -H 'accept: application/json' \
+  -H 'Authorization: Bearer test' \
+  -H 'Content-Type: application/json' \
+  -d '{
+  "qs": [
+    {
+      "query": "test",
+      "db": "default",
+      "method": "strict",
+      "is_sort": true,
+      "detailed_level": 2,
+      "match_top_n": 0
+    }
+  ]
+}'
+```
+
 直接调包使用：
 ```python
 from fast_multi_regex import MultiRegexMatcher
 mr = MultiRegexMatcher()
 targets = [
     {
         "mark": "test",
```

### Comparing `fast_multi_regex-0.3/setup.py` & `fast_multi_regex-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'https://github.com/aitsc/fast_multi_regex'
 
 setup(
     name='fast_multi_regex',
-    version='0.3',
+    version='0.4',
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tanshicheng',
     license='GPLv3',
     url='https://github.com/aitsc/fast_multi_regex',
     keywords='tools',
```

