# Comparing `tmp/mmo_tools-0.2.0.tar.gz` & `tmp/mmo_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.2.0.tar", last modified: Sun May 19 08:54:00 2024, max compression
+gzip compressed data, was "mmo_tools-0.2.1.tar", last modified: Sun May 19 09:02:31 2024, max compression
```

## Comparing `mmo_tools-0.2.0.tar` & `mmo_tools-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 08:54:00.535274 mmo_tools-0.2.0/
--rw-rw-rw-   0        0        0     3646 2024-05-19 08:54:00.534269 mmo_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2428 2024-05-14 13:12:43.000000 mmo_tools-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 08:54:00.535274 mmo_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-19 08:53:57.000000 mmo_tools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 08:54:00.519315 mmo_tools-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 08:54:00.522302 mmo_tools-0.2.0/src/mmo_tools/
--rw-rw-rw-   0        0        0      304 2024-05-05 08:46:45.000000 mmo_tools-0.2.0/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     5628 2024-05-19 08:46:16.000000 mmo_tools-0.2.0/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     3149 2024-05-19 08:53:19.000000 mmo_tools-0.2.0/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-19 08:54:00.533264 mmo_tools-0.2.0/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     3646 2024-05-19 08:54:00.000000 mmo_tools-0.2.0/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-19 08:54:00.000000 mmo_tools-0.2.0/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 08:54:00.000000 mmo_tools-0.2.0/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 08:54:00.000000 mmo_tools-0.2.0/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 09:02:31.482295 mmo_tools-0.2.1/
+-rw-rw-rw-   0        0        0     3646 2024-05-19 09:02:31.482295 mmo_tools-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2428 2024-05-14 13:12:43.000000 mmo_tools-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 09:02:31.482295 mmo_tools-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-19 09:01:40.000000 mmo_tools-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:02:31.461367 mmo_tools-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 09:02:31.469338 mmo_tools-0.2.1/src/mmo_tools/
+-rw-rw-rw-   0        0        0      296 2024-05-19 09:01:27.000000 mmo_tools-0.2.1/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     5628 2024-05-19 08:46:16.000000 mmo_tools-0.2.1/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     3149 2024-05-19 08:53:19.000000 mmo_tools-0.2.1/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 09:02:31.481297 mmo_tools-0.2.1/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     3646 2024-05-19 09:02:31.000000 mmo_tools-0.2.1/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-19 09:02:31.000000 mmo_tools-0.2.1/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 09:02:31.000000 mmo_tools-0.2.1/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 09:02:31.000000 mmo_tools-0.2.1/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.2.0/PKG-INFO` & `mmo_tools-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmo_tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
```

### Comparing `mmo_tools-0.2.0/README.md` & `mmo_tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.2.0/setup.py` & `mmo_tools-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.2.0',  # Phiên bản đầu tiên
+    version='0.2.1',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.2.0/src/mmo_tools/core.py` & `mmo_tools-0.2.1/src/mmo_tools/core.py`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.2.0/src/mmo_tools/utils.py` & `mmo_tools-0.2.1/src/mmo_tools/utils.py`

 * *Files identical despite different names*

### Comparing `mmo_tools-0.2.0/src/mmo_tools.egg-info/PKG-INFO` & `mmo_tools-0.2.1/src/mmo_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmo-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh
 Home-page: UNKNOWN
 Author: Lam Dinh
 Author-email: ldl.contact.booking@gmail.com
 License: UNKNOWN
 Description: # mmo_tools
         Đây là một thư viện Python chứa các hàm tiện ích để chuyển đổi dữ liệu và cấu hình proxy .
```

