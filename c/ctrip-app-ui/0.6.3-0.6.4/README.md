# Comparing `tmp/ctrip-app-ui-0.6.3.tar.gz` & `tmp/ctrip-app-ui-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.6.3.tar", last modified: Sun May 19 10:29:23 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.4.tar", last modified: Sun May 19 10:55:51 2024, max compression
```

## Comparing `ctrip-app-ui-0.6.3.tar` & `ctrip-app-ui-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.946246 ctrip-app-ui-0.6.3/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.3/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 10:29:23.944252 ctrip-app-ui-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.916325 ctrip-app-ui-0.6.3/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.3/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.3/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.3/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.3/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.3/capp_ui/dir.py
--rw-rw-rw-   0        0        0    52175 2024-05-19 10:28:51.000000 ctrip-app-ui-0.6.3/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.3/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.3/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.3/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.3/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.3/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.3/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.3/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:29:23.943255 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 10:29:23.000000 ctrip-app-ui-0.6.3/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:29:23.946246 ctrip-app-ui-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 10:29:17.000000 ctrip-app-ui-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.527949 ctrip-app-ui-0.6.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:55:51.526951 ctrip-app-ui-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.500051 ctrip-app-ui-0.6.4/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.4/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.4/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.4/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.4/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.4/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    52875 2024-05-19 10:50:18.000000 ctrip-app-ui-0.6.4/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.4/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.4/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.4/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.4/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.4/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.4/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.4/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:55:51.524957 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 10:55:51.000000 ctrip-app-ui-0.6.4/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:55:51.527949 ctrip-app-ui-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 10:55:46.000000 ctrip-app-ui-0.6.4/setup.py
```

### Comparing `ctrip-app-ui-0.6.3/LICENSE` & `ctrip-app-ui-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/config.py` & `ctrip-app-ui-0.6.4/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.4/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/device.py` & `ctrip-app-ui-0.6.4/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/dir.py` & `ctrip-app-ui-0.6.4/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.4/capp_ui/domain_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -927,28 +927,33 @@
                     logger.warning("提取钱包余额<{}>有异常，钱包为不可用状态，将选择银行卡支付".format(text))
             else:
                 logger.info("账户钱包被隐藏了，不能操作钱包.")
         except (PocoNoSuchNodeException, Exception):
             logger.warning("安全收银台界面，没有出现钱包的选择入口.")
         return flag, amount
 
-    @SleepWait(wait_time=1)
     def touch_wallet_payment(self) -> None:
-        wallet = self.__get_wallet_element()
-        wallet.click()
+        try:
+            wallet = self.__get_wallet_element()
+            wallet.click()
+            time.sleep(1)
+        except (Exception,):
+            pass
 
-    @SleepWait(wait_time=1)
     def select_gift_card(self, payment_method: str) -> None:
         """选择对应的礼品卡"""
-        gift_card = self.device.get_po(
-            type="android.widget.TextView", name="android.widget.TextView", text=payment_method
-        )
-        gift_card.click()
+        try:
+            gift_card = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text=payment_method
+            )
+            gift_card.click()
+            time.sleep(1)
+        except (Exception,):
+            pass
 
-    @SleepWait(wait_time=1)
     def get_gift_card_deduction_amount(self) -> str:
         """获取礼品卡抵扣金额"""
         value = ""
         try:
             gift_card = self.device.get_po(
                 type="android.widget.TextView", name="android.widget.TextView", textMatches=r"^使用.*"
             )
@@ -960,21 +965,24 @@
                 # logger.warning("当前礼品卡抵扣金额为：{}".format(value))
             else:
                 logger.warning("获取到的礼品卡抵扣金额文案未：{}".format(text_value))
         except (Exception,):
             logger.error("获取礼品卡抵扣金额出现异常")
         return value
 
-    @SleepWait(wait_time=1)
     def touch_wallet_immediate_payment(self) -> None:
         """选择对应的礼品卡，点击【使用钱包全额抵扣，立即支付】"""
-        wallet_immediate_payment = self.device.get_po(
-            type="android.widget.TextView", name="android.widget.TextView", text="使用钱包全额抵扣，立即支付"
-        )
-        wallet_immediate_payment.click()
+        try:
+            wallet_immediate_payment = self.device.get_po(
+                type="android.widget.TextView", name="android.widget.TextView", text="使用钱包全额抵扣，立即支付"
+            )
+            wallet_immediate_payment.click()
+            time.sleep(1)
+        except (Exception,):
+            pass
 
     @SleepWait(wait_time=1)
     def select_point_deduction(self) -> None:
         """
         支付界面，选择【积分抵扣】，这里的逻辑是，如果已经选中，再点击积分抵扣，就会变成取消抵扣
         """
         default_text = "100积分抵扣1元"
@@ -1001,61 +1009,72 @@
                     poco.click()
                     logger.info("积分抵扣已经选中，接下来将进行支付操作.")
             except (PocoNoSuchNodeException, Exception):
                 logger.warning("既没有找到默认的积分抵扣选项，也没有找到已选中的积分抵扣.")
         else:
             logger.info("积分抵扣已经选中，接下来将进行支付操作.")
 
