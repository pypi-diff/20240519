# Comparing `tmp/plsp-0.25.tar.gz` & `tmp/plsp-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plsp-0.25.tar", last modified: Thu May 16 14:50:09 2024, max compression
+gzip compressed data, was "plsp-0.26.tar", last modified: Sun May 19 16:34:14 2024, max compression
```

## Comparing `plsp-0.25.tar` & `plsp-0.26.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 14:50:09.938819 plsp-0.25/
--rw-rw-rw-   0        0        0     6288 2024-05-16 14:50:09.901322 plsp-0.25/PKG-INFO
--rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.25/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 14:50:09.938819 plsp-0.25/plsp/
--rw-rw-rw-   0        0        0     4630 2024-05-16 09:31:25.000000 plsp-0.25/plsp/DebugContext.py
--rw-rw-rw-   0        0        0      964 2024-05-16 09:31:25.000000 plsp-0.25/plsp/DebugMode.py
--rw-rw-rw-   0        0        0      267 2024-05-16 09:31:25.000000 plsp-0.25/plsp/Direction.py
--rw-rw-rw-   0        0        0     9084 2024-05-16 09:31:25.000000 plsp-0.25/plsp/Logger.py
--rw-rw-rw-   0        0        0     2102 2024-05-16 09:31:25.000000 plsp-0.25/plsp/SharedLogger.py
--rw-rw-rw-   0        0        0     7683 2024-05-16 14:50:09.000000 plsp-0.25/plsp/_README.py
--rw-rw-rw-   0        0        0     2516 2024-05-16 09:31:25.000000 plsp-0.25/plsp/__init__.py
--rw-rw-rw-   0        0        0     8401 2024-05-16 14:50:09.000000 plsp-0.25/plsp/_pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:50:09.897228 plsp-0.25/plsp/formatters/
--rw-rw-rw-   0        0        0     1114 2024-05-16 09:31:25.000000 plsp-0.25/plsp/formatters/FinalFormatter.py
--rw-rw-rw-   0        0        0     1445 2024-05-16 09:31:25.000000 plsp-0.25/plsp/formatters/Formatter.py
--rw-rw-rw-   0        0        0      103 2024-05-16 09:31:25.000000 plsp-0.25/plsp/formatters/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-05-16 09:31:25.000000 plsp-0.25/plsp/formatters/bundled.py
--rw-rw-rw-   0        0        0      243 2024-05-16 09:31:25.000000 plsp-0.25/plsp/formatters/defaults.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:50:09.899248 plsp-0.25/plsp/infoinject/
--rw-rw-rw-   0        0        0    10840 2024-05-16 09:31:25.000000 plsp-0.25/plsp/infoinject/InfoInjector.py
--rw-rw-rw-   0        0        0       38 2024-05-16 09:31:25.000000 plsp-0.25/plsp/infoinject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 14:50:09.900256 plsp-0.25/plsp.egg-info/
--rw-rw-rw-   0        0        0     6288 2024-05-16 14:50:09.000000 plsp-0.25/plsp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2024-05-16 14:50:09.000000 plsp-0.25/plsp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 14:50:09.000000 plsp-0.25/plsp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 14:50:09.000000 plsp-0.25/plsp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 14:50:09.902392 plsp-0.25/setup.cfg
--rw-rw-rw-   0        0        0      287 2024-05-16 13:01:06.000000 plsp-0.25/setup.py
--rw-rw-rw-   0        0        0    22532 2024-05-16 14:50:09.000000 plsp-0.25/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.458130 plsp-0.26/
+-rw-rw-rw-   0        0        0     2280 2024-05-19 16:34:14.420826 plsp-0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     1967 2024-05-19 16:09:31.000000 plsp-0.26/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.458130 plsp-0.26/plsp/
+-rw-rw-rw-   0        0        0     2575 2024-05-19 16:34:14.000000 plsp-0.26/plsp/_README.py
+-rw-rw-rw-   0        0        0     4947 2024-05-19 16:19:28.000000 plsp-0.26/plsp/__Debug_Context.py
+-rw-rw-rw-   0        0        0      975 2024-05-19 15:52:18.000000 plsp-0.26/plsp/__Debug_Mode.py
+-rw-rw-rw-   0        0        0      280 2024-05-19 15:52:08.000000 plsp-0.26/plsp/__IO_Direction.py
+-rw-rw-rw-   0        0        0     9073 2024-05-19 16:19:48.000000 plsp-0.26/plsp/__Logger.py
+-rw-rw-rw-   0        0        0     2114 2024-05-19 15:26:10.000000 plsp-0.26/plsp/__Shared_Logger.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.412620 plsp-0.26/plsp/__infoinject/
+-rw-rw-rw-   0        0        0    10831 2024-05-19 15:55:27.000000 plsp-0.26/plsp/__infoinject/__init__.py
+-rw-rw-rw-   0        0        0     2552 2024-05-19 15:56:02.000000 plsp-0.26/plsp/__init__.py
+-rw-rw-rw-   0        0        0     3165 2024-05-19 16:34:14.000000 plsp-0.26/plsp/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.417550 plsp-0.26/plsp/formatters/
+-rw-rw-rw-   0        0        0     1215 2024-05-19 16:19:07.000000 plsp-0.26/plsp/formatters/I_Final_Formatter.py
+-rw-rw-rw-   0        0        0     1557 2024-05-19 16:19:08.000000 plsp-0.26/plsp/formatters/I_Formatter.py
+-rw-rw-rw-   0        0        0        0 2024-05-19 15:38:35.000000 plsp-0.26/plsp/formatters/__init__.py
+-rw-rw-rw-   0        0        0     1323 2024-05-19 16:17:50.000000 plsp-0.26/plsp/formatters/bundled.py
+-rw-rw-rw-   0        0        0      242 2024-05-19 16:01:56.000000 plsp-0.26/plsp/formatters/defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.419587 plsp-0.26/plsp.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-05-19 16:34:14.000000 plsp-0.26/plsp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2024-05-19 16:34:14.000000 plsp-0.26/plsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:34:14.000000 plsp-0.26/plsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-19 16:34:14.000000 plsp-0.26/plsp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:34:14.421955 plsp-0.26/setup.cfg
+-rw-rw-rw-   0        0        0      287 2024-05-19 16:25:42.000000 plsp-0.26/setup.py
+-rw-rw-rw-   0        0        0    22532 2024-05-19 16:34:14.000000 plsp-0.26/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:34:14.418572 plsp-0.26/tests/
+-rw-rw-rw-   0        0        0     2434 2024-05-19 16:33:04.000000 plsp-0.26/tests/test.py
+-rw-rw-rw-   0        0        0     1333 2024-05-19 16:33:01.000000 plsp-0.26/tests/test_inner.py
```

### Comparing `plsp-0.25/plsp/DebugContext.py` & `plsp-0.26/plsp/__Debug_Context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import sys
-from .DebugMode import DebugMode
-from .formatters.Formatter import IFormatter
-from .formatters.FinalFormatter import IFinalFormatter
-from .formatters.defaults import DefaultFinalFormatter
-from .Direction import IODirection
+from .formatters.I_Formatter import I_Formatter
+from .formatters.I_Final_Formatter import I_Final_Formatter
+from .formatters.defaults import Default_Final_Formatter
+from .__Debug_Mode import Debug_Mode
+from .__IO_Direction import IO_Direction
 
 from io import IOBase, TextIOWrapper
