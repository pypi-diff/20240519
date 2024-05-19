# Comparing `tmp/ctrip-app-ui-0.5.9.tar.gz` & `tmp/ctrip-app-ui-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.5.9.tar", last modified: Sun May 19 04:09:30 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.6.0.tar", last modified: Sun May 19 04:15:53 2024, max compression
```

## Comparing `ctrip-app-ui-0.5.9.tar` & `ctrip-app-ui-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.277544 ctrip-app-ui-0.5.9/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-19 04:09:30.276548 ctrip-app-ui-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.249646 ctrip-app-ui-0.5.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.9/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    49836 2024-05-19 04:08:52.000000 ctrip-app-ui-0.5.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-19 04:09:30.274553 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 04:09:30.000000 ctrip-app-ui-0.5.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 04:09:30.277544 ctrip-app-ui-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-19 04:09:09.000000 ctrip-app-ui-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.184237 ctrip-app-ui-0.6.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-19 04:15:53.182241 ctrip-app-ui-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.156339 ctrip-app-ui-0.6.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.6.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.6.0/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.6.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.6.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.6.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    49857 2024-05-19 04:15:24.000000 ctrip-app-ui-0.6.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.6.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.6.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.6.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.6.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.6.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.6.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.6.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-19 04:15:53.181244 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 04:15:52.000000 ctrip-app-ui-0.6.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 04:15:53.184237 ctrip-app-ui-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-19 04:15:47.000000 ctrip-app-ui-0.6.0/setup.py
```

### Comparing `ctrip-app-ui-0.5.9/LICENSE` & `ctrip-app-ui-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/config.py` & `ctrip-app-ui-0.6.0/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.6.0/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/device.py` & `ctrip-app-ui-0.6.0/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/dir.py` & `ctrip-app-ui-0.6.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.6.0/capp_ui/domain_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
             if amount_text.exists() is True:
                 return {"element": amount_text}
         except (Exception,):
             pass
         return dict()
 
     def is_cancel_order(self, out_total_price: str, amount_loss_limit: str, profit_cap: str, passenger_number: int,
-                        discount_amount: str = None) -> tuple:
+                        platform: str, discount_amount: str = None) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
         flag = False
         remark = None
         attr = self.get_order_amount_with_order_detail()
         amount_text = attr.get("element")
         if amount_text:
             text = amount_text.get_text()
@@ -435,15 +435,15 @@
                 is_later = is_later_than_current_time(time_str=time_str, minutes=minutes)
                 if is_later is False:
                     flag = True
                     remark = "支付时间少于{}分钟".format(minutes)
                     string = string + "，" + remark
                 else:
                     amount_str = amount_match.group(1)
-                    string = "从携程订单获取的支付金额：{}，劲旅订单总价：{}".format(amount_str, out_total_price)
+                    string = "从{}订单获取的支付金额：{}，劲旅订单总价：{}".format(platform, amount_str, out_total_price)
                     # 预期订单利润
                     ex_order_profit = Decimal(out_total_price) - Decimal(amount_str)
                     if discount_amount:
                         # 实际订单利润
                         ac_order_profit = ex_order_profit + Decimal(discount_amount)
                     else:
                         ac_order_profit = ex_order_profit
```

### Comparing `ctrip-app-ui-0.5.9/capp_ui/fee.py` & `ctrip-app-ui-0.6.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/libs.py` & `ctrip-app-ui-0.6.0/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.6.0/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/platforms.py` & `ctrip-app-ui-0.6.0/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/test.py` & `ctrip-app-ui-0.6.0/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/utils.py` & `ctrip-app-ui-0.6.0/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/capp_ui/validators.py` & `ctrip-app-ui-0.6.0/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.5.9/setup.py` & `ctrip-app-ui-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.5.9',
+    version='0.6.0',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

