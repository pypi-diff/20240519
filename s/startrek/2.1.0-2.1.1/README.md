# Comparing `tmp/startrek-2.1.0.tar.gz` & `tmp/startrek-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/startrek-2.1.0.tar", last modified: Fri May 17 11:40:32 2024, max compression
+gzip compressed data, was "dist/startrek-2.1.1.tar", last modified: Sun May 19 17:25:29 2024, max compression
```

## Comparing `startrek-2.1.0.tar` & `startrek-2.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-17 11:40:32.000000 startrek-2.1.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-2.1.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 11:40:32.000000 startrek-2.1.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      826 2024-05-16 17:30:23.000000 startrek-2.1.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/
--rw-r--r--   0 moky       (501) staff       (20)     2570 2024-05-17 03:38:09.000000 startrek-2.1.0/startrek/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-2.1.0/startrek/arrival.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-2.1.0/startrek/departure.py
--rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-2.1.0/startrek/dock.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/fsm/
--rw-r--r--   0 moky       (501) staff       (20)     1806 2024-05-16 18:44:18.000000 startrek-2.1.0/startrek/fsm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2354 2024-05-16 18:44:59.000000 startrek-2.1.0/startrek/fsm/auto.py
--rw-r--r--   0 moky       (501) staff       (20)     8430 2024-05-07 05:02:58.000000 startrek-2.1.0/startrek/fsm/base.py
--rw-r--r--   0 moky       (501) staff       (20)     5884 2024-05-16 18:44:46.000000 startrek-2.1.0/startrek/fsm/machine.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/net/
--rw-r--r--   0 moky       (501) staff       (20)     3310 2024-05-17 03:36:47.000000 startrek-2.1.0/startrek/net/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7022 2024-05-17 03:27:10.000000 startrek-2.1.0/startrek/net/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     3390 2024-05-16 18:45:43.000000 startrek-2.1.0/startrek/net/connection.py
--rw-r--r--   0 moky       (501) staff       (20)     3416 2024-05-07 05:09:27.000000 startrek-2.1.0/startrek/net/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     3884 2024-05-17 10:08:40.000000 startrek-2.1.0/startrek/net/hub.py
--rw-r--r--   0 moky       (501) staff       (20)     4276 2024-05-17 10:11:09.000000 startrek-2.1.0/startrek/net/socket.py
--rw-r--r--   0 moky       (501) staff       (20)    17046 2024-05-07 05:11:00.000000 startrek-2.1.0/startrek/net/state.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/port/
--rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-2.1.0/startrek/port/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3130 2024-05-07 05:12:48.000000 startrek-2.1.0/startrek/port/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4448 2024-05-16 18:46:02.000000 startrek-2.1.0/startrek/port/docker.py
--rw-r--r--   0 moky       (501) staff       (20)     2649 2024-05-16 18:46:09.000000 startrek-2.1.0/startrek/port/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-2.1.0/startrek/port/ship.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/skywalker/
--rw-r--r--   0 moky       (501) staff       (20)     1768 2024-05-16 18:51:08.000000 startrek-2.1.0/startrek/skywalker/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3418 2024-05-16 18:33:35.000000 startrek-2.1.0/startrek/skywalker/daemon.py
--rw-r--r--   0 moky       (501) staff       (20)     5038 2024-05-16 18:38:35.000000 startrek-2.1.0/startrek/skywalker/runner.py
--rw-r--r--   0 moky       (501) staff       (20)     4524 2024-05-16 18:35:35.000000 startrek-2.1.0/startrek/skywalker/ticker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/socket/
--rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-2.1.0/startrek/socket/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4456 2024-05-16 18:46:20.000000 startrek-2.1.0/startrek/socket/active_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    13048 2024-05-17 10:17:03.000000 startrek-2.1.0/startrek/socket/base_channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10668 2024-05-07 05:24:27.000000 startrek-2.1.0/startrek/socket/base_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    10182 2024-05-17 03:39:37.000000 startrek-2.1.0/startrek/socket/base_hub.py
--rw-r--r--   0 moky       (501) staff       (20)    10900 2024-05-07 14:34:30.000000 startrek-2.1.0/startrek/stardocker.py
--rw-r--r--   0 moky       (501) staff       (20)    11689 2024-05-16 18:47:32.000000 startrek-2.1.0/startrek/stargate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/types/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-2.1.0/startrek/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-2.1.0/startrek/types/mapping.py
--rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-2.1.0/startrek/types/pair.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      989 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        9 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-19 17:25:29.000000 startrek-2.1.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-2.1.1/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-19 17:25:29.000000 startrek-2.1.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      826 2024-05-18 16:24:55.000000 startrek-2.1.1/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/
+-rw-r--r--   0 moky       (501) staff       (20)     2570 2024-05-17 03:38:09.000000 startrek-2.1.1/startrek/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-2.1.1/startrek/arrival.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-2.1.1/startrek/departure.py
+-rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-2.1.1/startrek/dock.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/fsm/
+-rw-r--r--   0 moky       (501) staff       (20)     1806 2024-05-16 18:44:18.000000 startrek-2.1.1/startrek/fsm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2024-05-16 18:44:59.000000 startrek-2.1.1/startrek/fsm/auto.py
+-rw-r--r--   0 moky       (501) staff       (20)     8430 2024-05-07 05:02:58.000000 startrek-2.1.1/startrek/fsm/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     5884 2024-05-16 18:44:46.000000 startrek-2.1.1/startrek/fsm/machine.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/net/
+-rw-r--r--   0 moky       (501) staff       (20)     3310 2024-05-17 03:36:47.000000 startrek-2.1.1/startrek/net/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7022 2024-05-17 03:27:10.000000 startrek-2.1.1/startrek/net/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     3390 2024-05-16 18:45:43.000000 startrek-2.1.1/startrek/net/connection.py
+-rw-r--r--   0 moky       (501) staff       (20)     3416 2024-05-07 05:09:27.000000 startrek-2.1.1/startrek/net/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     3884 2024-05-17 10:08:40.000000 startrek-2.1.1/startrek/net/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4276 2024-05-17 10:11:09.000000 startrek-2.1.1/startrek/net/socket.py
+-rw-r--r--   0 moky       (501) staff       (20)    17046 2024-05-07 05:11:00.000000 startrek-2.1.1/startrek/net/state.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/port/
+-rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-2.1.1/startrek/port/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3130 2024-05-07 05:12:48.000000 startrek-2.1.1/startrek/port/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4448 2024-05-16 18:46:02.000000 startrek-2.1.1/startrek/port/docker.py
+-rw-r--r--   0 moky       (501) staff       (20)     2649 2024-05-16 18:46:09.000000 startrek-2.1.1/startrek/port/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-2.1.1/startrek/port/ship.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/skywalker/
+-rw-r--r--   0 moky       (501) staff       (20)     1768 2024-05-16 18:51:08.000000 startrek-2.1.1/startrek/skywalker/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3298 2024-05-18 17:46:34.000000 startrek-2.1.1/startrek/skywalker/daemon.py
+-rw-r--r--   0 moky       (501) staff       (20)     5078 2024-05-18 17:41:45.000000 startrek-2.1.1/startrek/skywalker/runner.py
+-rw-r--r--   0 moky       (501) staff       (20)     4759 2024-05-18 17:56:56.000000 startrek-2.1.1/startrek/skywalker/ticker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/socket/
+-rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-2.1.1/startrek/socket/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4452 2024-05-18 17:40:10.000000 startrek-2.1.1/startrek/socket/active_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    13048 2024-05-17 10:17:03.000000 startrek-2.1.1/startrek/socket/base_channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10668 2024-05-07 05:24:27.000000 startrek-2.1.1/startrek/socket/base_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    10170 2024-05-18 17:40:46.000000 startrek-2.1.1/startrek/socket/base_hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    10900 2024-05-07 14:34:30.000000 startrek-2.1.1/startrek/stardocker.py
+-rw-r--r--   0 moky       (501) staff       (20)    11677 2024-05-18 17:41:03.000000 startrek-2.1.1/startrek/stargate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-2.1.1/startrek/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-2.1.1/startrek/types/mapping.py
+-rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-2.1.1/startrek/types/pair.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      989 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        9 2024-05-19 17:25:29.000000 startrek-2.1.1/startrek.egg-info/top_level.txt
```

### Comparing `startrek-2.1.0/setup.py` & `startrek-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~
 
     Interstellar Transport
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

