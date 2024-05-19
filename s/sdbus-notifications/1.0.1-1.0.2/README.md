# Comparing `tmp/sdbus-notifications-1.0.1.tar.gz` & `tmp/sdbus-notifications-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdbus-notifications-1.0.1.tar", last modified: Sat Jul 17 17:47:10 2021, max compression
+gzip compressed data, was "sdbus-notifications-1.0.2.tar", last modified: Sun May 19 11:49:47 2024, max compression
```

## Comparing `sdbus-notifications-1.0.1.tar` & `sdbus-notifications-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/
--rw-r--r--   0 user      (1000) user      (1000)    18092 2021-07-17 17:22:49.000000 sdbus-notifications-1.0.1/COPYING
--rw-r--r--   0 user      (1000) user      (1000)    26530 2021-07-17 17:22:49.000000 sdbus-notifications-1.0.1/COPYING.LESSER
--rw-r--r--   0 user      (1000) user      (1000)     2094 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1101 2021-07-17 17:46:06.000000 sdbus-notifications-1.0.1/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/sdbus_async/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/sdbus_async/notifications/
--rw-r--r--   0 user      (1000) user      (1000)    10072 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.1/sdbus_async/notifications/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.1/sdbus_async/notifications/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/sdbus_block/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/sdbus_block/notifications/
--rw-r--r--   0 user      (1000) user      (1000)     9057 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.1/sdbus_block/notifications/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.1/sdbus_block/notifications/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2094 2021-07-17 17:47:10.000000 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      401 2021-07-17 17:47:10.000000 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-07-17 17:47:10.000000 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       14 2021-07-17 17:47:10.000000 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       24 2021-07-17 17:47:10.000000 sdbus-notifications-1.0.1/sdbus_notifications.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2021-07-17 17:47:10.866089 sdbus-notifications-1.0.1/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     2403 2021-07-17 17:46:21.000000 sdbus-notifications-1.0.1/setup.py
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.795003 sdbus-notifications-1.0.2/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    18092 2021-07-17 17:22:49.000000 sdbus-notifications-1.0.2/COPYING
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    26530 2021-07-17 17:22:49.000000 sdbus-notifications-1.0.2/COPYING.LESSER
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2399 2024-05-19 11:49:47.795003 sdbus-notifications-1.0.2/PKG-INFO
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     1318 2024-05-19 11:48:29.000000 sdbus-notifications-1.0.2/README.md
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.791670 sdbus-notifications-1.0.2/sdbus_async/
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.791670 sdbus-notifications-1.0.2/sdbus_async/notifications/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)    10174 2024-05-19 09:30:06.000000 sdbus-notifications-1.0.2/sdbus_async/notifications/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.2/sdbus_async/notifications/py.typed
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.791670 sdbus-notifications-1.0.2/sdbus_block/
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.791670 sdbus-notifications-1.0.2/sdbus_block/notifications/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     9159 2024-05-19 09:30:06.000000 sdbus-notifications-1.0.2/sdbus_block/notifications/__init__.py
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        0 2021-07-17 17:19:12.000000 sdbus-notifications-1.0.2/sdbus_block/notifications/py.typed
+drwxr-xr-x   0 igo95862  (1000) igo95862  (1000)        0 2024-05-19 11:49:47.795003 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2399 2024-05-19 11:49:47.000000 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)      401 2024-05-19 11:49:47.000000 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)        1 2024-05-19 11:49:47.000000 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       14 2024-05-19 11:49:47.000000 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/requires.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       24 2024-05-19 11:49:47.000000 sdbus-notifications-1.0.2/sdbus_notifications.egg-info/top_level.txt
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)       38 2024-05-19 11:49:47.795003 sdbus-notifications-1.0.2/setup.cfg
+-rw-r--r--   0 igo95862  (1000) igo95862  (1000)     2554 2024-05-19 11:48:29.000000 sdbus-notifications-1.0.2/setup.py
```

### Comparing `sdbus-notifications-1.0.1/COPYING` & `sdbus-notifications-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `sdbus-notifications-1.0.1/COPYING.LESSER` & `sdbus-notifications-1.0.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `sdbus-notifications-1.0.1/PKG-INFO` & `sdbus-notifications-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: sdbus-notifications
-Version: 1.0.1
+Version: 1.0.2
 Summary: Freedesktop notifications binds for sdbus.
-Home-page: https://github.com/igo95862/python-sdbus
+Home-page: https://github.com/python-sdbus/python-sdbus-notifications
 Author: igo95862
 Author-email: igo95862@yandex.ru
 License: LGPL-2.1-or-later
