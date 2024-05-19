# Comparing `tmp/poium-1.5.1.tar.gz` & `tmp/poium-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poium-1.5.1.tar", max compression
+gzip compressed data, was "poium-1.5.2.tar", max compression
```

## Comparing `poium-1.5.1.tar` & `poium-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11565 2020-09-08 14:49:37.559569 poium-1.5.1/LICENSE
--rw-r--r--   0        0        0     1012 2024-04-15 10:26:56.400942 poium-1.5.1/poium/__init__.py
--rw-r--r--   0        0        0      243 2024-04-15 07:22:47.599517 poium-1.5.1/poium/base.py
--rw-r--r--   0        0        0    23173 2024-04-14 09:19:10.317901 poium-1.5.1/poium/base_page.py
--rw-r--r--   0        0        0       30 2022-05-28 07:23:50.479794 poium-1.5.1/poium/common/__init__.py
--rw-r--r--   0        0        0      282 2024-04-15 06:25:22.269094 poium-1.5.1/poium/common/assert_des.py
--rw-r--r--   0        0        0     1238 2023-03-05 15:19:00.769582 poium-1.5.1/poium/common/exceptions.py
--rw-r--r--   0        0        0     1898 2022-09-19 17:29:10.431905 poium-1.5.1/poium/common/keyboard.py
--rw-r--r--   0        0        0     2413 2022-05-30 16:02:04.689800 poium-1.5.1/poium/common/logging.py
--rw-r--r--   0        0        0     1201 2023-03-16 16:37:16.756829 poium-1.5.1/poium/common/selector.py
--rw-r--r--   0        0        0     1117 2024-04-14 09:36:16.327170 poium-1.5.1/poium/config.py
--rw-r--r--   0        0        0     7757 2022-05-11 16:46:59.563149 poium-1.5.1/poium/javascript.py
--rw-r--r--   0        0        0    16953 2022-09-20 16:25:40.779610 poium-1.5.1/poium/playwright.py
--rw-r--r--   0        0        0    21450 2024-04-15 10:18:45.634722 poium-1.5.1/poium/u2/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-14 09:47:11.370698 poium-1.5.1/poium/u2/driver.py
--rw-r--r--   0        0        0    24220 2024-04-15 10:17:02.276331 poium-1.5.1/poium/wda/__init__.py
--rw-r--r--   0        0        0      638 2024-04-14 09:46:59.188354 poium-1.5.1/poium/wda/driver.py
--rw-r--r--   0        0        0    10000 2024-04-15 07:20:38.329332 poium-1.5.1/poium/webdriver.py
--rw-r--r--   0        0        0     1086 2024-04-15 10:26:46.807821 poium-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     5728 2024-04-15 09:41:48.438155 poium-1.5.1/README.md
--rw-r--r--   0        0        0     6768 1970-01-01 00:00:00.000000 poium-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11565 2020-09-08 14:49:37.559569 poium-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1012 2024-05-19 12:48:50.040866 poium-1.5.2/poium/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-15 07:22:47.599517 poium-1.5.2/poium/base.py
+-rw-r--r--   0        0        0    23062 2024-05-19 12:48:50.040866 poium-1.5.2/poium/base_page.py
+-rw-r--r--   0        0        0       30 2022-05-28 07:23:50.479794 poium-1.5.2/poium/common/__init__.py
+-rw-r--r--   0        0        0      282 2024-04-15 06:25:22.269094 poium-1.5.2/poium/common/assert_des.py
+-rw-r--r--   0        0        0     1238 2023-03-05 15:19:00.769582 poium-1.5.2/poium/common/exceptions.py
+-rw-r--r--   0        0        0     1898 2022-09-19 17:29:10.431905 poium-1.5.2/poium/common/keyboard.py
+-rw-r--r--   0        0        0     2429 2024-05-19 12:48:50.041869 poium-1.5.2/poium/common/logging.py
+-rw-r--r--   0        0        0     1201 2023-03-16 16:37:16.756829 poium-1.5.2/poium/common/selector.py
+-rw-r--r--   0        0        0     1137 2024-05-19 12:48:50.042872 poium-1.5.2/poium/config.py
+-rw-r--r--   0        0        0     7757 2022-05-11 16:46:59.563149 poium-1.5.2/poium/javascript.py
+-rw-r--r--   0        0        0    16917 2024-05-19 12:48:50.043867 poium-1.5.2/poium/playwright.py
+-rw-r--r--   0        0        0    21450 2024-04-15 10:18:45.634722 poium-1.5.2/poium/u2/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-14 09:47:11.370698 poium-1.5.2/poium/u2/driver.py
+-rw-r--r--   0        0        0    24220 2024-04-15 10:17:02.276331 poium-1.5.2/poium/wda/__init__.py
+-rw-r--r--   0        0        0      638 2024-04-14 09:46:59.188354 poium-1.5.2/poium/wda/driver.py
+-rw-r--r--   0        0        0    10000 2024-04-15 07:20:38.329332 poium-1.5.2/poium/webdriver.py
+-rw-r--r--   0        0        0     1078 2024-05-19 12:48:50.044866 poium-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5968 2024-04-15 11:14:58.608286 poium-1.5.2/README.md
+-rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 poium-1.5.2/PKG-INFO
```

### Comparing `poium-1.5.1/LICENSE` & `poium-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/__init__.py` & `poium-1.5.2/poium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 from .base_page import Element, Elements
 from .config import Browser
 from .javascript import CSSElement
 from .webdriver import Page
 
 __author__ = "fnngj"
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
```

### Comparing `poium-1.5.1/poium/base_page.py` & `poium-1.5.2/poium/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,40 +125,40 @@
             self.by, self.value = selection_checker(selector)
         else:
             if not kwargs:
                 raise ValueError("Please specify a locator")
             if len(kwargs) > 1:
                 raise ValueError("Please specify only one locator")
             self.kwargs = kwargs
