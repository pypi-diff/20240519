# Comparing `tmp/config_center-0.0.3.tar.gz` & `tmp/config_center-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_center-0.0.3.tar", last modified: Fri May 17 16:43:45 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `config_center-0.0.3.tar` & `config_center-0.0.31.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.444336 config_center-0.0.3/
--rw-rw-rw-   0        0        0     1093 2024-05-17 15:58:59.000000 config_center-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1777 2024-05-17 16:43:45.443371 config_center-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.439011 config_center-0.0.3/cfgc/
--rw-rw-rw-   0        0        0      498 2024-05-17 14:26:52.000000 config_center-0.0.3/cfgc/__init__.py
--rw-rw-rw-   0        0        0     3836 2024-05-17 16:42:09.000000 config_center-0.0.3/cfgc/center.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.443371 config_center-0.0.3/config_center.egg-info/
--rw-rw-rw-   0        0        0     1777 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 16:43:45.444336 config_center-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1416 2024-05-17 16:43:32.000000 config_center-0.0.3/setup.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.31/MAINFEST.in
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.31/readme.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.31/test.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/config-center.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/vcs.xml
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.31/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.31/cfgc/__init__.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 config_center-0.0.31/cfgc/center.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.31/cfgc/envs/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.31/LICENSE.txt
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.31/README.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 config_center-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 config_center-0.0.31/PKG-INFO
```

### Comparing `config_center-0.0.3/LICENSE.txt` & `config_center-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_center-0.0.3/cfgc/center.py` & `config_center-0.0.31/cfgc/center.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,47 +12,55 @@
 # region |- Import -|
 from importlib import import_module
 from pathlib import Path
 import pickle
 import shutil
 import sys
 import os
+
+from . import envs
 # endregion
 
-# Absolute Path of cfgc package
-PATH_X = Path(os.path.split(os.path.realpath(__file__))[0])
-PATH_CUSTOM = PATH_X / 'custom'
-PATH_ENV = PATH_CUSTOM / 'envs'
 
 # Class Domain
 class Domain:
     def __init__(self, data: dict={}):
         assert isinstance(data, dict)
         self.data = data
     def __setitem__(self, key, val):
         self.data[key] = val
     def __getitem__(self, key):
         return self.data.get(key)
+    def __str__(self):
+        return str(self.data)
+
+
+# region |- Absolute Path of cfgc package -|
+PATH = Domain({"info": "envs"})
+PATH.center = Path(os.path.split(os.path.realpath(__file__))[0])
+PATH.envs = envs.PATH
+# endregion
+
 
 # Class Env
 class Environment:
-    def __init__(self, name='base', domain: dict={}, engine: Path='.', load: str=None):
+    def __init__(self, name='base', domain: dict or Domain={}, engine: str or Path='.', load: str=None):
         if load is None:
             self.define(name, domain, engine)
         else:   # 如果是加载环境则 直接构建 并 启动engine包
             self.load(load)
-            self.drive()
-    def define(self, name, domain: dict={}, engine: Path='.'):
+    def define(self, name, domain: dict or Domain={}, engine: str or Path='.'):
         """
         创建配置环境
 
         :param name: 环境名称
         :param data: 环境全局变量 [对于大型数据, 也可以存储数据仓库路径, 挂载访问]
         :param engine: 加载的驱动包目录 [不需要在site-packages里, 会自动加载管理]
         """
+        engine = os.path.normpath(engine)
         self.name = name
         self.domain = domain if isinstance(domain, Domain) else Domain(domain)
         self.__engine = str(engine)
         self.engine = Path(engine)
     def drive(self):
         """
         驱动, 加载驱动目录作为 包, 通过engine 调用内部函数
@@ -67,15 +75,15 @@
         储存该环境文件, 之后可以随时加载
 
         :param safe: 安全模式, 默认开启 ——当存在env时提示是否覆盖, 否则将直接覆盖
         :return:
         """
         assert self.engine.is_absolute(), "engine must be a Absolute Path"    # 仅支持绝对定位 & 目录
         assert self.engine.is_dir(), "engine only can be a Dir"
-        save_path = PATH_ENV / f'{self.name}.pkl'
+        save_path = PATH.envs / f'{self.name}.pkl'
         if os.path.exists(save_path):
             status = True and safe
             while status:
                 replace = input(f"There has been an env called: {self.name}, overwrite ?(yes/no)\n")
                 if replace == 'yes':
                     break
                 elif replace == 'no':
@@ -93,19 +101,49 @@
     def load(self, name):
         """
         由环境名称 加载
 
         :param name: 环境名称
         :return:
         """
-        with open(PATH_ENV / f'{name}.pkl', "rb") as cfg:
+        with open(PATH.envs / f'{name}.pkl', "rb") as cfg:
             cfg = pickle.load(cfg)
         self.define(**cfg)
+        self.drive()
+        return self
+    def load_path(self, path):
+        """
+        load from one export dir path
+        :param path: the 'path' of self.export
+        :return:
+        """
+        path = Path(os.path.normpath(path))
+        # load domain data
+        with open(path / "domain.pkl", "rb") as dd:
+            domain = pickle.load(dd)
+        self.define(name=os.path.basename(path), domain=domain, engine=path / "engine")
+        self.drive()
+        return self
+    def delete(self):
+        """
+        删除该环境的记录文件
+
+        :return:
+        """
+        envs.delete(self.name)
     def rename(self, name):
         self.name = name
+        return self
+    def export(self, path):
+        """
+        将Engine目录 即 domain数据导出至该路径 path
 
-
-# Check Envs
-def envList():
-    envs = os.listdir(PATH_ENV)
-    for i, e in enumerate(envs):
-        print(f"{i} -\t{e.split('.',maxsplit=1)[0]}")
+        :param path: 导出路径
+        :return:
+        """
+        path = Path(os.path.normpath(path))
+        assert not os.path.exists(path), f"The export path Existed! [{path}]"
+        shutil.copytree(self.__engine, path / "engine")     # 复制engine
+        # store domain data
+        with open(path / "domain.pkl", "wb") as dd:
+            pickle.dump(self.domain, dd)
+        print(f"Env export to: {path}\n Named as [{os.path.basename(path)}]")
```