-Project-URL: Documentation, https://python-sdbus.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/igo95862/python-sdbus/
-Project-URL: Tracker, https://github.com/igo95862/python-sdbus/issues/
+Project-URL: Documentation, https://python-sdbus-notifications.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/python-sdbus/python-sdbus-notifications
+Project-URL: Tracker, https://github.com/python-sdbus/python-sdbus-notifications/issues
 Keywords: dbus notifications linux freedesktop
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
+Requires-Dist: sdbus>=0.8rc2
+
+<!--
+SPDX-License-Identifier: LGPL-2.1-or-later
+SPDX-FileCopyrightText: 2024 igo95862
+-->
 
 [![Documentation Status](https://readthedocs.org/projects/python-sdbus-notifications/badge/?version=latest)](https://python-sdbus-notifications.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/sdbus-notifications)](https://pypi.org/project/sdbus-notifications/)
+
 # Freedesktop notifications binds for python-sdbus
 
-Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module) 
+Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module)
 
 Implemented:
 
 * NotificationsInterface - notifications interface to implement your own notifications daemon.
 * FreedesktopNotifications - notifications interface proxy connected to `org.freedesktop.Notifications` service and `/org/freedesktop/Notifications` path
 
 ## Requirements
 
 * `python-sdbus` version higher than 0.8rc2
 
