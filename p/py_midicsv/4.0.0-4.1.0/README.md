# Comparing `tmp/py_midicsv-4.0.0.tar.gz` & `tmp/py_midicsv-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_midicsv-4.0.0.tar", max compression
+gzip compressed data, was "py_midicsv-4.1.0.tar", max compression
```

## Comparing `py_midicsv-4.0.0.tar` & `py_midicsv-4.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/LICENSE
--rw-r--r--   0        0        0     3882 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/README.md
--rw-r--r--   0        0        0      174 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/__init__.py
--rw-r--r--   0        0        0     2707 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/cli.py
--rw-r--r--   0        0        0     4999 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/csv_converters.py
--rw-r--r--   0        0        0     1357 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/csvmidi.py
--rw-r--r--   0        0        0     2480 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/events.py
--rw-r--r--   0        0        0        0 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/__init__.py
--rw-r--r--   0        0        0     1571 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/constants.py
--rw-r--r--   0        0        0     2610 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/containers.py
--rw-r--r--   0        0        0    11190 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/events.py
--rw-r--r--   0        0        0     9796 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/fileio.py
--rw-r--r--   0        0        0      877 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi/util.py
--rw-r--r--   0        0        0     4530 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midi_converters.py
--rw-r--r--   0        0        0     1019 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/py_midicsv/midicsv.py
--rw-r--r--   0        0        0     1130 2023-02-12 20:44:40.805349 py_midicsv-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     4864 1970-01-01 00:00:00.000000 py_midicsv-4.0.0/setup.py
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 py_midicsv-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/LICENSE
+-rw-r--r--   0        0        0     3882 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/README.md
+-rw-r--r--   0        0        0      174 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/__init__.py
+-rw-r--r--   0        0        0     2707 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/cli.py
+-rw-r--r--   0        0        0     5018 2024-05-19 15:41:25.593467 py_midicsv-4.1.0/py_midicsv/csv_converters.py
+-rw-r--r--   0        0        0     1357 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/csvmidi.py
+-rw-r--r--   0        0        0     2480 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/events.py
+-rw-r--r--   0        0        0        0 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/__init__.py
+-rw-r--r--   0        0        0     1571 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/constants.py
+-rw-r--r--   0        0        0     2550 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/containers.py
+-rw-r--r--   0        0        0    11220 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/events.py
+-rw-r--r--   0        0        0     9796 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/fileio.py
+-rw-r--r--   0        0        0      877 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi/util.py
+-rw-r--r--   0        0        0     4534 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midi_converters.py
+-rw-r--r--   0        0        0     1019 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/py_midicsv/midicsv.py
+-rw-r--r--   0        0        0     1148 2024-05-19 15:41:25.597467 py_midicsv-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 py_midicsv-4.1.0/PKG-INFO
```

### Comparing `py_midicsv-4.0.0/LICENSE` & `py_midicsv-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/README.md` & `py_midicsv-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/cli.py` & `py_midicsv-4.1.0/py_midicsv/cli.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/csv_converters.py` & `py_midicsv-4.1.0/py_midicsv/csv_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,45 +18,45 @@
                 midi_bytes += struct.pack("B", int(Nstr, base=8))
         else:
             midi_bytes += struct.pack("B", ord(c))
     return midi_bytes
 
 
 def to_NoteOffEvent(track, time, identifier, line):
-    channel, pitch, velocity = map(int, line)
+    channel, pitch, velocity = map(int, line[:3])
     return NoteOffEvent(tick=time, channel=channel, pitch=pitch, velocity=velocity)
 
 
 def to_NoteOnEvent(track, time, identifier, line):
-    channel, pitch, velocity = map(int, line)
+    channel, pitch, velocity = map(int, line[:3])
     return NoteOnEvent(tick=time, channel=channel, pitch=pitch, velocity=velocity)
 
 
 def to_AfterTouchEvent(track, time, identifier, line):
-    channel, pitch, value = map(int, line)
+    channel, pitch, value = map(int, line[:3])
     return AfterTouchEvent(tick=time, channel=channel, pitch=pitch, value=value)
 
 
 def to_ControlChangeEvent(track, time, identifier, line):
