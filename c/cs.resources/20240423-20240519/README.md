# Comparing `tmp/cs.resources-20240423.tar.gz` & `tmp/cs.resources-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20240423.tar", last modified: Tue Apr 23 09:25:49 2024, max compression
+gzip compressed data, was "cs.resources-20240519.tar", last modified: Sun May 19 02:20:34 2024, max compression
```

## Comparing `cs.resources-20240423.tar` & `cs.resources-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.160856 cs.resources-20240423/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-23 09:25:18.000000 cs.resources-20240423/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    17501 2024-04-23 09:25:49.160427 cs.resources-20240423/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16744 2024-04-23 09:25:28.000000 cs.resources-20240423/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.153738 cs.resources-20240423/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.154038 cs.resources-20240423/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.156806 cs.resources-20240423/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    27539 2024-04-23 09:25:03.000000 cs.resources-20240423/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.159916 cs.resources-20240423/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    17501 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-23 09:25:49.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-23 09:25:49.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    18115 2024-04-23 09:25:47.000000 cs.resources-20240423/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-23 09:25:49.160958 cs.resources-20240423/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.072875 cs.resources-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:20:02.000000 cs.resources-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17728 2024-05-19 02:20:34.072564 cs.resources-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16971 2024-05-19 02:20:12.000000 cs.resources-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.068001 cs.resources-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.068329 cs.resources-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.069930 cs.resources-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27607 2024-05-19 02:19:49.000000 cs.resources-20240519/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.072014 cs.resources-20240519/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17728 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-05-19 02:20:34.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      206 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18338 2024-05-19 02:20:32.000000 cs.resources-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:20:34.072975 cs.resources-20240519/setup.cfg
```

### Comparing `cs.resources-20240423/PKG-INFO` & `cs.resources-20240519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240423
+Version: 20240519
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240423*:
-RunStateMixin: make the optional runstate parameter keyword only.
+*Latest release 20240519*:
+RunState now subclasses cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -207,15 +207,15 @@
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
 *Method `Pool.instance(self)`*:
 Context manager returning an object for use, which is returned to the pool afterwards.
 
-## Class `RunState(cs.threads.HasThreadState)`
+## Class `RunState(cs.fsm.FSM, cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -259,22 +259,22 @@
   to be called whenever `.cancel` is called.
 
 *Method `RunState.__bool__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.__enter_exit__(self)`*:
 The `__enter__`/`__exit__` generator function:
-* push this RunState via HasThreadState
-* catch signals
+* push this `RunState` via `HasThreadState`
+* catch signals if we are in the main `Thread`
 * start
 * `yield self` => run
-* cancel on exception during run
+* cancel on exception during the run
 * stop
 
-Note that if the `RunState` is already runnings we do not
+Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
 in the "running" state.
 
 *Method `RunState.__nonzero__(self)`*:
