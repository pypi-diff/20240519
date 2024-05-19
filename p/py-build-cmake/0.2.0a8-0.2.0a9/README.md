# Comparing `tmp/py_build_cmake-0.2.0a8.tar.gz` & `tmp/py_build_cmake-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_build_cmake-0.2.0a8.tar", last modified: Sat Oct 14 22:15:26 2023, max compression
+gzip compressed data, was "py_build_cmake-0.2.0a9.tar", last modified: Tue Nov 21 23:56:44 2023, max compression
```

## Comparing `py_build_cmake-0.2.0a8.tar` & `py_build_cmake-0.2.0a9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2023-10-14 22:15:12.025430 py_build_cmake-0.2.0a8/LICENSE
--rw-r--r--   0        0        0     6532 2023-10-14 22:15:12.025699 py_build_cmake-0.2.0a8/README.md
--rw-r--r--   0        0        0     3503 2023-10-14 22:15:12.055653 py_build_cmake-0.2.0a8/pyproject.toml
--rw-r--r--   0        0        0      136 2023-10-14 22:15:12.057124 py_build_cmake-0.2.0a8/src/py_build_cmake/__init__.py
--rw-r--r--   0        0        0    18462 2023-10-14 22:15:12.057342 py_build_cmake-0.2.0a8/src/py_build_cmake/build.py
--rw-r--r--   0        0        0     7440 2023-10-14 22:15:12.057547 py_build_cmake-0.2.0a8/src/py_build_cmake/build_component.py
--rw-r--r--   0        0        0     9161 2023-10-14 22:15:12.057811 py_build_cmake-0.2.0a8/src/py_build_cmake/cli.py
--rw-r--r--   0        0        0    10155 2023-10-14 22:15:12.058098 py_build_cmake-0.2.0a8/src/py_build_cmake/commands/cmake.py
--rw-r--r--   0        0        0     2483 2023-10-14 22:15:12.058244 py_build_cmake-0.2.0a8/src/py_build_cmake/commands/cmd_runner.py
--rw-r--r--   0        0        0     1832 2023-10-14 22:15:12.058553 py_build_cmake-0.2.0a8/src/py_build_cmake/commands/try_run.py
--rw-r--r--   0        0        0     7083 2023-10-14 22:15:12.058841 py_build_cmake-0.2.0a8/src/py_build_cmake/common/__init__.py
--rw-r--r--   0        0        0     1097 2023-10-14 22:15:12.059036 py_build_cmake-0.2.0a8/src/py_build_cmake/common/logformat.py
--rw-r--r--   0        0        0     2511 2023-10-14 22:15:12.059224 py_build_cmake-0.2.0a8/src/py_build_cmake/common/util.py
--rw-r--r--   0        0        0        0 2023-10-14 22:15:12.059400 py_build_cmake-0.2.0a8/src/py_build_cmake/config/__init__.py
--rw-r--r--   0        0        0    32549 2023-10-14 22:15:12.059691 py_build_cmake-0.2.0a8/src/py_build_cmake/config/config_options.py
--rw-r--r--   0        0        0     9307 2023-10-14 22:15:12.059954 py_build_cmake-0.2.0a8/src/py_build_cmake/config/dynamic.py
--rw-r--r--   0        0        0    11066 2023-10-14 22:15:12.060189 py_build_cmake-0.2.0a8/src/py_build_cmake/config/load.py
--rw-r--r--   0        0        0    25767 2023-10-14 22:15:12.060548 py_build_cmake-0.2.0a8/src/py_build_cmake/config/pyproject_options.py
--rw-r--r--   0        0        0     8241 2023-10-14 22:15:12.060817 py_build_cmake-0.2.0a8/src/py_build_cmake/config/quirks.py
--rw-r--r--   0        0        0        0 2023-10-14 22:15:12.061016 py_build_cmake-0.2.0a8/src/py_build_cmake/export/__init__.py
--rw-r--r--   0        0        0      748 2023-10-14 22:15:12.061668 py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/__init__.py
--rw-r--r--   0        0        0     1577 2023-10-14 22:15:12.061878 py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/hook.py
--rw-r--r--   0        0        0      684 2023-10-14 22:15:12.062110 py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/symlink.py
--rw-r--r--   0        0        0     1972 2023-10-14 22:15:12.062309 py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/wrapper.py
--rw-r--r--   0        0        0     1726 2023-10-14 22:15:12.062523 py_build_cmake-0.2.0a8/src/py_build_cmake/export/metadata.py
--rw-r--r--   0        0        0     2844 2023-10-14 22:15:12.062757 py_build_cmake-0.2.0a8/src/py_build_cmake/export/native_tags.py
--rw-r--r--   0        0        0     8684 2023-10-14 22:15:12.063001 py_build_cmake-0.2.0a8/src/py_build_cmake/export/sdist.py
--rw-r--r--   0        0        0     1870 2023-10-14 22:15:12.063199 py_build_cmake-0.2.0a8/src/py_build_cmake/export/tags.py
--rw-r--r--   0        0        0      589 2023-10-14 22:15:12.063460 py_build_cmake-0.2.0a8/src/py_build_cmake/export/util.py
--rw-r--r--   0        0        0     4213 2023-10-14 22:15:12.063733 py_build_cmake-0.2.0a8/src/py_build_cmake/help.py
--rw-r--r--   0        0        0     9104 1970-01-01 00:00:00.000000 py_build_cmake-0.2.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-11-21 23:56:23.763944 py_build_cmake-0.2.0a9/LICENSE
+-rw-r--r--   0        0        0     6532 2023-11-21 23:56:23.764604 py_build_cmake-0.2.0a9/README.md
+-rw-r--r--   0        0        0     3503 2023-11-21 23:56:23.809765 py_build_cmake-0.2.0a9/pyproject.toml
+-rw-r--r--   0        0        0      136 2023-11-21 23:56:23.811235 py_build_cmake-0.2.0a9/src/py_build_cmake/__init__.py
+-rw-r--r--   0        0        0    18679 2023-11-21 23:56:23.811663 py_build_cmake-0.2.0a9/src/py_build_cmake/build.py
+-rw-r--r--   0        0        0     7440 2023-11-21 23:56:23.811949 py_build_cmake-0.2.0a9/src/py_build_cmake/build_component.py
+-rw-r--r--   0        0        0     9161 2023-11-21 23:56:23.812206 py_build_cmake-0.2.0a9/src/py_build_cmake/cli.py
+-rw-r--r--   0        0        0    10285 2023-11-21 23:56:23.812554 py_build_cmake-0.2.0a9/src/py_build_cmake/commands/cmake.py
+-rw-r--r--   0        0        0     2483 2023-11-21 23:56:23.812795 py_build_cmake-0.2.0a9/src/py_build_cmake/commands/cmd_runner.py
+-rw-r--r--   0        0        0     1832 2023-11-21 23:56:23.813022 py_build_cmake-0.2.0a9/src/py_build_cmake/commands/try_run.py
+-rw-r--r--   0        0        0     7114 2023-11-21 23:56:23.813567 py_build_cmake-0.2.0a9/src/py_build_cmake/common/__init__.py
+-rw-r--r--   0        0        0     1097 2023-11-21 23:56:23.813914 py_build_cmake-0.2.0a9/src/py_build_cmake/common/logformat.py
+-rw-r--r--   0        0        0     2511 2023-11-21 23:56:23.814147 py_build_cmake-0.2.0a9/src/py_build_cmake/common/util.py
+-rw-r--r--   0        0        0        0 2023-11-21 23:56:23.814383 py_build_cmake-0.2.0a9/src/py_build_cmake/config/__init__.py
+-rw-r--r--   0        0        0    32549 2023-11-21 23:56:23.814722 py_build_cmake-0.2.0a9/src/py_build_cmake/config/config_options.py
+-rw-r--r--   0        0        0     9827 2023-11-21 23:56:23.815056 py_build_cmake-0.2.0a9/src/py_build_cmake/config/dynamic.py
+-rw-r--r--   0        0        0    11078 2023-11-21 23:56:23.815272 py_build_cmake-0.2.0a9/src/py_build_cmake/config/load.py
+-rw-r--r--   0        0        0    26087 2023-11-21 23:56:23.815725 py_build_cmake-0.2.0a9/src/py_build_cmake/config/pyproject_options.py
+-rw-r--r--   0        0        0     8241 2023-11-21 23:56:23.816024 py_build_cmake-0.2.0a9/src/py_build_cmake/config/quirks.py
+-rw-r--r--   0        0        0        0 2023-11-21 23:56:23.816381 py_build_cmake-0.2.0a9/src/py_build_cmake/export/__init__.py
+-rw-r--r--   0        0        0      748 2023-11-21 23:56:23.816613 py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/__init__.py
+-rw-r--r--   0        0        0     1577 2023-11-21 23:56:23.816780 py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/hook.py
+-rw-r--r--   0        0        0      684 2023-11-21 23:56:23.817211 py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/symlink.py
+-rw-r--r--   0        0        0     1972 2023-11-21 23:56:23.817489 py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/wrapper.py
+-rw-r--r--   0        0        0     1726 2023-11-21 23:56:23.817751 py_build_cmake-0.2.0a9/src/py_build_cmake/export/metadata.py
+-rw-r--r--   0        0        0     2844 2023-11-21 23:56:23.818013 py_build_cmake-0.2.0a9/src/py_build_cmake/export/native_tags.py
+-rw-r--r--   0        0        0     8731 2023-11-21 23:56:23.818382 py_build_cmake-0.2.0a9/src/py_build_cmake/export/sdist.py
+-rw-r--r--   0        0        0     1870 2023-11-21 23:56:23.818581 py_build_cmake-0.2.0a9/src/py_build_cmake/export/tags.py
+-rw-r--r--   0        0        0      589 2023-11-21 23:56:23.818921 py_build_cmake-0.2.0a9/src/py_build_cmake/export/util.py
+-rw-r--r--   0        0        0     4213 2023-11-21 23:56:23.819154 py_build_cmake-0.2.0a9/src/py_build_cmake/help.py
+-rw-r--r--   0        0        0     9104 1970-01-01 00:00:00.000000 py_build_cmake-0.2.0a9/PKG-INFO
```

### Comparing `py_build_cmake-0.2.0a8/LICENSE` & `py_build_cmake-0.2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/README.md` & `py_build_cmake-0.2.0a9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.2.0a8"]
+requires = ["py-build-cmake~=0.2.0a9"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

### Comparing `py_build_cmake-0.2.0a8/pyproject.toml` & `py_build_cmake-0.2.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/build.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,18 +199,19 @@
 
         # Set up all paths
         paths = self.get_default_paths(
             wheel_dir, tmp_build_dir, src_dir, cfg, cmake_cfg
         )
 
         # Copy the module's Python source files to the temporary folder
-        if not editable:
-            export_util.copy_pkg_source_to(paths.staging_dir, module)
-        else:
-            paths = export_editable.do_editable_install(cfg, paths, module)
+        if not module.is_generated:
+            if not editable:
+                export_util.copy_pkg_source_to(paths.staging_dir, module)
+            else:
+                paths = export_editable.do_editable_install(cfg, paths, module)
 
         # Create dist-info folder
         distinfo_dir = f"{pkg_info.norm_name}-{pkg_info.version}.dist-info"
         distinfo_dir = paths.pkg_staging_dir / distinfo_dir
         distinfo_dir.mkdir(parents=True, exist_ok=True)
 
         # Write metadata, license and entry points to Wheel's distinfo
@@ -261,23 +262,25 @@
             wheel_dir=Path(wheel_dir),
             temp_dir=Path(tmp_build_dir),
             staging_dir=Path(tmp_build_dir) / "staging",
             pkg_staging_dir=Path(tmp_build_dir) / "staging",
         )
 
     @staticmethod
