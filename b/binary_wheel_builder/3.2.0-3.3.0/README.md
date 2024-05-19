# Comparing `tmp/binary_wheel_builder-3.2.0.tar.gz` & `tmp/binary_wheel_builder-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary_wheel_builder-3.2.0.tar", max compression
+gzip compressed data, was "binary_wheel_builder-3.3.0.tar", max compression
```

## Comparing `binary_wheel_builder-3.2.0.tar` & `binary_wheel_builder-3.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/LICENSE
--rw-r--r--   0        0        0    11847 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/README.md
--rw-r--r--   0        0        0      126 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/__init__.py
--rw-r--r--   0        0        0       90 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/__main__.py
--rw-r--r--   0        0        0      516 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/__init__.py
--rw-r--r--   0        0        0     4000 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/build.py
--rw-r--r--   0        0        0     4770 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/meta.py
--rw-r--r--   0        0        0      912 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/well_known_platforms.py
--rw-r--r--   0        0        0      316 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/__init__.py
--rw-r--r--   0        0        0      420 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/exceptions.py
--rw-r--r--   0        0        0     2311 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github.py
--rw-r--r--   0        0        0     1469 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github_test.py
--rw-r--r--   0        0        0     2450 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry.py
--rw-r--r--   0        0        0     1572 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry_test.py
--rw-r--r--   0        0        0     1389 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py
--rw-r--r--   0        0        0      933 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
--rw-r--r--   0        0        0      465 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/static.py
--rw-r--r--   0        0        0      211 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/__init__.py
--rw-r--r--   0        0        0      534 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/config_file.py
--rw-r--r--   0        0        0      951 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/main.py
--rw-r--r--   0        0        0     4428 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml.py
--rw-r--r--   0        0        0     3982 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml_test.py
--rw-r--r--   0        0        0       90 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/__init__.py
--rw-r--r--   0        0        0      932 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible.py
--rw-r--r--   0        0        0      708 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible_test.py
--rw-r--r--   0        0        0     1015 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util.py
--rw-r--r--   0        0        0      936 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util_test.py
--rw-r--r--   0        0        0     4827 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates.py
--rw-r--r--   0        0        0      199 2024-04-20 09:58:28.491794 binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates_test.py
--rw-r--r--   0        0        0     1511 2024-04-20 09:58:28.495794 binary_wheel_builder-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     4282 2024-04-20 09:58:28.495794 binary_wheel_builder-3.2.0/wheel.schema.json
--rw-r--r--   0        0        0    13190 1970-01-01 00:00:00.000000 binary_wheel_builder-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/LICENSE
+-rw-r--r--   0        0        0    11813 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/README.md
+-rw-r--r--   0        0        0      126 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/__main__.py
+-rw-r--r--   0        0        0      516 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/__init__.py
+-rw-r--r--   0        0        0     4053 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/build.py
+-rw-r--r--   0        0        0     6052 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/meta.py
+-rw-r--r--   0        0        0      912 2024-05-19 16:13:01.565588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/well_known_platforms.py
+-rw-r--r--   0        0        0      375 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/exceptions.py
+-rw-r--r--   0        0        0     2397 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/github.py
+-rw-r--r--   0        0        0     1469 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/github_test.py
+-rw-r--r--   0        0        0     2549 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry.py
+-rw-r--r--   0        0        0     1572 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry_test.py
+-rw-r--r--   0        0        0     1562 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py
+-rw-r--r--   0        0        0      933 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
+-rw-r--r--   0        0        0      604 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/static.py
+-rw-r--r--   0        0        0      211 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/cli/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/cli/config_file.py
+-rw-r--r--   0        0        0      951 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/cli/main.py
+-rw-r--r--   0        0        0     4428 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/cli/yaml.py
+-rw-r--r--   0        0        0     3982 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/cli/yaml_test.py
+-rw-r--r--   0        0        0       90 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/__init__.py
+-rw-r--r--   0        0        0      932 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/reproducible.py
+-rw-r--r--   0        0        0      708 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/reproducible_test.py
+-rw-r--r--   0        0        0     1015 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/util.py
+-rw-r--r--   0        0        0      936 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/util_test.py
+-rw-r--r--   0        0        0     4877 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wrapper_templates.py
+-rw-r--r--   0        0        0      199 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/binary_wheel_builder/wrapper_templates_test.py
+-rw-r--r--   0        0        0     2050 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4282 2024-05-19 16:13:01.569588 binary_wheel_builder-3.3.0/wheel.schema.json
+-rw-r--r--   0        0        0    13106 1970-01-01 00:00:00.000000 binary_wheel_builder-3.3.0/PKG-INFO
```

### Comparing `binary_wheel_builder-3.2.0/LICENSE` & `binary_wheel_builder-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/README.md` & `binary_wheel_builder-3.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Build deterministic python wheels to distribute CLI tools (third party or your own with python and make them easily usable using python code.
 </p>
 
 ## Features
 
 - deterministic wheel file output
 - Use with Python Code or as CLI
-- [Prebuilt data sources](https://timo-reymann.github.io/python-binary-wheel-builder/binary_wheel_builder/api/wheel_sources/index.html) for your binaries
+- [Prebuilt data sources](https://timo-reymann.github.io/binary_wheel_builder.api.wheel_sources.html) for your binaries
 - Ready to release and ship your binaries
 - Wrapper for cli calls inside Python
 - Exposes wheel as module entrypoint (`python -m your_cli`) and adds to path (`your-cli`)
 
 ## Requirements
 
 - Python 3.8+ for host running wheel build
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/__init__.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/build.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Infrastructure to build deterministic wheels
+"""
 import hashlib
 import os
 from operator import attrgetter
 from collections.abc import Generator
 from zipfile import Path
 
 from binary_wheel_builder import wrapper_templates
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/meta.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,77 @@
+"""
+Meta data around wheels
+"""
 import functools
-from abc import abstractmethod, ABC
-from pathlib import Path
+from abc import ABC, abstractmethod
 from collections.abc import Sequence
+from pathlib import Path
 from typing import Any, Callable
 
-from pydantic import dataclasses, ConfigDict, Field, GetJsonSchemaHandler, BaseModel
+from pydantic import BaseModel, ConfigDict, Field, GetJsonSchemaHandler, dataclasses
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
 
 
 @dataclasses.dataclass(frozen=True)
 class WheelPlatformBuildResult:
+    """Result of a wheel file build"""
+
     checksum: str
     """Contains the SHA256 checksum of the created wheel file"""
+
     file_path: Path
     """Full qualified path to wheel"""
 
 
 @dataclasses.dataclass(frozen=True)
 class WheelPlatformIdentifier:
+    """Identifies a wheel target platform"""
+
     platform: str = Field(description="Name of the platform")
+    """Name of the platform"""
+
     python_tag: str = Field(default="py3", description="Python tag (e.g pyX)")
-    abi_tag: str = Field(default="none",
-                         description="Indicates which Python ABI is required by any included extension modules.")
+    """Python tag (e.g pyX)"""
+
+    abi_tag: str = Field(
+        default="none",
+        description="Indicates which Python ABI is required by any included extension modules."
+    )
+    """Indicates which Python ABI is required by any included extension modules."""
 
     def to_tag(self):
         """Build to python wheel tag format"""
-        return "-".join([
-            self.python_tag,
-            self.abi_tag,
-            self.platform,
-        ])
+        return "-".join(
+            [
+                self.python_tag,
+                self.abi_tag,
+                self.platform,
+            ]
+        )
 
 
 class WheelFileEntry(BaseModel):
+    """Source entry for a wheel"""
+
     path: str = Field(description="Path of the file in the wheel")
+    """Path of the file in the wheel"""
+
     content: bytes = Field(description="Binary content for the file")
+    """Binary content for the file"""
+
     permissions: int = Field(0o644, description="Permissions for the file in the archive")
+    """Permissions for the file in the archive"""
 
 
 class WheelSource(ABC):
+    """
+    Represents a source that can be used to build a wheel around
+    """
+
     @abstractmethod
     def generate_fileset(self, wheel_platform: WheelPlatformIdentifier) -> list[WheelFileEntry]:
         """
         Generate a list of files to add to the wheel
         :param wheel_platform: Platform of the wheel the files will be used on
         :return: List with wheel file entries for adding to the wheel archive
         """
@@ -72,30 +100,61 @@
             handler: Callable[[Any], core_schema.CoreSchema]
     ) -> core_schema.CoreSchema:
         return core_schema.with_info_plain_validator_function(cls.validate)
 
 
 @dataclasses.dataclass(frozen=True)
 class Wheel:
+    """
+    Metadata about a wheel to generate
+    """
     model_config = ConfigDict(arbitrary_types_allowed=True, extra="forbid")
 
     package: str = Field(description="Name of the generated package")
-    executable: str = Field(description="Path of the executable, relative to the package folder. It must match one of "
-                                        "the file names from the wheel sources in order to work")
+    """Name of the generated package"""
+
+    executable: str = Field(
+        description="Path of the executable, relative to the package folder. It must match one of "
+                    "the file names from the wheel sources in order to work"
+    )
+    """Path of the executable, relative to the package folder. 
+    It must match one of the file names from the wheel sources in order to work"""
+
     name: str = Field(description="Name of the wheel package")
+    """Name of the wheel package"""
+
     version: str = Field(description="Version of the package")
+    """Version of the package"""
+
     source: WheelSource = Field(description="Source to fetch files from")
+    """Source to fetch files from"""
+
     platforms: Sequence[WheelPlatformIdentifier] = Field(description="Platforms supported by the wheel")
+    """Platforms supported by the wheel"""
+
     summary: str | None = Field(None, description="Summary for package metadata")
+    """Summary for package metadata"""
+
     description: str | None = Field(None, description="Description for package metadata")
+    """Description for package metadata"""
+
     license: str | None = Field(None, description="Name of the license")
+    """Name of the license"""
+
     classifier: Sequence[str] | None = Field(None, description="Classifiers to show in frontends")
-    project_urls: dict[str, str] | None = Field(None, description="Incude project URLs like bugtrackers etc.")
+    """Classifiers to show in frontends"""
+
+    project_urls: dict[str, str] | None = Field(None, description="Include project URLs like bugtrackers etc.")
+    """Include project URLs like bugtrackers etc."""
+
     requires_python: str | None = Field(None, description="Python version constraint for the wheel")
+    """Python version constraint for the wheel"""
+
     add_to_path: bool = Field(True, description="Should the executable be added to the path (using python wrapper)")
+    """Should the executable be added to the path (using python wrapper)"""
 
     @functools.cached_property
     def normalized_name(self):
         """
         Normalize the name for use in wheel naming
         :return: Replaced all dashes with underscores
         """
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/well_known_platforms.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/well_known_platforms.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+"""
+Sources for GitHub
+"""
 from urllib.error import HTTPError
 
 from binary_wheel_builder.api.meta import WheelFileEntry, WheelPlatformIdentifier, WheelSource
 from binary_wheel_builder.api.wheel_sources.exceptions import SourceFileRequestFailed, UnsupportedWheelPlatformException
 
 
 class GithubReleaseBinarySource(WheelSource):
+    """
+    Provide source from GitHub Release API
+    """
     def __init__(
             self,
             project_slug: str,
             version: str,
             asset_name_mapping: dict[WheelPlatformIdentifier, str],
             binary_path: str,
             tag_prefix: str = "v",
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/github_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/github_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+"""
+Sources for GitLab
+"""
 from binary_wheel_builder import WheelFileEntry, WheelPlatformIdentifier, WheelSource
 from binary_wheel_builder.api.wheel_sources.exceptions import SourceFileRequestFailed
 
 
 class GitlabGenericPackageRegistrySource(WheelSource):
+    """
+    Provide source from Gitlab Generic Package Registry
+    """
     def __init__(
             self,
             asset_name_mapping: dict[WheelPlatformIdentifier, str],
             binary_path: str,
             project: int | str,
             version: str,
             package_name: str,
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/gitlab_package_registry_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+"""
+Source for local binaries, which differ based on the target platform
+"""
 from pathlib import Path
 
 from binary_wheel_builder.api.meta import WheelFileEntry, WheelPlatformIdentifier, WheelSource
 from binary_wheel_builder.api.wheel_sources.exceptions import SourceFileRequestFailed, UnsupportedWheelPlatformException
 
 
 class PlatformBasedFileSource(WheelSource):
+    """
+    Provide source from a local file, the name depending on the target platform
+    """
     def __init__(self, executable_path: str, file_name_mapping: dict[WheelPlatformIdentifier, Path | str]):
         """
 
         :param executable_path: Path to the executable that will be used in the generated wheel
         :param file_name_mapping: Map wheel platform identifiers to the local binary file names.
         """
         self.executable_path = executable_path
```

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/config_file.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/cli/config_file.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/main.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/cli/main.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/cli/yaml.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/cli/yaml_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/cli/yaml_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/reproducible.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/reproducible_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/reproducible_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/util.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/wheel/util_test.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/wheel/util_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/binary_wheel_builder/wrapper_templates.py` & `binary_wheel_builder-3.3.0/binary_wheel_builder/wrapper_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Wrapper templates for generating packages
+"""
 import textwrap
 
 from binary_wheel_builder.api.meta import Wheel
 
 
 def _preprocess(val: str):
     return textwrap.dedent(val).encode("utf-8")
```

### Comparing `binary_wheel_builder-3.2.0/pyproject.toml` & `binary_wheel_builder-3.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "binary_wheel_builder"
-version = "3.2.0"
+version = "3.3.0"
 description = "Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary"
 authors = ["Timo Reymann <mail@timo-reymann.de>"]
 readme = "README.md"
 packages = [
     { include = "binary_wheel_builder" }
 ]
 classifiers = [
@@ -25,23 +25,24 @@
 repository = "https://github.com/timo-reymann/python-binary-wheel-builder"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/timo-reymann/python-binary-wheel-builder/issues"
 
 
 [tool.poetry.dependencies]
-python = "> 3.8"
+python = "> 3.9"
 wheel = "> 0.30.0"
 pyyaml = { version = "^6.0.1", optional = true }
 pydantic = "^2.5.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 coverage = "^7.4.0"
 pdoc3 = "^0.10.0"
+pydoctor = "^24.3.3"
 
 [tool.poetry.extras]
 cli = ["pyyaml"]
 
 [tool.poetry.scripts]
 binary-wheel-builder = "binary_wheel_builder.cli.main:main"
 
@@ -56,7 +57,27 @@
 
 [tool.coverage.report]
 fail_under = 70
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pydoctor]
+verbose = 0
+warnings-as-errors = true
+
+intersphinx = ["https://docs.python.org/3/objects.inv"]
+docformat = "restructuredtext"
+html-output = "gh-pages"
+
+add-package = ["binary_wheel_builder.api"]
+project-name = "binary_wheel_builder"
+project-url = "https://github.com/timo-reymann/python-binary-wheel-builder"
+privacy = [
+    "HIDDEN:binary_wheel_builder.**.*_test",
+    "HIDDEN:binary_wheel_builder.*_test",
+    "HIDDEN:binary_wheel_builder.conftest"
+]
+
+theme = "base"
+template-dir = "pydoctor-theme"
```

### Comparing `binary_wheel_builder-3.2.0/wheel.schema.json` & `binary_wheel_builder-3.3.0/wheel.schema.json`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.2.0/PKG-INFO` & `binary_wheel_builder-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: binary_wheel_builder
-Version: 3.2.0
+Version: 3.3.0
 Summary: Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary
 Home-page: https://github.com/timo-reymann/python-binary-wheel-builder
 Author: Timo Reymann
 Author-email: mail@timo-reymann.de
-Requires-Python: >3.8
+Requires-Python: >3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: System :: Software Distribution
 Provides-Extra: cli
@@ -46,15 +45,15 @@
     Build deterministic python wheels to distribute CLI tools (third party or your own with python and make them easily usable using python code.
 </p>
 
 ## Features
 
 - deterministic wheel file output
 - Use with Python Code or as CLI
-- [Prebuilt data sources](https://timo-reymann.github.io/python-binary-wheel-builder/binary_wheel_builder/api/wheel_sources/index.html) for your binaries
+- [Prebuilt data sources](https://timo-reymann.github.io/binary_wheel_builder.api.wheel_sources.html) for your binaries
 - Ready to release and ship your binaries
 - Wrapper for cli calls inside Python
 - Exposes wheel as module entrypoint (`python -m your_cli`) and adds to path (`your-cli`)
 
 ## Requirements
 
 - Python 3.8+ for host running wheel build
```