@@ -294,16 +294,22 @@
 
 Parameters:
 * `sig`: an `int` signal number or an iterable of signal numbers
 * `call_previous`: optional flag (default `False`)
   passed to `cs.psutils.signal_handlers`
 
 *Method `RunState.end(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+Obsolete synonym for `.stop()`.
+
+*Method `RunState.fsm_event(self, event: str, **extra)`*:
+Override `FSM.fsm_event` to apply side effects to particular transitions.
+
+On `'cancel'` set the cancelled flag.
+On `'start'` clear the cancelled flag and set `.start_time`.
+On `'stop'`set `.stop_time`.
 
 *Method `RunState.handle_signal(self, sig, _)`*:
 `RunState` signal handler: cancel the run state.
 Warn if `self.verbose`.
 
 *Method `RunState.iter(self, it)`*:
 Iterate over `it` while not `self.cancelled`.
@@ -323,37 +329,37 @@
 
 *Property `RunState.run_time`*:
 Property returning most recent run time (`stop_time-start_time`).
 If still running, use now as the stop time.
 If not started, return `0.0`.
 
 *Property `RunState.running`*:
-Property expressing whether the task is running.
+Whether the state is `'RUNNING'` or `'STOPPING'`.
 
 *Method `RunState.start(self, running_ok=False)`*:
 Start: adjust state, set `start_time` to now.
 Sets `.cancelled` to `False` and sets `.running` to `True`.
 
-*Method `RunState.stop(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+*Property `RunState.state`*:
+The `RunState`'s state as a string.
+Deprecated, new uses should consult `self.fsm_state`.
 
-*Property `RunState.stopped`*:
-Was the process stopped? Running is false and cancelled is true.
+*Method `RunState.stop(self)`*:
+Fire the `'stop'` event.
 
 *Property `RunState.stopping`*:
-Is the process stopping? Running is true and cancelled is true.
+Is the process stopping?
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -372,14 +378,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240519*:
+RunState now subclasses cs.fsm.FSM.
+
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
```

### Comparing `cs.resources-20240423/README.md` & `cs.resources-20240519/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Resource management classes and functions.
 
-*Latest release 20240423*:
-RunStateMixin: make the optional runstate parameter keyword only.
+*Latest release 20240519*:
+RunState now subclasses cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -189,15 +189,15 @@
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
 *Method `Pool.instance(self)`*:
 Context manager returning an object for use, which is returned to the pool afterwards.
 
-## Class `RunState(cs.threads.HasThreadState)`
+## Class `RunState(cs.fsm.FSM, cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -241,22 +241,22 @@
   to be called whenever `.cancel` is called.
 
 *Method `RunState.__bool__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.__enter_exit__(self)`*:
 The `__enter__`/`__exit__` generator function:
-* push this RunState via HasThreadState
-* catch signals
+* push this `RunState` via `HasThreadState`
+* catch signals if we are in the main `Thread`
 * start
 * `yield self` => run
-* cancel on exception during run
+* cancel on exception during the run
 * stop
 
-Note that if the `RunState` is already runnings we do not
+Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
 in the "running" state.
 
 *Method `RunState.__nonzero__(self)`*:
@@ -276,16 +276,22 @@
 
 Parameters:
 * `sig`: an `int` signal number or an iterable of signal numbers
 * `call_previous`: optional flag (default `False`)
   passed to `cs.psutils.signal_handlers`
 
 *Method `RunState.end(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+Obsolete synonym for `.stop()`.
+
+*Method `RunState.fsm_event(self, event: str, **extra)`*:
+Override `FSM.fsm_event` to apply side effects to particular transitions.
+
+On `'cancel'` set the cancelled flag.
+On `'start'` clear the cancelled flag and set `.start_time`.
+On `'stop'`set `.stop_time`.
 
 *Method `RunState.handle_signal(self, sig, _)`*:
 `RunState` signal handler: cancel the run state.
 Warn if `self.verbose`.
 
 *Method `RunState.iter(self, it)`*:
 Iterate over `it` while not `self.cancelled`.
@@ -305,37 +311,37 @@
 
 *Property `RunState.run_time`*:
 Property returning most recent run time (`stop_time-start_time`).
 If still running, use now as the stop time.
 If not started, return `0.0`.
 
 *Property `RunState.running`*:
-Property expressing whether the task is running.
+Whether the state is `'RUNNING'` or `'STOPPING'`.
 
 *Method `RunState.start(self, running_ok=False)`*:
 Start: adjust state, set `start_time` to now.
 Sets `.cancelled` to `False` and sets `.running` to `True`.
 
-*Method `RunState.stop(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+*Property `RunState.state`*:
+The `RunState`'s state as a string.
+Deprecated, new uses should consult `self.fsm_state`.
 
-*Property `RunState.stopped`*:
-Was the process stopped? Running is false and cancelled is true.
+*Method `RunState.stop(self)`*:
+Fire the `'stop'` event.
 
 *Property `RunState.stopping`*:
-Is the process stopping? Running is true and cancelled is true.
+Is the process stopping?
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -354,14 +360,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240519*:
+RunState now subclasses cs.fsm.FSM.
+
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
```

### Comparing `cs.resources-20240423/lib/python/cs/resources.py` & `cs.resources-20240519/lib/python/cs/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,40 +15,40 @@
 from threading import Lock, current_thread, main_thread
 import time
 from typing import Any, Callable, Mapping, Optional, Tuple, Union
 
 from typeguard import typechecked
 
 from cs.context import contextif, stackattrs, setup_cmgr, ContextManagerMixin
-from cs.deco import default_params
+from cs.deco import default_params, OBSOLETE
+from cs.fsm import FSM
 from cs.gimmicks import error, warning, nullcontext
 from cs.obj import Proxy
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
-from cs.py.func import prop
-from cs.py.stack import caller, frames as stack_frames, stack_dump, StackSummary
+from cs.py.stack import caller, frames as stack_frames, StackSummary
 from cs.result import CancellationError
 from cs.threads import ThreadState, HasThreadState, NRLock
 
-__version__ = '20240423'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.context',
         'cs.deco',
+        'cs.fsm',
         'cs.gimmicks',
         'cs.obj',
         'cs.pfx',
         'cs.psutils',
-        'cs.py.func',
         'cs.py.stack',
         'cs.result',
         'cs.threads',
         'typeguard',
     ],
 }
 
