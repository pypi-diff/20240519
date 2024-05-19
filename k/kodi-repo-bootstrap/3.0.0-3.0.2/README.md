# Comparing `tmp/kodi_repo_bootstrap-3.0.0.tar.gz` & `tmp/kodi_repo_bootstrap-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodi_repo_bootstrap-3.0.0.tar", max compression
+gzip compressed data, was "kodi_repo_bootstrap-3.0.2.tar", max compression
```

## Comparing `kodi_repo_bootstrap-3.0.0.tar` & `kodi_repo_bootstrap-3.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    18047 2024-02-13 14:16:56.129688 kodi_repo_bootstrap-3.0.0/LICENSE
--rw-r--r--   0        0        0     2654 2024-02-13 14:16:56.129688 kodi_repo_bootstrap-3.0.0/README.md
--rw-r--r--   0        0        0        0 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/__init__.py
--rw-r--r--   0        0        0       48 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/__main__.py
--rw-r--r--   0        0        0        0 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/addon/__init__.py
--rw-r--r--   0        0        0     9046 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/addon/addon.py
--rw-r--r--   0        0        0     3601 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/addon/manager.py
--rw-r--r--   0        0        0        0 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/cli/__init__.py
--rw-r--r--   0        0        0     3458 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/cli/args.py
--rw-r--r--   0        0        0        0 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/fs/__init__.py
--rw-r--r--   0        0        0      957 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/fs/dir.py
--rw-r--r--   0        0        0     1010 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/fs/file.py
--rw-r--r--   0        0        0      470 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/main.py
--rw-r--r--   0        0        0        0 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/__init__.py
--rw-r--r--   0        0        0     5222 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/config.py
--rw-r--r--   0        0        0     4506 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/manager.py
--rw-r--r--   0        0        0     4019 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/version.py
--rw-r--r--   0        0        0      740 2024-02-13 14:16:56.133689 kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/res/repo_addon.xml.tpl
--rw-r--r--   0        0        0      743 2024-02-13 14:17:10.973850 kodi_repo_bootstrap-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 kodi_repo_bootstrap-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18047 2024-05-19 20:38:38.132459 kodi_repo_bootstrap-3.0.2/LICENSE
+-rw-r--r--   0        0        0     2686 2024-05-19 20:38:38.132459 kodi_repo_bootstrap-3.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 20:38:38.132459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-19 20:38:38.132459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/addon/__init__.py
+-rw-r--r--   0        0        0     9046 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/addon/addon.py
+-rw-r--r--   0        0        0     3586 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/addon/manager.py
+-rw-r--r--   0        0        0        0 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/cli/__init__.py
+-rw-r--r--   0        0        0     3458 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/cli/args.py
+-rw-r--r--   0        0        0        0 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/fs/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/fs/dir.py
+-rw-r--r--   0        0        0     1010 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/fs/file.py
+-rw-r--r--   0        0        0      470 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/main.py
+-rw-r--r--   0        0        0        0 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/__init__.py
+-rw-r--r--   0        0        0     5222 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/config.py
+-rw-r--r--   0        0        0     4573 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/manager.py
+-rw-r--r--   0        0        0     4019 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/version.py
+-rw-r--r--   0        0        0      740 2024-05-19 20:38:38.136459 kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/res/repo_addon.xml.tpl
+-rw-r--r--   0        0        0      743 2024-05-19 20:38:52.984376 kodi_repo_bootstrap-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 kodi_repo_bootstrap-3.0.2/PKG-INFO
```

### Comparing `kodi_repo_bootstrap-3.0.0/LICENSE` & `kodi_repo_bootstrap-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/README.md` & `kodi_repo_bootstrap-3.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # [Kodi](https://kodi.tv/) Repository Bootstrapper
-Many thanks to @Twilight0 and all the others who contributed code for this project before.
+Many thanks to [@Twilight0](https://github.com/Twilight0) and all the others who contributed code for this project before.
 
 
 ## Installation
 You can install this Python package via pip(x):
 
 ```shell
 pip(x) install kodi-repo-bootstrap
```

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/addon/addon.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/addon/addon.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/addon/manager.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/addon/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     else:
                         print(f"Skipping addon '{cur_addon.addon_path}', "
                               "because a newer version is present in addons_dir.")
                 else:
                     # add the current addon to the dict, because it's not known
                     self.__addons_latest_version[cur_addon.id] = cur_addon
 
-        return (addon for addon in self.__addons_latest_version.values())
+        return iter(self.__addons_latest_version.values())
 
     def get_addons_in_repo(self) -> Iterator[Addon]:
         return self.__glob_addon(self.__repo_dir,
                                  # valid directory structure for the existing addons (already in the repo):
                                  # repo_dir/
                                  #    |- plugin.addon.id/
                                  #    |    |- plugin.addon.id-versionX.zip
```

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/cli/args.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/cli/args.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/fs/dir.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/fs/dir.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/fs/file.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/fs/file.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/config.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/config.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/manager.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
         self.__addons_manager: AddonManager = AddonManager(addons_dir=config.addons_dir,
                                                            repo_dir=config.repo_dir)
 
         self.__repo_addon: RepoAddon = RepoAddon(config)
 
         # create addon directories for output in repo_dir
-        self.__addons_not_in_repo: List[Tuple[Path, Addon]] = []
+        self.__addons_not_in_repo_with_out_path: List[Tuple[Addon, Path]] = []
         addon: Addon
         for addon in self.__addons_manager.get_addons_not_in_repo():
             addon_out_path: Path = self.__config.repo_dir / addon.id
             addon_out_path.mkdir(exist_ok=True)
 
             # save for later use
-            self.__addons_not_in_repo.append((addon_out_path, addon))
+            self.__addons_not_in_repo_with_out_path.append((addon, addon_out_path))
 
     def create_repo_addons_xml(self) -> None:
         print("Generating addons.xml file")
 
         # addons.xml opening tags
         addons_xml_data: str = '<?xml version="1.0" encoding="UTF-8"?>\n<addons>\n'
 
@@ -78,22 +78,22 @@
         # create addons.xml.md5
         File.create_md5_file(addons_xml_path)
 
     def copy_addon_assets_to_repo(self) -> None:
         # get the addon ZIP and their corresponding md5 files
         # (for excluding them later from being deleted)
         previous_addon_zip_md5_files: Iterator[str] = chain.from_iterable(
-            chain((a[1].addon_path.name, f"{a[1].addon_path.name}.md5"))
-                for a in self.__addons_not_in_repo
+            chain((a.addon_path.name, f"{a.addon_path.name}.md5"))
+                for a in self.__addons_manager.get_addons_in_repo()
         )
 
         # iterate over the addon directories
-        addon_out_path: Path
         addon: Addon
-        for addon_out_path, addon in self.__addons_not_in_repo:
+        addon_out_path: Path
+        for addon, addon_out_path in self.__addons_not_in_repo_with_out_path:
             # first clear the destination directory
             # only keep any previous addon ZIP and their corresponding md5 files
             path_to_delete: Path
             for path_to_delete in Directory.multi_glob_exclude(addon_out_path, *previous_addon_zip_md5_files):
                 if path_to_delete.is_dir() and not path_to_delete.is_symlink():
                     shutil.rmtree(path_to_delete)
                 else:
@@ -102,11 +102,11 @@
             addon.copy_assets_to_dir(dest_dir=addon_out_path)
 
     def create_addon_zip_files(self) -> None:
         # create repo addon zip file
         self.__repo_addon.create_zip_file()
 
         # create the zip files for all other addons
-        addon_out_path: Path
         addon: Addon
-        for addon_out_path, addon in self.__addons_not_in_repo:
+        addon_out_path: Path
+        for addon, addon_out_path in self.__addons_not_in_repo_with_out_path:
             addon.create_zip_file(dest_dir=addon_out_path)
```

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/repo/version.py` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/repo/version.py`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/kodi_repo_bootstrap/res/repo_addon.xml.tpl` & `kodi_repo_bootstrap-3.0.2/kodi_repo_bootstrap/res/repo_addon.xml.tpl`

 * *Files identical despite different names*

### Comparing `kodi_repo_bootstrap-3.0.0/pyproject.toml` & `kodi_repo_bootstrap-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodi-repo-bootstrap"
-version = "3.0.0"
+version = "3.0.2"
 description = "Bootstrap GIT repo for setting up a Kodi repository"
 authors = ["mammo0 <marc.ammon@hotmail.de>"]
 homepage = "https://github.com/mammo0/kodi-repo-bootstrap"
 readme = "README.md"
 license = "GPL-2.0-only"
```

### Comparing `kodi_repo_bootstrap-3.0.0/PKG-INFO` & `kodi_repo_bootstrap-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodi-repo-bootstrap
-Version: 3.0.0
+Version: 3.0.2
 Summary: Bootstrap GIT repo for setting up a Kodi repository
 Home-page: https://github.com/mammo0/kodi-repo-bootstrap
 License: GPL-2.0-only
 Author: mammo0
 Author-email: marc.ammon@hotmail.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # [Kodi](https://kodi.tv/) Repository Bootstrapper
-Many thanks to @Twilight0 and all the others who contributed code for this project before.
+Many thanks to [@Twilight0](https://github.com/Twilight0) and all the others who contributed code for this project before.
 
 
 ## Installation
 You can install this Python package via pip(x):
 
 ```shell
 pip(x) install kodi-repo-bootstrap
```

