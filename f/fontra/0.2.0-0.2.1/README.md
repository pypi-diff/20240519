# Comparing `tmp/fontra-0.2.0.tar.gz` & `tmp/fontra-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontra-0.2.0.tar", last modified: Sat Apr  6 07:29:09 2024, max compression
+gzip compressed data, was "fontra-0.2.1.tar", last modified: Sun May 19 13:52:50 2024, max compression
```

## Comparing `fontra-0.2.0.tar` & `fontra-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:29:09.998001 fontra-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 07:29:05.000000 fontra-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-06 07:29:09.998001 fontra-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-06 07:29:05.000000 fontra-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:29:09.998001 fontra-0.2.0/fontra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-06 07:29:09.000000 fontra-0.2.0/fontra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-06 07:29:09.000000 fontra-0.2.0/fontra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:29:09.000000 fontra-0.2.0/fontra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 07:29:09.000000 fontra-0.2.0/fontra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 07:29:09.000000 fontra-0.2.0/fontra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-06 07:29:05.000000 fontra-0.2.0/fontra.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-06 07:29:05.000000 fontra-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:29:09.998001 fontra-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:52:50.941092 fontra-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 13:52:46.000000 fontra-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 13:52:50.941092 fontra-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-19 13:52:46.000000 fontra-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:52:50.941092 fontra-0.2.1/fontra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 13:52:50.000000 fontra-0.2.1/fontra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-19 13:52:50.000000 fontra-0.2.1/fontra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:52:50.000000 fontra-0.2.1/fontra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 13:52:50.000000 fontra-0.2.1/fontra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 13:52:50.000000 fontra-0.2.1/fontra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-19 13:52:46.000000 fontra-0.2.1/fontra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 13:52:46.000000 fontra-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:52:50.941092 fontra-0.2.1/setup.cfg
```

### Comparing `fontra-0.2.0/LICENSE` & `fontra-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fontra-0.2.0/PKG-INFO` & `fontra-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fontra
-Version: 0.2.0
+Version: 0.2.1
 Summary: Some small work with fonts.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/fontra
 Project-URL: Repository, https://github.com/NCBM/fontra
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: freetype-py<1,>=0.3.2
+Requires-Dist: freetype-py<3,>=2
 Requires-Dist: typing_extensions<5,>=4.6.0
 
 # fontra
 
 Some small work with fonts.
 
 ## Features
@@ -29,31 +29,31 @@
 pip install fontra
 ```
 
 ## Usage
 
 - Common font query
 
-```python-repl
+```python
 >>> import fontra
 >>> fontra.all_fonts()
 ['Noto Sans Lisu', 'Noto Serif Tamil SemiCondensed', 'Noto Serif Georgian', 'Noto Sans Armenian', ...]
 >>> fontra.get_font_styles("Arial")
 ['Regular', 'Italic', 'Bold', 'Bold Italic', 'Black']
 >>> fontra.get_font("Arial", "Italic")
 FontRef(path=PosixPath('/usr/share/fonts/TTF/ariali.ttf'), bank=0)
 >>> fontra.unlocalized_name("更紗ゴシック UI J")
 'Sarasa UI J'
 >>> fontra.get_font("更纱黑体 SC", "SemiBold Italic")
 FontRef(path=PosixPath('/usr/share/fonts/sarasa-gothic/Sarasa-SemiBoldItalic.ttc'), bank=1)
 ```
 
-- Custom font direciories
+- Custom font directories
 
-```python-repl
+```python
 >>> fontra.FONTDIR_CUSTOM.append("./data/fonts")
 >>> fontra.update_custom_fontfiles_index()
 >>> fontra.update_fontrefs_index()
 >>> fontra.all_fonts()
 [...]
 ```
```

