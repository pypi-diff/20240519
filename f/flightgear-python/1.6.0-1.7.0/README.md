# Comparing `tmp/flightgear_python-1.6.0.tar.gz` & `tmp/flightgear_python-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightgear_python-1.6.0.tar", max compression
+gzip compressed data, was "flightgear_python-1.7.0.tar", max compression
```

## Comparing `flightgear_python-1.6.0.tar` & `flightgear_python-1.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1083 2024-01-21 23:46:29.386607 flightgear_python-1.6.0/LICENSE
--rw-r--r--   0        0        0     3235 2024-01-21 23:46:29.386607 flightgear_python-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/__init__.py
--rw-r--r--   0        0        0     3686 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/ctrls_v27.py
--rw-r--r--   0        0        0     2915 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/fdm_v24.py
--rw-r--r--   0        0        0     3211 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/fdm_v25.py
--rwxr-xr-x   0        0        0    21190 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/fg_if.py
--rw-r--r--   0        0        0     1706 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/fg_util.py
--rw-r--r--   0        0        0     2939 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/general_util.py
--rw-r--r--   0        0        0     1666 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/flightgear_python/gui_v8.py
--rw-r--r--   0        0        0     1912 2024-01-21 23:46:29.390607 flightgear_python-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4006 2024-01-21 23:47:03.630063 flightgear_python-1.6.0/setup.py
--rw-r--r--   0        0        0     4161 2024-01-21 23:47:03.630662 flightgear_python-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-19 17:10:23.517816 flightgear_python-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3219 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/__init__.py
+-rw-r--r--   0        0        0     3686 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/ctrls_v27.py
+-rw-r--r--   0        0        0     2915 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/fdm_v24.py
+-rw-r--r--   0        0        0     3211 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/fdm_v25.py
+-rwxr-xr-x   0        0        0    24254 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/fg_if.py
+-rw-r--r--   0        0        0     1706 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/fg_util.py
+-rw-r--r--   0        0        0     2939 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/general_util.py
+-rw-r--r--   0        0        0     1666 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/flightgear_python/gui_v8.py
+-rw-r--r--   0        0        0     1912 2024-05-19 17:10:23.521816 flightgear_python-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3990 2024-05-19 17:11:03.855410 flightgear_python-1.7.0/setup.py
+-rw-r--r--   0        0        0     4145 2024-05-19 17:11:03.855766 flightgear_python-1.7.0/PKG-INFO
```

### Comparing `flightgear_python-1.6.0/LICENSE` & `flightgear_python-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/README.md` & `flightgear_python-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 
 """
 Start FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`
 (you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with
 these external commands)
 """
 if __name__ == '__main__':  # NOTE: This is REQUIRED on Windows!
-    fdm_conn = FDMConnection(fdm_version=24)  # May need to change version from 24
+    fdm_conn = FDMConnection()
     fdm_event_pipe = fdm_conn.connect_rx('localhost', 5501, fdm_callback)
     fdm_conn.connect_tx('localhost', 5502)
     fdm_conn.start()  # Start the FDM RX/TX loop
     
     phi_rad_parent = 0.0
     while True:
         phi_rad_parent += 0.1
         # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`
         fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple
         time.sleep(0.5)
 ```
 
 Supported interfaces:
 - [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)
-  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))
-  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))
-  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
+  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx)) version 24, 25
+  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx)) version 27
+  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx)) version 8
 - [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)
 - [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)
 - [x] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)
```

### Comparing `flightgear_python-1.6.0/flightgear_python/ctrls_v27.py` & `flightgear_python-1.7.0/flightgear_python/ctrls_v27.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/flightgear_python/fdm_v24.py` & `flightgear_python-1.7.0/flightgear_python/fdm_v24.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/flightgear_python/fdm_v25.py` & `flightgear_python-1.7.0/flightgear_python/fdm_v25.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/flightgear_python/fg_if.py` & `flightgear_python-1.7.0/flightgear_python/fg_if.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 import sys
 import re
 from typing import Any, ByteString, Callable, Dict, Optional, Tuple, Union, List, NamedTuple
 
 import multiprocess as mp
 import requests
 
