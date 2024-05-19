# Comparing `tmp/ctrip-app-ui-0.6.1.tar.gz` & `tmp/ctrip-app-ui-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.1.tar", last modified: Sun May 19 05:32:46 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.2.tar", last modified: Sun May 19 10:09:08 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.1.tar` & `ctrip-app-ui-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.664688 ctrip-app-ui-0.6.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 05:32:46.662693 ctrip-app-ui-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.634743 ctrip-app-ui-0.6.1/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.1/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.1/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.1/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.1/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.1/capp_ui/dir.py
--rw-rw-rw-   0        0        0    48501 2024-05-19 05:32:21.000000 ctrip-app-ui-0.6.1/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.1/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.1/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.1/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.1/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.1/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.1/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.1/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 05:32:46.661700 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 05:32:46.000000 ctrip-app-ui-0.6.1/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 05:32:46.664688 ctrip-app-ui-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 05:32:30.000000 ctrip-app-ui-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.959319 ctrip-app-ui-0.6.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:09:08.958337 ctrip-app-ui-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.931394 ctrip-app-ui-0.6.2/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.2/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.2/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.2/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.2/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.2/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    51478 2024-05-19 10:03:49.000000 ctrip-app-ui-0.6.2/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.2/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.2/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.2/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.2/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.2/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.2/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.2/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:09:08.956328 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 10:09:08.000000 ctrip-app-ui-0.6.2/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:09:08.960329 ctrip-app-ui-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 09:30:30.000000 ctrip-app-ui-0.6.2/setup.py
```

### Comparing `ctrip-app-ui-0.6.1/LICENSE` & `ctrip-app-ui-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/config.py` & `ctrip-app-ui-0.6.2/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.2/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/device.py` & `ctrip-app-ui-0.6.2/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/dir.py` & `ctrip-app-ui-0.6.2/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.2/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,26 @@
         self.device.poco = poco_poxy.poco
         self.device.get_po = poco_poxy.get_po
         self.device.get_po_extend = poco_poxy.get_po_extend
 
     def stop(self) -> None:
         stop_app(self.app_name, device_id=self.device.device_id)
 
-    def restart(self):
-        stop_app(self.app_name, device_id=self.device.device_id)
-        time.sleep(1.0)
-        self.device.start_app(self.app_name)
-        poco_poxy = PocoProxy()
-        self.device.poco = poco_poxy.poco
-        self.device.get_po = poco_poxy.get_po
-        self.device.get_po_extend = poco_poxy.get_po_extend
+    def restart(self) -> bool:
+        try:
+            stop_app(self.app_name, device_id=self.device.device_id)
+            time.sleep(1.0)
+            self.device.start_app(self.app_name)
+            poco_poxy = PocoProxy()
+            self.device.poco = poco_poxy.poco
+            self.device.get_po = poco_poxy.get_po
+            self.device.get_po_extend = poco_poxy.get_po_extend
+            return True
+        except (Exception,):
+            return False
 
     def hide_navigation_bar(self):
         """如果导航栏已打开，需要隐藏，导航栏很影响元素定位"""
         try:
             navigation_bar = self.device.get_po(
                 type="android.widget.ImageView", name="com.android.systemui:id/hide", desc="隐藏"
             )
@@ -254,20 +258,23 @@
             return True
         else:
             element.click()
             search_box = self.get_search_page_search_box()
             if not search_box:
                 return False
             element = search_box.get("element")
-            element.click()
-            element.set_text(ctrip_order_id)
-            # 模拟键盘按下回车键（keyCode为66表示回车键）
-            self.device.keyevent(keyname="66")
-            time.sleep(sleep)
-            return True
+            try:
+                element.click()
+                element.set_text(ctrip_order_id)
+                # 模拟键盘按下回车键（keyCode为66表示回车键）
+                self.device.keyevent(keyname="66")
+                time.sleep(sleep)
+                return True
+            except (Exception,):
+                return False
 
     def get_order_status_with_order_list(self) -> str:
         """检查搜索列表界面，获取订单的状态"""
         try:
             file_name = join_path([get_images_dir(), "订单状态_待支付.png"])
             if is_exists(file_name):
                 temp = self.device.get_cv_template(file_name=file_name, threshold=0.9)
