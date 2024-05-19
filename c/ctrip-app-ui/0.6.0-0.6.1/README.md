# Comparing `tmp/ctrip-app-ui-0.6.0.tar.gz` & `tmp/ctrip-app-ui-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.0.tar", last modified: Sun May 19 04:15:53 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.1.tar", last modified: Sun May 19 05:32:46 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.0.tar` & `ctrip-app-ui-0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.184237 ctrip-app-ui-0.6.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 04:15:53.182241 ctrip-app-ui-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.156339 ctrip-app-ui-0.6.0/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.0/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.0/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.0/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.0/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.0/capp_ui/dir.py
--rw-rw-rw-   0        0        0    49857 2024-05-19 04:15:24.000000 ctrip-app-ui-0.6.0/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.0/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.0/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.0/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.0/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.0/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.0/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.0/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.181244 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 04:15:53.184237 ctrip-app-ui-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 04:15:47.000000 ctrip-app-ui-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.664688 ctrip-app-ui-0.6.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 05:32:46.662693 ctrip-app-ui-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.634743 ctrip-app-ui-0.6.1/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.1/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.1/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.1/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.1/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.1/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    48501 2024-05-19 05:32:21.000000 ctrip-app-ui-0.6.1/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.1/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.1/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.1/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.1/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.1/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.1/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.1/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.661700 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 05:32:46.664688 ctrip-app-ui-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 05:32:30.000000 ctrip-app-ui-0.6.1/setup.py
```

### Comparing `ctrip-app-ui-0.6.0/LICENSE` & `ctrip-app-ui-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/config.py` & `ctrip-app-ui-0.6.1/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.1/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/device.py` & `ctrip-app-ui-0.6.1/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/dir.py` & `ctrip-app-ui-0.6.1/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.1/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,67 +785,37 @@
             if safe_cash.exists() is True:
                 # logger.warning("元素定位方式检测到页面已经进入安全收银台")
                 return {"element": safe_cash}
         except (Exception,):
             pass
         return dict()
 
-    @LoopExcute(action="检测是否出现支付小弹框", loop=20, sleep=1)
-    def select_more_payment(self) -> bool:
-        """
-        当【同意并支付】后，特殊情况下，会出现支付小弹框，这个时候需要先判断是否存在小框，如果存在，则切换到通用支付选择界面
-        """
-        # 1. 检测到小弹框， 图像识别定位特征是：【更多付款方式】
+    def get_preferential_popup(self) -> dict:
+        # 1. 检测到小弹框， 图像识别定位特征是：【关闭】
         try:
-            file_name = join_path([get_images_dir(), "更多付款方式.png"])
+            file_name = join_path([get_images_dir(), "安全收银台_优惠关闭.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
-                if temp:
-                    logger.warning("图像识别方式检测到有小弹框，需要点击【更多付款方式】")
-                    self.device.touch(v=temp)
-                    time.sleep(1)
-                    temp_inner = self.device.get_cv_template(file_name=file_name)
-                    if not temp_inner:
-                        time.sleep(1)
-                        return True
+                pos = self.device.exists(v=temp)
+                if pos:
+                    logger.warning("图像识别方式检测到页面弹出优惠小窗口，点击【关闭】")
+                    return {"pos": pos}
         except (Exception,):
             pass
-        # 2. 检测是否到了安全收银台，安全收银台的定位特征是：【安全收银台】|【银行卡支付】
+        # 2. 检测到小弹框， 元素定位方式特征是：【安全收银台】
         try:
-            safe_cash = self.device.get_po(
-                type="android.widget.TextView", name="android.widget.TextView", text="安全收银台"
+            preferential_popup = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text="关闭"
             )
-            if safe_cash.exists() is True:
-                time.sleep(1)
-                return True
-        except (Exception,):
-            pass
-        try:
-            bank_card_payment = self.device.get_po(
-                type="android.widget.TextView", name="android.widget.TextView", text="银行卡支付"
-            )
-            if bank_card_payment.exists() is True:
-                time.sleep(1)
-                return True
+            if preferential_popup.exists() is True:
+                logger.warning("元素定位方式检测到页面弹出优惠小窗口，点击【关闭】")
+                return {"element": preferential_popup}
         except (Exception,):
             pass
-        # 3. 检测到小弹框， 定位特征是：【更多付款方式】
-        try:
-            more_payment_type = self.device.get_po(
-                type="android.view.ViewGroup ", name="更多付款方式", desc="更多付款方式"
-            )
-            if more_payment_type.exists() is True:
-                logger.warning("元素定位方式检测到有小弹框，需要点击【更多付款方式】")
-                more_payment_type.click()
-                time.sleep(1)
-                return True
-        except (Exception,):
-            pass
-        time.sleep(1)
-        return False
+        return dict()
 
     def __get_wallet_element(self) -> UIObjectProxy:
         return self.device.get_po(
             type="android.widget.TextView", name="android.widget.TextView", textMatches=r'^钱包.*'
         )
 
     @SleepWait(wait_time=1)
```

### Comparing `ctrip-app-ui-0.6.0/capp_ui/fee.py` & `ctrip-app-ui-0.6.1/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/libs.py` & `ctrip-app-ui-0.6.1/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.1/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/platforms.py` & `ctrip-app-ui-0.6.1/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/test.py` & `ctrip-app-ui-0.6.1/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/utils.py` & `ctrip-app-ui-0.6.1/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/capp_ui/validators.py` & `ctrip-app-ui-0.6.1/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.0/setup.py` & `ctrip-app-ui-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.0',
+    version='0.6.1',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