-    def read_all_metadata(
-        src_dir, config_settings, verbose
-    ) -> tuple[Config, Module | None]:
+    def read_all_metadata(src_dir, config_settings, verbose) -> tuple[Config, Module]:
         cfg = _BuildBackend.read_config(src_dir, config_settings, verbose)
         module = find_module(cfg.module, src_dir)
         modfile = module.full_file
-        if module.is_namespace and cfg.standard_metadata.dynamic:
-            msg = "Dynamic metadata is not supported for namespace packages"
-            raise ConfigError(msg)
+        if cfg.standard_metadata.dynamic:
+            if module.is_generated:
+                msg = "Dynamic metadata is not supported for generated modules/packages"
+                raise ConfigError(msg)
+            elif module.is_namespace:
+                msg = "Dynamic metadata is not supported for namespace packages"
+                raise ConfigError(msg)
         try:
             update_dynamic_metadata(cfg.standard_metadata, modfile)
         except ImportError as e:
             logger.error("Error importing %s for reading metadata", str(modfile))
             msg = (
                 "\n"
                 "\n"
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/build_component.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/build_component.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/cli.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/cli.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/commands/cmake.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/commands/cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,23 +186,25 @@
             self.get_configure_options_package()
             + self.get_configure_options_python()
             + self.get_configure_options_toolchain()
             + self.get_configure_options_settings()
         )
 
     def get_cmake_generator_platform(self) -> list[str]:
