# Comparing `tmp/fast_multi_regex-0.4.tar.gz` & `tmp/fast_multi_regex-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_multi_regex-0.4.tar", last modified: Sun May 19 11:43:28 2024, max compression
+gzip compressed data, was "fast_multi_regex-0.5.tar", last modified: Sun May 19 11:47:43 2024, max compression
```

## Comparing `fast_multi_regex-0.4.tar` & `fast_multi_regex-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.899294 fast_multi_regex-0.4/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.4/LICENSE
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:43:28.898294 fast_multi_regex-0.4/PKG-INFO
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.882294 fast_multi_regex-0.4/fast_multi_regex/
--rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.4/fast_multi_regex/__init__.py
--rwxrwxrwx   0     1024 users      (100)     6199 2024-05-19 11:41:53.000000 fast_multi_regex-0.4/fast_multi_regex/api.py
--rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.4/fast_multi_regex/api_types.py
--rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.4/fast_multi_regex/matcher.py
--rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.4/fast_multi_regex/server.py
--rwxrwxrwx   0     1024 users      (100)    11517 2024-05-19 11:31:04.000000 fast_multi_regex-0.4/fast_multi_regex/utils.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:43:28.896294 fast_multi_regex-0.4/fast_multi_regex.egg-info/
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       73 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 11:43:28.000000 fast_multi_regex-0.4/fast_multi_regex.egg-info/top_level.txt
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 11:43:28.899294 fast_multi_regex-0.4/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1234 2024-05-19 11:33:04.000000 fast_multi_regex-0.4/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:47:43.637238 fast_multi_regex-0.5/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.5/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:47:43.636238 fast_multi_regex-0.5/PKG-INFO
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:47:43.619238 fast_multi_regex-0.5/fast_multi_regex/
+-rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.5/fast_multi_regex/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     6199 2024-05-19 11:41:53.000000 fast_multi_regex-0.5/fast_multi_regex/api.py
+-rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.5/fast_multi_regex/api_types.py
+-rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.5/fast_multi_regex/matcher.py
+-rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.5/fast_multi_regex/server.py
+-rwxrwxrwx   0     1024 users      (100)    11517 2024-05-19 11:31:04.000000 fast_multi_regex-0.5/fast_multi_regex/utils.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 11:47:43.633238 fast_multi_regex-0.5/fast_multi_regex.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       79 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 11:47:43.000000 fast_multi_regex-0.5/fast_multi_regex.egg-info/top_level.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 11:47:43.637238 fast_multi_regex-0.5/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1240 2024-05-19 11:47:34.000000 fast_multi_regex-0.5/setup.py
```

### Comparing `fast_multi_regex-0.4/LICENSE` & `fast_multi_regex-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/PKG-INFO` & `fast_multi_regex-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_multi_regex
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fast_multi_regex-0.4/fast_multi_regex/__init__.py` & `fast_multi_regex-0.5/fast_multi_regex/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex/api.py` & `fast_multi_regex-0.5/fast_multi_regex/api.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex/api_types.py` & `fast_multi_regex-0.5/fast_multi_regex/api_types.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex/matcher.py` & `fast_multi_regex-0.5/fast_multi_regex/matcher.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex/server.py` & `fast_multi_regex-0.5/fast_multi_regex/server.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex/utils.py` & `fast_multi_regex-0.5/fast_multi_regex/utils.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.4/fast_multi_regex.egg-info/PKG-INFO` & `fast_multi_regex-0.5/fast_multi_regex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-multi-regex
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fast_multi_regex-0.4/setup.py` & `fast_multi_regex-0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'https://github.com/aitsc/fast_multi_regex'
 
 setup(
     name='fast_multi_regex',
-    version='0.4',
+    version='0.5',
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tanshicheng',
     license='GPLv3',
     url='https://github.com/aitsc/fast_multi_regex',
     keywords='tools',
@@ -33,12 +33,12 @@
         'uvicorn',
         'watchdog',
         'asyncio',
         'requests',
     ],
     entry_points={  # 打包到bin
         'console_scripts': [
-            'fast_multi_regex_server=fast_multi_regex.server:main',  # 包不能有-符号
+            'fast_multi_regex_server=fast_multi_regex.server:app_server',  # 包不能有-符号
         ],
     },
     python_requires='>=3.7',
 )
```