-import base64
+import sys
 
 
 
 
 
 
 
@@ -49,65 +48,83 @@
 
 
 
 
 
 
 
-class DebugContext:
+class Debug_Context:
+
+
+
+	__slots__ = (
+		"name",
+		"format_layers",
+		"final_formatter",
+		"is_active",
+		"directions",
+		"__write_to_handle",
+		"__write_to_file"
+	)
 
 
 
 	def __init__(self, name:str) -> None:
 		self.name = name
 
-		self.format_layers:"list[IFormatter]" = []
-		self.final_formatter:"IFinalFormatter" = DefaultFinalFormatter()
+		self.format_layers:"list[I_Formatter]" = []
+		self.final_formatter:"I_Final_Formatter" = Default_Final_Formatter()
 
-		self.can_ever_write:"bool|None" = None
-		self.directions:"list[IODirection]|None" = None
+		self.is_active:"bool|None" = None
+		self.directions:"list[IO_Direction]|None" = None
 
 
 
-	def set_final_formatter(self, formatter:"IFinalFormatter") -> None:
+	def set_final_formatter(self, formatter:"I_Final_Formatter") -> None:
 		self.final_formatter = formatter
 
 
 
-	def set_can_ever_write(self, can_ever_write:bool) -> None:
-		self.can_ever_write = can_ever_write
+	def set_is_active(self, new_is_active:bool) -> None:
+		self.is_active = new_is_active
 
 
 