-See [python-sdbus requirements](https://github.com/igo95862/python-sdbus#requirements).
+See [python-sdbus requirements](https://github.com/python-sdbus/python-sdbus#requirements).
 
 ## Installation
 
 `pip install --only-binary ':all:' sdbus-notifications`
 
 # [Documentation](https://python-sdbus-notifications.readthedocs.io/en/latest/)
 
-This is the sub-project of [python-sdbus](https://github.com/igo95862/python-sdbus).
+This is the sub-project of [python-sdbus](https://github.com/python-sdbus/python-sdbus).
 
 See the [python-sdbus documentation](https://python-sdbus.readthedocs.io/en/latest/).
-
-
```

### Comparing `sdbus-notifications-1.0.1/README.md` & `sdbus-notifications-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+<!--
+SPDX-License-Identifier: LGPL-2.1-or-later
+SPDX-FileCopyrightText: 2024 igo95862
+-->
+
 [![Documentation Status](https://readthedocs.org/projects/python-sdbus-notifications/badge/?version=latest)](https://python-sdbus-notifications.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/sdbus-notifications)](https://pypi.org/project/sdbus-notifications/)
+
 # Freedesktop notifications binds for python-sdbus
 
-Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module) 
+Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module)
 
 Implemented:
 
 * NotificationsInterface - notifications interface to implement your own notifications daemon.
 * FreedesktopNotifications - notifications interface proxy connected to `org.freedesktop.Notifications` service and `/org/freedesktop/Notifications` path
 
 ## Requirements
 
 * `python-sdbus` version higher than 0.8rc2
 
-See [python-sdbus requirements](https://github.com/igo95862/python-sdbus#requirements).
+See [python-sdbus requirements](https://github.com/python-sdbus/python-sdbus#requirements).
 
 ## Installation
 
 `pip install --only-binary ':all:' sdbus-notifications`
 
 # [Documentation](https://python-sdbus-notifications.readthedocs.io/en/latest/)
 
-This is the sub-project of [python-sdbus](https://github.com/igo95862/python-sdbus).
+This is the sub-project of [python-sdbus](https://github.com/python-sdbus/python-sdbus).
 
 See the [python-sdbus documentation](https://python-sdbus.readthedocs.io/en/latest/).
```

### Comparing `sdbus-notifications-1.0.1/sdbus_async/notifications/__init__.py` & `sdbus-notifications-1.0.2/sdbus_async/notifications/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,18 @@
 
         # x
         # y
         if xy_pos is not None:
             hints_dict['x'] = ('i', xy_pos[0])
             hints_dict['y'] = ('i', xy_pos[1])
 
+        # urgency
+        if urgency is not None:
+            hints_dict['urgency'] = ('y', urgency)
+
         return hints_dict
 
 
 class FreedesktopNotifications(NotificationsInterface):
     def __init__(self, bus: Optional[SdBus] = None) -> None:
         """Dbus interface object path and service name is
         predetermined.
```

### Comparing `sdbus-notifications-1.0.1/sdbus_block/notifications/__init__.py` & `sdbus-notifications-1.0.2/sdbus_block/notifications/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,8 +230,12 @@
 
         # x
         # y
         if xy_pos is not None:
             hints_dict['x'] = ('i', xy_pos[0])
             hints_dict['y'] = ('i', xy_pos[1])
 
+        # urgency
+        if urgency is not None:
+            hints_dict['urgency'] = ('y', urgency)
+
         return hints_dict
```

### Comparing `sdbus-notifications-1.0.1/sdbus_notifications.egg-info/PKG-INFO` & `sdbus-notifications-1.0.2/sdbus_notifications.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: sdbus-notifications
-Version: 1.0.1
+Version: 1.0.2
 Summary: Freedesktop notifications binds for sdbus.
-Home-page: https://github.com/igo95862/python-sdbus
+Home-page: https://github.com/python-sdbus/python-sdbus-notifications
 Author: igo95862
 Author-email: igo95862@yandex.ru
 License: LGPL-2.1-or-later
-Project-URL: Documentation, https://python-sdbus.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/igo95862/python-sdbus/
-Project-URL: Tracker, https://github.com/igo95862/python-sdbus/issues/
+Project-URL: Documentation, https://python-sdbus-notifications.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/python-sdbus/python-sdbus-notifications
+Project-URL: Tracker, https://github.com/python-sdbus/python-sdbus-notifications/issues
 Keywords: dbus notifications linux freedesktop
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
+Requires-Dist: sdbus>=0.8rc2
+
+<!--
+SPDX-License-Identifier: LGPL-2.1-or-later
+SPDX-FileCopyrightText: 2024 igo95862
+-->
 
 [![Documentation Status](https://readthedocs.org/projects/python-sdbus-notifications/badge/?version=latest)](https://python-sdbus-notifications.readthedocs.io/en/latest/?badge=latest)
+[![PyPI - Version](https://img.shields.io/pypi/v/sdbus-notifications)](https://pypi.org/project/sdbus-notifications/)
+
 # Freedesktop notifications binds for python-sdbus
 
-Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module) 
+Supports both asyncio (under `sdbus_async.notifications` module) and blocking (under `sdbus_block.notifications` module)
 
 Implemented:
 
 * NotificationsInterface - notifications interface to implement your own notifications daemon.
 * FreedesktopNotifications - notifications interface proxy connected to `org.freedesktop.Notifications` service and `/org/freedesktop/Notifications` path
 
 ## Requirements
 
 * `python-sdbus` version higher than 0.8rc2
 
-See [python-sdbus requirements](https://github.com/igo95862/python-sdbus#requirements).
+See [python-sdbus requirements](https://github.com/python-sdbus/python-sdbus#requirements).
 
 ## Installation
 
 `pip install --only-binary ':all:' sdbus-notifications`
 
 # [Documentation](https://python-sdbus-notifications.readthedocs.io/en/latest/)
 
-This is the sub-project of [python-sdbus](https://github.com/igo95862/python-sdbus).
+This is the sub-project of [python-sdbus](https://github.com/python-sdbus/python-sdbus).
 
 See the [python-sdbus documentation](https://python-sdbus.readthedocs.io/en/latest/).
-
-
```

### Comparing `sdbus-notifications-1.0.1/setup.py` & `sdbus-notifications-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,27 +25,33 @@
     long_description = f.read()
 
 setup(
     name='sdbus-notifications',
     description=('Freedesktop notifications binds for sdbus.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.1',
-    url='https://github.com/igo95862/python-sdbus',
+    version='1.0.2',
+    url='https://github.com/python-sdbus/python-sdbus-notifications',
     author='igo95862',
     author_email='igo95862@yandex.ru',
     license='LGPL-2.1-or-later',
     keywords='dbus notifications linux freedesktop',
     project_urls={
-        'Documentation': 'https://python-sdbus.readthedocs.io/en/latest/',
-        'Source': 'https://github.com/igo95862/python-sdbus/',
-        'Tracker': 'https://github.com/igo95862/python-sdbus/issues/',
+        'Documentation': (
+            'https://python-sdbus-notifications.readthedocs.io/en/latest/'
+        ),
+        'Source': (
+            'https://github.com/python-sdbus/python-sdbus-notifications'
+        ),
+        'Tracker': (
+            'https://github.com/python-sdbus/python-sdbus-notifications/issues'
+        ),
     },
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         (
             'License :: OSI Approved :: '
             'GNU Lesser General Public License v2 or later (LGPLv2+)'
         ),
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3 :: Only',
```