### Comparing `fontra-0.2.0/README.md` & `fontra-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 pip install fontra
 ```
 
 ## Usage
 
 - Common font query
 
-```python-repl
+```python
 >>> import fontra
 >>> fontra.all_fonts()
 ['Noto Sans Lisu', 'Noto Serif Tamil SemiCondensed', 'Noto Serif Georgian', 'Noto Sans Armenian', ...]
 >>> fontra.get_font_styles("Arial")
 ['Regular', 'Italic', 'Bold', 'Bold Italic', 'Black']
 >>> fontra.get_font("Arial", "Italic")
 FontRef(path=PosixPath('/usr/share/fonts/TTF/ariali.ttf'), bank=0)
 >>> fontra.unlocalized_name("更紗ゴシック UI J")
 'Sarasa UI J'
 >>> fontra.get_font("更纱黑体 SC", "SemiBold Italic")
 FontRef(path=PosixPath('/usr/share/fonts/sarasa-gothic/Sarasa-SemiBoldItalic.ttc'), bank=1)
 ```
 
-- Custom font direciories
+- Custom font directories
 
-```python-repl
+```python
 >>> fontra.FONTDIR_CUSTOM.append("./data/fonts")
 >>> fontra.update_custom_fontfiles_index()
 >>> fontra.update_fontrefs_index()
 >>> fontra.all_fonts()
 [...]
 ```
```

### Comparing `fontra-0.2.0/fontra.egg-info/PKG-INFO` & `fontra-0.2.1/fontra.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fontra
-Version: 0.2.0
+Version: 0.2.1
 Summary: Some small work with fonts.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/fontra
 Project-URL: Repository, https://github.com/NCBM/fontra
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: freetype-py<1,>=0.3.2
+Requires-Dist: freetype-py<3,>=2
 Requires-Dist: typing_extensions<5,>=4.6.0
 
 # fontra
 
 Some small work with fonts.
 
 ## Features
@@ -29,31 +29,31 @@
 pip install fontra
 ```
 
 ## Usage
 
 - Common font query
 
-```python-repl
+```python
 >>> import fontra
 >>> fontra.all_fonts()
 ['Noto Sans Lisu', 'Noto Serif Tamil SemiCondensed', 'Noto Serif Georgian', 'Noto Sans Armenian', ...]
 >>> fontra.get_font_styles("Arial")
 ['Regular', 'Italic', 'Bold', 'Bold Italic', 'Black']
 >>> fontra.get_font("Arial", "Italic")
 FontRef(path=PosixPath('/usr/share/fonts/TTF/ariali.ttf'), bank=0)
 >>> fontra.unlocalized_name("更紗ゴシック UI J")
 'Sarasa UI J'
 >>> fontra.get_font("更纱黑体 SC", "SemiBold Italic")
 FontRef(path=PosixPath('/usr/share/fonts/sarasa-gothic/Sarasa-SemiBoldItalic.ttc'), bank=1)
 ```
 
-- Custom font direciories
+- Custom font directories
 
-```python-repl
+```python
 >>> fontra.FONTDIR_CUSTOM.append("./data/fonts")
 >>> fontra.update_custom_fontfiles_index()
 >>> fontra.update_fontrefs_index()
 >>> fontra.all_fonts()
 [...]
 ```
```

### Comparing `fontra-0.2.0/fontra.py` & `fontra-0.2.1/fontra.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,48 +9,81 @@
 
 import freetype
 from typing_extensions import NamedTuple, TypeAlias
 
 FontFamilyName: TypeAlias = str
 StyleName: TypeAlias = str
 
-FONTDIRS_SYSTEM: list[Path] = []
-FONTDIRS_CUSTOM: list[Path] = []
 SUPPORTED_EXT: tuple[str, ...] = (
     ".ttf", ".ttc", ".otf", ".otc", ".cff", ".woff", ".woff2",
     ".pfa", ".pfb", ".pcf", ".fnt", ".bdf", ".pfr"
 )
 SUPPORTED_EXT += tuple(f.upper() for f in SUPPORTED_EXT)