-	def add_direction(self, direction:IODirection) -> None:
+	def add_direction(self, do_encode:"bool", file_handle:"int|None"=None, file_path:"str|None"=None) -> None:
 		if self.directions is None:
 			self.directions = []
-		self.directions.append(direction)
+		self.directions.append(
+			IO_Direction(
+				do_encode=do_encode,
+				file_handle=file_handle,
+				file_path=file_path
+			)
+		)
 
 
 
 	def add_format_layer(self, formatter):
 		self.format_layers.append(formatter)
 
 
 
 
-	def _evaluate_instruction(self, instruction_part, arg_part):
+	def __evaluate_instruction(self, instruction_part, arg_part):
 		if instruction_part == "can_ever_write":
-			self.can_ever_write = eval(arg_part)
+			self.is_active = eval(arg_part)
 		
 		elif instruction_part == "write_to_handle":
-			self.write_to_handle = eval(arg_part)
+			self.__write_to_handle = eval(arg_part)
 
 		elif instruction_part == "write_to_file":
-			self.write_to_file = eval(arg_part)
+			self.__write_to_file = eval(arg_part)
 
 
 
-	def __add_contents_to_log(self, contents:str, direction: IODirection) -> None:
+	def __inner__add_contents_to_log(self, contents:str, direction: IO_Direction) -> None:
 		try:
 
 			f = None
 
 			direction.validate()
 
 			if direction.file_handle is not None:
@@ -133,49 +150,55 @@
 				f.close()
 
 
 
 	def _add_contents_to_log(self, contents:str) -> None:
 		assert self.directions is not None, "No directions to write to."
 		for direction in self.directions:
-			self.__add_contents_to_log(contents, direction)
+			self.__inner__add_contents_to_log(contents, direction)
 
 
 
-	def handle(self, debug_mode:"DebugMode", active_debug_level:"DebugMode", *args, **kwargs):
+	def _handle(self, debug_mode:"Debug_Mode", active_debug_level:"Debug_Mode", *args, **kwargs):
 		# QUICK NOTE: the `debug_mode` parameter should be used to change the output and the
 		# `active_debug_mode` parameter should be used to determine if we should write to the output.
 
 		# First check that this context is valid.
-		if self.can_ever_write is None and self.write_to_handle is None:
+		if self.is_active is None and self.__write_to_handle is None:
 			raise Exception("`can_ever_write` and `write_to_handle` cannot both be None.")
 
 		str = ""
 		
 		is_first = True
 		for format_layer in self.format_layers:
-			str = IFormatter.handle(format_layer, str, is_first)
+			str = I_Formatter._handle(format_layer, str, is_first)
 			is_first = False
 		
 		str = self.final_formatter.raw_handle(str)
 		
 		override_instructions = debug_mode.override_instructions or []
 
 		for instruction in override_instructions:
 			instruction_part, arg_part = instruction.split("=")