-    channel, control, value = map(int, line)
+    channel, control, value = map(int, line[:3])
     return ControlChangeEvent(tick=time, channel=channel, control=control, value=value)
 
 
 def to_ProgramChangeEvent(track, time, identifier, line):
-    channel, value = map(int, line)
+    channel, value = map(int, line[:2])
     return ProgramChangeEvent(tick=time, channel=channel, value=value)
 
 
 def to_ChannelAfterTouchEvent(track, time, identifier, line):
-    channel, value = map(int, line)
+    channel, value = map(int, line[:2])
     return ChannelAfterTouchEvent(tick=time, channel=channel, value=value)
 
 
 def to_PitchWheelEvent(track, time, identifier, line):
-    channel, value = map(int, line)
+    channel, value = map(int, line[:2])
     return PitchWheelEvent(tick=time, channel=channel, pitch=value - 0x2000)
 
 
 def to_SequenceNumberMetaEvent(track, time, identifier, line):
     value = int(line[0])
     return SequenceNumberMetaEvent(tick=time, value=value)
 
@@ -126,20 +126,20 @@
 
 def to_SetTempoEvent(track, time, identifier, line):
     mpqn = int(line[0])
     return SetTempoEvent(tick=time, mpqn=mpqn)
 
 
 def to_SmpteOffsetEvent(track, time, identifier, line):
-    hr, mn, se, fr, ff = map(int, line)
+    hr, mn, se, fr, ff = map(int, line[:5])
     return SmpteOffsetEvent(tick=time, hr=hr, mn=mn, se=se, fr=fr, ff=ff)
 
 
 def to_TimeSignatureEvent(track, time, identifier, line):
-    data = {i: val for i, val in enumerate(map(int, line))}
+    data = dict(enumerate(map(int, line[:4])))
     return TimeSignatureEvent(
         tick=time,
         numerator=data.get(0),
         denominator=data.get(1),
         metronome=data.get(2, 24),
         thirtyseconds=data.get(3, 8),
     )
```

### Comparing `py_midicsv-4.0.0/py_midicsv/csvmidi.py` & `py_midicsv-4.1.0/py_midicsv/csvmidi.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/events.py` & `py_midicsv-4.1.0/py_midicsv/events.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/midi/constants.py` & `py_midicsv-4.1.0/py_midicsv/midi/constants.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/midi/containers.py` & `py_midicsv-4.1.0/py_midicsv/midi/containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 ### System ###
 from pprint import pformat
 
 
 class Pattern(list):
-
     useRunningStatus = True
 
     def __init__(self, tracks=None, resolution=220, format=1, tick_relative=True):
         self.format = format
         self.resolution = resolution
         self.tick_relative = tick_relative
         super().__init__(tracks or [])
 
     def __repr__(self):
-        return "midi.Pattern(format={!r}, resolution={!r}, tracks=\\\n{})".format(
-            self.format,
-            self.resolution,
-            pformat(list(self)),
-        )
+        return f"midi.Pattern(format={self.format!r}, resolution={self.resolution!r}, tracks=\\\n{pformat(list(self))})"
 
     def make_ticks_abs(self):
         self.tick_relative = False
         for track in self:
             track.make_ticks_abs()
 
     def make_ticks_rel(self):
```

### Comparing `py_midicsv-4.0.0/py_midicsv/midi/events.py` & `py_midicsv-4.1.0/py_midicsv/midi/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 ### System ###
 import struct
 from abc import abstractmethod
 from functools import total_ordering
+from typing import ClassVar
 
 # Reference: http://midi.teragonaudio.com/tech/midispec.htm
 
 
 class EventRegistry:
-    Events = {}
-    MetaEvents = {}
+    Events: ClassVar = {}
+    MetaEvents: ClassVar = {}
 
     @classmethod
     def register_event(cls, event, bases):
         if (Event in bases) or (NoteEvent in bases) or (SysexEvent in bases):
-            assert event.statusmsg not in cls.Events, "Event %s already registered" % event.name
+            assert event.statusmsg not in cls.Events, f"Event {event.name} already registered"
             cls.Events[event.statusmsg] = event
         elif (MetaEvent in bases) or (MetaEventWithText in bases):
