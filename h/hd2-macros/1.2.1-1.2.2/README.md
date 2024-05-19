# Comparing `tmp/hd2_macros-1.2.1.tar.gz` & `tmp/hd2_macros-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hd2_macros-1.2.1.tar", last modified: Mon May 13 03:30:30 2024, max compression
+gzip compressed data, was "hd2_macros-1.2.2.tar", last modified: Sun May 19 06:07:41 2024, max compression
```

## Comparing `hd2_macros-1.2.1.tar` & `hd2_macros-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/
--rw-rw-rw-   0        0        0     1099 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       91 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6058 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4972 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/hd2_macros/
--rw-rw-rw-   0        0        0       23 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/__init__.py
--rw-rw-rw-   0        0        0       95 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/__main__.py
--rw-rw-rw-   0        0        0     2569 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/config.py
--rw-rw-rw-   0        0        0     1967 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/config.toml
--rw-rw-rw-   0        0        0     5364 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/constants.py
--rw-rw-rw-   0        0        0     6472 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/macro.py
--rw-rw-rw-   0        0        0        0 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/hd2_macros/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/hd2_macros.egg-info/
--rw-rw-rw-   0        0        0     6058 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 03:30:30.000000 hd2_macros-1.2.1/hd2_macros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2024-05-13 03:29:57.000000 hd2_macros-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-05-13 03:30:30.027908 hd2_macros-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 06:07:41.004721 hd2_macros-1.2.2/
+-rw-rw-rw-   0        0        0     1099 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0       91 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6269 2024-05-19 06:07:41.004721 hd2_macros-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 06:07:41.004721 hd2_macros-1.2.2/hd2_macros/
+-rw-rw-rw-   0        0        0       23 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/__init__.py
+-rw-rw-rw-   0        0        0       95 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/__main__.py
+-rw-rw-rw-   0        0        0     2621 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/config.py
+-rw-rw-rw-   0        0        0     2181 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/config.toml
+-rw-rw-rw-   0        0        0     5364 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/constants.py
+-rw-rw-rw-   0        0        0     6853 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/macro.py
+-rw-rw-rw-   0        0        0        0 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/hd2_macros/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-19 06:07:41.004721 hd2_macros-1.2.2/hd2_macros.egg-info/
+-rw-rw-rw-   0        0        0     6269 2024-05-19 06:07:40.000000 hd2_macros-1.2.2/hd2_macros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-05-19 06:07:40.000000 hd2_macros-1.2.2/hd2_macros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 06:07:40.000000 hd2_macros-1.2.2/hd2_macros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-19 06:07:40.000000 hd2_macros-1.2.2/hd2_macros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 06:07:40.000000 hd2_macros-1.2.2/hd2_macros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2024-05-19 06:07:06.000000 hd2_macros-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-05-19 06:07:41.004721 hd2_macros-1.2.2/setup.cfg
```

### Comparing `hd2_macros-1.2.1/LICENSE` & `hd2_macros-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.1/PKG-INFO` & `hd2_macros-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.2.1
+Version: 1.2.2
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
@@ -89,17 +89,21 @@
 # The time in between key UP/DOWN events when inputting macros.
 # Lowering this value will make inputs faster, but may cause inputs to be dropped.
 key_delay = 0.1
 
 # If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
 # autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
 
-# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# You can explicitly specify the version of AutoHotkey (v1 or v2). Usually, this is not necessary.
+# When omitted, the version of Autohotkey is determined automatically
 # autohotkey_version = ""
 
+# The default input type is 'WASD' - you can change this to arrow keys by uncommenting this setting:
+# input_type = "Arrows"
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.2.1/README.md` & `hd2_macros-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,21 @@
 # The time in between key UP/DOWN events when inputting macros.
 # Lowering this value will make inputs faster, but may cause inputs to be dropped.
 key_delay = 0.1
 
 # If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
 # autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
 
-# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# You can explicitly specify the version of AutoHotkey (v1 or v2). Usually, this is not necessary.
+# When omitted, the version of Autohotkey is determined automatically
 # autohotkey_version = ""
 
