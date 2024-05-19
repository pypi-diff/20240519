# Comparing `tmp/cs.fsm-20240316.tar.gz` & `tmp/cs.fsm-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fsm-20240316.tar", last modified: Sat Mar 16 07:05:24 2024, max compression
+gzip compressed data, was "cs.fsm-20240519.tar", last modified: Sun May 19 02:11:36 2024, max compression
```

## Comparing `cs.fsm-20240316.tar` & `cs.fsm-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:05:24.300293 cs.fsm-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 07:05:10.000000 cs.fsm-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6286 2024-03-16 07:05:24.300039 cs.fsm-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     9659 2024-03-16 07:05:14.000000 cs.fsm-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:05:24.296615 cs.fsm-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:05:24.296882 cs.fsm-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:05:24.298107 cs.fsm-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    13722 2024-03-16 07:05:00.000000 cs.fsm-20240316/lib/python/cs/fsm.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 07:05:24.299643 cs.fsm-20240316/lib/python/cs.fsm.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6286 2024-03-16 07:05:23.000000 cs.fsm-20240316/lib/python/cs.fsm.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-03-16 07:05:24.000000 cs.fsm-20240316/lib/python/cs.fsm.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 07:05:23.000000 cs.fsm-20240316/lib/python/cs.fsm.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       87 2024-03-16 07:05:24.000000 cs.fsm-20240316/lib/python/cs.fsm.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 07:05:24.000000 cs.fsm-20240316/lib/python/cs.fsm.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6714 2024-03-16 07:05:22.000000 cs.fsm-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 07:05:24.300386 cs.fsm-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:11:36.139968 cs.fsm-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:11:22.000000 cs.fsm-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10653 2024-05-19 02:11:36.139684 cs.fsm-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9913 2024-05-19 02:11:26.000000 cs.fsm-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:11:36.135559 cs.fsm-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:11:36.135851 cs.fsm-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:11:36.137224 cs.fsm-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    13848 2024-05-19 02:11:09.000000 cs.fsm-20240519/lib/python/cs/fsm.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:11:36.139109 cs.fsm-20240519/lib/python/cs.fsm.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    10653 2024-05-19 02:11:35.000000 cs.fsm-20240519/lib/python/cs.fsm.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-05-19 02:11:36.000000 cs.fsm-20240519/lib/python/cs.fsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:11:35.000000 cs.fsm-20240519/lib/python/cs.fsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      104 2024-05-19 02:11:35.000000 cs.fsm-20240519/lib/python/cs.fsm.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:11:35.000000 cs.fsm-20240519/lib/python/cs.fsm.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11110 2024-05-19 02:11:34.000000 cs.fsm-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:11:36.140085 cs.fsm-20240519/setup.cfg
```

### Comparing `cs.fsm-20240316/PKG-INFO` & `cs.fsm-20240519/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-Metadata-Version: 2.1
-Name: cs.fsm
-Version: 20240316
-Summary: Basic Finite State Machine (FSM) tools.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Basic Finite State Machine (FSM) tools.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
 
 ## Class `FSM(cs.gvutils.DOTNodeMixin)`
 
 Base class for a finite state machine (FSM).
 
 The allowed states and transitions are defined by the class
 attribute `FSM_TRANSITIONS`, a mapping of
@@ -34,15 +16,15 @@
 * `fsm_history`: an optional iterable of `FSMTransitionEvent`
   state transitions recorded by the `fsm_event` method.
   Usually this would be `None` (the default) or a `list`.
 
 *Method `FSM.__init__(self, state=None, *, history=None, lock=None, transitions=None)`*:
 Initialise the `FSM` from:
 * `state`: optional _positional_ parameter for the initial state,
-  default `self.FSM_DEFAULT_STATE`
+  default `self.FSM_DEFAULT_STATE` or the first key from `self.FSM_TRANSITIONS`
 * `history`: an optional object to record state transition
   history, default `None`; if not `None` this should be an
   iterable object with a `.append(entry)` method such as a
   `list`.
 * `lock`: an optional mutex to control access;
   if presupplied and shared with the caller
   it should probably be an `RLock`;
