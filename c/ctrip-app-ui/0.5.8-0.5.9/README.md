# Comparing `tmp/ctrip-app-ui-0.5.8.tar.gz` & `tmp/ctrip-app-ui-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.5.8.tar", last modified: Sun May 19 03:47:59 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.5.9.tar", last modified: Sun May 19 04:09:30 2024, max compression
```

## Comparing `ctrip-app-ui-0.5.8.tar` & `ctrip-app-ui-0.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 03:47:59.656175 ctrip-app-ui-0.5.8/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 03:47:59.654180 ctrip-app-ui-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 03:47:59.624260 ctrip-app-ui-0.5.8/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.8/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.8/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.8/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.8/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.8/capp_ui/dir.py
--rw-rw-rw-   0        0        0    49828 2024-05-19 03:46:26.000000 ctrip-app-ui-0.5.8/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.8/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.8/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.8/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.8/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.8/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.8/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.8/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 03:47:59.653183 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 03:47:59.000000 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 03:47:59.000000 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 03:47:59.000000 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 03:47:59.000000 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 03:47:59.000000 ctrip-app-ui-0.5.8/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 03:47:59.656175 ctrip-app-ui-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 03:46:38.000000 ctrip-app-ui-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.277544 ctrip-app-ui-0.5.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 04:09:30.276548 ctrip-app-ui-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.249646 ctrip-app-ui-0.5.9/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.9/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.9/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.9/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.9/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.9/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    49836 2024-05-19 04:08:52.000000 ctrip-app-ui-0.5.9/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.9/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.9/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.9/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.9/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.9/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.9/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.9/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.274553 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 04:09:30.277544 ctrip-app-ui-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 04:09:09.000000 ctrip-app-ui-0.5.9/setup.py
```

### Comparing `ctrip-app-ui-0.5.8/LICENSE` & `ctrip-app-ui-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/config.py` & `ctrip-app-ui-0.5.9/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/date_extend.py` & `ctrip-app-ui-0.5.9/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/device.py` & `ctrip-app-ui-0.5.9/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/dir.py` & `ctrip-app-ui-0.5.9/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/domain_service.py` & `ctrip-app-ui-0.5.9/capp_ui/domain_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,49 +745,49 @@
         # 1. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
         try:
             file_name = join_path([get_images_dir(), "更多付款方式.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
+                    # logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
                     return {"pos": pos}
         except (Exception,):
             pass
         # 2. 检测到小弹框， 元素定位方式特征是：【更多付款方式】
         try:
             more_payment_type = self.device.get_po(
                 type="android.view.ViewGroup ", name="更多付款方式", desc="更多付款方式"
             )
             if more_payment_type.exists() is True:
-                logger.warning("元素定位方式检测到有小弹框，需要点击【更多付款方式】")
+                # logger.warning("元素定位方式检测到有小弹框，需要点击【更多付款方式】")
                 return {"element": more_payment_type}
         except (Exception,):
             pass
         return dict()
 
     def get_safe_cash(self) -> dict:
         # 1. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
         try:
             file_name = join_path([get_images_dir(), "安全收银台.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
                 if pos:
-                    logger.warning("图像识别方式检测到页面已经进入安全收银台")
+                    # logger.warning("图像识别方式检测到页面已经进入安全收银台")
                     return {"pos": pos}
         except (Exception,):
             pass
         # 2. 检测到小弹框， 元素定位方式特征是：【安全收银台】
         try:
             safe_cash = self.device.get_po(
                 type="android.widget.TextView", name="android.widget.TextView", text="安全收银台"
             )
             if safe_cash.exists() is True:
-                logger.warning("元素定位方式检测到页面已经进入安全收银台")
+                # logger.warning("元素定位方式检测到页面已经进入安全收银台")
                 return {"element": safe_cash}
         except (Exception,):
             pass
         return dict()
 
     @LoopExcute(action="检测是否出现支付小弹框", loop=20, sleep=1)
     def select_more_payment(self) -> bool:
```

### Comparing `ctrip-app-ui-0.5.8/capp_ui/fee.py` & `ctrip-app-ui-0.5.9/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/libs.py` & `ctrip-app-ui-0.5.9/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.5.9/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/platforms.py` & `ctrip-app-ui-0.5.9/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/test.py` & `ctrip-app-ui-0.5.9/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/utils.py` & `ctrip-app-ui-0.5.9/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/capp_ui/validators.py` & `ctrip-app-ui-0.5.9/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.8/setup.py` & `ctrip-app-ui-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.5.8',
+    version='0.5.9',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