@@ -468,28 +475,91 @@
             else:
                 string = "从元素的文案<{}>提取时间与金额信息有异常".format(text)
         else:
             string = "元素定位存在异常，订单详情页没有找到订单支付金额和过期时间"
         logger.warning(string)
         return flag, remark
 
-    @LoopFindElementSubmit(loop=1, action="取消订单")
-    def touch_cancel_order(self):
-        cancel_order = self.device.poco(
-            type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
-        )
-        cancel_order.click()
+    @LoopFindElementObject(action="订单详情页查找【取消订单】按钮", loop=20, sleep=1)
+    def get_cancel_order_with_order_detail(self) -> dict:
+        try:
+            file_name = join_path([get_images_dir(), "订单详情_取消订单.png"])
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
+            cancel_order = self.device.poco(
+                type="android.widget.TextView", name="operateBtnList_Text_取消订单", text="取消订单"
+            )
+            if cancel_order.exists() is True:
+                return {"element": cancel_order}
+        except (Exception,):
+            pass
+        try:
+            cancel_order = self.device.poco(
+                type="android.view.ViewGroup", name="operateBtnList_TouchableOpacity_button",
+                desc="operateBtnList_TouchableOpacity_button"
+            )
+            if cancel_order.exists() is True:
+                return {"element": cancel_order}
+        except (Exception,):
+            pass
+        return dict()
 
-    @LoopFindElementSubmit(loop=1, action="确认取消订单")
-    def touch_submit_cancel_order(self):
-        """再次确认是否要取消订单"""
-        submit_cancel_order = self.device.poco(
-            type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
-        )
-        submit_cancel_order.click()
+    @LoopFindElementObject(action="取消订单确认小弹框查找【取消订单】按钮", loop=20, sleep=1)
+    def get_submit_cancel_order(self):
+        try:
+            file_name = join_path([get_images_dir(), "取消订单弹框_取消订单.png"])
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
+            cancel_order = self.device.poco(
+                type="android.widget.TextView", name="Button_Text_取消订单", text="取消订单"
+            )
+            if cancel_order.exists() is True:
+                return {"element": cancel_order}
+        except (Exception,):
+            pass
+        return dict()
+
+    @LoopFindElementObject(action="申请取消订单查找【申请退款】按钮", loop=20, sleep=1)
+    def get_cancel_order_with_pay_refund(self) -> dict:
+        try:
+            file_name = join_path([get_images_dir(), "取消订单弹框_申请退票.png"])
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
+            pay_refund = self.device.poco(
+                type="android.widget.TextView", name="NewCancelOrderLayer_Text_申请退票", text="申请退票"
+            )
+            if pay_refund.exists() is True:
+                return {"element": pay_refund}
+        except (Exception,):
+            pass
+        return dict()
 
     @LoopFindElementSubmit(loop=1, action="知道了")
     def touch_know_the_cancel_order(self):
         """确认取消后，会有一个【知道了】的小弹框"""
         submit_cancel_order = self.device.poco(
             type="android.widget.TextView", name="Button_Text_知道了", text="知道了"
         )
```

### Comparing `ctrip-app-ui-0.6.1/capp_ui/fee.py` & `ctrip-app-ui-0.6.2/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/libs.py` & `ctrip-app-ui-0.6.2/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.2/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/platforms.py` & `ctrip-app-ui-0.6.2/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/test.py` & `ctrip-app-ui-0.6.2/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/utils.py` & `ctrip-app-ui-0.6.2/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/capp_ui/validators.py` & `ctrip-app-ui-0.6.2/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.1/setup.py` & `ctrip-app-ui-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.1',
+    version='0.6.2',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