@@ -59,15 +41,108 @@
 whose `refresh_from_db` method seems to not refresh fields
 which already exist, and setting `.fsm_state` from a
 `FSM_DEFAULT_STATE` class attribute thus breaks this method.
 Subclasses of this class and `Model` should _not_ provide a
 `FSM_DEFAULT_STATE` attribute, instead relying on the field
 definition to provide this default in the usual way.
 
-## Class `FSMError(builtins.Exception, builtins.BaseException)`
+*Method `FSM.__getattr__(self, attr)`*:
+Provide the following attributes:
+- present the state names as attributes, for example:
+  `self.PENDING=='PENDING'` if there is a `'PENDING'` state
+- present `is_`*statename* as a Boolean testing whether
+  `self.fsm_state==`*statename*`.upper()`
+- a callable calling `self.fsm_event(attr)` if `attr`
+  is an event name for the current state
+Fall back to the superclass `__getattr__`.
+
+*Property `FSM.dot_node_palette_key`*:
+Default palette index is `self.fsm_state`,
+overriding `DOTNodeMixin.dot_node_palette_key`.
+
+*Method `FSM.fsm_as_svg(self, layout=None, history_style=None, **dot_kw)`*:
+Render the state transition diagram as SVG.
+
+*Method `FSM.fsm_callback(self, state, callback)`*:
+Register a callback to be called immediately on transition
+to `state` as `callback(self,FSMEventTransition)`.
+The special `state` value `FSM.FSM_ANY_STATE` may be supplied
+to register a callback which fires for every state transition.
+
+    >>> fsm = FSM('state1',transitions={
+    ...   'state1':{'ev_a':'state2'},
+    ...   'state2':{'ev_b':'state1'},
+    ... })
+    >>> fsm.fsm_callback('state2',lambda task, transition: print(task, transition))
+    >>> fsm.fsm_callback(FSM.FSM_ANY_STATE,lambda task, transition: print("ANY", task, transition))
+    >>> fsm.ev_a(foo=3) # doctest: +ELLIPSIS
+    ANY FSM:state2 FSMTransitionEvent(old_state='state1', new_state='state2', event='ev_a', when=..., extra={'foo': 3})
+    FSM:state2 FSMTransitionEvent(old_state='state1', new_state='state2', event='ev_a', when=..., extra={'foo': 3})
+    'state2'
+    >>> fsm.ev_b(foo=4) # doctest: +ELLIPSIS
+    ANY FSM:state1 FSMTransitionEvent(old_state='state2', new_state='state1', event='ev_b', when=..., extra={'foo': 4})
+    'state1'
+
+*Method `FSM.fsm_callback_discard(self, state, callback)`*:
+Deregister a callback for `state`.
+
+*Property `FSM.fsm_dot`*:
+A DOT syntax description of `self.FSM_TRANSITIONS`.
+
+*Method `FSM.fsm_event(self, event, **extra)`*:
+Transition the FSM from the current state to a new state based on `event`.
+Call any callbacks associated with the new state.
+Returns the new state.
+
+Optional information may be passed as keyword arguments.
+
+A `transition` instance of `FSMTransitionEvent` is created
+with the following attributes:
+* `old_state`: the state when `fsm_event` was called
+* `new_state`: the new state
+* `event`: the `event`
+* `when`: a UNIX timestamp from `time.time()`
+* `extra`: a `dict` with the `extra` information
+If `self.fsm_history` is not `None`,
+`transition` is appended to it.
+If there are callbacks for `new_state` or `FSM.FSM_ANY_STATE`,
+call each callback as `callback(self,transition)`.
+
+*Method `FSM.fsm_event_is_allowed(self, event)`*:
+Test whether `event` is permitted in the current state.
+This can be handy as a pretest.
+
+*Property `FSM.fsm_events`*:
+Return a list of the events valid for the current state.
+
+*Property `FSM.fsm_history`*:
+History property wrapping private attribute.
+This aids subclassing where the history is not a local attribute.
+
+*Method `FSM.fsm_print(self, file=None, fmt=None, layout=None, **dot_kw)`*:
+Print the state transition diagram to `file`, default `sys.stdout`,
+in format `fmt` using the engine specified by `layout`, default `'dot'`.
+This is a wrapper for `cs.gvutils.gvprint`.
+
+*Property `FSM.fsm_svg`*:
+The state transition diagram as SVG.
+
+*Method `FSM.fsm_transitions_as_dot(self, fsm_transitions=None, *, sep='\n', graph_name=None, history_style=None)`*:
+Compute a DOT syntax graph description from a transitions dictionary.
+
+        Parameters:
+        * `fsm_transitions`: optional mapping of *state*->*event*->*state*,
+          default `self.FSM_TRANSITIONS`
+        * `sep`: optional separator between "lines", default `'
+'`
+        * `graph_name`: optional name for the graph, default the class name
+        * `history_style`: optional style mapping for event transition history,
+          used to style edges which have been traversed
+
+## Class `FSMError(builtins.Exception)`
 
 An exception associated with an `FSM`.
 
 These have a `.fsm` attribute storing an (optional) `FSM`
 reference supplied at initialisation.
 
 ## `FSMSubType = ~FSMSubType`
