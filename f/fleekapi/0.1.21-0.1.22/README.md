# Comparing `tmp/fleekapi-0.1.21.tar.gz` & `tmp/fleekapi-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.21.tar", last modified: Sun May 19 12:21:32 2024, max compression
+gzip compressed data, was "fleekapi-0.1.22.tar", last modified: Sun May 19 12:23:16 2024, max compression
```

## Comparing `fleekapi-0.1.21.tar` & `fleekapi-0.1.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:21:32.388099 fleekapi-0.1.21/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:21:32.384099 fleekapi-0.1.21/FleekAPI/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.21/FleekAPI/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.21/FleekAPI/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.21/FleekAPI/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.21/FleekAPI/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:21:32.384099 fleekapi-0.1.21/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7725 2024-05-19 12:21:32.000000 fleekapi-0.1.21/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 12:21:32.000000 fleekapi-0.1.21/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 12:21:32.000000 fleekapi-0.1.21/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 12:21:32.000000 fleekapi-0.1.21/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 12:21:32.000000 fleekapi-0.1.21/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7725 2024-05-19 12:21:32.388099 fleekapi-0.1.21/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     6862 2024-05-19 12:21:15.000000 fleekapi-0.1.21/README.md
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 12:21:32.388099 fleekapi-0.1.21/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3980 2024-05-19 12:21:30.000000 fleekapi-0.1.21/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.012002 fleekapi-0.1.22/
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.004002 fleekapi-0.1.22/FleekAPI/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.22/FleekAPI/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.22/FleekAPI/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.22/FleekAPI/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.22/FleekAPI/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.008002 fleekapi-0.1.22/FleekAPI.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/top_level.txt
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 12:23:16.012002 fleekapi-0.1.22/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     6861 2024-05-19 12:22:45.000000 fleekapi-0.1.22/README.md
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 12:23:16.012002 fleekapi-0.1.22/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3980 2024-05-19 12:23:11.000000 fleekapi-0.1.22/setup.py
```

### Comparing `fleekapi-0.1.21/FleekAPI/app.py` & `fleekapi-0.1.22/FleekAPI/app.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.21/FleekAPI/middleware.py` & `fleekapi-0.1.22/FleekAPI/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.21/FleekAPI/response.py` & `fleekapi-0.1.22/FleekAPI/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.21/FleekAPI.egg-info/PKG-INFO` & `fleekapi-0.1.22/FleekAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.1.21
+Version: 0.1.22
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -32,15 +32,15 @@
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
 I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
 about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/fleekapi).
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
```

### Comparing `fleekapi-0.1.21/PKG-INFO` & `fleekapi-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.1.21
+Version: 0.1.22
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -32,15 +32,15 @@
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
 I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
 about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/fleekapi).
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
```

### Comparing `fleekapi-0.1.21/README.md` & `fleekapi-0.1.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
 I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
 about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/fleekapi).
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
```

### Comparing `fleekapi-0.1.21/setup.py` & `fleekapi-0.1.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'FleekAPI'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.21'
+VERSION = '0.1.22'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