-			self._evaluate_instruction(instruction_part, arg_part)
+			self.__evaluate_instruction(instruction_part, arg_part)
 
 		# All conditions where we cannot write.
 		if active_debug_level.level == -1 and debug_mode.level == -1:
 			if not active_debug_level.name == debug_mode.name:
 				return
 		elif active_debug_level.level < debug_mode.level:
 			return
-		elif self.can_ever_write is None or (self.can_ever_write is not None and not self.can_ever_write):
+		elif self.is_active is None or (self.is_active is not None and not self.is_active):
 			return
 
 		if active_debug_level.level >= debug_mode.level:
 			_debug_print(self, str, *args, **kwargs)
 			return
 
 		raise Exception("This should never happen.")
-			
+
+
+
+
+
+
+
```

### Comparing `plsp-0.25/plsp/DebugMode.py` & `plsp-0.26/plsp/__Debug_Mode.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 
 
 
 
 
 @dataclasses.dataclass
-class DebugMode:
+class Debug_Mode:
 
 
 
 	name: str
 	level: int
 	override_instructions: "list[str]|None"
 
 
 
-	def set_override_do_ever_write(self, do_ever_write: bool) -> None:
+	def set_override_is_active(self, do_ever_write: bool) -> None:
 		if self.override_instructions is None:
 			self.override_instructions = []
 		self.override_instructions.append(
 			f"do_ever_write={'None' if do_ever_write is None else do_ever_write}"
 		)
 	
 
@@ -37,7 +37,14 @@
 	
 	def set_override_write_to_file(self, file_name: "str|None") -> None:
 		if self.override_instructions is None:
 			self.override_instructions = []
 		self.override_instructions.append(
 			f"write_to_file={'None' if file_name is None else file_name}"
 		)
+
+
+
+
+
+
+
```

### Comparing `plsp-0.25/plsp/Logger.py` & `plsp-0.26/plsp/__Logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .DebugContext import DebugContext, DebugMode
+from .__Debug_Context import Debug_Context, Debug_Mode
 
 from pickle import dumps as pickle_X_dumps
 from pickle import loads as pickle_X_loads
-from typing import Any
+from typing import Any, Literal, TypeAlias
+
+Logger_X_set__ACCEPTED_LITS_T = Literal["global_context"]
 
 
 
 
 
 
 
@@ -174,15 +176,15 @@
 		inst.configuration_vars = data["configuration_vars"]
 		inst.active_debug_mode = data["active_debug_mode"]
 		inst.debug_modes = data["debug_modes"]
 		inst.debug_contexts = data["debug_contexts"]
 		for name in inst.debug_contexts:
 			inst.LOGGER_HELPER.set(name, DynamicVariableContainer(name))
 		for name in inst.debug_modes:
-			inst._update_state_after_adding_debug_mode(name, inst.debug_modes[name].level)
+			inst.__update_state_after_adding_debug_mode(name, inst.debug_modes[name].level)
 		return inst
 
 
 
 	def __init__(self) -> None:
 		"""
 		YOU MUST NEVER CALL THIS DIRECTLY.
@@ -191,22 +193,23 @@
 		    Exception: If the Logger is already initialized. Hence why i said never call this directly.
 
 		Side Effects:
 		- Adds a "disabled" debug mode to the system.
 		"""
 
 		self.configuration_vars = {}
-		self.debug_modes:"dict[str,DebugMode]" = {}
-		self.debug_contexts = {}
-		self.active_debug_mode = None
+		self.debug_modes:"dict[str,Debug_Mode]" = {}
+		self.debug_contexts:"dict[str,Debug_Context]" = {}
 
 		self.LOGGER_HELPER = DynamicVariableContainer("LOGGER_HELPER")
 
-		self._add_debug_mode("disabled", 0)
-		self.get_debug_mode("disabled").set_override_do_ever_write(False)
+		self.__add_debug_mode("disabled", 0)
+		self.debug_modes["disabled"].set_override_is_active(False)
+
+		self.active_debug_mode:"Debug_Mode" = self.debug_modes["disabled"]
 
 
 	
 	def __call__(self, *args: Any, **kwds: Any) -> Any:
 		return self.LOGGER_HELPER
 
 
