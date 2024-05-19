# Comparing `tmp/mentabotix-0.1.4.7.tar.gz` & `tmp/mentabotix-0.1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.7.tar", last modified: Sat May 18 06:02:41 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.8.tar", last modified: Sun May 19 06:08:40 2024, max compression
```

## Comparing `mentabotix-0.1.4.7.tar` & `mentabotix-0.1.4.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-18 06:02:15.047079 mentabotix-0.1.4.7/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-18 06:02:15.047079 mentabotix-0.1.4.7/README.md
--rw-r--r--   0        0        0      680 2024-05-18 06:02:41.475514 mentabotix-0.1.4.7/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    70559 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/find_tests.py
--rw-r--r--   0        0        0    15535 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/test_menta.py
--rw-r--r--   0        0        0     7747 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/test_moving_state.py
--rw-r--r--   0        0        0     5759 2024-05-18 06:02:15.051079 mentabotix-0.1.4.7/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/README.md
+-rw-r--r--   0        0        0      680 2024-05-19 06:08:40.046571 mentabotix-0.1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    70823 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/find_tests.py
+-rw-r--r--   0        0        0    15941 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_menta.py
+-rw-r--r--   0        0        0     7747 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5759 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.8/PKG-INFO
```

### Comparing `mentabotix-0.1.4.7/LICENSE` & `mentabotix-0.1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/README.md` & `mentabotix-0.1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/pyproject.toml` & `mentabotix-0.1.4.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.7"
+version = "0.1.4.8"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.4.7/src/mentabotix/__init__.py` & `mentabotix-0.1.4.8/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.8/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1233,14 +1233,20 @@
         match_expression = "".join(match_expression) if isinstance(match_expression, list) else match_expression
 
         lines: List[str] = [f"match {match_expression}:"]
         for key, value in cases.items():
             case_expr: str = f"'{key}'" if isinstance(key, str) else f"{key}"
             lines.append(self._add_indent(f"case {case_expr}:", count=1))
             lines.extend(self._add_indent(value.split("\n") if isinstance(value, str) else value, count=2))
+        lines.append(self._add_indent(f"case undefined:", count=1))
+        lines.append(
+            self._add_indent(
+                f"raise ValueError(f'No matching case found, got {{undefined}}, not in {list(cases.keys())}')", count=2
+            )
+        )
         return lines
 
     @staticmethod
     def _add_indent(lines: T_EXPR, indent: str = "    ", count: int = 1) -> T_EXPR:
         """
         Adds an indent to each line in the given list of lines or string.
```

### Comparing `mentabotix-0.1.4.7/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.8/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.8/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.8/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.8/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.8/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/tests/find_tests.py` & `mentabotix-0.1.4.8/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/tests/test_botix.py` & `mentabotix-0.1.4.8/tests/test_botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 import unittest
 from typing import List
-from unittest.mock import Mock
 
 from bdmc.modules.controller import CloseLoopController
 
 from mentabotix import Botix, MovingState, MovingTransition
 from mentabotix.modules.exceptions import StructuralError
 
 
@@ -19,15 +18,15 @@
         self.state_c = MovingState(2)
         # 创建一些假的MovingTransition对象用于测试
         self.transition_start_a = MovingTransition(duration=0.1, from_states=self.start_state, to_states=self.state_a)
         self.transition_ab = MovingTransition(duration=1, from_states=[self.state_a], to_states=self.state_b)
         self.transition_bc = MovingTransition(duration=2, from_states=[self.state_b], to_states=self.state_c)
 
         # 初始化一个Botix实例用于测试
-        self.controller_mock = Mock(spec=CloseLoopController)
+        self.controller_mock = CloseLoopController()
         self.token_pool = [self.transition_start_a, self.transition_ab, self.transition_bc]
         self.botix_instance = Botix(controller=self.controller_mock, token_pool=self.token_pool)
 
     def test_get_start(self):
         self.assertEqual(self.start_state, self.botix_instance.acquire_unique_start(self.botix_instance.token_pool))
 
     def test_initialization(self):
@@ -222,14 +221,16 @@
         expected_match_cases = [
             "match some_variable:",
             "    case 'case1':",
             "        result1",
             "            more_result1",
             "    case 'case2':",
             "        result2",
+            "    case undefined:",
+            "        raise ValueError(f'No matching case found, got {undefined}, not in " "['case1', 'case2']')",
         ]
         self.assertEqual(test_instance._assembly_match_cases(match_expression, cases), expected_match_cases)
 
         # Test _add_indent TypeError
         with self.assertRaises(TypeError):
             test_instance._add_indent(123)  # This should raise a TypeError
 
@@ -274,26 +275,29 @@
 
         self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
 
         compiled = self.botix_instance.compile(True)
         self.assertEqual(
             [
                 "def _func():",
-                "    match con.set_motors_speed((100, 100, 100, " "100)).delay_b_match(1,transition0_breaker_1,0.01):",
+                "    match con.set_motors_speed((100, 100, 100, 100)).delay_b_match(1,transition0_breaker_1,0.01):",
                 "        case 1:",
                 "            con.set_motors_speed((200, 200, 200, 200))",
                 "        case 2:",
                 "            con.set_motors_speed((300, 300, 300, 300))",
                 "        case 3:",
-                "            match con.set_motors_speed((400, 400, 400, "
-                "400)).delay_b_match(1,transition1_breaker_1,0.01):",
+                "            match con.set_motors_speed((400, 400, 400, 400)).delay_b_match(1,transition1_breaker_1,0.01):",
                 "                case 1:",
                 "                    con.set_motors_speed((500, 500, 500, 500))",
                 "                case 2:",
                 "                    con.set_motors_speed((600, 600, 600, 600))",
+                "                case undefined:",
+                "                    raise ValueError(f'No matching case found, got {undefined}, not in [1, 2]')",
+                "        case undefined:",
+                "            raise ValueError(f'No matching case found, got {undefined}, not in [1, 2, 3]')",
             ],
             compiled[0],
         )
 
         obj = self.botix_instance.compile()
         obj()
         self.botix_instance.export_structure("test.puml", self.botix_instance.token_pool)
```

### Comparing `mentabotix-0.1.4.7/tests/test_composer.py` & `mentabotix-0.1.4.8/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/tests/test_menta.py` & `mentabotix-0.1.4.8/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/tests/test_moving_state.py` & `mentabotix-0.1.4.8/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/tests/test_moving_transition.py` & `mentabotix-0.1.4.8/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.7/PKG-INFO` & `mentabotix-0.1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.7
+Version: 0.1.4.8
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
```