-    @SleepWait(wait_time=1)
     def touch_bank_card_payment(self) -> None:
         """
         支付界面，选择【银行卡支付】
         """
-        point_deduction = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            text="银行卡支付",
-            global_num=0,
-            local_num=1,
-            touchable=False,
-        )[0]
-        point_deduction.click()
+        try:
+            point_deduction = self.device.get_po_extend(
+                type="android.widget.TextView",
+                name="android.widget.TextView",
+                text="银行卡支付",
+                global_num=0,
+                local_num=1,
+                touchable=False,
+            )[0]
+            point_deduction.click()
+            time.sleep(1)
+        except (Exception,):
+            pass
 
     def get_ticket_actual_amount(self) -> Decimal:
         """
         确定使用积分抵扣后，票据的实际支付金额
         """
-        ticket_actual_amount = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            textMatches_inner=r"^¥\d+.\d*",
-            global_num=0,
-            local_num=2,
-            touchable=False,
-        )[0]
-        actual_amount = ticket_actual_amount.get_text()
-        actual_amount = Decimal(actual_amount[1:]) if isinstance(
-            actual_amount, str) else 9999999999.9999999999
+        actual_amount = Decimal("9999999999.9999999999")
+        try:
+            ticket_actual_amount = self.device.get_po_extend(
+                type="android.widget.TextView",
+                name="android.widget.TextView",
+                textMatches_inner=r"^¥\d+.\d*",
+                global_num=0,
+                local_num=2,
+                touchable=False,
+            )[0]
+            actual_amount = ticket_actual_amount.get_text()
+            actual_amount = Decimal(actual_amount[1:]) if actual_amount and isinstance(
+                actual_amount, str) else Decimal("9999999999.9999999999")
+        except (Exception,):
+            pass
         return actual_amount
 
     def get_ticket_deduction_amount(self) -> Decimal:
         """
         使用积分抵扣的金额
         """
-        tickect_deduction_amount = self.device.get_po_extend(
-            type="android.widget.TextView",
-            name="android.widget.TextView",
-            textMatches_inner=r"^-¥\d+.\d*",
-            global_num=0,
-            local_num=4,
-            touchable=False,
-        )[0]
-        deduction_amount = tickect_deduction_amount.get_text()
-        deduction_amount = Decimal(deduction_amount[2:]) if isinstance(deduction_amount,
-                                                                       str) else -9999999999.9999999999
+        deduction_amount = Decimal("-9999999999.9999999999")
+        try:
+            tickect_deduction_amount = self.device.get_po_extend(
+                type="android.widget.TextView",
+                name="android.widget.TextView",
+                textMatches_inner=r"^-¥\d+.\d*",
+                global_num=0,
+                local_num=4,
+                touchable=False,
+            )[0]
+            deduction_amount = tickect_deduction_amount.get_text()
+            deduction_amount = Decimal(deduction_amount[2:]) if deduction_amount and isinstance(
+                deduction_amount, str) else Decimal("-9999999999.9999999999")
+        except (Exception,):
+            pass
         return deduction_amount
 
     @SleepWait(wait_time=8)
     def enter_payment_pass(self, payment_pass: str, device_id: str, enable_debug: bool = False, port: int = 0,
                            platform: str = "Android") -> None:
         """
         请输入支付密码
@@ -1073,18 +1092,21 @@
                 raise ValueError("文件<{}>缺失...", format(file_name))
 
     @SleepWait(wait_time=8)
     def enter_payment_pass_by_position(self, payment_pass: str) -> None:
         """
         请输入支付密码
         """
-        payment_pass = payment_pass if isinstance(payment_pass, str) else str(payment_pass)
-        for char in payment_pass:
-            char_position = ctrip_soft_keyboard_position.get(char)
-            self.device.touch(v=char_position)
+        try:
+            payment_pass = payment_pass if isinstance(payment_pass, str) else str(payment_pass)
+            for char in payment_pass:
+                char_position = ctrip_soft_keyboard_position.get(char)
+                self.device.touch(v=char_position)
+        except (Exception,):
+            pass
 
     @SleepWait(wait_time=1)
     def is_balance(self, payment_card: str) -> bool:
         """
         判断是否出现余额不足的小弹框
         """
         flag = False
```

### Comparing `ctrip-app-ui-0.6.3/capp_ui/fee.py` & `ctrip-app-ui-0.6.4/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/libs.py` & `ctrip-app-ui-0.6.4/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.4/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/platforms.py` & `ctrip-app-ui-0.6.4/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/test.py` & `ctrip-app-ui-0.6.4/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/utils.py` & `ctrip-app-ui-0.6.4/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/capp_ui/validators.py` & `ctrip-app-ui-0.6.4/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.6.3/setup.py` & `ctrip-app-ui-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.6.3',
+    version='0.6.4',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