@@ -218,51 +221,51 @@
 		Args:
 		    name (str): The name of the debug mode to set as active.
 		"""
 		self.active_debug_mode = self.debug_modes[name]
 
 
 
-	def _add_debug_mode(self, name:"str", level:"int"):
+	def __add_debug_mode(self, name:"str", level:"int"):
 		"""
 		YOU MUST NEVER CALL THIS DIRECTLY.
 
 		This is an inner function used by the `add_debug_mode` method (note without the underscore).
 		"""
 
 		# Check that the name isn't already in use.
 		if name in self.debug_modes:
 			raise Exception(f"Debug mode {name} already exists.")
 
 		# Construct the debug mode.
-		self.debug_modes[name] = DebugMode(name, level, None)
+		self.debug_modes[name] = Debug_Mode(name, level, None)
 
-		self._update_state_after_adding_debug_mode(
+		self.__update_state_after_adding_debug_mode(
 			name,
 			level
 		)
 
 	
 
-	def _update_state_after_adding_debug_mode(self, name_of_debug_mode, level):
+	def __update_state_after_adding_debug_mode(self, name_of_debug_mode, level):
 		# The below wrapper is what actually gets called when you do `plsp().<insert name of debug mode>(...)`
 		# NOTE: Remember, this is only for the global context.
 		def wrapper_for_global_handler(*args, **kwargs):
 			context = self.debug_contexts[self.configuration_vars["global_context"]]
 			mode = self.debug_modes[name_of_debug_mode]
-			context.handle(mode, self.active_debug_mode, *args, **kwargs)
+			context._handle(mode, self.active_debug_mode, *args, **kwargs)
 
 		# And here is the wrapper for when we specify a context.
 		# E.g., `plsp().our_context.our_debug_mode(...)`...
 		# This wrapper is the `our_debug_mode` part.
 		# The actual `our_context` is made in the `add_debug_context` method and it is a `DynamicVariableContainer`
 		#  instance that is a child of the `LOGGER_HELPER` instance.
 		def wrapper_for_context_specified_handler(context, *args, **kwargs):
 			mode = self.debug_modes[name_of_debug_mode]
-			context.handle(mode, self.active_debug_mode, *args, **kwargs)
+			context._handle(mode, self.active_debug_mode, *args, **kwargs)
 
 		# We only want to use the `wrapper_for_global_handler` if the global context is set.
 		if self.configuration_vars.get("global_context") is not None:
 			self.LOGGER_HELPER.set(name_of_debug_mode, wrapper_for_global_handler)
 
 		# Now to update the context-specific wrappers.
 		keys_no_globals = [k for k in self.LOGGER_HELPER.get_children().keys() if k not in self.debug_modes.keys()]
@@ -294,41 +297,33 @@
 		"""
 
 		if separate:
 			level = -1
 		else:
 			level = len(self.debug_modes)+1
 
-		self._add_debug_mode(name, level)
+		self.__add_debug_mode(name, level)
 
 
 
 	def add_debug_context(self, name:"str"):
 		if name in self.debug_contexts:
 			raise Exception(f"Debug context {name} already exists.")
-		self.debug_contexts[name] = DebugContext(name)
+		self.debug_contexts[name] = Debug_Context(name)
 		self.LOGGER_HELPER.set(name, DynamicVariableContainer(name))
 
 
 
-	def get_debug_context(self, name:"str") -> "DebugContext":
-		return self.debug_contexts[name]
-	
-
-
-	def get_debug_mode(self, name:"str") -> "DebugMode":
-		return self.debug_modes[name]
-
-
-
-	def set(self, name:"str", value) -> None:
+	def set(self, name:"Logger_X_set__ACCEPTED_LITS_T", value) -> None:
 		accepted_vars = ["global_context"]
 
 		if name not in accepted_vars:
 			raise Exception(f"Variable {name} not accepted.")
 
 		self.configuration_vars[name] = value
 
