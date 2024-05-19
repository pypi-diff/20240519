# Comparing `tmp/ctrip-app-ui-0.5.4.tar.gz` & `tmp/ctrip-app-ui-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.5.4.tar", last modified: Sun May 19 02:43:32 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.5.5.tar", last modified: Sun May 19 03:08:17 2024, max compression
```

## Comparing `ctrip-app-ui-0.5.4.tar` & `ctrip-app-ui-0.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 02:43:32.678506 ctrip-app-ui-0.5.4/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 02:43:32.676510 ctrip-app-ui-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 02:43:32.649583 ctrip-app-ui-0.5.4/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.4/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.4/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.4/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.4/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.4/capp_ui/dir.py
--rw-rw-rw-   0        0        0    47381 2024-05-19 02:42:05.000000 ctrip-app-ui-0.5.4/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.4/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.4/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.4/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.4/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.4/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.4/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.4/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 02:43:32.675548 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 02:43:32.000000 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 02:43:32.000000 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 02:43:32.000000 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 02:43:32.000000 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 02:43:32.000000 ctrip-app-ui-0.5.4/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 02:43:32.678506 ctrip-app-ui-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 02:43:28.000000 ctrip-app-ui-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:08:17.878175 ctrip-app-ui-0.5.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 03:08:17.876180 ctrip-app-ui-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 03:08:17.848255 ctrip-app-ui-0.5.5/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.5/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.5/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.5/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.5/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.5/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    47483 2024-05-19 03:08:02.000000 ctrip-app-ui-0.5.5/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.5/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.5/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.5/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.5/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.5/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.5/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.5/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:08:17.875182 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 03:08:17.000000 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 03:08:17.000000 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 03:08:17.000000 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 03:08:17.000000 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 03:08:17.000000 ctrip-app-ui-0.5.5/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 03:08:17.878175 ctrip-app-ui-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 03:08:14.000000 ctrip-app-ui-0.5.5/setup.py
```

### Comparing `ctrip-app-ui-0.5.4/LICENSE` & `ctrip-app-ui-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/config.py` & `ctrip-app-ui-0.5.5/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/date_extend.py` & `ctrip-app-ui-0.5.5/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/device.py` & `ctrip-app-ui-0.5.5/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/dir.py` & `ctrip-app-ui-0.5.5/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/domain_service.py` & `ctrip-app-ui-0.5.5/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,16 @@
 
     @LoopFindElementObject(action="检测点击详情页去支付后，是否出现机舱售罄小弹框", loop=1, sleep=1)
     def get_sold_out_with_after_to_payment(self) -> dict:
         # 1. 图像识别方式检测是否出现航班售罄小弹框
         try:
             file_name = join_path([get_images_dir(), "订单详情_舱位售完.png"])
             if is_exists(file_name):
-                pos = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
                 if pos:
                     logger.warning("图像识别方式检测到有小弹框【价格舱位已售罄】")
                     return {"pos": pos}
         except (Exception,):
             pass
         # 2. 元素定位方式检测是否出现航班售罄小弹框
         try:
@@ -717,15 +718,16 @@
 
     @LoopFindElementObject(action="检测点击详情页去支付后，是否出现行程冲突小弹框", loop=1, sleep=1)
     def get_itinerary_conflict_with_after_to_payment(self) -> dict:
         # 1. 图像识别方式检测是否出现行程冲突小弹框
         try:
             file_name = join_path([get_images_dir(), "订单详情_行程冲突.png"])
             if is_exists(file_name):
-                pos = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
                 if pos:
                     logger.warning("图像识别方式检测到有小弹框【行程冲突】，需要点击【继续支付】")
                     return {"pos": pos}
         except (Exception,):
             pass
         # 2. 元素定位方式检测是否出现行程冲突小弹框
         try:
```

### Comparing `ctrip-app-ui-0.5.4/capp_ui/fee.py` & `ctrip-app-ui-0.5.5/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/libs.py` & `ctrip-app-ui-0.5.5/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.5.5/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/platforms.py` & `ctrip-app-ui-0.5.5/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/test.py` & `ctrip-app-ui-0.5.5/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/utils.py` & `ctrip-app-ui-0.5.5/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/capp_ui/validators.py` & `ctrip-app-ui-0.5.5/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.4/setup.py` & `ctrip-app-ui-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.5.4',
+    version='0.5.5',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