+# The default input type is 'WASD' - you can change this to arrow keys by uncommenting this setting:
+# input_type = "Arrows"
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.2.1/hd2_macros/config.py` & `hd2_macros-1.2.2/hd2_macros/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     no_tray_icon: bool = False
     win_wait: int = 120
     hotkey_start_delay: int | float = 1.0
     key_delay: int | float = 0.1
     exit_hotkey: str = '#q'
     autohotkey_executable_path: str | None = None
     autohotkey_version: Literal['v1', 'v2'] | None = None
+    input_type: Literal['WASD', 'Arrows'] = 'WASD'
 
 
 class MacroConfig(pydantic.BaseModel):
     general: GeneralSection = pydantic.Field(..., description='General settings')
     loadouts_: dict[str, Loadout] = pydantic.Field(default_factory=dict, alias='loadouts')
     default_loadout: Loadout = pydantic.Field(..., description='The loadout that is used by default at startup')
```

### Comparing `hd2_macros-1.2.1/hd2_macros/config.toml` & `hd2_macros-1.2.2/hd2_macros/config.toml`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,20 @@
 # The time in between key UP/DOWN events when inputting macros.
 # Lowering this value will make inputs faster, but may cause inputs to be dropped.
 key_delay = 0.1
 
 # If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
 # autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
 
-# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# You can explicitly specify the version of AutoHotkey (v1 or v2). Usually, this is not necessary.
+# When omitted, the version of Autohotkey is determined automatically
 # autohotkey_version = ""
 
+# The default input type is 'WASD' - you can change this to arrow keys with by uncommenting this setting:
+# input_type = "Arrows"
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.2.1/hd2_macros/constants.py` & `hd2_macros-1.2.2/hd2_macros/constants.py`

 * *Files identical despite different names*

### Comparing `hd2_macros-1.2.1/hd2_macros/macro.py` & `hd2_macros-1.2.2/hd2_macros/macro.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,32 +62,46 @@
             logging.debug(f'error in getting window process path {e}')
             continue
         if 'helldivers2' in process_path:
             return window
     return None
 
 
-def do_strat_input(strat: T_Stratagems, target: Window, startup_delay: float | int = 1, key_delay: float = 0.1) -> None:
+def do_strat_input(
+    strat: T_Stratagems,
+    target: Window,
+    startup_delay: float | int = 1,
+    key_delay: float = 0.1,
+    input_type: Literal['WASD', 'Arrows'] = 'WASD',
+) -> None:
     time.sleep(startup_delay)
     input_code = STRATAGEMS[strat]
+    is_wasd = input_type == 'WASD'
     for direction in input_code:
-        key = INPUT_MAPPING[direction]
+        if is_wasd:
+            key = INPUT_MAPPING[direction]
+        else:
+            key = direction
         target.send(f'{{Blind}}{{{key} DOWN}}', blocking=False)
         time.sleep(key_delay)
         target.send(f'{{Blind}}{{{key} UP}}', blocking=False)
         time.sleep(key_delay)
     return None
 
 
 def create_macro_function(
-    stratagem: T_Stratagems, target: Window, startup_delay: float | int = 1, key_delay: float = 0.1
+    stratagem: T_Stratagems,
+    target: Window,
+    startup_delay: float | int = 1,
+    key_delay: float = 0.1,
+    input_type: Literal['WASD', 'Arrows'] = 'WASD',
 ) -> Callable[[], Any]:
     def macro() -> None:
         logger.info(f'Performing input for {stratagem}')
-        do_strat_input(stratagem, target, startup_delay, key_delay)
+        do_strat_input(stratagem, target, startup_delay, key_delay, input_type)
 
     return macro
 
 
 def error_handler(key: str, error: Exception) -> None:
     logger.error(f'{key}: {error}')
 
@@ -130,15 +144,17 @@
 
     def create_loadout_switcher(this_name: str, hotkeys: dict[T_Stratagems, str]) -> Callable[[], None]:
         def switch_loadout() -> None:
             logger.info('Switching to loadout %s', this_name)
             ahk.stop_hotkeys()
             ahk.clear_hotkeys()
             for strat, hotkey in hotkeys.items():