-            assert event.metacommand not in cls.MetaEvents, "Event %s already registered" % event.name
+            assert event.metacommand not in cls.MetaEvents, f"Event {event.name} already registered"
             cls.MetaEvents[event.metacommand] = event
         else:
-            raise ValueError("Unknown bases class in event type: " + event.name)
+            raise ValueError(f"Unknown bases class in event type: {event.name}")
 
 
 class AutoRegister(type):
     def __init__(cls, name, bases, dict):
         if name not in {
             "AbstractEvent",
             "Event",
@@ -355,18 +356,18 @@
 
 class SetTempoEvent(MetaEvent):
     name = "Set Tempo"
     metacommand = 0x51
     length = 3
 
     def set_bpm(self, bpm):
-        self.mpqn = int(float(6e7) / bpm)
+        self.mpqn = int(6e7 / bpm)
 
     def get_bpm(self):
-        return float(6e7) / self.mpqn
+        return 6e7 / self.mpqn
 
     bpm = property(get_bpm, set_bpm)
 
     def get_mpqn(self):
         assert len(self.data) == 3
         vals = [self.data[x] << (16 - (8 * x)) for x in range(3)]
         return sum(vals)
```

### Comparing `py_midicsv-4.0.0/py_midicsv/midi/fileio.py` & `py_midicsv-4.1.0/py_midicsv/midi/fileio.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/midi/util.py` & `py_midicsv-4.1.0/py_midicsv/midi/util.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/py_midicsv/midi_converters.py` & `py_midicsv-4.1.0/py_midicsv/midi_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 def write_event(track, time, identifier, data):
     Items = [f"{track}, {time}, {identifier}"]
     if identifier.startswith("System") or identifier == "Sequencer_specific":
         fmt = "{:02X}"
     else:
         fmt = "{}"
-    Items.extend(fmt.format(x) if type(x) == int else x for x in data)
+    Items.extend(fmt.format(x) if isinstance(x, int) else x for x in data)
     return ", ".join(Items) + "\n"
 
 
 def from_NoteOffEvent(track, time, event):
     return write_event(track, time, "Note_off_c", [event.channel, *event.data])
```

### Comparing `py_midicsv-4.0.0/py_midicsv/midicsv.py` & `py_midicsv-4.1.0/py_midicsv/midicsv.py`

 * *Files identical despite different names*

### Comparing `py_midicsv-4.0.0/pyproject.toml` & `py_midicsv-4.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_midicsv"
-version = "4.0.0"
+version = "4.1.0"
 description = "A library for converting MIDI files from and to CSV format"
 authors = ["Tim Wedde <timwedde@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwedde/py_midicsv"
 homepage = "https://github.com/timwedde/py_midicsv"
 
@@ -16,15 +16,15 @@
 python = "^3.8"
 rich-click = "^1.6.1"
 
 [tool.poetry.dev-dependencies]
 pdoc3 = "^0.10.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-pre-commit = "^3.0.4"
+pre-commit = "^3.5.0"
 pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy]
@@ -35,23 +35,25 @@
 
 [tool.ruff]
 fix = true
 force-exclude = true # necessary for excludes to work in pre-commit
 exclude = [
     # "path/",
 ]
+line-length = 120
+
+[tool.ruff.lint]
 ignore = [
     "E402",
     "E722",
     "TID252",
     "C901",
     "F405",
     "F403",
 ]
-line-length = 120
 select = [
     "E",
     "F",
     "W",
     "I",
     "UP",
     "S105",
```

### Comparing `py_midicsv-4.0.0/PKG-INFO` & `py_midicsv-4.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: py-midicsv
-Version: 4.0.0
+Name: py_midicsv
+Version: 4.1.0
 Summary: A library for converting MIDI files from and to CSV format
 Home-page: https://github.com/timwedde/py_midicsv
 License: MIT
 Author: Tim Wedde
 Author-email: timwedde@icloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Project-URL: Repository, https://github.com/timwedde/py_midicsv
 Description-Content-Type: text/markdown
 
 # py_midicsv
 
 [![Downloads](https://pepy.tech/badge/py-midicsv)](https://pepy.tech/project/py-midicsv)
```