-from construct import ConstError, Struct, Container
+from construct import ConstError, Struct, Container, Construct, Int32ub, Int32ul
 
 from .general_util import EventPipe, strip_end, deprecate_rename_wrapper
 from .fg_util import FGConnectionError, FGCommunicationError, fix_fg_radian_parsing
+from .fdm_v24 import fdm_struct as fdm_struct_v24
+from .fdm_v25 import fdm_struct as fdm_struct_v25
+from .ctrls_v27 import ctrls_struct as ctrls_struct_v27
+from .gui_v8 import gui_struct as gui_struct_v8
 
 rx_callback_type = Callable[[Container, EventPipe], Optional[Container]]
 """
 RX callback function type, signature should be:
 
 .. code-block:: python
 
@@ -30,14 +34,15 @@
     Base class for FlightGear connections
     sphinx-no-autodoc
     :param rx_timeout_s: Optional timeout value in seconds when receiving data
     """
 
     # These are filled from the child class
     fg_net_struct: Optional[Struct] = None
+    fg_auto_partial_parse: Optional['PartialParseSwitchStruct'] = None
 
     def __init__(self, rx_timeout_s: float = 2.0):
         self.event_pipe = EventPipe(duplex=True)
 
         self.fg_rx_sock: Optional[socket.socket] = None
         self.fg_rx_cb: Optional[rx_callback_type] = None
 
@@ -103,14 +108,19 @@
             """
             if '10035' in str(e):
                 self.fg_rx_sock.setblocking(True)
                 return
             else:
                 raise e
 
+        # Auto-version logic
+        if self.fg_auto_partial_parse and self.fg_net_struct is None:
+            # We lazily create the actual struct that will be used for parsing
+            self.fg_net_struct = self.fg_auto_partial_parse.resolve(rx_msg)
+
         try:
             s: Container = self.fg_net_struct.parse(rx_msg)
         except ConstError as e:
             raise FGCommunicationError(f'Could not decode FG stream. Did you set the right version?\n{e}') from e
 
         if isinstance(self, FDMConnection):
             # Fix FG's radian parsing error :(
@@ -134,81 +144,128 @@
             self._fg_packet_roundtrip()
 
     def start(self):
         """
         Start the RX/TX loop with FlightGear
         """
         self.rx_proc = mp.Process(target=self._rx_process)
+        self.rx_proc.daemon = True  # rx_proc should exit when parent exits
         self.rx_proc.start()
         _ = self.event_pipe.parent_recv()  # Wait for child to actually run
 
     def stop(self):
         """
         Stop the RX/TX loop
         """
         self.rx_proc.terminate()
 
 
+class PartialParseSwitchStruct:
+    """
+    A utility class that allows runtime switching of which version of a struct
+    is used to parse an incoming message. We use this (complexity) instead of
+    construct's conditional utilities because it makes looking at the individual
+    struct versions a bit less overwhelming, and easier to compare.
+    sphinx-no-autodoc
+    :param partial_parse_construct: The Construct that will be used to switch which
+    version of the Struct is resolved
+    :param replacement_full_structs: Mapping of struct versions to Structs
+    """
+
+    def __init__(self, partial_parse_construct: Construct, replacement_full_structs: Dict[Any, Struct]):
+        self.partial_parse_construct = partial_parse_construct
+        self.replacement_full_structs = replacement_full_structs
+
+    def resolve(self, message: bytes) -> Struct:
+        """
+        Resolve a message to a full Struct
+        :param message: The message to partially parse
+        :return: The full Struct based on the partial parsing of the message
+        """
+        version: Any = self.partial_parse_construct.parse(message)
+        supported_version_list = list(self.replacement_full_structs.keys())
+        if version not in supported_version_list:
+            raise FGCommunicationError(
+                f'Auto-version detected {version} is not in the list of supported versions: {supported_version_list}'
+            )
+        return self.replacement_full_structs[version]
+
+
 class FDMConnection(FGConnection):
     """
     FlightGear Flight Dynamics Model Connection
 