-            by, self.value = next(iter(kwargs.items()))
+            self.by, self.value = next(iter(kwargs.items()))
 
-            self.by = LOCATOR_LIST.get(by, None)
+            self.by = LOCATOR_LIST.get(self.by, None)
             if self.by is None:
                 raise FindElementTypesError("Element positioning of type '{}' is not supported.".format(self.by))
 
     def __get__(self, instance, owner):
         if instance is None:
             return None
 
-        Browser.driver = instance.driver
+        self.driver = instance.driver
         return self
 
     def __set__(self, instance, value):
         self.__get__(instance, instance.__class__)
         self.send_keys(value)
 
     @func_set_timeout(1)
-    def find_elements_timeout(self, key: str, value: str):
+    def find_elements_timeout(self, by: str, value: str):
         """
         set find element timeout.
-        :param key:
+        :param by:
         :param value:
         :return:
         """
-        return Browser.driver.find_elements(key, value)
+        return self.driver.find_elements(by, value)
 
     def find(self, by: str, value: str) -> list:
         """
         Find if the element exists.
         """
         for i in range(self.times):
             try:
@@ -178,44 +178,43 @@
 
         return elems
 
     def get_element_object(self, by: str = None, value: str = None):
         """
         Judge element positioning way, and returns the element.
         """
-        if by is None:
+        if by is None or value is None:
             by = self.by
-        if value is None:
             value = self.value
 
-        if by in BY_LIST:
-            elem = self.find(by, value)
-            if len(elem) == 0:
-                self.exist = False
-                return None
-            else:
-                self.exist = True
-                elem = Browser.driver.find_elements(by, value)[self.index]
-        else:
+        if by not in BY_LIST:
             raise FindElementTypesError("Please enter the correct targeting elements")
 
+        elems = self.find(by, value)
+        if len(elems) == 0:
+            self.exist = False
+            return None
+        else:
+            self.exist = True
+            elem = elems[self.index]
+
         if Browser.show is True:
             try:
                 style_red = 'arguments[0].style.border="2px solid #FF0000"'
                 style_blue = 'arguments[0].style.border="2px solid #00FF00"'
                 style_null = 'arguments[0].style.border=""'
 
                 for _ in range(2):
-                    Browser.driver.execute_script(style_red, elem)
+                    self.driver.execute_script(style_red, elem)
                     sleep(0.1)
-                    Browser.driver.execute_script(style_blue, elem)
+                    self.driver.execute_script(style_blue, elem)
                     sleep(0.1)
-                Browser.driver.execute_script(style_blue, elem)
+                self.driver.execute_script(style_blue, elem)
                 sleep(0.5)