+		
+
```

### Comparing `plsp-0.25/plsp/SharedLogger.py` & `plsp-0.26/plsp/__Shared_Logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .Logger import Logger
+from .__Logger import Logger
 
 from os.path import exists as os_path_X_exists
 from os import remove as os_X_remove
 from os.path import dirname as os_path_X_dirname
 from os.path import join as os_path_X_join
 from os import mkdir as os_X_mkdir
 from os import walk as os_X_walk
@@ -65,7 +65,12 @@
 		raise Exception("Could not find the specified file.")
 
 	with open(os_path_X_join(temp_dir, found_file), "rb") as file:
 		return Logger._pickle_load(
 			pickle_X_loads(file.read())
 		)
 				
+
+
+
+
+
```

### Comparing `plsp-0.25/plsp/__init__.py` & `plsp-0.26/plsp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 
 
 
 
 
 
-from .Logger import Logger
-from .SharedLogger import load as load_logger
-from .SharedLogger import save as save_logger
-from .DebugContext import DebugContext
-from .DebugMode import DebugMode
-from .Direction import IODirection
+from .__Shared_Logger import load as load_logger
+from .__Shared_Logger import save as save_logger
+from .__Logger import Logger
+from .__Debug_Context import Debug_Context
+from .__Debug_Mode import Debug_Mode
+from .__IO_Direction import IO_Direction
 
-from . import infoinject
+from .__infoinject import infoinject
 from . import formatters
 
 
 
 
 
 
