# Comparing `tmp/config_center-0.0.39.tar.gz` & `tmp/config_center-0.0.40.tar.gz`

## Comparing `config_center-0.0.39.tar` & `config_center-0.0.40.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.39/MAINFEST.in
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.39/readme.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.39/test.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/config-center.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/misc.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/vcs.xml
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.39/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/__init__.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/center.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.39/cfgc/envs/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.39/LICENSE.txt
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.39/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 config_center-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 config_center-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.40/MAINFEST.in
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40/readme.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40/test.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/config-center.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/vcs.xml
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.40/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.40/cfgc/__init__.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 config_center-0.0.40/cfgc/center.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40/cfgc/envs/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.40/LICENSE.txt
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40/README.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 config_center-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 config_center-0.0.40/PKG-INFO
```

### Comparing `config_center-0.0.39/readme.md` & `config_center-0.0.40/readme.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/test.py` & `config_center-0.0.40/test.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/.idea/workspace.xml` & `config_center-0.0.40/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `config_center-0.0.39/.idea/workspace.xml` & `config_center-0.0.40/.idea/workspace.xml`

```diff
@@ -1,13 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="3aef8cc2-14b5-468e-8927-eb128873056f" name="默认变更列表" comment="building... 🏗️">
-      <change beforePath="$PROJECT_DIR$/dist/config_center-0.0.1a5-py3-none-any.whl" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/dist/config_center-0.0.1a5.tar.gz" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -76,15 +74,15 @@
       <created>1716036017945</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1716036017945</updated>
       <workItem from="1716036020520" duration="187000"/>
       <workItem from="1716036371070" duration="1933000"/>
       <workItem from="1716102721317" duration="114000"/>
-      <workItem from="1716104323900" duration="440000"/>
+      <workItem from="1716104323900" duration="563000"/>
     </task>
     <task id="LOCAL-00001" summary="building... 🏗️">
       <created>1716036119683</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1716036119683</updated>
@@ -127,15 +125,22 @@
     <task id="LOCAL-00007" summary="building... 🏗️">
       <created>1716037720187</created>
       <option name="number" value="00007"/>
       <option name="presentableId" value="LOCAL-00007"/>
       <option name="project" value="LOCAL"/>
       <updated>1716037720187</updated>
     </task>
-    <option name="localTasksCounter" value="8"/>
+    <task id="LOCAL-00008" summary="building... 🏗️">
+      <created>1716104848807</created>
+      <option name="number" value="00008"/>
+      <option name="presentableId" value="LOCAL-00008"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716104848807</updated>
+    </task>
+    <option name="localTasksCounter" value="9"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -148,13 +153,14 @@
       </map>
     </option>
     <option name="oldMeFiltersMigrated" value="true"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="building... ️"/>
     <MESSAGE value="building... ️"/>
+    <MESSAGE value="building... ️"/>
     <option name="LAST_COMMIT_MESSAGE" value="building... ️"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/config_center$test.coverage" NAME="test 覆盖结果" MODIFIED="1716036960838" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
   </component>
 </project>
```

### Comparing `config_center-0.0.39/cfgc/__init__.py` & `config_center-0.0.40/cfgc/__init__.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/cfgc/center.py` & `config_center-0.0.40/cfgc/center.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/cfgc/envs/__init__.py` & `config_center-0.0.40/cfgc/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/LICENSE.txt` & `config_center-0.0.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/README.md` & `config_center-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.39/pyproject.toml` & `config_center-0.0.40/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["cfgc"]
 
 [project] 
 name = "config-center"
-version = "0.0.39"
+version = "0.0.40"
 keywords = ["config", "pipeline", "local", "tool"]
 description = "A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">= 3.4"
 dependencies = [
   "importlib",
   "pathlib",
-  "pickle",
 ]
 authors = [
   {name = "VaterFus", email = "1107818699@qq.com"},
 ]
 
 [project.urls]
 Repository = "https://github.com/WhatMelonGua/config-center"
```

### Comparing `config_center-0.0.39/PKG-INFO` & `config_center-0.0.40/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.3
 Name: config-center
-Version: 0.0.39
+Version: 0.0.40
 Summary: A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!
 Project-URL: Repository, https://github.com/WhatMelonGua/config-center
 Author-email: VaterFus <1107818699@qq.com>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: config,local,pipeline,tool
 Requires-Python: >=3.4
 Requires-Dist: importlib
 Requires-Dist: pathlib
-Requires-Dist: pickle
 Description-Content-Type: text/markdown
 
 ## **<u>CFGC</u>**  构建自己本地的 PYPI
 
 **快速构建项目的自定义python运行环境**
 
 ------
```