-                Browser.driver.execute_script(style_null, elem)
+                self.driver.execute_script(style_null, elem)
             except WebDriverException:
                 pass
 
         return elem
 
     def is_exist(self) -> bool:
         """element is existed """
@@ -395,15 +394,15 @@
 
     def switch_to_frame(self) -> None:
         """
         selenium API
         Switches focus to the specified frame
         """
         elem = self.get_element_object()
-        Browser.driver.switch_to.frame(elem)
+        self.driver.switch_to.frame(elem)
         logging.info(f"✅ switch_to_frame().")
 
     def frame(self) -> None:
         """
         selenium API
         Switches focus to the specified frame
         """
@@ -411,68 +410,68 @@
 
     def move_to_element(self) -> None:
         """
         selenium API
         Moving the mouse to the middle of an element
         """
         elem = self.get_element_object()
-        ActionChains(Browser.driver).move_to_element(elem).perform()
+        ActionChains(self.driver).move_to_element(elem).perform()
         logging.info(f"✅ move_to_element().")
 
     def click_and_hold(self) -> None:
         """
         selenium API
         Holds down the left mouse button on an element.
         """
         elem = self.get_element_object()
-        ActionChains(Browser.driver).click_and_hold(elem).perform()
+        ActionChains(self.driver).click_and_hold(elem).perform()
         logging.info(f"✅ click_and_hold().")
 
     def double_click(self) -> None:
         """
         selenium API
         Holds down the left mouse button on an element.
         """
         elem = self.get_element_object()
-        ActionChains(Browser.driver).double_click(elem).perform()
+        ActionChains(self.driver).double_click(elem).perform()
         logging.info(f"✅ double_click().")
 
     def context_click(self) -> None:
         """
         selenium API
         Performs a context-click (right click) on an element.
         """
         elem = self.get_element_object()
-        ActionChains(Browser.driver).context_click(elem).perform()
+        ActionChains(self.driver).context_click(elem).perform()
         logging.info(f"✅ context_click().")
 
     def drag_and_drop_by_offset(self, x: int, y: int) -> None:
         """
         selenium API
         Holds down the left mouse button on the source element,
            then moves to the target offset and releases the mouse button.
         :param x: X offset to move to.
         :param y: Y offset to move to.
         """
         elem = self.get_element_object()
-        ActionChains(Browser.driver).drag_and_drop_by_offset(elem, xoffset=x, yoffset=y).perform()
+        ActionChains(self.driver).drag_and_drop_by_offset(elem, xoffset=x, yoffset=y).perform()
         logging.info(f"✅ drag_and_drop_by_offset('{x}', '{y}').")
 
     def refresh_element(self, timeout: int = 10) -> None:
         """
         selenium API
         Refreshes the current page, retrieve elements.
         """
         elem = self.get_element_object()
         for i in range(timeout):
             if elem is not None:
                 try:
                     elem
                 except StaleElementReferenceException:
-                    Browser.driver.refresh()
+                    self.driver.refresh()
                 else:
                     break
             else:
                 sleep(1)
         else:
             raise TimeoutError("stale element reference: element is not attached to the page document.")
```

### Comparing `poium-1.5.1/poium/common/exceptions.py` & `poium-1.5.2/poium/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/common/keyboard.py` & `poium-1.5.2/poium/common/keyboard.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/common/logging.py` & `poium-1.5.2/poium/common/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Logger:
 
     def __init__(self, level: str = "DEBUG", colorlog: bool = True):
         self.logger = logger
         self._colorlog = colorlog
-        self._console_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</> {file} <level>| {level} | {message}</level>"
+        self._console_format = "<green>{time:YYYY-MM-DD HH:mm:ss}</> {file} <level>| {thread.name} | {level} | {message}</level>"
         self._level = level
         self.set_level(self._colorlog, self._console_format, self._level)
 
     def set_level(self, colorlog: bool = True, format: str = None, level: str = "DEBUG"):
         if format is None:
             format = self._console_format
         logger.remove()
```

### Comparing `poium-1.5.1/poium/common/selector.py` & `poium-1.5.2/poium/common/selector.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/config.py` & `poium-1.5.2/poium/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 printLog = False
 
 
 class Browser:
     """
     web config
     """
