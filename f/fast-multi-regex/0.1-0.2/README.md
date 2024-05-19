# Comparing `tmp/fast_multi_regex-0.1.tar.gz` & `tmp/fast_multi_regex-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_multi_regex-0.1.tar", last modified: Sun May 19 10:26:52 2024, max compression
+gzip compressed data, was "fast_multi_regex-0.2.tar", last modified: Sun May 19 10:36:24 2024, max compression
```

## Comparing `fast_multi_regex-0.1.tar` & `fast_multi_regex-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:26:52.533538 fast_multi_regex-0.1/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.1/LICENSE
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:26:52.532539 fast_multi_regex-0.1/PKG-INFO
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:26:52.515538 fast_multi_regex-0.1/fast_multi_regex/
--rwxrwxrwx   0     1024 users      (100)      510 2024-05-19 09:13:52.000000 fast_multi_regex-0.1/fast_multi_regex/__init__.py
--rwxrwxrwx   0     1024 users      (100)     6126 2024-05-19 10:09:51.000000 fast_multi_regex-0.1/fast_multi_regex/api.py
--rwxrwxrwx   0     1024 users      (100)     3087 2024-05-19 07:13:16.000000 fast_multi_regex-0.1/fast_multi_regex/api_types.py
--rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.1/fast_multi_regex/matcher.py
--rwxrwxrwx   0     1024 users      (100)    11395 2024-05-19 09:47:05.000000 fast_multi_regex-0.1/fast_multi_regex/utils.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:26:52.529538 fast_multi_regex-0.1/fast_multi_regex.egg-info/
--rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      395 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       56 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 10:26:52.000000 fast_multi_regex-0.1/fast_multi_regex.egg-info/top_level.txt
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 10:26:52.533538 fast_multi_regex-0.1/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1217 2024-05-19 10:17:33.000000 fast_multi_regex-0.1/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:36:24.681007 fast_multi_regex-0.2/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.2/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:36:24.680008 fast_multi_regex-0.2/PKG-INFO
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:36:24.661007 fast_multi_regex-0.2/fast_multi_regex/
+-rwxrwxrwx   0     1024 users      (100)      510 2024-05-19 09:13:52.000000 fast_multi_regex-0.2/fast_multi_regex/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     6126 2024-05-19 10:09:51.000000 fast_multi_regex-0.2/fast_multi_regex/api.py
+-rwxrwxrwx   0     1024 users      (100)     3087 2024-05-19 07:13:16.000000 fast_multi_regex-0.2/fast_multi_regex/api_types.py
+-rwxrwxrwx   0     1024 users      (100)    35706 2024-05-19 06:39:15.000000 fast_multi_regex-0.2/fast_multi_regex/matcher.py
+-rwxrwxrwx   0     1024 users      (100)     3192 2024-05-19 10:36:08.000000 fast_multi_regex-0.2/fast_multi_regex/server.py
+-rwxrwxrwx   0     1024 users      (100)    11395 2024-05-19 09:47:05.000000 fast_multi_regex-0.2/fast_multi_regex/utils.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 10:36:24.677008 fast_multi_regex-0.2/fast_multi_regex.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     2050 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       73 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 10:36:24.000000 fast_multi_regex-0.2/fast_multi_regex.egg-info/top_level.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 10:36:24.681007 fast_multi_regex-0.2/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1234 2024-05-19 10:36:22.000000 fast_multi_regex-0.2/setup.py
```

### Comparing `fast_multi_regex-0.1/LICENSE` & `fast_multi_regex-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.1/PKG-INFO` & `fast_multi_regex-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_multi_regex
-Version: 0.1
+Version: 0.2
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fast_multi_regex-0.1/fast_multi_regex/api.py` & `fast_multi_regex-0.2/fast_multi_regex/api.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.1/fast_multi_regex/api_types.py` & `fast_multi_regex-0.2/fast_multi_regex/api_types.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.1/fast_multi_regex/matcher.py` & `fast_multi_regex-0.2/fast_multi_regex/matcher.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.1/fast_multi_regex/utils.py` & `fast_multi_regex-0.2/fast_multi_regex/utils.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.1/fast_multi_regex.egg-info/PKG-INFO` & `fast_multi_regex-0.2/fast_multi_regex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-multi-regex
-Version: 0.1
+Version: 0.2
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `fast_multi_regex-0.1/setup.py` & `fast_multi_regex-0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'https://github.com/aitsc/fast_multi_regex'
 
 setup(
     name='fast_multi_regex',
-    version='0.1',
+    version='0.2',
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
-            'fast_multi_regex_server=server:main',  # 包不能有-符号
+            'fast_multi_regex_server=fast_multi_regex.server:main',  # 包不能有-符号
         ],
     },
     python_requires='>=3.7',
 )
```