-    :param fdm_version: Net FDM version (24 or 25)
+    :param fdm_version: Net FDM version (24, 25, or None for auto-detection)
     :param rx_timeout_s: Optional timeout value in seconds when receiving data
     """
 
-    def __init__(self, fdm_version: int, rx_timeout_s: float = 2.0):
+    def __init__(self, fdm_version: Optional[int] = None, rx_timeout_s: float = 2.0):
         super().__init__(rx_timeout_s=rx_timeout_s)
-        # TODO: Support auto-version check
-        if fdm_version == 24:
-            from .fdm_v24 import fdm_struct
-        elif fdm_version == 25:
-            from .fdm_v25 import fdm_struct
+        fdm_support_dict: Dict[int, Struct] = {
+            24: fdm_struct_v24,
+            25: fdm_struct_v25,
+        }
+
+        if fdm_version is None:
+            self.fg_auto_partial_parse = PartialParseSwitchStruct(
+                partial_parse_construct=Int32ub,
+                replacement_full_structs=fdm_support_dict,
+            )
         else:
-            raise NotImplementedError(f'FDM version {fdm_version} not supported yet')
-
-        self.fg_net_struct = fdm_struct
+            self.fg_net_struct = fdm_support_dict.get(fdm_version)
+            if self.fg_net_struct is None:
+                raise NotImplementedError(f'Manually specified FDM version {fdm_version} not supported yet')
 
 
 class CtrlsConnection(FGConnection):
     """
     FlightGear Controls Connection
 
-    :param ctrls_version: Net Ctrls version (27)
+    :param ctrls_version: Net Ctrls version (27, or None for auto-detection)
     :param rx_timeout_s: Optional timeout value in seconds when receiving data
     """
 
-    def __init__(self, ctrls_version: int, rx_timeout_s: float = 2.0):
+    def __init__(self, ctrls_version: Optional[int] = None, rx_timeout_s: float = 2.0):
         super().__init__(rx_timeout_s=rx_timeout_s)
-        # TODO: Support auto-version check
-        if ctrls_version == 27:
-            from .ctrls_v27 import ctrls_struct
+        ctrls_support_dict: Dict[int, Struct] = {
+            27: ctrls_struct_v27,
+        }
+        if ctrls_version is None:
+            self.fg_auto_partial_parse = PartialParseSwitchStruct(
+                partial_parse_construct=Int32ub,
+                replacement_full_structs=ctrls_support_dict,
+            )
         else:
-            raise NotImplementedError(f'Controls version {ctrls_version} not supported yet')
-
-        self.fg_net_struct = ctrls_struct
+            self.fg_net_struct = ctrls_support_dict.get(ctrls_version)
+            if self.fg_net_struct is None:
+                raise NotImplementedError(f'Manually specified Controls version {ctrls_version} not supported yet')
 
 
 class GuiConnection(FGConnection):
     """
     FlightGear GUI Connection
 
