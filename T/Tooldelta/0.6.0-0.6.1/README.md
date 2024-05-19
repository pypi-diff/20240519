# Comparing `tmp/tooldelta-0.6.0.tar.gz` & `tmp/tooldelta-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.6.0.tar", max compression
+gzip compressed data, was "tooldelta-0.6.1.tar", max compression
```

## Comparing `tooldelta-0.6.0.tar` & `tooldelta-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-05-05 15:13:40.927657 tooldelta-0.6.0/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-05-05 15:13:40.927657 tooldelta-0.6.0/README.md
--rw-r--r--   0        0        0      891 2024-05-05 15:13:50.547635 tooldelta-0.6.0/pyproject.toml
--rwxr-xr-x   0        0        0      618 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/auths.py
--rwxr-xr-x   0        0        0    12372 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/color_print.py
--rw-r--r--   0        0        0     1885 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/constants.py
--rwxr-xr-x   0        0        0    34694 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/frame.py
--rwxr-xr-x   0        0        0    13149 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    23741 2024-05-05 15:13:40.927657 tooldelta-0.6.0/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1832 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/logger.py
--rw-r--r--   0        0        0    29752 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1295 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/packets.py
--rwxr-xr-x   0        0        0    16965 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7792 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0     9975 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     6318 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/movent.py
--rw-r--r--   0        0        0     7025 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_load/utils.py
--rwxr-xr-x   0        0        0    17005 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16754 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1932 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/starter.py
--rwxr-xr-x   0        0        0     1110 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9215 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/urlmethod.py
--rw-r--r--   0        0        0    20711 2024-05-05 15:13:40.931657 tooldelta-0.6.0/tooldelta/utils.py
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 tooldelta-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-05-19 08:25:37.225191 tooldelta-0.6.1/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-05-19 08:25:37.225191 tooldelta-0.6.1/README.md
+-rw-r--r--   0        0        0      891 2024-05-19 08:25:50.897200 tooldelta-0.6.1/pyproject.toml
+-rwxr-xr-x   0        0        0      618 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12372 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10441 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    34764 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13149 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23814 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    17541 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7821 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0    10499 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7025 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17005 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16754 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1996 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0    10039 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20711 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/utils.py
+-rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 tooldelta-0.6.1/PKG-INFO
```

### Comparing `tooldelta-0.6.0/LICENSE` & `tooldelta-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/README.md` & `tooldelta-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/pyproject.toml` & `tooldelta-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.6.0" # This field is automatically set to the value in the version file
+version = "0.6.1" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.6.0/tooldelta/__init__.py` & `tooldelta-0.6.1/tooldelta/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/auths.py` & `tooldelta-0.6.1/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/cfg.py` & `tooldelta-0.6.1/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/color_print.py` & `tooldelta-0.6.1/tooldelta/color_print.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 "支持mc颜色代码的输出模块"
 
 import datetime
 import threading
 import colorama
+from .logger import publicLogger
 
 colorama.init(autoreset=True)
 
-try:
-    from .logger import publicLogger
-except ImportError:
-    pass
-
-unicode = type("")
-
-
 def simple_fmt(kw: dict, arg: str) -> str:
     """简单的字符串格式化
 
     Args:
         kw (dict): 颜色列表（key为颜色代码，value为颜色代码对应的颜色）
         arg (str): 需要格式化的字符串
 
@@ -25,19 +18,17 @@
         str: 格式化后的字符串
     """
     for k, v in kw.items():
         arg = arg.replace(k, str(v))
     return arg
 
 