@@ -517,15 +517,15 @@
       yield o
     finally:
       with self._lock:
         if self.max_size == 0 or len(self.pool) < self.max_size:
           self.pool.append(o)
 
 # pylint: disable=too-many-instance-attributes
-class RunState(HasThreadState):
+class RunState(FSM, HasThreadState):
   ''' A class to track a running task whose cancellation may be requested.
 
       Its purpose is twofold, to provide easily queriable state
       around tasks which can start and stop, and to provide control
       methods to pronounce that a task has started (`.start`),
       should stop (`.cancel`)
       and has stopped (`.stop`).
@@ -566,24 +566,44 @@
         to be called whenever `.running` becomes false.
       * `notify_cancel`: a set of callables called with the `RunState` instance
         to be called whenever `.cancel` is called.
   '''
 
   perthread_state = ThreadState()
 
+  FSM_TRANSITIONS = {
+      'IDLE': {
+          'start': 'RUNNING',
+      },
+      'RUNNING': {
+          'cancel': 'STOPPING',
+          'stop': 'STOPPED',
+      },
+      'STOPPING': {
+          'stop': 'STOPPED',
+          'cancel': 'STOPPING',
+      },
+      'STOPPED': {
+          'start': 'RUNNING',
+      },
+  }
+
+  FSM_DEFAULT_STATE = 'IDLE'
+
   def __init__(
       self,
       name=None,
       *,
       signals=None,
       handle_signal=None,
       poll_cancel: Optional[Callable] = None,
       verbose=False,
       thread_wide=False,
   ):
+    FSM.__init__(self)
     self.name = name
     self.verbose = verbose
     self.thread_wide = thread_wide
     self._started_from = None
     self._signals = tuple(signals) if signals else ()
     self._sigstack = None
     self._sighandler = handle_signal or self.handle_signal
@@ -604,32 +624,40 @@
     ''' Return true if the task is running.
     '''
     return self.running
 
   __nonzero__ = __bool__
 
   def __str__(self):
