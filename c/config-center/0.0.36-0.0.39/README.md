# Comparing `tmp/config_center-0.0.36.tar.gz` & `tmp/config_center-0.0.39.tar.gz`

## Comparing `config_center-0.0.36.tar` & `config_center-0.0.39.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.36/MAINFEST.in
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.36/readme.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.36/test.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/config-center.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/misc.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/vcs.xml
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.36/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.36/cfgc/__init__.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 config_center-0.0.36/cfgc/center.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.36/cfgc/envs/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.36/LICENSE.txt
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.36/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 config_center-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 config_center-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.39/MAINFEST.in
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.39/readme.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.39/test.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/config-center.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/vcs.xml
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/__init__.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/center.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/envs/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.39/LICENSE.txt
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.39/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 config_center-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 config_center-0.0.39/PKG-INFO
```

### Comparing `config_center-0.0.36/readme.md` & `config_center-0.0.39/readme.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/test.py` & `config_center-0.0.39/test.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/.idea/workspace.xml` & `config_center-0.0.39/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `config_center-0.0.36/.idea/workspace.xml` & `config_center-0.0.39/.idea/workspace.xml`

```diff
@@ -76,15 +76,15 @@
       <created>1716036017945</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1716036017945</updated>
       <workItem from="1716036020520" duration="187000"/>
       <workItem from="1716036371070" duration="1933000"/>
       <workItem from="1716102721317" duration="114000"/>
-      <workItem from="1716104323900" duration="249000"/>
+      <workItem from="1716104323900" duration="440000"/>
     </task>
     <task id="LOCAL-00001" summary="building... 🏗️">
       <created>1716036119683</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1716036119683</updated>
```

### Comparing `config_center-0.0.36/cfgc/__init__.py` & `config_center-0.0.39/cfgc/__init__.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/cfgc/center.py` & `config_center-0.0.39/cfgc/center.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/cfgc/envs/__init__.py` & `config_center-0.0.39/cfgc/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/LICENSE.txt` & `config_center-0.0.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/README.md` & `config_center-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.36/pyproject.toml` & `config_center-0.0.39/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["cfgc"]
 
 [project] 
 name = "config-center"
-version = "0.0.36"
+version = "0.0.39"
 keywords = ["config", "pipeline", "local", "tool"]
 description = "A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">= 3.4"
 dependencies = [
   "importlib",
   "pathlib",
   "pickle",
-  "shutil",
 ]
 authors = [
   {name = "VaterFus", email = "1107818699@qq.com"},
 ]
 
 [project.urls]
 Repository = "https://github.com/WhatMelonGua/config-center"
```

### Comparing `config_center-0.0.36/PKG-INFO` & `config_center-0.0.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.3
 Name: config-center
-Version: 0.0.36
+Version: 0.0.39
 Summary: A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!
 Project-URL: Repository, https://github.com/WhatMelonGua/config-center
 Author-email: VaterFus <1107818699@qq.com>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: config,local,pipeline,tool
 Requires-Python: >=3.4
 Requires-Dist: importlib
 Requires-Dist: pathlib
 Requires-Dist: pickle
-Requires-Dist: shutil
 Description-Content-Type: text/markdown
 
 ## **<u>CFGC</u>**  构建自己本地的 PYPI
 
 **快速构建项目的自定义python运行环境**
 
 ------
```

