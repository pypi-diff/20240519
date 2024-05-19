# Comparing `tmp/py92-1.0.2.tar.gz` & `tmp/py92-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py92-1.0.2.tar", last modified: Fri May 17 19:04:24 2024, max compression
+gzip compressed data, was "py92-1.0.3.tar", last modified: Sun May 19 17:15:35 2024, max compression
```

## Comparing `py92-1.0.2.tar` & `py92-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:04:24.434579 py92-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 19:04:21.000000 py92-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 19:04:21.000000 py92-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-17 19:04:24.434579 py92-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-17 19:04:21.000000 py92-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:04:24.430579 py92-1.0.2/py92/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-17 19:04:21.000000 py92-1.0.2/py92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   184052 2024-05-17 19:04:21.000000 py92-1.0.2/py92/cn_schools.csv
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 19:04:21.000000 py92-1.0.2/py92/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-17 19:04:21.000000 py92-1.0.2/py92/py92utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:04:24.434579 py92-1.0.2/py92.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-17 19:04:24.000000 py92-1.0.2/py92.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 19:04:24.000000 py92-1.0.2/py92.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:04:24.000000 py92-1.0.2/py92.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 19:04:24.000000 py92-1.0.2/py92.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 19:04:24.000000 py92-1.0.2/py92.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:04:24.434579 py92-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-17 19:04:21.000000 py92-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:04:24.434579 py92-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:04:21.000000 py92-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-17 19:04:21.000000 py92-1.0.2/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:35.436530 py92-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 17:15:27.000000 py92-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 17:15:27.000000 py92-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-19 17:15:35.436530 py92-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-19 17:15:27.000000 py92-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:35.432530 py92-1.0.3/py92/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-19 17:15:27.000000 py92-1.0.3/py92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184052 2024-05-19 17:15:27.000000 py92-1.0.3/py92/cn_schools.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 17:15:27.000000 py92-1.0.3/py92/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-19 17:15:27.000000 py92-1.0.3/py92/py92utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55420 2024-05-19 17:15:27.000000 py92-1.0.3/py92/qs2024.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:35.432530 py92-1.0.3/py92.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-19 17:15:35.000000 py92-1.0.3/py92.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-19 17:15:35.000000 py92-1.0.3/py92.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:15:35.000000 py92-1.0.3/py92.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 17:15:35.000000 py92-1.0.3/py92.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 17:15:35.000000 py92-1.0.3/py92.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:15:35.436530 py92-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-19 17:15:27.000000 py92-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:35.432530 py92-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:15:27.000000 py92-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 17:15:27.000000 py92-1.0.3/tests/test_module.py
```

### Comparing `py92-1.0.2/LICENSE` & `py92-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py92-1.0.2/PKG-INFO` & `py92-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py92
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Packages for Labeling(985/211/双一流/本科) Schools in China
 Home-page: https://github.com/stanleysun233/py92
 Author: Stanley SUN
 Author-email: stanleysun233@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,38 +16,40 @@
 # PY92
 快速确定中国的学校是否是
 * 985
 * 211
 * 双一流
 * 本科
 * 民办
+* QS2024 TOP 1500
 
-# 下版本(v1.0.3)目标
-* 增加**英文**学校信息
-* 考虑是否添加一二本属性（有争议）
-* 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+# 下版本(v1.0.4)目标
+- [ ] 增加**英文**学校信息
+- [ ] 考虑是否添加一二本属性（有争议）
+- [ ] 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+  * [x] QS2024 实际获取QSTOP1500
+  * [ ] USNEWS
+  * [ ] 泰晤士
+- [x] 自动推送pypi
 
 # 数据来源
