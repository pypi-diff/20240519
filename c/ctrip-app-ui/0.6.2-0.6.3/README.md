# Comparing `tmp/ctrip-app-ui-0.6.2.tar.gz` & `tmp/ctrip-app-ui-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.2.tar", last modified: Sun May 19 10:09:08 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.3.tar", last modified: Sun May 19 10:29:23 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.2.tar` & `ctrip-app-ui-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.959319 ctrip-app-ui-0.6.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 10:09:08.958337 ctrip-app-ui-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.931394 ctrip-app-ui-0.6.2/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.2/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.2/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.2/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.2/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.2/capp_ui/dir.py
--rw-rw-rw-   0        0        0    51478 2024-05-19 10:03:49.000000 ctrip-app-ui-0.6.2/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.2/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.2/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.2/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.2/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.2/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.2/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.2/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.956328 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:09:08.960329 ctrip-app-ui-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 09:30:30.000000 ctrip-app-ui-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.946246 ctrip-app-ui-0.6.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:29:23.944252 ctrip-app-ui-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.916325 ctrip-app-ui-0.6.3/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.3/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.3/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.3/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.3/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.3/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    52175 2024-05-19 10:28:51.000000 ctrip-app-ui-0.6.3/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.3/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.3/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.3/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.3/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.3/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.3/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.3/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.943255 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:29:23.946246 ctrip-app-ui-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 10:29:17.000000 ctrip-app-ui-0.6.3/setup.py
```

### Comparing `ctrip-app-ui-0.6.2/LICENSE` & `ctrip-app-ui-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/config.py` & `ctrip-app-ui-0.6.3/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.3/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/device.py` & `ctrip-app-ui-0.6.3/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/dir.py` & `ctrip-app-ui-0.6.3/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.3/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,21 +553,37 @@
             )
             if pay_refund.exists() is True:
                 return {"element": pay_refund}
         except (Exception,):
             pass
         return dict()
 
-    @LoopFindElementSubmit(loop=1, action="知道了")
-    def touch_know_the_cancel_order(self):
+    @LoopFindElementObject(action="申请取消订单查找【知道了】按钮", loop=20, sleep=1)
+    def get_know_the_cancel_order(self):
         """确认取消后，会有一个【知道了】的小弹框"""
-        submit_cancel_order = self.device.poco(
-            type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
-        )
-        submit_cancel_order.click()
+        try:
+            file_name = join_path([get_images_dir(), "订单取消_知道了.png"])
+            if is_exists(file_name):
+                temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
+                pos = self.device.exists(v=temp)
+                if pos:
+                    return {"pos": pos}
+            else:
+                logger.warning("文件{}，没找到".format(file_name))
+        except (Exception,):
+            pass
+        try:
+            submit_cancel_order = self.device.poco(
+                type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
+            )
+            if submit_cancel_order.exists() is True:
+                return {"element": submit_cancel_order}
+        except (Exception,):
+            pass
+        return dict()
 
     def get_order_detail_page_order_state(self) -> str:
         try:
             file_name = join_path([get_images_dir(), "订单详情.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
                 pos = self.device.exists(v=temp)
```

### Comparing `ctrip-app-ui-0.6.2/capp_ui/fee.py` & `ctrip-app-ui-0.6.3/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/libs.py` & `ctrip-app-ui-0.6.3/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.3/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/platforms.py` & `ctrip-app-ui-0.6.3/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/test.py` & `ctrip-app-ui-0.6.3/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/utils.py` & `ctrip-app-ui-0.6.3/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/capp_ui/validators.py` & `ctrip-app-ui-0.6.3/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.2/setup.py` & `ctrip-app-ui-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.2',
+    version='0.6.3',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