-        if self.cmake_settings.os == "windows" and not self.cross_compiling():
+        win = self.cmake_settings.os == "windows"
+        gen = self.conf_settings.generator
+        vs_gen = win and (not gen or gen.lower().startswith("visual studio"))
+        if vs_gen and not self.cross_compiling():
             plat = sysconfig.get_platform()
             cmake_plat = python_sysconfig_platform_to_cmake_platform_win(plat)
             if cmake_plat:
                 return ["-A", cmake_plat]
             else:
-                logger.warning(
-                    "Unknown platform, CMake generator platform option (-A) will not be set"
-                )
+                msg = "Unknown platform, CMake generator platform option (-A) will not be set"
+                logger.warning(msg)
         return []
 
     def get_configure_command(self):
         options = self.get_configure_options()
         cmd = [str(self.cmake_settings.command)]
         cmd += ["-S", str(self.cmake_settings.source_path)]
         if self.conf_settings.preset:
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/commands/cmd_runner.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/commands/cmd_runner.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/commands/try_run.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/commands/try_run.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/common/__init__.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     """Describes the location and name of a Python package or module"""
 
     name: str
     full_path: Path
     base_path: Path
     is_package: bool
     is_namespace: bool
+    is_generated: bool = False
 
     @property
     def prefix(self):
         return self.full_path.parent
 
     @property
     def full_file(self):
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/common/logformat.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/common/logformat.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/common/util.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/common/util.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/config/config_options.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/config/config_options.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/config/dynamic.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/config/dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,14 +215,29 @@
     metadata.dynamic = []
 
 
 def find_module(module_metadata: dict, src_dir: Path) -> Module:
     name: str = module_metadata["name"]
     base_dir: Path = src_dir / module_metadata["directory"]
     is_namespace: bool = module_metadata["namespace"]