-                callback = create_macro_function(strat, hd, config.general.hotkey_start_delay, config.general.key_delay)
+                callback = create_macro_function(
+                    strat, hd, config.general.hotkey_start_delay, config.general.key_delay, config.general.input_type
+                )
                 ahk.add_hotkey(hotkey, callback, ex_handler=error_handler)
             for name, loadout_config in config.loadouts.items():
                 switch_callback = create_loadout_switcher(name, loadout_config.hotkeys)
                 ahk.add_hotkey(loadout_config.switch_hotkey, switch_callback, ex_handler=error_handler)
             ahk.add_hotkey(config.general.exit_hotkey, _exit, ex_handler=error_handler)
             ahk.start_hotkeys()
             return None
@@ -148,15 +164,17 @@
     for loadout_name, loadout in config.loadouts.items():
         logger.debug(f'Initializing loader {loadout_name}')
         callback = create_loadout_switcher(loadout_name, loadout.hotkeys)
         ahk.add_hotkey(loadout.switch_hotkey, callback, ex_handler=error_handler)
 
     for strat, hotkey in config.default_loadout.hotkeys.items():
         logger.debug('Initializing default loadout')
-        callback = create_macro_function(strat, hd, config.general.hotkey_start_delay, config.general.key_delay)
+        callback = create_macro_function(
+            strat, hd, config.general.hotkey_start_delay, config.general.key_delay, config.general.input_type
+        )
         ahk.add_hotkey(hotkey, callback, ex_handler=error_handler)
 
     ahk.add_hotkey(config.general.exit_hotkey, _exit, ex_handler=error_handler)
 
     ahk.start_hotkeys()
     logger.info('hotkey listener started')
     try:
```

### Comparing `hd2_macros-1.2.1/hd2_macros.egg-info/PKG-INFO` & `hd2_macros-1.2.2/hd2_macros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hd2_macros
-Version: 1.2.1
+Version: 1.2.2
 Summary: Helldivers 2 macros
 Home-page: https://github.com/spyoungtech/helldivers2-macros
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Source, https://github.com/spyoungtech/helldivers2-macros
 Project-URL: Tracker, https://github.com/spyoungtech/helldivers2-macros/issues
@@ -89,17 +89,21 @@
 # The time in between key UP/DOWN events when inputting macros.
 # Lowering this value will make inputs faster, but may cause inputs to be dropped.
 key_delay = 0.1
 
 # If you have AutoHotkey in a non-default location, you may specify it by uncommenting this line:
 # autohotkey_executable_path = "C:\Path\To\AutoHotkey64.exe"
 
-# You can explicitly specify the version of AutoHotkey. Usually, this is not necessary.
+# You can explicitly specify the version of AutoHotkey (v1 or v2). Usually, this is not necessary.
+# When omitted, the version of Autohotkey is determined automatically
 # autohotkey_version = ""
 
+# The default input type is 'WASD' - you can change this to arrow keys by uncommenting this setting:
+# input_type = "Arrows"
+
 
 
 # A Loadout provides a mapping of Strategems to hotkeys. Each loadout specifies a hotkey used to switch to that loadout.
 # For hotkey/modifiers syntax, see https://www.autohotkey.com/docs/v2/Hotkeys.htm and https://www.autohotkey.com/docs/v2/KeyList.htm
 
 # The default loadout is the loadout used at program starts
 [ default_loadout ]
```

### Comparing `hd2_macros-1.2.1/setup.cfg` & `hd2_macros-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6432 5f6d 6163 726f 730d 0a76   = hd2_macros..v
-00000020: 6572 7369 6f6e 203d 2031 2e32 2e31 0d0a  ersion = 1.2.1..
+00000020: 6572 7369 6f6e 203d 2031 2e32 2e32 0d0a  ersion = 1.2.2..
 00000030: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000040: 7065 6e63 6572 2e79 6f75 6e67 4073 7079  pencer.young@spy
 00000050: 6f75 6e67 2e63 6f6d 0d0a 6175 7468 6f72  oung.com..author
 00000060: 203d 2053 7065 6e63 6572 2059 6f75 6e67   = Spencer Young
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4865 6c6c 6469 7665 7273 2032 206d 6163  Helldivers 2 mac
 00000090: 726f 730d 0a6c 6f6e 675f 6465 7363 7269  ros..long_descri
```