-[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+国内院校：[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+QS2024：[QS2024](https://www.qschina.cn/university-rankings/world-university-rankings/2024)
 
 如果学校类型有误、遗漏学校，欢迎提交issue。
 
 # 安装
 
 ```shell
 pip install py92
 ```
 or
 ```shell
 pip install git+https://github.com/stanleysun233/py92.git
 ```
-or
-```shell
-pip install https://github.com/StanleySun233/py92/raw/main/dist/py92-1.0.1-py3-none-any.whl
-```
 
 本库仅依赖`pandas`。
 
 # 示例
 前言：
 * 如果是，返回1；
 * 如果不是，返回0；
@@ -124,14 +126,22 @@
 返回学校所有标签。
 
 ```python
 print(py92.get_label("上海海事大学"))
 # {'name': '上海海事大学', '985': 0, '211': 0, '双一流': 0, '本科': 1, '公办': 1}
 ```
 
-9. `is_[xxx]s`
+9. `get_qs`
+返回学校的qs排名，选填参数`year`，默认为2024。
+
+```python
+print(py92.get_qs("新加坡国立大学"))
+8
+```
+
+10. `is_[xxx]s`
 返回学校组是否属于**xxx**。
 输入：`[name1, name2, name3]`
 ```python
 schools = ["北京大学","上海海事大学","纽约大学"]
 print(py92.is_ins(schools)) # [1, 1, 0]
 ```
```

### Comparing `py92-1.0.2/README.md` & `py92-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # PY92
 快速确定中国的学校是否是
 * 985
 * 211
 * 双一流
 * 本科
 * 民办
+* QS2024 TOP 1500
 
-# 下版本(v1.0.3)目标
-* 增加**英文**学校信息
-* 考虑是否添加一二本属性（有争议）
-* 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+# 下版本(v1.0.4)目标
+- [ ] 增加**英文**学校信息
+- [ ] 考虑是否添加一二本属性（有争议）
+- [ ] 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+  * [x] QS2024 实际获取QSTOP1500
+  * [ ] USNEWS
+  * [ ] 泰晤士
+- [x] 自动推送pypi
 
 # 数据来源
-[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+国内院校：[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+QS2024：[QS2024](https://www.qschina.cn/university-rankings/world-university-rankings/2024)
 
 如果学校类型有误、遗漏学校，欢迎提交issue。
 
 # 安装
 
 ```shell
 pip install py92
 ```
 or
 ```shell
 pip install git+https://github.com/stanleysun233/py92.git
 ```
-or
-```shell
-pip install https://github.com/StanleySun233/py92/raw/main/dist/py92-1.0.1-py3-none-any.whl
-```
 
 本库仅依赖`pandas`。
 
 # 示例
 前言：
 * 如果是，返回1；
 * 如果不是，返回0；
@@ -109,14 +111,22 @@
 返回学校所有标签。
 
 ```python
 print(py92.get_label("上海海事大学"))
 # {'name': '上海海事大学', '985': 0, '211': 0, '双一流': 0, '本科': 1, '公办': 1}
 ```
 
-9. `is_[xxx]s`
+9. `get_qs`
+返回学校的qs排名，选填参数`year`，默认为2024。
+
+```python
+print(py92.get_qs("新加坡国立大学"))
+8
+```
+
+10. `is_[xxx]s`
 返回学校组是否属于**xxx**。
 输入：`[name1, name2, name3]`
 ```python
 schools = ["北京大学","上海海事大学","纽约大学"]
 print(py92.is_ins(schools)) # [1, 1, 0]
-```
+```
```

### Comparing `py92-1.0.2/py92/__init__.py` & `py92-1.0.3/py92/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,7 +62,15 @@
 
 def get_label(name):
     return py92utils.get_label(name)
 
 
 def get_labels(names):
     return py92utils.get_labels(names)
+
+
+def get_qs(name):
+    return py92utils.get_qs(name)
+
+
+def get_qss(names):
+    return py92utils.get_qss(names)
```

### Comparing `py92-1.0.2/py92/cn_schools.csv` & `py92-1.0.3/py92/cn_schools.csv`

 * *Files identical despite different names*

### Comparing `py92-1.0.2/py92/py92utils.py` & `py92-1.0.3/py92/py92utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 import pandas as pd
 import py92
 
 
 class py92utils:
     def __init__(self):
-        self.df = pd.read_csv(py92.config.CN_SCHOOLS_DIR, encoding='utf-8')
+        self.cn_school = pd.read_csv(py92.config.CN_SCHOOLS_DIR, encoding='utf-8')
+        self.qs2024 = pd.read_csv(py92.config.QS2024_DIR, encoding='utf-8')
 
     def is_in(self, name):
-        return int(name in self.df["学校"].tolist())
+        return int(name in self.cn_school["学校"].tolist()) or int(name in self.qs2024["name_cn"].tolist())
 
     def is_ins(self, names):
         return [self.is_in(_) for _ in names]
 
     def is_985(self, name):
-        if name not in self.df["学校"].tolist(): return -1
-        return int(self.df[self.df["学校"] == name]["985"].values[0] == '是')
+        if not self.is_in(name): return -1
+        return int(self.cn_school[self.cn_school["学校"] == name]["985"].values[0] == '是')
 
     def is_985s(self, names):
         return [self.is_985(_) for _ in names]
 
     def is_211(self, name):
-        if name not in self.df["学校"].tolist():
+        if not self.is_in(name):
             return -1
         else:
-            return int(self.df[self.df["学校"] == name]["211"].values[0] == '是')
+            return int(self.cn_school[self.cn_school["学校"] == name]["211"].values[0] == '是')
 
     def is_211s(self, names):
         return [self.is_211(_) for _ in names]
 
     def is_db1(self, name):
-        if name not in self.df["学校"].tolist():
+        if not self.is_in(name):
             return -1
         else:
-            return int(self.df[self.df["学校"] == name]["双一流"].values[0] == '是')
+            return int(self.cn_school[self.cn_school["学校"] == name]["双一流"].values[0] == '是')
 
     def is_db1s(self, names):
         return [self.is_db1(_) for _ in names]
 
     def is_university(self, name):
-        if name not in self.df["学校"].tolist():
+        if not self.is_in(name):
             return -1
         else:
-            return int(self.df[self.df["学校"] == name]["层次"].values[0] == '本科')
+            return int(self.cn_school[self.cn_school["学校"] == name]["层次"].values[0] == '本科')
 
     def is_universitys(self, names):
         return [self.is_university(_) for _ in names]
 
     def is_public(self, name):
-        if name not in self.df["学校"].tolist():
+        if not self.is_in(name):
             return -1
         else:
-            return int(self.df[self.df["学校"] == name]["性质"].values[0] == '公办')
+            return int(self.cn_school[self.cn_school["学校"] == name]["性质"].values[0] == '公办')
 
     def is_publics(self, names):
         return [self.is_public(_) for _ in names]
 
     def get_highest_label(self, name):
-        if name not in self.df["学校"].tolist():
+        if not self.is_in(name):
             return ''
         elif self.is_985(name):
             return "985"
         elif self.is_211(name):
             return "211"
         elif self.is_db1(name):
             return "双一流"
@@ -79,7 +80,16 @@
                 "211": self.is_211(name),
                 "双一流": self.is_db1(name),
                 "本科": self.is_university(name),
                 "公办": self.is_public(name)}
 
     def get_labels(self, names):
         return [self.get_label(k) for k in names]
+
+    def get_qs(self, name, year=2024):
+        if not self.is_in(name):
+            return -1
+        else:
+            return int(self.qs2024[self.qs2024["name_cn"] == name]["rank"].values[0])
+
+    def get_qss(self, names, year=2024):
+        return [self.get_qs(_, year) for _ in names]
```

### Comparing `py92-1.0.2/py92.egg-info/PKG-INFO` & `py92-1.0.3/py92.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py92
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Packages for Labeling(985/211/双一流/本科) Schools in China
 Home-page: https://github.com/stanleysun233/py92
 Author: Stanley SUN
 Author-email: stanleysun233@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,38 +16,40 @@
 # PY92
 快速确定中国的学校是否是
 * 985
 * 211
 * 双一流
 * 本科
 * 民办
+* QS2024 TOP 1500
 
-# 下版本(v1.0.3)目标
-* 增加**英文**学校信息
-* 考虑是否添加一二本属性（有争议）
-* 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+# 下版本(v1.0.4)目标
+- [ ] 增加**英文**学校信息
+- [ ] 考虑是否添加一二本属性（有争议）
+- [ ] 准备开发[QS, USNEWS, 泰晤士]TOP1000院校信息表
+  * [x] QS2024 实际获取QSTOP1500
+  * [ ] USNEWS
+  * [ ] 泰晤士
+- [x] 自动推送pypi
 
 # 数据来源
-[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+国内院校：[大学生必备网](https://www.dxsbb.com/news/list_88.html) -> [cn_schools.csv](./data/cn_schools.csv)
+QS2024：[QS2024](https://www.qschina.cn/university-rankings/world-university-rankings/2024)
 
 如果学校类型有误、遗漏学校，欢迎提交issue。
 
 # 安装
 
 ```shell
 pip install py92
 ```
 or
 ```shell
 pip install git+https://github.com/stanleysun233/py92.git
 ```
-or
-```shell
-pip install https://github.com/StanleySun233/py92/raw/main/dist/py92-1.0.1-py3-none-any.whl
-```
 
 本库仅依赖`pandas`。
 
 # 示例
 前言：
 * 如果是，返回1；
 * 如果不是，返回0；
@@ -124,14 +126,22 @@
 返回学校所有标签。
 
 ```python
 print(py92.get_label("上海海事大学"))
 # {'name': '上海海事大学', '985': 0, '211': 0, '双一流': 0, '本科': 1, '公办': 1}
 ```
 
-9. `is_[xxx]s`
+9. `get_qs`
+返回学校的qs排名，选填参数`year`，默认为2024。
+
+```python
+print(py92.get_qs("新加坡国立大学"))
+8
+```
+
+10. `is_[xxx]s`
 返回学校组是否属于**xxx**。
 输入：`[name1, name2, name3]`
 ```python
 schools = ["北京大学","上海海事大学","纽约大学"]
 print(py92.is_ins(schools)) # [1, 1, 0]
 ```
```

### Comparing `py92-1.0.2/setup.py` & `py92-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="py92",  # 包的名称
-    version="1.0.2",  # 包的版本
+    version="1.0.3",  # 包的版本
     author="Stanley SUN",  # 作者名称
     author_email="stanleysun233@163.com",  # 作者邮箱
     description="Python Packages for Labeling(985/211/双一流/本科) Schools in China",  # 简短描述
     long_description=long_description,  # 长描述，通常从 README.md 文件中读取
     long_description_content_type="text/markdown",
     url="https://github.com/stanleysun233/py92",  # 项目主页
     packages=find_packages(),  # 自动找到项目中的包
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.5',  # 依赖的Python版本
     package_data={
-        'py92': ['cn_schools.csv'],
+        'py92': ['cn_schools.csv',
+                 'qs2024.csv'],
     },
     install_requires=[
         "pandas"
     ],
 )
```

### Comparing `py92-1.0.2/tests/test_module.py` & `py92-1.0.3/tests/test_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,7 +21,12 @@
 
     print(py92.get_label("上海海事大学"))
     # {'name': '上海海事大学', '985': 0, '211': 0, '双一流': 0, '本科': 1, '公办': 1}
     print(py92.get_label("上海纽约大学"))
     # {'name': '上海海事大学', '985': 0, '211': 0, '双一流': 0, '本科': 1, '公办': 1}
     print(py92.get_label("纽约大学"))
     # {'name': '纽约大学', '985': -1, '211': -1, '双一流': -1, '本科': -1, '公办': -1}
+
+    print(py92.get_qs("新加坡国立大学"))
+    # 8
+    print(py92.get_qs("清华大学"))
+    # 25
```