@@ -114,21 +189,36 @@
 
 Note that only type variables defined in global scope can be pickled.
 
 ## Class `FSMTransitionEvent(builtins.tuple)`
 
 FSMTransitionEvent(old_state, new_state, event, when, extra)
 
-*Method `FSMTransitionEvent.__new__(_cls, old_state, new_state, event, when, extra)`*:
-Create new instance of FSMTransitionEvent(old_state, new_state, event, when, extra)
+*Property `FSMTransitionEvent.event`*:
+Alias for field number 2
+
+*Property `FSMTransitionEvent.extra`*:
+Alias for field number 4
+
+*Property `FSMTransitionEvent.new_state`*:
+Alias for field number 1
+
+*Property `FSMTransitionEvent.old_state`*:
+Alias for field number 0
+
+*Property `FSMTransitionEvent.when`*:
+Alias for field number 3
 
 # Release Log
 
 
 
+*Release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 FSM.__getattr__: return None for missing self.fsm_state, happens in too-early call to __str__.
 
 *Release 20231020*:
@@ -163,8 +253,7 @@
 
 *Release 20220805.1*:
 * FSM: subclass DOTNodeMixin and provide a hook for a colour palette for node fillcolors.
 * Other minor changes.
 
 *Release 20220805*:
 Initial PyPI release.
-
```

### Comparing `cs.fsm-20240316/README.md` & `cs.fsm-20240519/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+Metadata-Version: 2.1
+Name: cs.fsm
+Version: 20240519
+Summary: Basic Finite State Machine (FSM) tools.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Basic Finite State Machine (FSM) tools.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
 
 ## Class `FSM(cs.gvutils.DOTNodeMixin)`
 
 Base class for a finite state machine (FSM).
 
 The allowed states and transitions are defined by the class
 attribute `FSM_TRANSITIONS`, a mapping of
@@ -16,15 +34,15 @@
 * `fsm_history`: an optional iterable of `FSMTransitionEvent`
   state transitions recorded by the `fsm_event` method.
   Usually this would be `None` (the default) or a `list`.
 
 *Method `FSM.__init__(self, state=None, *, history=None, lock=None, transitions=None)`*:
 Initialise the `FSM` from:
 * `state`: optional _positional_ parameter for the initial state,
-  default `self.FSM_DEFAULT_STATE`
+  default `self.FSM_DEFAULT_STATE` or the first key from `self.FSM_TRANSITIONS`
 * `history`: an optional object to record state transition
   history, default `None`; if not `None` this should be an
   iterable object with a `.append(entry)` method such as a
   `list`.
 * `lock`: an optional mutex to control access;
   if presupplied and shared with the caller
   it should probably be an `RLock`;
@@ -134,15 +152,15 @@
           default `self.FSM_TRANSITIONS`
         * `sep`: optional separator between "lines", default `'
 '`
         * `graph_name`: optional name for the graph, default the class name
         * `history_style`: optional style mapping for event transition history,
           used to style edges which have been traversed
 