-    :param gui_version: Net GUI version (8)
+    :param gui_version: Net GUI version (8, or None for auto-detection)
     :param rx_timeout_s: Optional timeout value in seconds when receiving data
     """
 
-    def __init__(self, gui_version: int, rx_timeout_s: float = 2.0):
+    def __init__(self, gui_version: Optional[int] = None, rx_timeout_s: float = 2.0):
         super().__init__(rx_timeout_s=rx_timeout_s)
-        # TODO: Support auto-version check
-        if gui_version == 8:
-            from .gui_v8 import gui_struct
+        gui_support_dict: Dict[int, Struct] = {
+            8: gui_struct_v8,
+        }
+        if gui_version is None:
+            self.fg_auto_partial_parse = PartialParseSwitchStruct(
+                partial_parse_construct=Int32ul,
+                replacement_full_structs=gui_support_dict,
+            )
         else:
-            raise NotImplementedError(f'GUI version {gui_version} not supported yet')
-
-        self.fg_net_struct = gui_struct
+            self.fg_net_struct = gui_support_dict.get(gui_version)
+            if self.fg_net_struct is None:
+                raise NotImplementedError(f'Manually specified GUI version {gui_version} not supported yet')
 
 
 class PropertyTreeValue(NamedTuple):
     """
     Internal representation for working with values from the property tree
     sphinx-no-autodoc
     """
```

### Comparing `flightgear_python-1.6.0/flightgear_python/fg_util.py` & `flightgear_python-1.7.0/flightgear_python/fg_util.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/flightgear_python/general_util.py` & `flightgear_python-1.7.0/flightgear_python/general_util.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/flightgear_python/gui_v8.py` & `flightgear_python-1.7.0/flightgear_python/gui_v8.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.6.0/pyproject.toml` & `flightgear_python-1.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flightgear_python"
-version = "1.6.0"
+version = "1.7.0"
 description = "Interface for FlightGear network connections"
 authors = ["Julianne Swinoga <julianneswinoga@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
```

### Comparing `flightgear_python-1.6.0/setup.py` & `flightgear_python-1.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['construct>=2.10,<3.0', 'multiprocess==0.70.12.2', 'requests==2.27.1']
 
 setup_kwargs = {
     'name': 'flightgear-python',
-    'version': '1.6.0',
+    'version': '1.7.0',
     'description': 'Interface for FlightGear network connections',
-    'long_description': '# FlightGear Python Interface\n[![Documentation Status](https://readthedocs.org/projects/flightgear-python/badge/?version=latest)](https://flightgear-python.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/flightgear-python.svg?style=shield)](https://circleci.com/gh/julianneswinoga/flightgear-python)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/flightgear-python/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/flightgear-python?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flightgear_python)](https://pypi.org/project/flightgear-python/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/flightgear-python)](https://pypistats.org/packages/flightgear-python)\n\n`flightgear-python` is an interface package to the [FlightGear flight simulation software](https://www.flightgear.org/) aimed at simplicity.\n\nInstall: `pip3 install flightgear-python`\n\nDon\'t know where to begin? Check out the [quick-start](https://flightgear-python.readthedocs.io/en/latest/quickstart.html) documentation.\n\nFlight Dynamics Model (FDM) example, from `examples/simple_fdm.py`\n```python\n"""\nSimple Flight Dynamics Model (FDM) example that makes the altitude increase and the plane roll in the air.\n"""\nimport time\nfrom flightgear_python.fg_if import FDMConnection\n\ndef fdm_callback(fdm_data, event_pipe):\n    if event_pipe.child_poll():\n        phi_rad_child, = event_pipe.child_recv()  # unpack tuple\n        # set only the data that we need to\n        fdm_data[\'phi_rad\'] = phi_rad_child  # we can force our own values\n    fdm_data.alt_m = fdm_data.alt_m + 0.5  # or just make a relative change\n    return fdm_data  # return the whole structure\n\n"""\nStart FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`\n(you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with\nthese external commands)\n"""\nif __name__ == \'__main__\':  # NOTE: This is REQUIRED on Windows!\n    fdm_conn = FDMConnection(fdm_version=24)  # May need to change version from 24\n    fdm_event_pipe = fdm_conn.connect_rx(\'localhost\', 5501, fdm_callback)\n    fdm_conn.connect_tx(\'localhost\', 5502)\n    fdm_conn.start()  # Start the FDM RX/TX loop\n    \n    phi_rad_parent = 0.0\n    while True:\n        phi_rad_parent += 0.1\n        # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`\n        fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple\n        time.sleep(0.5)\n```\n\nSupported interfaces:\n- [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)\n  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))\n  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))\n  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))\n- [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)\n- [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)\n- [x] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)\n',
+    'long_description': '# FlightGear Python Interface\n[![Documentation Status](https://readthedocs.org/projects/flightgear-python/badge/?version=latest)](https://flightgear-python.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/flightgear-python.svg?style=shield)](https://circleci.com/gh/julianneswinoga/flightgear-python)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/flightgear-python/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/flightgear-python?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flightgear_python)](https://pypi.org/project/flightgear-python/)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/flightgear-python)](https://pypistats.org/packages/flightgear-python)\n\n`flightgear-python` is an interface package to the [FlightGear flight simulation software](https://www.flightgear.org/) aimed at simplicity.\n\nInstall: `pip3 install flightgear-python`\n\nDon\'t know where to begin? Check out the [quick-start](https://flightgear-python.readthedocs.io/en/latest/quickstart.html) documentation.\n\nFlight Dynamics Model (FDM) example, from `examples/simple_fdm.py`\n```python\n"""\nSimple Flight Dynamics Model (FDM) example that makes the altitude increase and the plane roll in the air.\n"""\nimport time\nfrom flightgear_python.fg_if import FDMConnection\n\ndef fdm_callback(fdm_data, event_pipe):\n    if event_pipe.child_poll():\n        phi_rad_child, = event_pipe.child_recv()  # unpack tuple\n        # set only the data that we need to\n        fdm_data[\'phi_rad\'] = phi_rad_child  # we can force our own values\n    fdm_data.alt_m = fdm_data.alt_m + 0.5  # or just make a relative change\n    return fdm_data  # return the whole structure\n\n"""\nStart FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`\n(you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with\nthese external commands)\n"""\nif __name__ == \'__main__\':  # NOTE: This is REQUIRED on Windows!\n    fdm_conn = FDMConnection()\n    fdm_event_pipe = fdm_conn.connect_rx(\'localhost\', 5501, fdm_callback)\n    fdm_conn.connect_tx(\'localhost\', 5502)\n    fdm_conn.start()  # Start the FDM RX/TX loop\n    \n    phi_rad_parent = 0.0\n    while True:\n        phi_rad_parent += 0.1\n        # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`\n        fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple\n        time.sleep(0.5)\n```\n\nSupported interfaces:\n- [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)\n  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx)) version 24, 25\n  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx)) version 27\n  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx)) version 8\n- [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)\n- [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)\n- [x] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)\n',
     'author': 'Julianne Swinoga',
     'author_email': 'julianneswinoga@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `flightgear_python-1.6.0/PKG-INFO` & `flightgear_python-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightgear-python
-Version: 1.6.0
+Version: 1.7.0
 Summary: Interface for FlightGear network connections
 License: MIT
 Author: Julianne Swinoga
 Author-email: julianneswinoga@gmail.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,29 +51,29 @@
 
 """
 Start FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`
 (you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with
 these external commands)
 """
 if __name__ == '__main__':  # NOTE: This is REQUIRED on Windows!
-    fdm_conn = FDMConnection(fdm_version=24)  # May need to change version from 24
+    fdm_conn = FDMConnection()
     fdm_event_pipe = fdm_conn.connect_rx('localhost', 5501, fdm_callback)
     fdm_conn.connect_tx('localhost', 5502)
     fdm_conn.start()  # Start the FDM RX/TX loop
     
     phi_rad_parent = 0.0
     while True:
         phi_rad_parent += 0.1
         # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`
         fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple
         time.sleep(0.5)
 ```
 
 Supported interfaces:
 - [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)
-  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))
-  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))
-  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
+  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx)) version 24, 25
+  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx)) version 27
+  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx)) version 8
 - [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)
 - [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)
 - [x] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)
```