+
 """
 
 =====================
 Pieces of the puzzle.
 =====================
 
 Logger 			- The piece that does the logging.
```

### Comparing `plsp-0.25/plsp/formatters/FinalFormatter.py` & `plsp-0.26/plsp/formatters/I_Final_Formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from abc import ABC, abstractmethod
+from abc import ABC as __abc_X_ABC
+from abc import abstractmethod as _abc_X_abstractmethod
 
-import base64
+import base64 as _base64
 
 
 
 
 
 
 
-class IFinalFormatter(ABC):
+class I_Final_Formatter(__abc_X_ABC):
 
 
 
 	# NOTE: The point of having postfixes is so the final formatter can know the different pieces.
 	def _get_unique_postfix(self) -> str:
 		name = self.__class__.__name__
-		b64_name = base64.b64encode(name.encode("utf-8")).decode("utf-8")
+		b64_name = _base64.b64encode(name.encode("utf-8")).decode("utf-8")
 		return f"|`FORMATTER_POSTFIX`{b64_name}|"
 
 
 
 	def _strip_postfixes(self, string:str) -> str:
 		# example string: `abc - foo|def - bar|ghi - hi|`
 
@@ -43,10 +44,17 @@
 			assert end is not None
 			ret_str += splitted[end:]
 		
 		return ret_str
 				
 
 
-	@abstractmethod
+	@_abc_X_abstractmethod
 	def raw_handle(self, string:str) -> str:
-		pass
+		pass
+
+
+
+
+
+
+
```

### Comparing `plsp-0.25/plsp/formatters/Formatter.py` & `plsp-0.26/plsp/formatters/I_Formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from abc import ABC, abstractmethod
+from abc import ABC as __abc_X_ABC
+from abc import abstractmethod as _abc_X_abstractmethod
 
-import base64
+import base64 as _base64
 
 
 
 
 
 
 
-class IFormatter(ABC):
+class I_Formatter(__abc_X_ABC):
 
 
 
 	def __init__(self):
 		super().__init__()
 
 
 
 	# NOTE: The point of having postfixes is so the final formatter can know the different pieces.
 	def _get_unique_postfix(self) -> str:
 		name = self.__class__.__name__
-		b64_name = base64.b64encode(name.encode("utf-8")).decode("utf-8")
+		b64_name = _base64.b64encode(name.encode("utf-8")).decode("utf-8")
 		return f"|`FORMATTER_POSTFIX`{b64_name}|"
 
 
 
 	@staticmethod
-	def _strip_postfixes(string:str) -> str:
+	def __strip_postfixes(string:str) -> str:
 		# example string: `abc - foo|def - bar|ghi - hi|`
 
 		if not string.endswith("|"):
 			raise Exception("This should never happen.")
 
 		ret_str = ""
 		_splitted = string.split("|`FORMATTER_POSTFIX`")[:-1]  # last is always fluff.
@@ -47,20 +48,26 @@
 			ret_str += splitted[end:]
 		
 		return ret_str
 				
 
 
 	@staticmethod
-	def handle(inst, string:str, is_first: bool) -> str:
+	def _handle(inst, string:str, is_first: bool) -> str:
 		if not is_first:
-			string = IFormatter._strip_postfixes(string)
-		addition = inst._handle(string)
+			string = I_Formatter.__strip_postfixes(string)
+		addition = inst._impl_handle(string)
 		if addition is None:
 			raise Exception("The formatter did not return a string.")
 		return f"{addition}{inst._get_unique_postfix()}"
 
 
 
-	@abstractmethod
-	def _handle(self, string:str) -> str:
-		pass
+	@_abc_X_abstractmethod
+	def _impl_handle(self, string:str) -> str:
+		pass
+
+
+
+
+
+
```

### Comparing `plsp-0.25/plsp/formatters/bundled.py` & `plsp-0.26/plsp/formatters/bundled.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from .Formatter import IFormatter
+from .I_Formatter import I_Formatter as __I_Formatter
 
-from typing import Callable
-from datetime import datetime
+from typing import Callable as __typing_X_Callable
+from datetime import datetime as _datetime_X_datetime
 
 
 
-class TimeFormatter (IFormatter):
+class Time_Formatter (__I_Formatter):
 	def __default_further_parse_data(self, string:str) -> str:
 		rd_or_st_or_th = None
 		day_part = string.split("/")[0]
 		rest_part = "/".join(string.split("/")[1:])
 		if day_part.endswith("1"):
 			rd_or_st_or_th = "st"
 		elif day_part.endswith("2"):
 			rd_or_st_or_th = "nd"
 		elif day_part.endswith("3"):
 			rd_or_st_or_th = "rd"
 		else:
 			rd_or_st_or_th = "th"
 		return f"{day_part}{rd_or_st_or_th}/{rest_part}"
 
-	def __init__(self, format_string:"str|None"=None, further_parse_data:"Callable[[str],str]|None"=None):
+	def __init__(self, format_string:"str|None"=None, further_parse_data:"__typing_X_Callable[[str],str]|None"=None):
 		super().__init__()
 		self.format_string = "%d/%m/%y@%H:%M:%S.%f" if not format_string else format_string
 		if further_parse_data is None:
 			self.format_string = self.__default_further_parse_data(self.format_string)
 		else:
 			self.format_string = further_parse_data(self.format_string)
 
-	def _handle(self, string:str) -> str:
-		formatted_time = datetime.now().strftime(self.format_string)
+	def _impl_handle(self, string:str) -> str:
+		formatted_time = _datetime_X_datetime.now().strftime(self.format_string)
 		ret_str = ""
 		sep = "|||"
 		for line in string.split("\n"):
 			ret_str += f"[{formatted_time}] {sep} {line}"
 			sep = "---"
 		return ret_str
```

### Comparing `plsp-0.25/plsp/infoinject/InfoInjector.py` & `plsp-0.26/plsp/__infoinject/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Callable
 import inspect
 import re
 
 
 
 
 
 
 
-class _InfoInjector:
+class __Info_Injector:
 
 
 
 	def __init__(self):
 
 		self._instruction_stack = []
 
@@ -390,8 +389,16 @@
 		return s == str
 
 		# End of `def _find_if_str_ahead(self, source, i, str):`
 
 
 
 
-InfoInjector = _InfoInjector()
+infoinject = __Info_Injector()
+
+
+
+
+
+
+
+
```

### Comparing `plsp-0.25/templated_setup.py` & `plsp-0.26/templated_setup.py`

 * *Files identical despite different names*