-    # Default browser driver
+    # Default browser driver (abandon)
     driver = None
 
-    # Default playwright page driver
+    # Default playwright page driver (abandon)
     page = None
 
     # Adds a border to the action element of the operation
     show = True
 
 
 class App:
```

### Comparing `poium-1.5.1/poium/javascript.py` & `poium-1.5.2/poium/javascript.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/playwright.py` & `poium-1.5.2/poium/playwright.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import pathlib
 from poium.common import logging
-from poium.config import Browser
 
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Pattern,
@@ -73,26 +72,26 @@
         self.timeout = timeout
         self.force = force
         self.no_wait_after = no_wait_after
         self.trial = trial
 
     @property
     def find(self):
-        elem = Browser.page.locator(self.selector)
+        elem = self.driver.locator(self.selector)
         if self.desc == "":
             logging.info(f"✨ Find element.")
         else:
             logging.info(f"✨ Find element: {self.desc}.")
         return elem
 
     def __get__(self, instance, owner):
         if instance is None:
             return None
 
-        Browser.page = instance.page
+        self.driver = instance.page
         return self
 
     def __set__(self, instance, value):
         elem = self.__get__(instance, instance.__class__)
         elem.fill(value)
 
     def all_inner_texts(self) -> List[str]:
```

### Comparing `poium-1.5.1/poium/u2/__init__.py` & `poium-1.5.2/poium/u2/__init__.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/u2/driver.py` & `poium-1.5.2/poium/u2/driver.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/wda/__init__.py` & `poium-1.5.2/poium/wda/__init__.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/wda/driver.py` & `poium-1.5.2/poium/wda/driver.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/poium/webdriver.py` & `poium-1.5.2/poium/webdriver.py`

 * *Files identical despite different names*

### Comparing `poium-1.5.1/pyproject.toml` & `poium-1.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poium"
-version = "1.5.1"
+version = "1.5.2"
 description = "Page Objects design pattern test library."
 authors = ["fnngj <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 homepage = "https://seldomqa.github.io"
 repository = "https://github.com/SeldomQA/poium"
@@ -20,19 +20,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.11"
 Appium-Python-Client = "^3.1.0"
 loguru = "~0.6.0"
 func-timeout = "^4.3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
-name = "tsinghua"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
+name = "douban"
+url = "https://pypi.doubanio.com/simple"
```

### Comparing `poium-1.5.1/README.md` & `poium-1.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -213,15 +213,23 @@
         self.assertTitle("seldom_百度搜索")
 
 
 if __name__ == '__main__':
     seldom.main(browser='edge')
 ```
 
-### Star History
+## 微信（WeChat）
+
+> 欢迎添加微信，交流和反馈问题。
+
+<div style="display: flex;justify-content: space-between;width: 100%">
+    <p><img alt="微信" src="wechat.jpg" style="width: 200px;height: 100%" ></p>
+</div>
+
+## Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/poium&type=Date)
 
 ## Project History
 
 * [page-objects](https://github.com/eeaston/page-objects)
```

### Comparing `poium-1.5.1/PKG-INFO` & `poium-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 Metadata-Version: 2.1
 Name: poium
-Version: 1.5.1
+Version: 1.5.2
 Summary: Page Objects design pattern test library.
 Home-page: https://seldomqa.github.io
 License: Apache-2.0
 Keywords: selenium,appium,playwright
 Author: fnngj
 Author-email: fnngj@126.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: Appium-Python-Client (>=3.1.0,<4.0.0)
 Requires-Dist: func-timeout (>=4.3.5,<5.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Project-URL: Repository, https://github.com/SeldomQA/poium
@@ -244,15 +240,23 @@
         self.assertTitle("seldom_百度搜索")
 
 
 if __name__ == '__main__':
     seldom.main(browser='edge')
 ```
 
-### Star History
+## 微信（WeChat）
+
+> 欢迎添加微信，交流和反馈问题。
+
+<div style="display: flex;justify-content: space-between;width: 100%">
+    <p><img alt="微信" src="wechat.jpg" style="width: 200px;height: 100%" ></p>
+</div>
+
+## Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/poium&type=Date)
 
 ## Project History
 
 * [page-objects](https://github.com/eeaston/page-objects)
```