+    generated: str = module_metadata.get("generated")
+
+    # If the module is to be generated later by CMake, don't search for it now
+    if generated:
+        is_pkg = generated == "package"
+        # This won't have the right extension, but that's not an issue
+        full_path = base_dir / name
+        return Module(
+            name=name,
+            full_path=full_path,
+            base_path=src_dir,
+            is_package=is_pkg,
+            is_namespace=is_namespace,
+            is_generated=True,
+        )
 
     # Look for the module
     dir = lambda p: p.is_dir()
     file = lambda p: not is_namespace and p.is_file()
     options = [
         (base_dir / name, dir),
         (base_dir / "src" / name, dir),
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/config/load.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/config/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         pyproject["project"][f] = normname
 
     # Parse the [project] section for metadata
     try:
         Metadata = pyproject_metadata.StandardMetadata
         meta = Metadata.from_pyproject(pyproject, pyproject_path.parent)
     except pyproject_metadata.ConfigurationError as e:
-        raise ConfigError() from e
+        raise ConfigError(str(e)) from e
 
     # Create our own config data structure
     cfg = Config(meta)
     cfg.package_name = meta.name
 
     # Additional options from command-line overrides
     opts = get_options(pyproject_path.parent, test=test)
@@ -307,15 +307,15 @@
 
         # Parse the [project] section for metadata
     try:
         meta = pyproject_metadata.StandardMetadata.from_pyproject(
             pyproject, pyproject_path.parent
         )
     except pyproject_metadata.ConfigurationError as e:
-        raise ConfigError() from e
+        raise ConfigError(str(e)) from e
 
     # Create our own config data structure
     cfg = ComponentConfig(meta)
     cfg.package_name = meta.name
 
     opts = get_component_options(pyproject_path.parent)
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/config/pyproject_options.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/config/pyproject_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
                          "Directory containing the Python module/package.",
                          default=DefaultValueValue("."),
                          base_path=RelativeToProject(project_path),
                          must_exist=not test),
         BoolConfigOption("namespace",
                          "Set to true for PEP 420 namespace packages.",
                          default=DefaultValueValue(False)),
