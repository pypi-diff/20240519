# Comparing `tmp/cstructs-0.2.3.tar.gz` & `tmp/cstructs-0.2.5.tar.gz`

## Comparing `cstructs-0.2.3.tar` & `cstructs-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,34 @@
--rw-r--r--   0        0        0    23005 2020-02-02 00:00:00.000000 cstructs-0.2.3/cstructs-0.2.1-py3-none-any.whl
--rw-r--r--   0        0        0    86072 2020-02-02 00:00:00.000000 cstructs-0.2.3/cstructs-0.2.1.tar.gz
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 cstructs-0.2.3/cstructs-0.2.2-py3-none-any.whl
--rw-r--r--   0        0        0   140837 2020-02-02 00:00:00.000000 cstructs-0.2.3/cstructs-0.2.2.tar.gz
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 cstructs-0.2.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/.gitignore
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/cstructs.iml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/discord.xml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/modules.xml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/vcs.xml
--rw-r--r--   0        0        0    28018 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/workspace.xml
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/copyright/gplv3.xml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/copyright/profiles_settings.xml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM__Changes_.xml
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 cstructs-0.2.3/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cstructs-0.2.3/docs/nativetypes
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/__about__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/exc.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/nativetypes.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/util.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/datastruct/__init__.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 cstructs-0.2.3/src/cstructs/datastruct/metadata.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_decorator.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_inheritance.py
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_metaclass.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_metadata.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_read.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 cstructs-0.2.3/tests/test_write.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cstructs-0.2.3/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 cstructs-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 cstructs-0.2.3/README.md
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 cstructs-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cstructs-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 cstructs-0.2.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/.gitignore
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/cstructs.iml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/discord.xml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/modules.xml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    27257 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/copyright/gplv3.xml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/copyright/profiles_settings.xml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM__Changes_.xml
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 cstructs-0.2.5/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cstructs-0.2.5/docs/nativetypes
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/__about__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/exc.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/nativetypes.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/util.py
+-rw-r--r--   0        0        0    16373 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/datastruct/__init__.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 cstructs-0.2.5/src/cstructs/datastruct/metadata.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_decorator.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_inheritance.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_metaclass.py
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_metadata.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_read.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cstructs-0.2.5/tests/test_write.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cstructs-0.2.5/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 cstructs-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cstructs-0.2.5/README.md
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 cstructs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 cstructs-0.2.5/PKG-INFO
```

### Comparing `cstructs-0.2.3/.github/workflows/run-tests.yml` & `cstructs-0.2.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/.idea/cstructs.iml` & `cstructs-0.2.5/.idea/cstructs.iml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/.idea/workspace.xml` & `cstructs-0.2.5/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `cstructs-0.2.3/.idea/workspace.xml` & `cstructs-0.2.5/.idea/workspace.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="57393ae3-50d6-450c-870a-fbeb47abdc3d" name="Changes" comment="Project cleanup and docstrings added.">
+    <list default="true" id="57393ae3-50d6-450c-870a-fbeb47abdc3d" name="Changes" comment="Update README.md">
       <change beforePath="$PROJECT_DIR$/src/cstructs/__about__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/cstructs/__about__.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -57,15 +57,15 @@
     "ignore.virus.scanning.warn.message": "true",
     "last_opened_file_path": "C:/Users/anthy/Documents/dev/py/cstructs",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "preferences.pluginManager",
+    "settings.editor.selected.configurable": "Errors",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\anthy\Documents\dev\py\cstructs\"/>
     </key>
@@ -114,87 +114,15 @@
       <workItem from="1701985877259" duration="3367000"/>
       <workItem from="1710988496657" duration="646000"/>
       <workItem from="1711200100969" duration="6000"/>
       <workItem from="1713623099607" duration="4160000"/>
       <workItem from="1715727875622" duration="40917000"/>
       <workItem from="1715880880748" duration="2518000"/>
       <workItem from="1715884342597" duration="50000"/>
-      <workItem from="1715884716793" duration="7044000"/>
-    </task>
-    <task id="LOCAL-00019" summary="Adjusted `NativeType` `__repr__`">
-      <option name="closed" value="true"/>
-      <created>1701537964738</created>
-      <option name="number" value="00019"/>
-      <option name="presentableId" value="LOCAL-00019"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701537964738</updated>
-    </task>
-    <task id="LOCAL-00020" summary="Minor changes to `StructMeta`
-The class now has a new field `size` that increments with the size of a typedef each time `add_item` is called.">
-      <option name="closed" value="true"/>
-      <created>1701538176537</created>
-      <option name="number" value="00020"/>
-      <option name="presentableId" value="LOCAL-00020"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701538176537</updated>
-    </task>
-    <task id="LOCAL-00021" summary="Fix `cstructs/datastruct/__init__.py`
-`meta` and `size` fields of a datastruct are now set by the decorator.">
-      <option name="closed" value="true"/>
-      <created>1701538267025</created>
-      <option name="number" value="00021"/>
-      <option name="presentableId" value="LOCAL-00021"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701538267025</updated>
-    </task>
-    <task id="LOCAL-00022" summary="Fix bug
-NameError: name 'item_type' is not defined">
-      <option name="closed" value="true"/>
-      <created>1701538374483</created>
-      <option name="number" value="00022"/>
-      <option name="presentableId" value="LOCAL-00022"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701538374483</updated>
-    </task>
-    <task id="LOCAL-00023" summary="Minor changes
-* Convert the class object into a dataclass
-* Fix bug:
-  * `cstructs.exc.InvalidTypeDef: Invalid type definition for on_read: typing.Callable`">
-      <option name="closed" value="true"/>
-      <created>1701539727891</created>
-      <option name="number" value="00023"/>
-      <option name="presentableId" value="LOCAL-00023"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701539727891</updated>
-    </task>
-    <task id="LOCAL-00024" summary="Revert changes
-Removed the `size` field from `StructMeta` as it breaks the expected behavior of `StructMeta.__getitem__`.">
-      <option name="closed" value="true"/>
-      <created>1701540075458</created>
-      <option name="number" value="00024"/>
-      <option name="presentableId" value="LOCAL-00024"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701540075458</updated>
-    </task>
-    <task id="LOCAL-00025" summary="Fix bug
-Ensure that an attribute is not callable when iterating `StructMeta` instances.">
-      <option name="closed" value="true"/>
-      <created>1701540206769</created>
-      <option name="number" value="00025"/>
-      <option name="presentableId" value="LOCAL-00025"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701540206769</updated>
-    </task>
-    <task id="LOCAL-00026" summary="Implement datastruct `size` attribute">
-      <option name="closed" value="true"/>
-      <created>1701619233860</created>
-      <option name="number" value="00026"/>
-      <option name="presentableId" value="LOCAL-00026"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1701619233860</updated>
+      <workItem from="1715884716793" duration="58775000"/>
     </task>
     <task id="LOCAL-00027" summary="Fix bug
 AttributeError: type object 'Test' has no attribute 'a'">
       <option name="closed" value="true"/>
       <created>1701620260124</created>
       <option name="number" value="00027"/>
       <option name="presentableId" value="LOCAL-00027"/>
@@ -527,15 +455,79 @@
       <option name="closed" value="true"/>
       <created>1715894368021</created>
       <option name="number" value="00067"/>
       <option name="presentableId" value="LOCAL-00067"/>
       <option name="project" value="LOCAL"/>
       <updated>1715894368021</updated>
     </task>
-    <option name="localTasksCounter" value="68"/>
+    <task id="LOCAL-00068" summary="Bump project version">
+      <option name="closed" value="true"/>
+      <created>1715894455781</created>
+      <option name="number" value="00068"/>
+      <option name="presentableId" value="LOCAL-00068"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715894455781</updated>
+    </task>
+    <task id="LOCAL-00069" summary="Update installation instructions in README.md">
+      <option name="closed" value="true"/>
+      <created>1715894564047</created>
+      <option name="number" value="00069"/>
+      <option name="presentableId" value="LOCAL-00069"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715894564047</updated>
+    </task>
+    <task id="LOCAL-00070" summary="Allow datastruct classes to be members of other datastruct classes">
+      <option name="closed" value="true"/>
+      <created>1715897452972</created>
+      <option name="number" value="00070"/>
+      <option name="presentableId" value="LOCAL-00070"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715897452972</updated>
+    </task>
+    <task id="LOCAL-00071" summary="Partial codebase rewrite. Better support for sequences">
+      <option name="closed" value="true"/>
+      <created>1716001997013</created>
+      <option name="number" value="00071"/>
+      <option name="presentableId" value="LOCAL-00071"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716001997013</updated>
+    </task>
+    <task id="LOCAL-00072" summary="Fix failing run `actions/runs/9136890483`.">
+      <option name="closed" value="true"/>
+      <created>1716048759423</created>
+      <option name="number" value="00072"/>
+      <option name="presentableId" value="LOCAL-00072"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716048759423</updated>
+    </task>
+    <task id="LOCAL-00073" summary="Update/add docstrings">
+      <option name="closed" value="true"/>
+      <created>1716088597155</created>
+      <option name="number" value="00073"/>
+      <option name="presentableId" value="LOCAL-00073"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716088597155</updated>
+    </task>
+    <task id="LOCAL-00074" summary="Fix failing run `actions/runs/9144685014`">
+      <option name="closed" value="true"/>
+      <created>1716088741608</created>
+      <option name="number" value="00074"/>
+      <option name="presentableId" value="LOCAL-00074"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716088741608</updated>
+    </task>
+    <task id="LOCAL-00075" summary="Update README.md">
+      <option name="closed" value="true"/>
+      <created>1716091069936</created>
+      <option name="number" value="00075"/>
+      <option name="presentableId" value="LOCAL-00075"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716091069936</updated>
+    </task>
+    <option name="localTasksCounter" value="76"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -545,55 +537,50 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Fix bug
-`TypeError: type.__new__() takes exactly 3 arguments (0 given)`"/>
-    <MESSAGE value="Fix README.md
-Will now attempt to track the build status separate from the master branch."/>
-    <MESSAGE value="Fix bug
-`cstructs.exc.InvalidTypeDef: Invalid type definition for on_read: typing.Callable`"/>
-    <MESSAGE value="Fix bug
-`TypeError: type.__new__() takes exactly 3 arguments (1 given)`"/>
-    <MESSAGE value="Major changes
-datastruct classes are no longer callable as this interferes a lot with the underlying dataclass among other issues."/>
-    <MESSAGE value="New NativeType &quot;padding&quot;"/>
-    <MESSAGE value="Extra NativeTypes"/>
     <MESSAGE value="Extra NativeTypes, finally finished implementing read"/>
     <MESSAGE value="Add proper string reading. Can now specify which encoding to use for `char`."/>
     <MESSAGE value="Disable flake8 fatal error(for now)"/>
     <MESSAGE value="Begin work on improving typehints"/>
     <MESSAGE value="Typehints improved. New format: `Annotation[typedef, repeat_count[, encoding]]`"/>
     <MESSAGE value="Fixed improper syntax for Annotated. New format is `Annotated[python_type, typedef, repeat_count[, encoding]]`"/>
     <MESSAGE value="Modified Annotated format. New format: `Annotated[python_type, typedef(repeat_count, encoding: str = &quot;ascii&quot;]`"/>
     <MESSAGE value="Update README.md with new read feature."/>
     <MESSAGE value="Begin work for serializing DataStructs back into raw data."/>
     <MESSAGE value="Successful implementation of basic serialization"/>
     <MESSAGE value="Finished serialization implementation"/>
-    <MESSAGE value="Update README.md"/>
     <MESSAGE value="Begin r/w hook implementation"/>
     <MESSAGE value="Finish r/w hook implementation"/>
     <MESSAGE value="Add inheritance test"/>
     <MESSAGE value="Update usage examples in README.md"/>
     <MESSAGE value="Bump version to 0.2.2 and fix urls in pyproject.toml"/>
     <MESSAGE value="Project cleanup and docstrings added."/>
-    <option name="LAST_COMMIT_MESSAGE" value="Project cleanup and docstrings added."/>
+    <MESSAGE value="Bump project version"/>
+    <MESSAGE value="Update installation instructions in README.md"/>
+    <MESSAGE value="Allow datastruct classes to be members of other datastruct classes"/>
+    <MESSAGE value="Partial codebase rewrite. Better support for sequences"/>
+    <MESSAGE value="Fix failing run `actions/runs/9136890483`."/>
+    <MESSAGE value="Update/add docstrings"/>
+    <MESSAGE value="Fix failing run `actions/runs/9144685014`"/>
+    <MESSAGE value="Update README.md"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Update README.md"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/cstructs/nativetypes.py</url>
-          <line>120</line>
-          <option name="timeStamp" value="2"/>
+          <url>file://$PROJECT_DIR$/tests/test_read.py</url>
+          <line>124</line>
+          <option name="timeStamp" value="46"/>
         </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
-    <SUITE FILE_PATH="coverage/cstructs$pytest_in_cstructs.coverage" NAME="pytest in cstructs Coverage Results" MODIFIED="1715894317502" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/cstructs$pytest_in_cstructs.coverage" NAME="pytest in cstructs Coverage Results" MODIFIED="1716088664426" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
     <SUITE FILE_PATH="coverage/cstructs$__init__.coverage" NAME="__init__ Coverage Results" MODIFIED="1701484236652" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/cstructs/datastruct"/>
   </component>
 </project>
```

### Comparing `cstructs-0.2.3/.idea/copyright/gplv3.xml` & `cstructs-0.2.5/.idea/copyright/gplv3.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/.idea/copyright/profiles_settings.xml` & `cstructs-0.2.5/.idea/copyright/profiles_settings.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/.idea/inspectionProfiles/Project_Default.xml` & `cstructs-0.2.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch` & `cstructs-0.2.5/.idea/shelf/Uncommitted_changes_before_Update_at_5_16_2024_2_44_PM_[Changes]/shelved.patch`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/docs/nativetypes` & `cstructs-0.2.5/docs/nativetypes`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/src/cstructs/__about__.py` & `cstructs-0.2.5/src/cstructs/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A     -
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 
-__version__ = "0.2.3"
+__version__ = "0.2.5"
```

### Comparing `cstructs-0.2.3/src/cstructs/__init__.py` & `cstructs-0.2.5/src/cstructs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,13 +9,19 @@
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY     -
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A     -
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
-from cstructs.datastruct import datastruct as backend_datastruct, DataStruct
+from cstructs.datastruct import (
+    datastruct as backend_datastruct,
+    DataStruct,
+    Sequence,
+    Member,
+    MemberRef,
+)
 from cstructs.nativetypes import NativeTypes
 
 
 def datastruct(*args, **kwargs):
     return backend_datastruct(*args, **kwargs)
```

### Comparing `cstructs-0.2.3/src/cstructs/exc.py` & `cstructs-0.2.5/src/cstructs/exc.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,39 @@
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 class InvalidByteOrder(Exception):
     """
     Exception raised when an invalid byte order is encountered.
     """
+
     pass
 
 
 class InvalidTypeDef(Exception):
     """
     Exception raised when an invalid type definition is encountered.
     """
+
+    pass
+
+
+class SequenceLengthMismatch(Exception):
+    """
+    Exception raised when the length of a Sequence does not match the expected length.
+    """
+
+    pass
+
+
+class InvalidSequence(Exception):
+    """
+    Exception raised when an invalid Sequence is encountered.
+    """
     pass
 
 
-class ByteStringLengthMismatch(Exception):
+class InvalidMember(Exception):
     """
-    Exception raised when the length of a byte string does not match the expected length.
+    Exception raised when an invalid Member is encountered.
     """
     pass
```

### Comparing `cstructs-0.2.3/src/cstructs/nativetypes.py` & `cstructs-0.2.5/src/cstructs/nativetypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,71 +12,59 @@
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 import typing
 import struct
 
-from cstructs.exc import InvalidTypeDef, ByteStringLengthMismatch
+from cstructs.exc import InvalidTypeDef, SequenceLengthMismatch
 
 
 class NativeType:
     def __init__(
         self,
         name: str,
         size: int | None,
         python_type: type,
         struct_type: str,
         signed: bool,
-        repeat_length: int = 1,
         encoding: str = "ascii",
         enforce_length: bool = False,
     ):
         self.name = name
         self.size = size
         self.python_type = python_type
         self.struct_type = struct_type
         self.signed = signed
 
-        # repeat length is set in the __call__ method
-        self.repeat_length = repeat_length
-
         # encoding is set in the __call__ method. it is used only by NativeTypes.char
         self.encoding = encoding
         self.enforce_length = enforce_length
 
     def __call__(
-        self, repeat_length: int, encoding: str = "ascii", enforce_length: bool = False
+        self,
+        encoding: str = "ascii",
+        enforce_length: bool = False,
     ):
         """
-        Create a new instance of the native type with the specified repeat length, encoding, and enforce length option.
+        Create a new instance of the native type with the specified encoding and length enforcement.
 
         Args:
-            repeat_length (int): The number of times the native type repeats in the data.
-            encoding (str, optional): The character encoding to use for string types. Defaults to "ascii".
-            enforce_length (bool, optional): Whether to enforce the length of the repeated native type. Defaults to False.
+            encoding (str, optional): The encoding to be used for string conversions. Defaults to "ascii".
+            enforce_length (bool, optional): Whether to enforce the length of the native type. Defaults to False.
 
         Returns:
-            NativeType: A new instance of the native type with the specified repeat length, encoding, and enforce length option.
-
-        Raises:
-            InvalidTypeDef: If the repeat length is less than or equal to 0.
+            NativeType: A new instance of the native type with the specified encoding and length enforcement.
         """
-        if repeat_length <= 0:
-            raise InvalidTypeDef(
-                f"repeat length must be greater than 0, got {repeat_length}"
-            )
-
         return type(self)(
             self.name,
             self.size,
             self.python_type,
             self.struct_type,
             self.signed,
-            repeat_length,
             encoding,
             enforce_length,
         )
 
     def __eq__(self, other):
         return (
             hasattr(other, "name")
@@ -88,88 +76,88 @@
             and hasattr(other, "struct_type")
             and self.struct_type == other.struct_type
             and hasattr(other, "signed")
             and self.signed == other.signed
         )
 
     def __repr__(self):
-        return f"NativeType(typedef={self.name}, size={self.size}, repeat_length={self.repeat_length})"
+        return (
+            f"NativeType(typedef={self.name}, "
+            f"size={self.size}, "
+            f"python_type={self.python_type}, "
+            f"struct_type={self.struct_type}, "
+            f"signed={self.signed}, "
+            f"encoding={self.encoding}, "
+            f"enforce_length={self.enforce_length}"
+            ")"
+        )
 
     def __str__(self):
         return self.name
 
     def read(self, stream: typing.BinaryIO, byteorder: str):
         """
         Reads data from the given stream according to the specified byte order.
 
         Args:
             stream (typing.BinaryIO): The binary stream to read from.
             byteorder (str): The byte order to use for reading the data.
 
         Returns:
-            The read data, based on the type and byte order.
+            The read data, based on the type of the native type.
 
         Raises:
             None.
         """
+
         if self.name == "char":
-            return stream.read(self.repeat_length).decode(self.encoding)
+            return stream.read(self.size).decode(self.encoding)
         if self.name in ("pad", "bytestring"):
-            return stream.read(self.repeat_length)
+            return stream.read(self.size)
 
-        format_str = f"{byteorder}{self.repeat_length}{self.struct_type}"
+        format_str = f"{byteorder}{self.struct_type}"
 
-        return struct.unpack(format_str, stream.read(self.size * self.repeat_length))[0]
+        return struct.unpack(format_str, stream.read(self.size))
 
-    def serialize(self, value, byteorder: str) -> bytes:
+    def serialize(self, value: typing.Any, byteorder: str) -> bytes:
         """
-        Serializes the given value into bytes according to the specified byte order.
+        Serializes the given value into bytes using the specified byte order.
 
         Args:
-            value: The value to be serialized.
-            byteorder: The byte order to be used for serialization.
+            value (typing.Any): The value to be serialized.
+            byteorder (str): The byte order to be used for serialization.
 
         Returns:
             The serialized value as bytes.
 
         Raises:
-            ByteStringLengthMismatch: If the length of the value does not match the repeat length
-                and length enforcement is enabled.
+            None.
         """
         if self.name == "char":
             if value is None:
-                return b"\x00" * self.repeat_length
-
-            if len(value) != self.repeat_length and self.enforce_length:
-                raise ByteStringLengthMismatch(f"{len(value)} != {self.repeat_length}")
+                return b"\x00" * self.size
 
             return value.encode(self.encoding)
         if self.name == "bytestring":
             if value is None:
-                return b"\x00" * self.repeat_length
-
-            if len(value) != self.repeat_length and self.enforce_length:
-                raise ByteStringLengthMismatch(f"{len(value)} != {self.repeat_length}")
+                return b"\x00" * self.size
 
             return value
         if self.name == "pad":
-            if len(value) != self.repeat_length and self.enforce_length:
-                raise ByteStringLengthMismatch(f"{len(value)} != {self.repeat_length}")
-
-            return b"\x00" * self.repeat_length
+            return b"\x00" * self.size
 
         if value is None:
             if self.python_type is float:
                 value = 0.0
             elif self.python_type is bool:
                 value = False
             else:
                 value = 0
 
-        format_str = f"{byteorder}{self.repeat_length}{self.struct_type}"
+        format_str = f"{byteorder}{self.struct_type}"
         value &= (1 << (self.size * 8)) - 1
 
         if self.signed:
             bit_length = self.size * 8
             sign_bit = 1 << (bit_length - 1)
 
             if value & sign_bit:
@@ -215,16 +203,16 @@
     int16 = NativeType("int16", 2, int, "h", True)
     int8 = NativeType("int8", 1, int, "b", True)
     double = NativeType("double", 8, float, "d", False)
     float = NativeType("float", 4, float, "f", False)
     char = NativeType("char", 1, str, "s", False)
     bool = NativeType("bool", 1, bool, "?", False)
 
-    bytestring = NativeType("bytestring", None, bytes, "", False)
-    pad = NativeType("pad", None, type(None), "", False)
+    bytestring = NativeType("bytestring", 1, bytes, "", False)
+    pad = NativeType("pad", 1, type(None), "", False)
 
     u64 = uint64
     u32 = uint32
     u16 = uint16
     u8 = uint8
     i64 = int64
     i32 = int32
```

### Comparing `cstructs-0.2.3/src/cstructs/util.py` & `cstructs-0.2.5/src/cstructs/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 
     Args:
         cls (type): The class to check.
 
     Returns:
         bool: True if the class is a data structure, False otherwise.
     """
-    return cls.__qualname__.startswith("cstructs.datastruct.")
+    return hasattr(cls, "__qualname__") and cls.__qualname__.startswith(
+        "cstructs.datastruct."
+    )
```

### Comparing `cstructs-0.2.3/src/cstructs/datastruct/metadata.py` & `cstructs-0.2.5/src/cstructs/datastruct/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,42 +9,42 @@
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY     -
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A     -
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
+from __future__ import annotations
+
 import enum
+import copy
 import typing
 
 from dataclasses import dataclass
 from cstructs.nativetypes import NativeType
 from cstructs.util import is_datastruct
 
+from collections.abc import Iterator
+
+if typing.TYPE_CHECKING:
+    from cstructs.datastruct import Sequence, DataStruct
+
 
 @dataclass
 class MetadataItem:
-    """
-    Represents a metadata item with name, type, size, offset, and value.
-
-    Attributes:
-        name (str): The name of the metadata item.
-        type (NativeType): The type of the metadata item.
-        size (int): The size of the metadata item.
-        offset (int): The offset of the metadata item.
-        value (Any): The value of the metadata item.
-    """
 
     name: str
-    type: NativeType
+    type: NativeType | DataStruct
     size: int
+    sequence: typing.Optional[Sequence]
 
     # these fields are set later on
+    default: typing.Optional[typing.Any] = None
     offset: int = None
-    value: typing.Any = None
+    value: typing.Any | list | typing.Generator = None
 
     def __repr__(self):
         return str(self.__dict__)
 
     def __str__(self):
         """
         Returns a string representation of the Metadata object.
@@ -86,26 +86,43 @@
             item (MetadataItem): The MetadataItem to be added.
 
         Returns:
             None
         """
         setattr(self, item.name, item)
 
-    def __iter__(self):
+    def clone(self) -> typing.Self:
+        """
+        Creates a deep copy of the current instance.
+
+        Returns:
+            A new instance of the same type as the current instance, with all items deeply copied.
+        """
+        copy_metadata: StructMeta = type(self)()
+
+        for item in self:
+            copy_metadata.add_item(copy.deepcopy(item))
+
+        return copy_metadata
+
+    def __contains__(self, item):
+        return hasattr(self, item)
+
+    def __iter__(self) -> Iterator[MetadataItem]:
         """
         Iterates over the attributes of the object and yields their values.
 
         Yields:
             Any: The value of each non-callable attribute of the object.
         """
         for attr in dir(self):
             if not attr.startswith('__') and not callable(getattr(self, attr)):
                 yield getattr(self, attr)
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> MetadataItem:
         """
         Retrieve the value associated with the given item.
 
         If the item is a string, it is assumed to be the name of an attribute
         and the corresponding value is returned. If the item is an integer,
         it is treated as an index and the value at that index in the internal
         dictionary is returned.
```

### Comparing `cstructs-0.2.3/tests/__init__.py` & `cstructs-0.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/tests/test_decorator.py` & `cstructs-0.2.5/tests/test_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,32 @@
 import pytest
 
 from cstructs import datastruct
 from cstructs.exc import InvalidByteOrder
 
 
 def test_bare_decorator_call():
+    """
+    Test case for a bare decorator call.
+    """
     @datastruct
     class Test:
         pass
 
 
 def fn_decorator_call_with_byteorder(byteorder: str):
     @datastruct(byteorder=byteorder)
     class Test:
         pass
 
 
 def test_decorator_call_with_byteorder():
+    """
+    Test the decorator with different byte orders.
+    """
     fn_decorator_call_with_byteorder("little")
     fn_decorator_call_with_byteorder("big")
     fn_decorator_call_with_byteorder("native")  # native is the default
     fn_decorator_call_with_byteorder("network")
 
     # test improper byteorder
     with pytest.raises(InvalidByteOrder):
```

### Comparing `cstructs-0.2.3/tests/test_inheritance.py` & `cstructs-0.2.5/tests/test_metaclass.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,47 +9,64 @@
 #  This program is distributed in the hope that it will be useful, but WITHOUT ANY     -
 #  WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A     -
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
+import pytest
 import io
 
-from cstructs import datastruct, DataStruct, NativeTypes
+from cstructs import datastruct, DataStruct
+from cstructs.datastruct.metadata import StructMeta
 
 
-def test_inheritance():
+def test_metaclass():
     """
-    Test case for inheritance in datastructs.
+    Test case for the metaclass functionality.
 
-    This test case defines two classes, `Test` and `Test2`, which inherit from each other.
-    The `Test` class has two attributes, `a` and `b`, both of type `uint32`.
-    The `Test2` class inherits from `Test` and adds an additional attribute `c` of type `u8`.
-    The `on_read` method of `Test2` is defined to perform assertions on the values of `a`, `b`, and `c`.
-
-    The test case writes some data to a `BytesIO` stream and then reads it using the `read` method of `Test`.
-    The assertions in the `on_read` method of `Test2` validate that the values read from the stream are correct.
+    This test case checks that the metaclass transforms the class qualname,
+    adds the required fields, initializes them correctly, and ensures that
+    the read function only accepts the stream argument.
     """
-
-    @datastruct(byteorder="big")
+    @datastruct
     class Test(metaclass=DataStruct):
-        a: NativeTypes.uint32
-        b: NativeTypes.uint32
-
-    @datastruct(byteorder="big")
-    class Test2(Test, metaclass=DataStruct):
-        c: NativeTypes.u8
-
-        def on_read(self):
-            assert self.a == 1
-            assert self.b == 2
-            assert self.c == 3
-
-    stream = io.BytesIO()
-    stream.write(b"00 00 00 01")
-    stream.write(b"00 00 00 02")
-    stream.write(b"03")
+        pass
 
-    stream.seek(0)
+    # check that the metaclass transforms the class qualname
+    # this serves as a marker for classes that have been transformed
+    # by the metaclass.
+    assert Test.__qualname__ == "cstructs.datastruct.Test"
+
+    # check that the metaclass adds the following fields:
+    # - on_read: a callback function that is called after the struct is read
+    # - on_write: a callback function that is called after the struct is written
+    # - meta: a collection of member metadata
+    # - byteorder: the byteorder of the struct
+    # - size: the size of the struct
+    assert hasattr(Test, "on_read")
+    assert hasattr(Test, "on_write")
+    assert hasattr(Test, "meta")
+    assert hasattr(Test, "byteorder")
+    assert hasattr(Test, "size")
+
+    # on_read and on_write should both be initialized to None if the user does not
+    # provide a callback function.
+    assert Test.on_read is None
+    assert Test.on_write is None
+
+    # byteorder should NOT be None.
+    assert Test.byteorder is not None
+
+    # size should always be 0 for now.
+    assert Test.size == 0
+
+    # ensure that the only argument of the read function is the stream we
+    # want to read from.
+    with pytest.raises(TypeError):
+        Test.read()
+    with pytest.raises(TypeError):
+        Test.read(1, 2, 3)
+    with pytest.raises(TypeError):
+        Test.read(None)
 
-    Test.read(stream)
+    Test.read(io.BytesIO(b""))
```

### Comparing `cstructs-0.2.3/tests/test_metadata.py` & `cstructs-0.2.5/tests/test_metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,27 +13,22 @@
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 import pytest
 
 from cstructs.datastruct.metadata import StructMeta, MetadataItem
 from cstructs.exc import InvalidTypeDef
-from cstructs import datastruct, DataStruct, NativeTypes
+from cstructs import datastruct, DataStruct, NativeTypes, Sequence, Member
 
 from typing import Annotated
 
 
 def test_struct_meta_empty_class():
     """
     Test case to verify the behavior of metadata for an empty datastruct.
-
-    This test case checks that the metadata for an empty datastruct is correctly
-    created and accessible. It verifies that the `meta` attribute of the class
-    is not None and is an instance of `StructMeta`. It also ensures that the
-    metadata is iterable by iterating over it.
     """
 
     @datastruct
     class Test(metaclass=DataStruct):
         pass
 
     # meta should NOT be None and should be an instance of StructMeta
@@ -43,22 +38,20 @@
     for item in Test.meta:
         pass
 
 
 def test_struct_meta_class_with_fields():
     """
     This test ensures that the metadata behaves like a sequence and implements dict-like behavior for metadata items.
-    It also verifies that the metadata fields are accessible as instance fields and that each metadata item has a name, type, and size field.
-    Additionally, it checks the correctness of the size of the bytestring field.
     """
 
     @datastruct
     class Test(metaclass=DataStruct):
         a: NativeTypes.uint32
-        b: Annotated[bytes, NativeTypes.bytestring(8)]
+        b: Annotated[bytes, Member(NativeTypes.bytestring, Sequence(8))]
 
     # ensure that meta behaves like a sequence
     assert isinstance(Test.meta[0], MetadataItem)
     assert isinstance(Test.meta[1], MetadataItem)
 
     # ensure that the metadata also implements dict-like behavior
     assert isinstance(Test.meta["a"], MetadataItem)
@@ -97,29 +90,29 @@
         AssertionError: If any of the assertions fail.
     """
 
     @datastruct
     class Test(metaclass=DataStruct):
         a: NativeTypes.uint32
         b: NativeTypes.u32
-        c: Annotated[int, NativeTypes.uint16(4)]
+        c: Annotated[list, Member(NativeTypes.uint16, Sequence(4))]
         d: NativeTypes.u16
         e: NativeTypes.uint8
         f: NativeTypes.u8
         g: NativeTypes.int32
         h: NativeTypes.i32
         i: NativeTypes.int16
         j: NativeTypes.i16
         k: NativeTypes.int8
         l: NativeTypes.i8
         m: NativeTypes.float
         n: NativeTypes.double
         o: NativeTypes.bool
         p: NativeTypes.char
-        q: Annotated[bytes, NativeTypes.bytestring(10)]
+        q: Annotated[bytes, Member(NativeTypes.bytestring, Sequence(10))]
         r: NativeTypes.uint64
         s: NativeTypes.u64
         t: NativeTypes.int64
         u: NativeTypes.i64
 
     # ensure that the metadata fields are also instance fields
     assert isinstance(Test.meta.a, MetadataItem)
```

### Comparing `cstructs-0.2.3/tests/test_write.py` & `cstructs-0.2.5/tests/test_write.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 #  PARTICULAR PURPOSE. See the GNU General Public License for more details.            -
 #                                                                                      -
 #  You should have received a copy of the GNU General Public License along with        -
 #  this program. If not, see <http://www.gnu.org/licenses/>.                           -
 # --------------------------------------------------------------------------------------
 import pytest
 
-from cstructs import datastruct, NativeTypes, DataStruct
-from cstructs.exc import ByteStringLengthMismatch
+from cstructs import datastruct, NativeTypes, DataStruct, Member, Sequence
+from cstructs.exc import SequenceLengthMismatch
 from typing import Annotated
 
 
 def test_write_basic():
     """
     Test case for basic write functionality of a datastruct.
     """
@@ -49,29 +49,23 @@
 
     assert hexstr == bytes.fromhex("01FF").hex()
 
 
 def test_write_complex():
     """
     Test case for serializing a complex datastruct.
-
-    Raises:
-        ByteStringLengthMismatch: If the length of the `d` field is not equal to 6.
-
-    Returns:
-        None
     """
 
     @datastruct(byteorder="big")
     class Test(metaclass=DataStruct):
         a: NativeTypes.uint32
         b: NativeTypes.i8
         c: NativeTypes.char
-        d: Annotated[str, NativeTypes.char(6, enforce_length=True)]
-        e: Annotated[bytes, NativeTypes.bytestring(8)]
+        d: Annotated[str, Member(NativeTypes.char, Sequence(6, enforce_length=True))]
+        e: Annotated[bytes, Member(NativeTypes.bytestring, Sequence(8))]
 
     test = Test.init_empty()
 
     test.a = 1
 
     # ensure all None values get properly encoded to 0(null)
     # fmt: off
@@ -97,11 +91,11 @@
         "21"
         "41 6E 74 68 79 21"
         "00 01 02 03 04 05 06 07"
     )
     # fmt: on
 
     # ensure that mismatching lengths are reported
-    with pytest.raises(ByteStringLengthMismatch):
+    with pytest.raises(SequenceLengthMismatch):
         test.d = "Anthy!!!"
 
         test.serialize()
```

### Comparing `cstructs-0.2.3/.gitignore` & `cstructs-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/LICENSE.txt` & `cstructs-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cstructs-0.2.3/pyproject.toml` & `cstructs-0.2.5/pyproject.toml`

 * *Files identical despite different names*