-## Class `FSMError(builtins.Exception, builtins.BaseException)`
+## Class `FSMError(builtins.Exception)`
 
 An exception associated with an `FSM`.
 
 These have a `.fsm` attribute storing an (optional) `FSM`
 reference supplied at initialisation.
 
 ## `FSMSubType = ~FSMSubType`
@@ -208,14 +226,17 @@
 *Property `FSMTransitionEvent.when`*:
 Alias for field number 3
 
 # Release Log
 
 
 
+*Release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 FSM.__getattr__: return None for missing self.fsm_state, happens in too-early call to __str__.
 
 *Release 20231020*:
@@ -250,7 +271,8 @@
 
 *Release 20220805.1*:
 * FSM: subclass DOTNodeMixin and provide a hook for a colour palette for node fillcolors.
 * Other minor changes.
 
 *Release 20220805*:
 Initial PyPI release.
+
```

### Comparing `cs.fsm-20240316/lib/python/cs/fsm.py` & `cs.fsm-20240519/lib/python/cs/fsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 
 from typeguard import typechecked
 
 from cs.gimmicks import exception
 from cs.gvutils import gvprint, gvsvg, quote as gvq, DOTNodeMixin
 from cs.lex import cutprefix
 from cs.pfx import Pfx, pfx_call
+from cs.seq import first
 
-__version__ = '20240316'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.gimmicks',
         'cs.gvutils>=20230816',
         'cs.lex',
         'cs.pfx',
+        'cs.seq',
         'typeguard',
     ],
 }
 
 FSMSubType = TypeVar('FSMSubType', bound='FSM')
 
 class FSMError(Exception):
@@ -70,15 +72,15 @@
 
   # allowed state transitions
   FSM_TRANSITIONS = {}
 
   def __init__(self, state=None, *, history=None, lock=None, transitions=None):
     ''' Initialise the `FSM` from:
         * `state`: optional _positional_ parameter for the initial state,
-          default `self.FSM_DEFAULT_STATE`
+          default `self.FSM_DEFAULT_STATE` or the first key from `self.FSM_TRANSITIONS`
         * `history`: an optional object to record state transition
           history, default `None`; if not `None` this should be an
           iterable object with a `.append(entry)` method such as a
           `list`.
         * `lock`: an optional mutex to control access;
           if presupplied and shared with the caller
           it should probably be an `RLock`;
@@ -99,15 +101,15 @@
         `FSM_DEFAULT_STATE` attribute, instead relying on the field
         definition to provide this default in the usual way.
     '''
     if state is None:
       try:
         state = self.FSM_DEFAULT_STATE
       except AttributeError:
-        pass
+        state = first(self.FSM_TRANSITIONS.keys())
     if lock is None:
       lock = Lock()
     if transitions is not None:
       self.FSM_TRANSITIONS = transitions
     if state is not None:
       if state not in self.FSM_TRANSITIONS:
         raise ValueError(
```

### Comparing `cs.fsm-20240316/pyproject.toml` & `cs.fsm-20240519/lib/python/cs.fsm.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-[project]
-name = "cs.fsm"
-description = "Basic Finite State Machine (FSM) tools."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python3",
-]
-dependencies = [
-    "cs.gimmicks>=20240316",
-    "cs.gvutils>=20230816",
-    "cs.lex>=20240316",
-    "cs.pfx>=20230604",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240316"
+Metadata-Version: 2.1
+Name: cs.fsm
+Version: 20240519
+Summary: Basic Finite State Machine (FSM) tools.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Basic Finite State Machine (FSM) tools.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
 
 ## Class `FSM(cs.gvutils.DOTNodeMixin)`
 
 Base class for a finite state machine (FSM).
 
 The allowed states and transitions are defined by the class
 attribute `FSM_TRANSITIONS`, a mapping of
@@ -51,15 +34,15 @@
 * `fsm_history`: an optional iterable of `FSMTransitionEvent`
   state transitions recorded by the `fsm_event` method.
   Usually this would be `None` (the default) or a `list`.
 
 *Method `FSM.__init__(self, state=None, *, history=None, lock=None, transitions=None)`*:
 Initialise the `FSM` from:
 * `state`: optional _positional_ parameter for the initial state,
-  default `self.FSM_DEFAULT_STATE`
+  default `self.FSM_DEFAULT_STATE` or the first key from `self.FSM_TRANSITIONS`
 * `history`: an optional object to record state transition
   history, default `None`; if not `None` this should be an
   iterable object with a `.append(entry)` method such as a
   `list`.
 * `lock`: an optional mutex to control access;
   if presupplied and shared with the caller
   it should probably be an `RLock`;
@@ -76,15 +59,108 @@
 whose `refresh_from_db` method seems to not refresh fields
 which already exist, and setting `.fsm_state` from a
 `FSM_DEFAULT_STATE` class attribute thus breaks this method.
 Subclasses of this class and `Model` should _not_ provide a
 `FSM_DEFAULT_STATE` attribute, instead relying on the field
 definition to provide this default in the usual way.
 
-## Class `FSMError(builtins.Exception, builtins.BaseException)`
+*Method `FSM.__getattr__(self, attr)`*:
+Provide the following attributes:
+- present the state names as attributes, for example:
+  `self.PENDING=='PENDING'` if there is a `'PENDING'` state
+- present `is_`*statename* as a Boolean testing whether
+  `self.fsm_state==`*statename*`.upper()`
+- a callable calling `self.fsm_event(attr)` if `attr`
+  is an event name for the current state
+Fall back to the superclass `__getattr__`.
+
+*Property `FSM.dot_node_palette_key`*:
+Default palette index is `self.fsm_state`,
+overriding `DOTNodeMixin.dot_node_palette_key`.
+
+*Method `FSM.fsm_as_svg(self, layout=None, history_style=None, **dot_kw)`*:
+Render the state transition diagram as SVG.
+
+*Method `FSM.fsm_callback(self, state, callback)`*:
+Register a callback to be called immediately on transition
+to `state` as `callback(self,FSMEventTransition)`.
+The special `state` value `FSM.FSM_ANY_STATE` may be supplied
+to register a callback which fires for every state transition.
+
+    >>> fsm = FSM('state1',transitions={
+    ...   'state1':{'ev_a':'state2'},
+    ...   'state2':{'ev_b':'state1'},
+    ... })
+    >>> fsm.fsm_callback('state2',lambda task, transition: print(task, transition))
+    >>> fsm.fsm_callback(FSM.FSM_ANY_STATE,lambda task, transition: print("ANY", task, transition))
+    >>> fsm.ev_a(foo=3) # doctest: +ELLIPSIS
+    ANY FSM:state2 FSMTransitionEvent(old_state='state1', new_state='state2', event='ev_a', when=..., extra={'foo': 3})
+    FSM:state2 FSMTransitionEvent(old_state='state1', new_state='state2', event='ev_a', when=..., extra={'foo': 3})
+    'state2'
+    >>> fsm.ev_b(foo=4) # doctest: +ELLIPSIS
+    ANY FSM:state1 FSMTransitionEvent(old_state='state2', new_state='state1', event='ev_b', when=..., extra={'foo': 4})
+    'state1'
+
+*Method `FSM.fsm_callback_discard(self, state, callback)`*:
+Deregister a callback for `state`.
+
+*Property `FSM.fsm_dot`*:
+A DOT syntax description of `self.FSM_TRANSITIONS`.
+
+*Method `FSM.fsm_event(self, event, **extra)`*:
+Transition the FSM from the current state to a new state based on `event`.
+Call any callbacks associated with the new state.
+Returns the new state.
+
+Optional information may be passed as keyword arguments.
+
+A `transition` instance of `FSMTransitionEvent` is created
+with the following attributes:
+* `old_state`: the state when `fsm_event` was called
+* `new_state`: the new state
+* `event`: the `event`
+* `when`: a UNIX timestamp from `time.time()`
+* `extra`: a `dict` with the `extra` information
+If `self.fsm_history` is not `None`,
+`transition` is appended to it.
+If there are callbacks for `new_state` or `FSM.FSM_ANY_STATE`,
+call each callback as `callback(self,transition)`.
+
+*Method `FSM.fsm_event_is_allowed(self, event)`*:
+Test whether `event` is permitted in the current state.
+This can be handy as a pretest.
+
+*Property `FSM.fsm_events`*:
+Return a list of the events valid for the current state.
+
+*Property `FSM.fsm_history`*:
+History property wrapping private attribute.
+This aids subclassing where the history is not a local attribute.
+
+*Method `FSM.fsm_print(self, file=None, fmt=None, layout=None, **dot_kw)`*:
+Print the state transition diagram to `file`, default `sys.stdout`,
+in format `fmt` using the engine specified by `layout`, default `'dot'`.
+This is a wrapper for `cs.gvutils.gvprint`.
+
+*Property `FSM.fsm_svg`*:
+The state transition diagram as SVG.
+
+*Method `FSM.fsm_transitions_as_dot(self, fsm_transitions=None, *, sep='\n', graph_name=None, history_style=None)`*:
+Compute a DOT syntax graph description from a transitions dictionary.
+
+        Parameters:
+        * `fsm_transitions`: optional mapping of *state*->*event*->*state*,
+          default `self.FSM_TRANSITIONS`
+        * `sep`: optional separator between "lines", default `'
+'`
+        * `graph_name`: optional name for the graph, default the class name
+        * `history_style`: optional style mapping for event transition history,
+          used to style edges which have been traversed
+
+## Class `FSMError(builtins.Exception)`
 
 An exception associated with an `FSM`.
 
 These have a `.fsm` attribute storing an (optional) `FSM`
 reference supplied at initialisation.
 
 ## `FSMSubType = ~FSMSubType`
@@ -131,21 +207,36 @@
 
 Note that only type variables defined in global scope can be pickled.
 
 ## Class `FSMTransitionEvent(builtins.tuple)`
 
 FSMTransitionEvent(old_state, new_state, event, when, extra)
 
-*Method `FSMTransitionEvent.__new__(_cls, old_state, new_state, event, when, extra)`*:
-Create new instance of FSMTransitionEvent(old_state, new_state, event, when, extra)
+*Property `FSMTransitionEvent.event`*:
+Alias for field number 2
+
+*Property `FSMTransitionEvent.extra`*:
+Alias for field number 4
+
+*Property `FSMTransitionEvent.new_state`*:
+Alias for field number 1
+
+*Property `FSMTransitionEvent.old_state`*:
+Alias for field number 0
+
+*Property `FSMTransitionEvent.when`*:
+Alias for field number 3
 
 # Release Log
 
 
 
+*Release 20240519*:
+FSM: default for FSM_DEFAULT_STATE is the first key from FSM_TRANSITIONS (relies on ordered dicts, so Python 3.6 onward).
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 FSM.__getattr__: return None for missing self.fsm_state, happens in too-early call to __str__.
 
 *Release 20231020*:
@@ -155,15 +246,15 @@
 * FSM.fsm_transitions_as_dot: new optional history_style parameter to style transitioned edges.
 * FSM.fsm_as_svg: plumb optional history_style parameter.
 
 *Release 20230816.3*:
 Bump cs.gvutils requirement.
 
 *Release 20230816.2*:
-FSM.fsm_transitions_as_dot: bugfix: the style needs \"style=filled\" as well as the fillcolor.
+FSM.fsm_transitions_as_dot: bugfix: the style needs "style=filled" as well as the fillcolor.
 
 *Release 20230816.1*:
 FSM.fsm_transitions_as_dot: now an instance method so that we can colour the current state.
 
 *Release 20230816*:
 FSM: new fsm_as_svg method and fsm_svg property.
 
@@ -179,25 +270,9 @@
 Replace callback exception warning() with exception() for the traceback.
 
 *Release 20220805.1*:
 * FSM: subclass DOTNodeMixin and provide a hook for a colour palette for node fillcolors.
 * Other minor changes.
 
 *Release 20220805*:
-Initial PyPI release."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.fsm",
-]
+Initial PyPI release.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