### Comparing `startrek-2.1.0/startrek/__init__.py` & `startrek-2.1.1/startrek/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/arrival.py` & `startrek-2.1.1/startrek/arrival.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/departure.py` & `startrek-2.1.1/startrek/departure.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/dock.py` & `startrek-2.1.1/startrek/dock.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/fsm/__init__.py` & `startrek-2.1.1/startrek/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/fsm/auto.py` & `startrek-2.1.1/startrek/fsm/auto.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/fsm/base.py` & `startrek-2.1.1/startrek/fsm/base.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/fsm/machine.py` & `startrek-2.1.1/startrek/fsm/machine.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/__init__.py` & `startrek-2.1.1/startrek/net/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/channel.py` & `startrek-2.1.1/startrek/net/channel.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/connection.py` & `startrek-2.1.1/startrek/net/connection.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/delegate.py` & `startrek-2.1.1/startrek/net/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/hub.py` & `startrek-2.1.1/startrek/net/hub.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/socket.py` & `startrek-2.1.1/startrek/net/socket.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/net/state.py` & `startrek-2.1.1/startrek/net/state.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/port/__init__.py` & `startrek-2.1.1/startrek/port/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/port/delegate.py` & `startrek-2.1.1/startrek/port/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/port/docker.py` & `startrek-2.1.1/startrek/port/docker.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/port/gate.py` & `startrek-2.1.1/startrek/port/gate.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/port/ship.py` & `startrek-2.1.1/startrek/port/ship.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/skywalker/__init__.py` & `startrek-2.1.1/startrek/skywalker/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/skywalker/daemon.py` & `startrek-2.1.1/startrek/skywalker/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,20 +61,18 @@
         if thr is not None:
             return thr.is_alive()
 
     def start(self):
         """ Run the target in background thread """
         self.__force_stop()
         target = self.target