+        EnumConfigOption("generated",
+                         "Do not try to locate the module in the source "
+                         "directory, but assume that it is generated by CMake. "
+                         "Dynamic metadata cannot be used when set.",
+                         options=["module", "package"]),
     ])  # fmt: skip
 
     # [tool.py-build-cmake.editable]
     editable = pbc.insert(
         ConfigOption("editable",
                      "Defines how to perform an editable install (PEP 660). "
                      "See https://tttapa.github.io/py-build-cmake/"
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/config/quirks.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/config/quirks.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/__init__.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/__init__.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/hook.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/hook.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/symlink.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/symlink.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/editable/wrapper.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/editable/wrapper.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/metadata.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/metadata.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/native_tags.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/native_tags.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/sdist.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/sdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,24 +146,22 @@
 
     def select_files(self):
         """Pick which files from the source tree will be included in the sdist
 
         This is overridden in flit itself to use information from a VCS to
         include tests, docs, etc. for a 'gold standard' sdist.
         """
-
-        def make_rel(p: Path) -> Path:
-            return p.relative_to(self.module.base_path)
-
-        yield from map(make_rel, self.module.iter_files_abs())
+        make_rel = lambda p: p.relative_to(self.module.base_path)
+        if not self.module.is_generated:
+            yield from map(make_rel, self.module.iter_files_abs())
         yield from map(make_rel, self.extra_files)
 
     def crucial_files(self):
         make_rel = lambda p: p.relative_to(self.module.base_path)
-        if not self.module.is_namespace:
+        if not self.module.is_generated and not self.module.is_namespace:
             yield make_rel(self.module.full_file)
         yield from map(make_rel, self.extra_files)
 
     def apply_includes_excludes(self, files: Iterable[Path]):
         files = {f for f in files if not self.excludes.match_file(f)}
 
         for f_rel in self.includes.files:
```

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/tags.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/tags.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/export/util.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/export/util.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/src/py_build_cmake/help.py` & `py_build_cmake-0.2.0a9/src/py_build_cmake/help.py`

 * *Files identical despite different names*

### Comparing `py_build_cmake-0.2.0a8/PKG-INFO` & `py_build_cmake-0.2.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-build-cmake
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: Modern, PEP 517 compliant build backend for creating Python packages with
 Keywords: pep517 cmake
 Author-Email: Pieter P <pieter.p.dev@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Pieter P
         
@@ -115,15 +115,15 @@
 keywords = ["some", "keywords"]
 classifiers = ["Topic :: Scientific/Engineering"]
 urls = { "Documentation" = "https://tttapa.github.io/py-build-cmake" }
 dependencies = ["numpy"]
 dynamic = ["version", "description"]
 
 [build-system] # How pip and other frontends should build this project
-requires = ["py-build-cmake~=0.2.0a8"]
+requires = ["py-build-cmake~=0.2.0a9"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "src/*"]
```

