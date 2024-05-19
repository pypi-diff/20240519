# Comparing `tmp/binary_to_text-0.0.1.tar.gz` & `tmp/binary_to_text-0.0.2.tar.gz`

## Comparing `binary_to_text-0.0.1.tar` & `binary_to_text-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/btt.iml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/src/binary_to_text/__init__.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/src/binary_to_text/main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/README.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 binary_to_text-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/btt.iml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/src/binary_to_text/__init__.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/src/binary_to_text/main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/LICENSE
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/README.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 binary_to_text-0.0.2/PKG-INFO
```

### Comparing `binary_to_text-0.0.1/.idea/workspace.xml` & `binary_to_text-0.0.2/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `binary_to_text-0.0.1/.idea/workspace.xml` & `binary_to_text-0.0.2/.idea/workspace.xml`

```diff
@@ -13,22 +13,27 @@
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
-  <component name="ProjectColorInfo"><![CDATA[{
-  "associatedIndex": 3
-}]]></component>
+  <component name="ProjectColorInfo">{
+  &quot;associatedIndex&quot;: 3
+}</component>
   <component name="ProjectId" id="2geP9Cd0D24MRj0UBNESrQHrKI3"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToStringList": {
+    "stardust.markdown.MarkdownSplitEditorSuppressor:keyList": []
+  }
+}]]></component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
         <option value="bundled-python-sdk-0509580d9d50-746f403e7f0c-com.jetbrains.pycharm.community.sharedIndexes.bundled-PC-241.14494.241"/>
       </set>
     </attachedChunks>
   </component>
```

### Comparing `binary_to_text-0.0.1/src/binary_to_text/main.py` & `binary_to_text-0.0.2/src/binary_to_text/main.py`

 * *Files identical despite different names*

### Comparing `binary_to_text-0.0.1/LICENSE` & `binary_to_text-0.0.2/LICENSE`

 * *Files identical despite different names*