-        if target is None:
-            return False
-        thr = Thread(target=_bg_target, args=(target,), daemon=True)
-        thr.start()
-        self.__thread = thr
-        return True
+        if target is not None:
+            thr = Runner.async_thread(coro=target.run())
+            thr.start()
+            self.__thread = thr
 
     def stop(self):
         """ Stop the background thread """
         self.__force_stop()
 
     def __del__(self):
         self.__force_stop()
@@ -96,11 +94,7 @@
         """ Stop the thread """
         try:
             if thr.is_alive():
                 thr.join(timeout=timeout)
         except RuntimeError as error:
             print('[Daemon] failed to join thread: %s, timeout: %d' % (error, timeout))
             traceback.print_exc()
-
-
-def _bg_target(target: Runnable):
-    Runner.sync_run(main=target.run())
```

### Comparing `startrek-2.1.0/startrek/skywalker/runner.py` & `startrek-2.1.1/startrek/skywalker/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import asyncio
 from abc import ABC, abstractmethod
 from threading import Thread
+from typing import Coroutine
 
 
 class Processor(ABC):
 
     @abstractmethod
     async def process(self) -> bool:
         """
@@ -45,20 +46,20 @@
         raise NotImplemented
 
 
 class Handler(ABC):
 
     @abstractmethod
     async def setup(self):
-        """ Prepare for Handling """
+        """ Prepare before Handling """
         raise NotImplemented
     
     @abstractmethod
     async def handle(self):
-        """ Handling run loop """
+        """ Run loop for handling """
         raise NotImplemented
 
     @abstractmethod
     async def finish(self):
         """ Cleanup after handled """
         raise NotImplemented
 
@@ -73,17 +74,15 @@
 
 # noinspection PyAbstractClass
 class Runner(Runnable, Handler, Processor, ABC):
     """
         Runner
         ~~~~~~
 