+
+TT_MS_ENCODING_MAPPING = [
+    "utf-16-be", "utf-16-be", "sjis", "cp936", "big5", "cp949", "johab",
+    "", "", "", "utf-16-be"
+]
+TT_MAC_ENCODING_MAPPING = [
+    "mac-roman", "sjis", "big5", "euc-kr", "mac-arabic", "hebrew",
+    "mac-greek", "", "", "", "", "", "", "", "", "", "", "", "", "", "", "",
+    "", "", "", "", "", "", "", "", "", "", ""
+]  # undone as less use
+
+FONTDIRS_SYSTEM: list[Path] = []
+FONTDIRS_CUSTOM: list[Path] = []
 _indexed_fontfiles_system: set[Path] = set()
 _indexed_fontfiles_custom: set[Path] = set()
 
 
 class FontRef(NamedTuple):
     """Data for locating font style."""
     path: Path
     bank: int
 
 
 _indexed_fontrefs: dict[FontFamilyName, dict[StyleName, FontRef]] = {}
 _indexed_langnames: dict[FontFamilyName, FontFamilyName] = {}
 
 
-def sfnt_decode(data: bytes, platform_id: int, language_id: int = -1) -> str:
-    """Decode SFNT content data."""
-    if platform_id != 1:
-        return data.decode("utf-16-be")
-    if language_id == 11:
-        return data.decode("sjis")
-    if language_id == 19:
-        return data.decode("big5")
-    if language_id == 23:
-        return data.decode("euc-kr")
-    if language_id == 33:
-        return data.decode("gb18030")
-    return data.decode()
+def _get_encoding(pid: int, eid: int, lid: int) -> str:
+    # assert freetype.TT_PLATFORM_APPLE_UNICODE == 0
+    if pid == 0:
+        return "utf-16-be"
+    # assert freetype.TT_PLATFORM_MACINTOSH == 1
+    if pid == 1:
+        if eid == 25 and lid == 33:
+            return "gb18030"
+        return TT_MAC_ENCODING_MAPPING[eid] or "unicode_escape"
+    # assert freetype.TT_PLATFORM_MICROSOFT == 3
+    if pid == 3:
+        return TT_MS_ENCODING_MAPPING[eid]
+    return "unicode_escape"
+
+
+def _get_localized_family_name(face: freetype.Face) -> list[tuple[str, int, int, int]]:
+    # assert freetype.TT_NAME_ID_FONT_FAMILY == 1
+    # assert freetype.TT_NAME_ID_PREFERRED_FAMILY == 16
+    _ffname = [
+        (x.string, x.name_id, x.platform_id, x.encoding_id, x.language_id)
+        for x in (
+            face.get_sfnt_name(i) for i in range(face.sfnt_name_count)
+        ) if x.name_id == 16
+    ]
+    if not _ffname:
+        _ffname = [
+            (x.string, x.name_id, x.platform_id, x.encoding_id, x.language_id)
+            for x in (
+                face.get_sfnt_name(i) for i in range(face.sfnt_name_count)
+            ) if x.name_id == 1
+        ]
+    return [
+        (s.decode(_get_encoding(pid, eid, lid)), pid, eid, lid)
+        for s, _, pid, eid, lid in _ffname
+    ]
 
 
 def update_system_fontdirs() -> None:
     """Update system font directories (in `FONTDIRS_SYSTEM`)."""
     FONTDIRS_SYSTEM.clear()
     if sys.platform == "win32":
         if localappdata := os.getenv("LOCALAPPDATA"):
@@ -60,17 +93,17 @@
             ).is_dir():
                 FONTDIRS_SYSTEM.append(_localfontdir)
         if windir := os.getenv("WINDIR"):
             # include system-site font directory
             FONTDIRS_SYSTEM.append(Path(windir) / "fonts")
     elif sys.platform in ("linux", "linux2"):
         if not (xdgdata := os.getenv("XDG_DATA_DIRS")):