-class _Print:
-    """输出状态栏
-
-    Raises:
-        AssertionError: 无法找到对应的颜色代码
+class Print:
+    """
+    生成多样彩色输出的类
     """
     INFO_NORMAL = "§f 信息 "
     INFO_WARN = "§6 警告 "
     INFO_ERROR = "§4 报错 "
     INFO_FAIL = "§c 失败 "
     INFO_SUCC = "§a 成功 "
     INFO_LOAD = "§d 加载 "
@@ -58,76 +49,69 @@
         ["d", "#FF55FF"],
         ["e", "#FFFF55"],
         ["f", "#FFFFFF"],
         ["g", "#DDD605"],
         ["r", "/"],
     ]
 
-    def __init__(self) -> None:
-        "初始化"
-        self.lock = threading.RLock()
-
-    def __call__(self, text: str) -> None:
-        "输出信息"
-        with self.lock:
-            self.print_inf(text)
+    lock = threading.RLock()
 
-    def simple_fmt(self, kw: dict, arg: str) -> str:
+    @staticmethod
+    def simple_fmt(kw: dict, arg: str) -> str:
         """简单的字符串格式化
 
         Args:
             kw (dict): 颜色列表（key为颜色代码，value为颜色代码对应的颜色）
             arg (str): 需要格式化的字符串
 
         Returns:
             str: 格式化后的字符串
         """
 
-        with self.lock:
-            return simple_fmt(kw, arg)
+        return simple_fmt(kw, arg)
 
-    def colormode_replace(self, text: str, showmode=0) -> str:
+    @staticmethod
+    def colormode_replace(text: str, showmode=0) -> str:
         """颜色代码替换
 
         Args:
             text (str): 需要替换的字符串
             showmode (int, optional): 显示模式
 
         Returns:
             str: 替换后的字符串
         """
-        with self.lock:
             # 1 = bg_color
-            text = self._strike(text)
-            return (
-                simple_fmt(
-                    {
-                        "§1": f"\033[{showmode};37;34m",
-                        "§2": f"\033[{showmode};37;32m",
-                        "§3": f"\033[{showmode};37;36m",
-                        "§4": f"\033[{showmode};37;31m",
-                        "§5": f"\033[{showmode};37;35m",
-                        "§6": f"\033[{showmode};37;33m",
-                        "§7": f"\033[{showmode};37;90m",
-                        "§8": f"\033[{showmode};37;2m",
-                        "§9": f"\033[{showmode};37;94m",
-                        "§a": f"\033[{showmode};37;92m",
-                        "§b": f"\033[{showmode};37;96m",
-                        "§c": f"\033[{showmode};37;91m",
-                        "§d": f"\033[{showmode};37;95m",
-                        "§e": f"\033[{showmode};37;93m",
-                        "§f": f"\033[{showmode};37;1m",
-                        "§r": "\033[0m",
-                        "§u": "\033[4m",
-                        "§l": "\033[1m",
-                    },
-                    text,
-                )
-                + "\033[0m"
+        text = Print._strike(text)
+        return (
+            simple_fmt(
+                {
+                    "§1": f"\033[{showmode};37;34m",
+                    "§2": f"\033[{showmode};37;32m",
+                    "§3": f"\033[{showmode};37;36m",
+                    "§4": f"\033[{showmode};37;31m",
+                    "§5": f"\033[{showmode};37;35m",
+                    "§6": f"\033[{showmode};37;33m",
+                    "§7": f"\033[{showmode};37;90m",
+                    "§8": f"\033[{showmode};37;2m",
+                    "§9": f"\033[{showmode};37;94m",
+                    "§a": f"\033[{showmode};37;92m",
+                    "§b": f"\033[{showmode};37;96m",
+                    "§c": f"\033[{showmode};37;91m",
+                    "§d": f"\033[{showmode};37;95m",
+                    "§e": f"\033[{showmode};37;93m",
+                    "§f": f"\033[{showmode};37;1m",
+                    "§r": "\033[0m",
+                    "§u": "\033[4m",
+                    "§l": "\033[1m",
+                },
+            text,
             )
+            + "\033[0m"
+        )
 
     @staticmethod
     def align(text: str, length: int = 15) -> str:
         """对齐字符串
 
         Args:
             text (str): 需要对齐的字符串
@@ -171,31 +155,32 @@
             if strikeMode:
                 text_ok += "\u0336" + char
             else:
                 text_ok += char
             i += 1
         return text_ok
 
+    @staticmethod
     def print_with_info(
-        self, text: str, info: str = INFO_NORMAL, need_log: bool = True, **print_kwargs
+        text: str, info: str = INFO_NORMAL, need_log: bool = True, **print_kwargs
     ):
         """输出带有信息的文本
 
         Args:
             text (str): 输出的文本
             info (str, optional): 输出的信息
             need_log (bool, optional): 是否需要记录日志
             **print_kwargs: 原print函数的参数
 
         Raises:
             AssertionError: 无法找到对应的颜色代码
         """
-        with self.lock:
+        with Print.lock:
             if need_log:
-                self.c_log(info, text)
+                Print.c_log(info, text)
             setNextColor = "§r"
             if "\n" in text:
                 output_txts = []
                 for text_line in str(text).split("\n"):
                     if "§" in text_line:
                         try:
                             n = text_line.rfind("§")
@@ -203,109 +188,112 @@
                             if setNextColor == -1:
                                 raise AssertionError
                             setNextColor = _setNextCol
                         except Exception:
                             pass
                     output_txts.append(
                         datetime.datetime.now().strftime("[%H:%M] ")
-                        + self.colormode_replace(info, 7)
+                        + Print.colormode_replace(info, 7)
                         + " "
-                        + self.colormode_replace(setNextColor + text_line)
+                        + Print.colormode_replace(setNextColor + text_line)
                     )
                 print("\n".join(output_txts), **print_kwargs)
             else:
                 print(
                     datetime.datetime.now().strftime("[%H:%M] ")
-                    + self.colormode_replace(info, 7)
+                    + Print.colormode_replace(info, 7)
                     + " "
-                    + self.colormode_replace(text),
+                    + Print.colormode_replace(text),
                     **print_kwargs,
                 )
 
-    def clean_print(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def clean_print(text: str, **print_kwargs) -> None:
         """依照mc的颜色代码输出文本，可带有print函数的参数
 
         Args:
             text (str): 输出的文本
             **print_kwargs: 原print函数的参数
         """
-        with self.lock:
-            print(self.colormode_replace(text), **print_kwargs)
+        with Print.lock:
+            print(Print.colormode_replace(text), **print_kwargs)
 
-    def clean_fmt(self, text: str) -> str:
+    @staticmethod
+    def clean_fmt(text: str) -> str:
         """依照mc的颜色代码格式化文本
 
         Args:
             text (str): 需要格式化的文本
 
         Returns:
             str: 格式化后的文本
         """
-        with self.lock:
-            return self.colormode_replace(text)
+        return Print.colormode_replace(text)
 
-    def print_err(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def print_err(text: str, **print_kwargs) -> None:
         """输出错误信息
 
         Args:
             text (str): 输出的文本
         """
-        with self.lock:
-            self.print_with_info(f"§c{text}", self.INFO_ERROR, **print_kwargs)
+        Print.print_with_info(f"§c{text}", Print.INFO_ERROR, **print_kwargs)
 
-    def print_inf(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def print_inf(text: str, **print_kwargs) -> None:
         """输出INDO信息
 
         Args:
             text (str): 输出的文本
         """
-        with self.lock:
-            self.print_with_info(f"{text}", self.INFO_NORMAL, **print_kwargs)
+        Print.print_with_info(f"{text}", Print.INFO_NORMAL, **print_kwargs)
 
-    def print_suc(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def print_suc(text: str, **print_kwargs) -> None:
         """输出成功信息
 
         Args:
             text (str): 输出的文本
         """
-        with self.lock:
-            self.print_with_info(f"§a{text}", self.INFO_SUCC, **print_kwargs)
+        Print.print_with_info(f"§a{text}", Print.INFO_SUCC, **print_kwargs)
 
-    def print_war(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def print_war(text: str, **print_kwargs) -> None:
         """输出警告信息
 
         Args:
             text (str): 输出的文本
         """
-        with self.lock:
-            self.print_with_info(f"§6{text}", self.INFO_WARN, **print_kwargs)
+        Print.print_with_info(f"§6{text}", Print.INFO_WARN, **print_kwargs)
 
-    def print_load(self, text: str, **print_kwargs) -> None:
+    @staticmethod
+    def print_load(text: str, **print_kwargs) -> None:
         """输出加载信息
 
         Args:
             text (str): 输出的文本
         """
-        with self.lock:
-            self.print_with_info(f"§d{text}", self.INFO_LOAD, **print_kwargs)
+        with Print.lock:
+            Print.print_with_info(f"§d{text}", Print.INFO_LOAD, **print_kwargs)
 
-    def fmt_info(self, text: str, info: str = "§f 信息 ") -> str:
+    @staticmethod
+    def fmt_info(text: str, info: str = "§f 信息 ") -> str:
         """格式化信息
 
         Args:
             text (str): 输出的文本
             info (str, optional): 输出的信息
 
         Raises:
             AssertionError: 无法找到对应的颜色代码
 
         Returns:
             str: 格式化后的信息
         """
-        with self.lock:
+        with Print.lock:
             setNextColor = "§r"
             if "\n" in text:
                 output_txts = []
                 for text_line in str(text).split("\n"):
                     if "§" in text_line:
                         try:
                             n = text_line.rfind("§")
@@ -313,48 +301,46 @@
                             if setNextColor == -1:
                                 raise AssertionError
                             setNextColor = _setNextCol
                         except Exception:
                             pass
                     output_txts.append(
                         datetime.datetime.now().strftime("[%H:%M] ")
-                        + self.colormode_replace(info, 7)
+                        + Print.colormode_replace(info, 7)
                         + " "
-                        + self.colormode_replace(setNextColor + text_line)
+                        + Print.colormode_replace(setNextColor + text_line)
                     )
                 return "\n".join(output_txts)
             return (
                 datetime.datetime.now().strftime("[%H:%M] ")
-                + self.colormode_replace(info, 7)
+                + Print.colormode_replace(info, 7)
                 + " "
-                + self.colormode_replace(text)
+                + Print.colormode_replace(text)
             )
 
-    def c_log(self, inf: str, msg: str) -> None:
+    @staticmethod
+    def c_log(inf: str, msg: str) -> None:
         """记录日志
 
         Args:
             inf (str): 信息
             msg (str): 记录的信息
         """
-        with self.lock:
+        with Print.lock:
             for _g, _s in [
                 ("§6 警告 ", "WARN"),
                 ("§a 成功 ", "INFO"),
                 ("§f 信息 ", "INFO"),
                 ("§c 失败 ", "FAIL"),
                 ("§4 报错 ", "ERROR"),
             ]:
                 if inf == _g:
                     inf = _s
                     break
-            for col, _ in self.STD_COLOR_LIST:
+            for col, _ in Print.STD_COLOR_LIST:
                 col = "§" + col
                 msg = msg.replace(col, "")
-            for col, _ in self.STD_COLOR_LIST:
+            for col, _ in Print.STD_COLOR_LIST:
                 col = "§" + col
                 inf = inf.replace(col, "")
             inf = inf.replace(" ", "")
-            publicLogger.log_in(msg, inf)
-
-
-Print = _Print()
+            publicLogger.log_in(msg, inf)
```

### Comparing `tooldelta-0.6.0/tooldelta/constants.py` & `tooldelta-0.6.1/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/frame.py` & `tooldelta-0.6.1/tooldelta/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,14 +502,15 @@
                     self.link_game_ctrl.say_to('@a', f'[§bToolDelta控制台§r] §3{rsp}§r')
 
         self.createThread(_console_cmd_thread, usage="控制台指令")
 
     def system_exit(self) -> None:
         """系统退出"""
         asyncio.run(safe_jump())
+        self.link_plugin_group.execute_frame_exit(self.on_plugin_err)
         exit_status_code = getattr(self.launcher, "secret_exit_key", "null")
         if self.link_game_ctrl.allplayers and not isinstance(
             self.launcher, (FrameNeOmgRemote,)
         ):
             try:
                 self.link_game_ctrl.sendwscmd(
                     f"/kick {self.link_game_ctrl.bot_name} ToolDelta 退出中(看到这条消息请重新加入游戏)\nSTATUS CODE: {exit_status_code}"
```

### Comparing `tooldelta-0.6.0/tooldelta/game_texts.py` & `tooldelta-0.6.1/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/launch_cli.py` & `tooldelta-0.6.1/tooldelta/launch_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             NotImplementedError: 未实现此方法
 
         Returns:
             bool: 是否为OP
         """
         raise NotImplementedError
 
-    def place_command_block_with_nbt_data(self, block_name:str, block_states:str, 
+    def place_command_block_with_nbt_data(self, block_name:str, block_states:str,
                                           position: tuple[int, int, int],
                                           nbt_data: neo_conn.CommandBlockNBTData):
         """在 position 放置方块名为 block_name 且方块状态为 block_states 的命令块，
         同时向该方块写入 nbt_data 所指代的 NBT 数据
 
         Args:
             block_name (str): 命令块的方块名，如 chain_command_block
@@ -259,14 +259,15 @@
         """启动 NeOmega 进程
 
         Returns:
             int: 端口号
         """
         free_port = get_free_port(24016)
         sys_machine = platform.uname().machine
+        sys_machine = "amd64" if sys_machine == "x86_64" else sys_machine
         access_point_file = (
             f"neomega_{platform.uname().system.lower()}_access_point_{sys_machine}"
         )
         if "TERMUX_VERSION" in os.environ:
             access_point_file = f"neomega_android_access_point_{sys_machine}"
         if platform.system() == "Windows":
             access_point_file += ".exe"
```

### Comparing `tooldelta-0.6.0/tooldelta/launch_options.py` & `tooldelta-0.6.1/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/logger.py` & `tooldelta-0.6.1/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/neo_conn.py` & `tooldelta-0.6.1/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/packets.py` & `tooldelta-0.6.1/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.6.1/tooldelta/plugin_load/PluginGroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .injected_plugin import (
     execute_init,
     execute_player_prejoin,
     execute_player_join,
     execute_player_message,
     execute_death_message,
     execute_player_left,
+    execute_frame_exit,
     execute_repeat
 )
 from ..plugin_load import (
     classic_plugin,
     injected_plugin,
     NON_FUNC,
     NotValidPluginError,
@@ -39,14 +40,15 @@
         "on_def": [],
         "on_inject": [],
         "on_player_prejoin": [],
         "on_player_join": [],
         "on_player_message": [],
         "on_player_death": [],
         "on_player_leave": [],
+        "on_frame_exit": []
     }
     plugin_added_cache = {"plugin": None, "packets": []}
     pluginAPI_added_cache = []
     broadcast_evts_cache = {}
 
     def __init__(self):
         "初始化"
@@ -428,15 +430,15 @@
     def execute_player_death(
         self,
         player: str,
         killer: str | None,
         msg: str,
         onerr: Callable[[str, Exception, str], None] = NON_FUNC,
     ):
-        """
+        """执行玩家死亡的方法
 
         Args:
             player (str): 玩家
             killer (str | None): 击杀者
             msg (str): 消息
             onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
         """
@@ -447,14 +449,27 @@
                 onerr(name, err, traceback.format_exc())
         asyncio.run(
             execute_death_message(
                 player, killer, msg
             )
         )
 
+    def execute_frame_exit(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC):
+        """执行框架退出的方法
+
+        Args:
+            onerr (Callable[[str, Exception, str], None], optional): 插件出错时的处理方法
+        """
+        for name, func in self.plugins_funcs["on_frame_exit"]:
+            try:
+                func()
+            except Exception as err:
+                onerr(name, err, traceback.format_exc())
+        asyncio.run(execute_frame_exit())
+
     def processPacketFunc(self, pktID: int, pkt: dict) -> bool:
         """处理数据包监听器
 
         Args:
             pktID (int): 数据包ID
             pkt (dict): 数据包
```

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/__init__.py` & `tooldelta-0.6.1/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.6.1/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
         for evt_name in (
             "on_def",
             "on_inject",
             "on_player_prejoin",
             "on_player_join",
             "on_player_message",
             "on_player_death",
-            "on_player_leave"
+            "on_player_leave",
+            "on_frame_exit"
         ):
             if hasattr(plugin_ins, evt_name):
                 plugin_grp.plugins_funcs[evt_name].append(
                     [plugin_ins.name, getattr(plugin_ins, evt_name)]
                 )
         Print.print_suc(
             f"成功载入插件 {plugin_ins.name} 版本: {_v0}.{_v1}.{_v2} 作者：{plugin_ins.author}"
```

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 player_message_funcs: dict[Callable, int | None] = {}
 player_prejoin_funcs: dict[Callable, int | None] = {}
 player_join_funcs: dict[Callable, int | None] = {}
 player_left_funcs: dict[Callable, int | None] = {}
 player_death_funcs: dict[Callable, int | None] = {}
 repeat_funcs: dict[Callable, int | float] = {}
 init_plugin_funcs: dict[Callable, int | None] = {}
+frame_exit_funcs: dict[Callable, int | None] = {}
 
 
 def player_message(priority: int | None = None) -> Callable:
     """载入处理玩家消息
 
     Args:
         priority (int, optional): 插件优先级
@@ -118,14 +119,30 @@
     def decorator(func):
         init_plugin_funcs[func] = priority
         return func
 
     return decorator
 
 
+def frame_exit(priority: int | None = None) -> Callable:
+    """载入处理框架退出事件的插件
+
+    Args:
+        priority (int | None, optional): 插件优先级
+
+    Returns:
+        Callable: 插件处理函数
+    """
+    def decorator(func):
+        frame_exit_funcs[func] = priority
+        return func
+
+    return decorator
+
+
 def repeat(retime: int | float = 5) -> Callable:
     """载入重复任务
 
     Args:
         retime (int, optional): 重复时间
 
     Returns:
@@ -282,14 +299,19 @@
 
     Args:
         playername (str): 玩家名字
     """
     await execute_asyncio_task(player_left_funcs, player_name(playername=playername))
 
 
+async def execute_frame_exit() -> None:
+    """执行框架退出处理函数"""
+    await execute_asyncio_task(frame_exit_funcs)
+
+
 class PluginMetadata:
     "插件元数据"
 
     def __init__(
         self,
         name,
         author,
```

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/plugin_load/utils.py` & `tooldelta-0.6.1/tooldelta/plugin_load/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/plugin_manager.py` & `tooldelta-0.6.1/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/plugin_market.py` & `tooldelta-0.6.1/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/starter.py` & `tooldelta-0.6.1/tooldelta/starter.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,13 +46,13 @@
         exit_directly (bool, optional): 是否三秒强制直接退出
     """
     if out_task:
         frame.system_exit()
     frame.safelyExit()
     if exit_directly:
         for _ in range(2, 0, -1):
-            Print.print_war(f"{_}秒后强制退出...", end="\r")
+            with Print.lock:Print.print_war(f"{_}秒后强制退出...", end="\r")
             time.sleep(1)
-        Print.print_war("0秒后强制退出...", end="\r")
-        Print.print_suc("ToolDelta 已退出.")
+        with Print.lock:Print.print_war("0秒后强制退出...", end="\r")
+        with Print.lock:Print.print_suc("ToolDelta 已退出.")
         os._exit(0)
-    Print.print_suc("ToolDelta 已退出.")
+    with Print.lock:Print.print_suc("ToolDelta 已退出.")
```

### Comparing `tooldelta-0.6.0/tooldelta/sys_args.py` & `tooldelta-0.6.1/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/tooldelta/urlmethod.py` & `tooldelta-0.6.1/tooldelta/urlmethod.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,43 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import pyspeedtest
 import requests
 
 from .get_tool_delta_version import get_tool_delta_version
 from .color_print import Print
 
+# 使用方法 mirror_github[value: int].format(url: str)
+mirror_github = ["https://hub.gitmirror.com/{}", "https://gh.con.sh/{}", "https://mirror.ghproxy.com/{}"]
+
+def format_mirror_url(url: str) -> list:
+    """填充url到镜像url列表
+
+    Args:
+        url (str): 原始URL
+
+    Returns:
+        list: 填充原始url后的镜像列表
+    """
+    mir_url: list = []
+    for mirror in mirror_github:mir_url.append(mirror.format(url))
+    return mir_url
+
+def githubdownloadurl_to_rawurl(url: str) -> str:
+    """将github下载链接转换为原始链接
+
+    Args:
+        url (str): 原始链接
+
+    Returns:
+        str: 原始链接
+    """
+    try:
+        if url.startswith("https://github.com/"):return requests.head(url, allow_redirects=True).url
+        else:return url
+    except:return url
 
 def progress_bar(
     current: float | int, total: float | int, length: int | float = 20, color1: str = "§f", color2: str = "§b"
 ) -> str:
     """执行进度条
 
     Args:
@@ -44,15 +73,15 @@
         total_bytes (int): 文件总字节数
         speed ( float): 下载速度.
     """
     progressBar = progress_bar(current_bytes, total_bytes)
     b = f"{progressBar} {pretty_kb(current_bytes)}B / {pretty_kb(total_bytes)}B"
     if speed != 0:
         b += f" ({pretty_kb(speed)}B/s)    "
-    Print.print_with_info(b, "§a 下载 ", need_log=False, end="\r")
+    with Print.lock:Print.print_with_info(b, "§a 下载 ", need_log=False, end="\r")
 
 
 def pretty_kb(n: float) -> str:
     """将字节数转换为可读性更好的字符串表示形式
 
     Args:
         n (float): 字节数
```

### Comparing `tooldelta-0.6.0/tooldelta/utils.py` & `tooldelta-0.6.1/tooldelta/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.0/PKG-INFO` & `tooldelta-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.6.0
+Version: 0.6.1
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.0 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.1 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
```