-        @abstract methods:
-            - setup()
-            - finish()
+        @abstract method:
             - process()
     """
 
     # Frames Per Second
     # ~~~~~~~~~~~~~~~~~
     # (1) The human eye can process 10-12 still images per second,
     #     and the dynamic compensation function can also deceive us.
@@ -123,14 +122,24 @@
         await self.setup()
         try:
             await self.handle()
         finally:
             await self.finish()
 
     # Override
+    async def setup(self):
+        # TODO: override to prepare before handling
+        pass
+
+    # Override
+    async def finish(self):
+        # TODO: override to cleanup after handled
+        pass
+
+    # Override
     async def handle(self):
         while self.running:
             if await self.process():
                 # runner is busy, return True to go on.
                 pass
             else:
                 # if nothing to do now, return False here
@@ -143,31 +152,20 @@
         # time.sleep(self.interval)
 
     @classmethod
     async def sleep(cls, seconds: float):
         await asyncio.sleep(seconds)
 
     @classmethod
-    def sync_run(cls, main):
+    def sync_run(cls, main: Coroutine):
         """ Run main coroutine until complete """
-        asyncio.run(main)
+        return asyncio.run(main)
 
     @classmethod
-    def async_run(cls, coroutine) -> asyncio.Task:
+    def async_task(cls, coro: Coroutine) -> asyncio.Task:
         """ Create an async task to run the coroutine """
-        return asyncio.create_task(coroutine)
+        return asyncio.create_task(coro)
 
     @classmethod
-    def thread_run(cls, runner) -> Thread:
-        """ Run target in a daemon thread """
-        thr = Thread(target=_bg_runner, args=(runner,), daemon=True)
-        thr.start()
-        return thr
-
-
-def _bg_runner(runner: Runner):
-    Runner.sync_run(main=_bg_start(runner=runner))
-
-
-async def _bg_start(runner: Runner):
-    await runner.start()
-    await runner.run()
+    def async_thread(cls, coro: Coroutine) -> Thread:
+        """ Create a daemon thread to run the coroutine """
+        return Thread(target=cls.sync_run, args=(coro,), daemon=True)
```

### Comparing `startrek-2.1.0/startrek/skywalker/ticker.py` & `startrek-2.1.1/startrek/skywalker/ticker.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 
     # Override
     async def setup(self):
         # update process time
         self.__last_time = time.time()
 
     # Override
-    async def finish(self):
-        pass
-
-    # Override
     async def process(self) -> bool:
         tickers = self.tickers
         if len(tickers) == 0:
             # nothing to do now,
             # return False to have a rest ^_^
             return False
         # 1. check time
@@ -139,15 +135,28 @@
 
 @Singleton
 class PrimeMetronome:
 
     def __init__(self):
         super().__init__()
         metronome = Metronome(interval=Runner.INTERVAL_SLOW)
-        Runner.thread_run(runner=metronome)
         self.__metronome = metronome
+        start_runner(runner=metronome)
 
     def add_ticker(self, ticker: Ticker):
-        self.__metronome.add_ticker(ticker=ticker)
+        metronome = self.__metronome
+        metronome.add_ticker(ticker=ticker)
 
     def remove_ticker(self, ticker: Ticker):
-        self.__metronome.remove_ticker(ticker=ticker)
+        metronome = self.__metronome
+        metronome.remove_ticker(ticker=ticker)
+
+
+def start_runner(runner: Runner) -> threading.Thread:
+    thr = Runner.async_thread(coro=_bg_runner(runner=runner))
+    thr.start()
+    return thr
+
+
+async def _bg_runner(runner: Runner):
+    await runner.start()
+    await runner.run()
```

### Comparing `startrek-2.1.0/startrek/socket/__init__.py` & `startrek-2.1.1/startrek/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/socket/active_conn.py` & `startrek-2.1.1/startrek/socket/active_conn.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     # Override
     async def start(self, hub: Hub):
         self.__hub_ref = weakref.ref(hub)
         # 1. start state machine
         await self._start_machine()
         # 2. start an async task to check channel
-        Runner.async_run(coroutine=self.run())
+        Runner.async_task(coro=self.run())
         # await self.run()
 
     # Override
     async def run(self):
         expired = 0
         last_time = 0
         interval = 8
```

### Comparing `startrek-2.1.0/startrek/socket/base_channel.py` & `startrek-2.1.1/startrek/socket/base_channel.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/socket/base_conn.py` & `startrek-2.1.1/startrek/socket/base_conn.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/socket/base_hub.py` & `startrek-2.1.1/startrek/socket/base_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 
     # Override
     def set(self, item: Optional[Connection],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            Runner.async_run(coroutine=cached.close())
+            Runner.async_task(coro=cached.close())
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
         assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Connection],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            Runner.async_run(coroutine=cached.close())
+            Runner.async_task(coro=cached.close())
         if item is not None:
-            Runner.async_run(coroutine=item.close())
+            Runner.async_task(coro=item.close())
         return cached
 
 
 class BaseHub(Hub, ABC):
 
     """
         Maximum Segment Size
```

### Comparing `startrek-2.1.0/startrek/stardocker.py` & `startrek-2.1.1/startrek/stardocker.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/stargate.py` & `startrek-2.1.1/startrek/stargate.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,28 @@
 
     # Override
     def set(self, item: Optional[Docker],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            Runner.async_run(coroutine=cached.close())
+            Runner.async_task(coro=cached.close())
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
         assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Docker],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            Runner.async_run(coroutine=cached.close())
+            Runner.async_task(coro=cached.close())
         if item is not None:
-            Runner.async_run(coroutine=item.close())
+            Runner.async_task(coro=item.close())
         return cached
 
 
 class StarGate(Gate, ConnectionDelegate, ABC):
     """
         Star Gate
         ~~~~~~~~~
```

### Comparing `startrek-2.1.0/startrek/types/__init__.py` & `startrek-2.1.1/startrek/types/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/types/mapping.py` & `startrek-2.1.1/startrek/types/mapping.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek/types/pair.py` & `startrek-2.1.1/startrek/types/pair.py`

 * *Files identical despite different names*

### Comparing `startrek-2.1.0/startrek.egg-info/SOURCES.txt` & `startrek-2.1.1/startrek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