-    return "%s:%s[%s:%gs]" % (
-        (
-            type(self).__name__ if self.name is None else ':'.join(
-                (type(self).__name__, repr(self.name))
-            )
-        ), id(self), self.state, self.run_time
+    return "%s(%s):%s:%gs" % (
+        self.__class__.__name__,
+        '' if self.name is None else repr(self.name),
+        self.fsm_state,
+        self.run_time,
+    )
+
+  def __repr__(self):
+    return "%s:%d(%s):%s:%gs" % (
+        self.__class__.__name__,
+        id(self),
+        '' if self.name is None else repr(self.name),
+        self.fsm_state,
+        self.run_time,
     )
 
   def __enter_exit__(self):
     ''' The `__enter__`/`__exit__` generator function:
-        * push this RunState via HasThreadState
-        * catch signals
+        * push this `RunState` via `HasThreadState`
+        * catch signals if we are in the main `Thread`
         * start
         * `yield self` => run
-        * cancel on exception during run
+        * cancel on exception during the run
         * stop
 
-        Note that if the `RunState` is already runnings we do not
+        Note that if the `RunState` is already running we do not
         do any of that stuff apart from the `yield self` because
         we assume whatever setup should have been done has already
         been done.
         In particular, the `HasThreadState.Thread` factory calls this
         in the "running" state.
     '''
     with contextif(self.thread_wide, HasThreadState.as_contextmanager, self):
@@ -641,68 +669,74 @@
         # if we're not in the main thread we suppress the signal shuffling as well
         in_main = current_thread() is main_thread()
         with (self.catch_signal(self._signals, call_previous=False,
                                 handle_signal=self._sighandler)
               if in_main else nullcontext()) as sigstack:
           with (stackattrs(self, _sigstack=sigstack)
                 if sigstack is not None else nullcontext()):
-            self.start(running_ok=True)
+            self.fsm_event('start')
             try:
               yield self
             except Exception:
-              self.cancel()
+              self.fsm_event('cancel')
               raise
             finally:
-              self.stop()
+              self.fsm_event('stop')
+
+  def fsm_event(self, event: str, **extra):
+    ''' Override `FSM.fsm_event` to apply side effects to particular transitions.
 
-  @prop
+        On `'cancel'` set the cancelled flag.
+        On `'start'` clear the cancelled flag and set `.start_time`.
+        On `'stop'`set `.stop_time`.
+    '''
+    new_state = super().fsm_event(event, **extra)
+    if event == 'cancel':
+      self._canceled = True
+    elif event == 'start':
+      self._cancelled = False
+      self.start_time = time.time()
+      self._started_from = stack_frames()
+    elif event == 'stop':
+      self.stop_time = time.time()
+    return new_state
+
+  @property
+  @OBSOLETE('.fsm_event')
   def state(self):
     ''' The `RunState`'s state as a string.
-
-        Meanings:
-        * `"pending"`: not yet running/started.
-        * `"stopping"`: running and cancelled.
-        * `"running"`: running and not cancelled.
-        * `"cancelled"`: cancelled and no longer running.
-        * `"stopped"`: no longer running and not cancelled.
+        Deprecated, new uses should consult `self.fsm_state`.
     '''
-    start_time = self.start_time
-    if start_time is None:
-      label = "pending"
-    elif self.running:
-      if self.cancelled:
-        label = "stopping"
-      else:
-        label = "running"
-    elif self.cancelled:
-      label = "cancelled"
+    fsm_state = self.fsm_state
+    if fsm_state == 'IDLE':
+      label = 'pending'
     else:
-      label = "stopped"
+      label = fsm_state.lower()
     return label
 
   @pfx_method
   def start(self, running_ok=False):
     ''' Start: adjust state, set `start_time` to now.
         Sets `.cancelled` to `False` and sets `.running` to `True`.
     '''
-    if not running_ok and self.running:
+    if self.fsm_state in ('RUNNING', 'STOPPING') and not running_ok:
       warning("already running")
-    else:
-      self._started_from = stack_frames()
-    self.cancelled = False
-    self.running = True
+    self.fsm_event('start')
 
   def stop(self):
-    ''' Stop: adjust state, set `stop_time` to now.
-        Sets sets `.running` to `False`.
+    ''' Fire the `'stop'` event.
     '''
-    self.running = False
+    self.fsm_event('stop')
 
   # compatibility
-  end = stop
+  @OBSOLETE('.stop')
+  def end(self):
+    ''' Obsolete synonym for `.stop()`.
+    '''
+    self.stop()
 
   @property
   def cancelled(self):
     ''' Test the .cancelled attribute, including a poll if supplied.
     '''
     if self._cancelled:
       return True
@@ -735,69 +769,41 @@
       else:
         if a:
           msg = msg % a
       raise CancellationError(msg)
 
   @property
   def running(self):
-    ''' Property expressing whether the task is running.
+    ''' Whether the state is `'RUNNING'` or `'STOPPING'`.
     '''
-    return self._running
-
-  @running.setter
-  def running(self, status):
-    ''' Set the running property.
-
-        `status`: the new running state, a Boolean
-
-        A change in status triggers the time measurements.
-    '''
-    if self._running:
-      # running -> not running
-      if not status:
-        self.stop_time = time.time()
-        self.total_time += self.run_time
-        for notify in self.notify_end:
-          notify(self)
-    elif status:
-      # not running -> running
-      self.start_time = time.time()
-      for notify in self.notify_start:
-        notify(self)
-    self._running = status
+    return self.fsm_state in ('RUNNING', 'STOPPING')
 
   @property
   def stopping(self):
-    ''' Is the process stopping? Running is true and cancelled is true.
-    '''
-    return self.running and self.cancelled
-
-  @property
-  def stopped(self):
-    ''' Was the process stopped? Running is false and cancelled is true.
+    ''' Is the process stopping?
     '''
-    return self.cancelled and not self.running
+    return self.fsm_state == 'STOPPING'
 
   def cancel(self):
     ''' Set the cancelled flag; the associated process should notice and stop.
     '''
-    self.cancelled = True
+    self.fsm_event('cancel')
     for notify in self.notify_cancel:
       notify(self)
 
   @property
   def run_time(self):
     ''' Property returning most recent run time (`stop_time-start_time`).
         If still running, use now as the stop time.
         If not started, return `0.0`.
     '''
     start_time = self.start_time
     if start_time is None:
       return 0.0
-    if self.running:
+    if self.is_running:
       stop_time = time.time()
     else:
       stop_time = self.stop_time
     return max(0, stop_time - start_time)
 
   def iter(self, it):
     ''' Iterate over `it` while not `self.cancelled`.
```

### Comparing `cs.resources-20240423/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20240519/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240423
+Version: 20240519
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240423*:
-RunStateMixin: make the optional runstate parameter keyword only.
+*Latest release 20240519*:
+RunState now subclasses cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -207,15 +207,15 @@
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
 *Method `Pool.instance(self)`*:
 Context manager returning an object for use, which is returned to the pool afterwards.
 
-## Class `RunState(cs.threads.HasThreadState)`
+## Class `RunState(cs.fsm.FSM, cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -259,22 +259,22 @@
   to be called whenever `.cancel` is called.
 
 *Method `RunState.__bool__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.__enter_exit__(self)`*:
 The `__enter__`/`__exit__` generator function:
-* push this RunState via HasThreadState
-* catch signals
+* push this `RunState` via `HasThreadState`
+* catch signals if we are in the main `Thread`
 * start
 * `yield self` => run
-* cancel on exception during run
+* cancel on exception during the run
 * stop
 
-Note that if the `RunState` is already runnings we do not
+Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
 in the "running" state.
 
 *Method `RunState.__nonzero__(self)`*:
@@ -294,16 +294,22 @@
 
 Parameters:
 * `sig`: an `int` signal number or an iterable of signal numbers
 * `call_previous`: optional flag (default `False`)
   passed to `cs.psutils.signal_handlers`
 
 *Method `RunState.end(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+Obsolete synonym for `.stop()`.
+
+*Method `RunState.fsm_event(self, event: str, **extra)`*:
+Override `FSM.fsm_event` to apply side effects to particular transitions.
+
+On `'cancel'` set the cancelled flag.
+On `'start'` clear the cancelled flag and set `.start_time`.
+On `'stop'`set `.stop_time`.
 
 *Method `RunState.handle_signal(self, sig, _)`*:
 `RunState` signal handler: cancel the run state.
 Warn if `self.verbose`.
 
 *Method `RunState.iter(self, it)`*:
 Iterate over `it` while not `self.cancelled`.
@@ -323,37 +329,37 @@
 
 *Property `RunState.run_time`*:
 Property returning most recent run time (`stop_time-start_time`).
 If still running, use now as the stop time.
 If not started, return `0.0`.
 
 *Property `RunState.running`*:
-Property expressing whether the task is running.
+Whether the state is `'RUNNING'` or `'STOPPING'`.
 
 *Method `RunState.start(self, running_ok=False)`*:
 Start: adjust state, set `start_time` to now.
 Sets `.cancelled` to `False` and sets `.running` to `True`.
 
-*Method `RunState.stop(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+*Property `RunState.state`*:
+The `RunState`'s state as a string.
+Deprecated, new uses should consult `self.fsm_state`.
 
-*Property `RunState.stopped`*:
-Was the process stopped? Running is false and cancelled is true.
+*Method `RunState.stop(self)`*:
+Fire the `'stop'` event.
 
 *Property `RunState.stopping`*:
-Is the process stopping? Running is true and cancelled is true.
+Is the process stopping?
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -372,14 +378,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240519*:
+RunState now subclasses cs.fsm.FSM.
+
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
```

### Comparing `cs.resources-20240423/pyproject.toml` & `cs.resources-20240519/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.context>=20240412",
     "cs.deco>=20240412",
+    "cs.fsm>=20240519",
     "cs.gimmicks>=20240316",
     "cs.obj>=20220918",
     "cs.pfx>=20240412",
     "cs.psutils>=20240316",
-    "cs.py.func>=20230331",
-    "cs.py.stack>=20240412",
+    "cs.py.stack>=20240519",
     "cs.result>=20240412",
     "cs.threads>=20240422",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240423"
+version = "20240519"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Resource management classes and functions.
 
-*Latest release 20240423*:
-RunStateMixin: make the optional runstate parameter keyword only.
+*Latest release 20240519*:
+RunState now subclasses cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -231,15 +231,15 @@
     If omitted or `None`, defaults to 4.
     If 0, no upper limit is applied.
 * `lock`: optional shared Lock; if omitted or `None` a new Lock is allocated
 
 *Method `Pool.instance(self)`*:
 Context manager returning an object for use, which is returned to the pool afterwards.
 
-## Class `RunState(cs.threads.HasThreadState)`
+## Class `RunState(cs.fsm.FSM, cs.threads.HasThreadState)`
 
 A class to track a running task whose cancellation may be requested.
 
 Its purpose is twofold, to provide easily queriable state
 around tasks which can start and stop, and to provide control
 methods to pronounce that a task has started (`.start`),
 should stop (`.cancel`)
@@ -283,22 +283,22 @@
   to be called whenever `.cancel` is called.
 
 *Method `RunState.__bool__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.__enter_exit__(self)`*:
 The `__enter__`/`__exit__` generator function:
-* push this RunState via HasThreadState
-* catch signals
+* push this `RunState` via `HasThreadState`
+* catch signals if we are in the main `Thread`
 * start
 * `yield self` => run
-* cancel on exception during run
+* cancel on exception during the run
 * stop
 
-Note that if the `RunState` is already runnings we do not
+Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
 in the \"running\" state.
 
 *Method `RunState.__nonzero__(self)`*:
@@ -318,16 +318,22 @@
 
 Parameters:
 * `sig`: an `int` signal number or an iterable of signal numbers
 * `call_previous`: optional flag (default `False`)
   passed to `cs.psutils.signal_handlers`
 
 *Method `RunState.end(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+Obsolete synonym for `.stop()`.
+
+*Method `RunState.fsm_event(self, event: str, **extra)`*:
+Override `FSM.fsm_event` to apply side effects to particular transitions.
+
+On `'cancel'` set the cancelled flag.
+On `'start'` clear the cancelled flag and set `.start_time`.
+On `'stop'`set `.stop_time`.
 
 *Method `RunState.handle_signal(self, sig, _)`*:
 `RunState` signal handler: cancel the run state.
 Warn if `self.verbose`.
 
 *Method `RunState.iter(self, it)`*:
 Iterate over `it` while not `self.cancelled`.
@@ -347,37 +353,37 @@
 
 *Property `RunState.run_time`*:
 Property returning most recent run time (`stop_time-start_time`).
 If still running, use now as the stop time.
 If not started, return `0.0`.
 
 *Property `RunState.running`*:
-Property expressing whether the task is running.
+Whether the state is `'RUNNING'` or `'STOPPING'`.
 
 *Method `RunState.start(self, running_ok=False)`*:
 Start: adjust state, set `start_time` to now.
 Sets `.cancelled` to `False` and sets `.running` to `True`.
 
-*Method `RunState.stop(self)`*:
-Stop: adjust state, set `stop_time` to now.
-Sets sets `.running` to `False`.
+*Property `RunState.state`*:
+The `RunState`'s state as a string.
+Deprecated, new uses should consult `self.fsm_state`.
 
-*Property `RunState.stopped`*:
-Was the process stopped? Running is false and cancelled is true.
+*Method `RunState.stop(self)`*:
+Fire the `'stop'` event.
 
 *Property `RunState.stopping`*:
-Is the process stopping? Running is true and cancelled is true.
+Is the process stopping?
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -396,14 +402,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240519*:
+RunState now subclasses cs.fsm.FSM.
+
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
```

