# Comparing `tmp/baosight-0.0.5.tar.gz` & `tmp/baosight-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baosight-0.0.5.tar", last modified: Sat May 18 18:54:28 2024, max compression
+gzip compressed data, was "baosight-0.0.7.tar", last modified: Sat May 18 18:57:56 2024, max compression
```

## Comparing `baosight-0.0.5.tar` & `baosight-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.675547 baosight-0.0.5/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1296 2024-05-18 18:54:28.675547 baosight-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      689 2024-05-18 18:35:53.000000 baosight-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.641611 baosight-0.0.5/baosight/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.5/baosight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.667611 baosight-0.0.5/baosight/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.5/baosight/cli/__init__.py
--rw-rw-rw-   0        0        0     1415 2024-05-18 18:53:44.000000 baosight-0.0.5/baosight/cli/gl_runner.py
--rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.5/baosight/cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.672546 baosight-0.0.5/baosight/tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.5/baosight/tools/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.5/baosight/tools/gitlab_runner.py
--rw-rw-rw-   0        0        0     1526 2024-05-18 18:52:57.000000 baosight-0.0.5/baosight/tools/gitlab_runner_config_generator.py
--rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.5/baosight/tools/gitlab_runner_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:54:28.673545 baosight-0.0.5/baosight.egg-info/
--rw-rw-rw-   0        0        0     1296 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 18:54:28.000000 baosight-0.0.5/baosight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2024-05-18 18:54:28.677549 baosight-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.581632 baosight-0.0.7/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1380 2024-05-18 18:57:56.581632 baosight-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-18 18:57:41.000000 baosight-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.549467 baosight-0.0.7/baosight/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.7/baosight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.574666 baosight-0.0.7/baosight/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.7/baosight/cli/__init__.py
+-rw-rw-rw-   0        0        0     1409 2024-05-18 18:56:55.000000 baosight-0.0.7/baosight/cli/gl_runner.py
+-rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.7/baosight/cli/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.578664 baosight-0.0.7/baosight/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.7/baosight/tools/__init__.py
+-rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.7/baosight/tools/gitlab_runner.py
+-rw-rw-rw-   0        0        0     1593 2024-05-18 18:56:44.000000 baosight-0.0.7/baosight/tools/gitlab_runner_config_generator.py
+-rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.7/baosight/tools/gitlab_runner_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.579663 baosight-0.0.7/baosight.egg-info/
+-rw-rw-rw-   0        0        0     1380 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-18 18:57:55.000000 baosight-0.0.7/baosight.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2024-05-18 18:57:56.583666 baosight-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.7/setup.py
```

### Comparing `baosight-0.0.5/LICENSE` & `baosight-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `baosight-0.0.5/PKG-INFO` & `baosight-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.5
+Version: 0.0.7
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
@@ -46,7 +46,13 @@
 
 2. 安装命令
 
 ```shell
 baosight gl-runner --quite  # 使用当前目录config.json静默安装runner
 baosight gl-runner # 使用gui选择配置文件并安装
 ```
+
+3. 快速生成配置文件
+
+```shell
+baosight gl-runner --create-config
+```
```

### Comparing `baosight-0.0.5/README.md` & `baosight-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,14 @@
 ```
 
 2. 安装命令
 
 ```shell
 baosight gl-runner --quite  # 使用当前目录config.json静默安装runner
 baosight gl-runner # 使用gui选择配置文件并安装
+```
+
+3. 快速生成配置文件
+
+```shell
+baosight gl-runner --create-config
 ```
```

### Comparing `baosight-0.0.5/baosight/cli/gl_runner.py` & `baosight-0.0.7/baosight/cli/gl_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     }
     """
 
     @staticmethod
     def add_arguments(parser: ArgumentParser):
         add = parser.add_argument
         add("--quite", action='store_true', help="静默安装当前目录下的config.json")
-        add("--create-config", dest="config", action='store_true', help="静默安装当前目录下的config.json")
+        add("--create-config", dest="config", action='store_true', help="交互式生成配置文件")
 
     @staticmethod
     def run(args, parser):
         if args.config:
-            generator()
-            deploy("config.json")
+            if generator():
+                deploy("config.json")
             return
         if args.quite:
             deploy("config.json")
         else:
             create_installation_ui()
```

### Comparing `baosight-0.0.5/baosight/cli/main.py` & `baosight-0.0.7/baosight/cli/main.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.5/baosight/tools/gitlab_runner.py` & `baosight-0.0.7/baosight/tools/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.5/baosight/tools/gitlab_runner_config_generator.py` & `baosight-0.0.7/baosight/tools/gitlab_runner_config_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,7 +36,8 @@
         'runners': runners
     }
 
     file_path = input("请输入配置文件保存的路径及名称（例如 C:/path/to/config.json）: ") or "./config.json"
     with open(file_path, 'w') as f:
         json.dump(config, f, indent=4)
     print(f"配置文件已保存到 {file_path}")
+    return input("是否立即执行？（y/n）").lower() == "y"
```

### Comparing `baosight-0.0.5/baosight/tools/gitlab_runner_gui.py` & `baosight-0.0.7/baosight/tools/gitlab_runner_gui.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.5/baosight.egg-info/PKG-INFO` & `baosight-0.0.7/baosight.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.5
+Version: 0.0.7
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
@@ -46,7 +46,13 @@
 
 2. 安装命令
 
 ```shell
 baosight gl-runner --quite  # 使用当前目录config.json静默安装runner
 baosight gl-runner # 使用gui选择配置文件并安装
 ```
+
+3. 快速生成配置文件
+
+```shell
+baosight gl-runner --create-config
+```
```

### Comparing `baosight-0.0.5/setup.cfg` & `baosight-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 616f 7369 6768 740d 0a76 6572   = baosight..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 6465  sion = 0.0.5..de
+00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6465  sion = 0.0.7..de
 00000030: 7363 7269 7074 696f 6e20 3d20 6261 6f73  scription = baos
 00000040: 6967 6874 2074 6f6f 6c73 0d0a 6c6f 6e67  ight tools..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
```