-            # thank you xdg
-            # (some weird platforms does not have `/usr/share`)
+            # some weird platforms does not have `/usr/share`
             xdgdata = "/usr/share" if os.path.exists("/usr/share") else ""
+        # thank you xdg
         FONTDIRS_SYSTEM.extend(
             Path(datadir) / "fonts"
             for datadir in xdgdata.split(":") if datadir
         )
     elif sys.platform == "darwin":
         FONTDIRS_SYSTEM.extend(
             (
@@ -107,27 +140,16 @@
 
 def _update_fontref_index(fn: Path, face: freetype.Face) -> None:
     family = cast(bytes, face.family_name).decode()
     style = cast(bytes, face.style_name).decode()
     _indexed_fontrefs.setdefault(family, {})
     _indexed_fontrefs[family][style] = FontRef(fn, face.face_index)
     if face.is_sfnt:
-        _sfnt_dat = [face.get_sfnt_name(i) for i in range(face.sfnt_name_count)]
-        _ffname = [
-            sfnt_decode(x.string, x.platform_id, x.language_id)
-            for x in _sfnt_dat if x.name_id == 16
-        ]  # use short family name first
-        if not _ffname:  # short family name not exist, use standard name
-            _ffname = [
-                sfnt_decode(x.string, x.platform_id, x.language_id)
-                for x in _sfnt_dat if x.name_id == 1
-            ]
-        _indexed_langnames.update({fn: family for fn in _ffname})
-    else:
-        _indexed_langnames.update({family: family})
+        _ffname = _get_localized_family_name(face)
+        _indexed_langnames.update({fn: family for fn, *_ in _ffname if fn != family})
 
 
 def update_fontrefs_index():
     """Update font references index."""
     _indexed_fontrefs.clear()
     _indexed_langnames.clear()
     for fn in (*_indexed_fontfiles_system, *_indexed_fontfiles_custom):
@@ -146,46 +168,48 @@
     The name list is not guaranteed to be sorted.
     """
     return list(_indexed_fontrefs)
 
 
 def unlocalized_name(name: FontFamilyName) -> FontFamilyName:
     """Try convert a name into an unlocalized name."""
-    if name in _indexed_langnames:
-        return _indexed_langnames[name]
-    return name
+    return _indexed_langnames.get(name, name)
 
 
 def get_font(name: str, style: str, localized: bool = True) -> FontRef:
     """Get info for loading correct font faces.
     
     Params:
     - name: font family name.
     - style: font style.
     - localized: whether to lookup localized index.
 
     Return: a named tuple includes file path and collection index.
     """
-    if localized:
-        return _indexed_fontrefs[unlocalized_name(name)][style]
-    return _indexed_fontrefs[name][style]
+    name = unlocalized_name(name) if localized else name
+    if name not in _indexed_fontrefs:
+        raise KeyError(f"Font {name!r} not found")
+    if style not in (_fonts := _indexed_fontrefs[name]):
+        raise KeyError(f"Font style {style!r} of font {name!r} not found")
+    return _fonts[style]
 
 
 def get_font_styles(name: str, localized: bool = True) -> list[StyleName]:
     """Get available font styles.
     
     Params:
     - name: font family name.
     - localized: whether to lookup localized index.
 
     Return: a list includes style names.
     """
-    if localized:
-        return list(_indexed_fontrefs[unlocalized_name(name)].keys())
-    return list(_indexed_fontrefs[name].keys())
+    name = unlocalized_name(name) if localized else name
+    if name not in _indexed_fontrefs:
+        raise KeyError(f"Font {name!r} not found")
+    return [st for st in _indexed_fontrefs[name]]
 
 
 update_system_fontdirs()
 update_system_fontfiles_index()
 update_fontrefs_index()
 
 if __name__ == "__main__":
```

