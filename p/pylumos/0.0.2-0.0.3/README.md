# Comparing `tmp/pylumos-0.0.2.tar.gz` & `tmp/pylumos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylumos-0.0.2.tar", last modified: Thu May 16 17:08:34 2024, max compression
+gzip compressed data, was "pylumos-0.0.3.tar", last modified: Sun May 19 01:51:08 2024, max compression
```

## Comparing `pylumos-0.0.2.tar` & `pylumos-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 17:08:34.931721 pylumos-0.0.2/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     3078 2024-04-29 21:54:16.000000 pylumos-0.0.2/.gitignore
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1073 2024-03-29 15:32:32.000000 pylumos-0.0.2/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)      318 2024-05-16 17:08:34.931721 pylumos-0.0.2/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        7 2024-03-29 15:34:56.000000 pylumos-0.0.2/README.md
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 17:08:34.931721 pylumos-0.0.2/lumos/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      108 2024-05-16 15:22:03.000000 pylumos-0.0.2/lumos/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-29 15:34:56.000000 pylumos-0.0.2/lumos/__main__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 17:08:34.931721 pylumos-0.0.2/lumos/__pycache__/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      164 2024-05-16 15:22:28.000000 pylumos-0.0.2/lumos/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      650 2024-03-29 15:34:59.000000 pylumos-0.0.2/lumos/__pycache__/__main__.cpython-38.pyc
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4786 2024-05-16 15:54:58.000000 pylumos-0.0.2/lumos/__pycache__/cli.cpython-38.pyc
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4977 2024-05-16 15:46:16.000000 pylumos-0.0.2/lumos/cli.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 17:08:34.931721 pylumos-0.0.2/lumos/examples/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      378 2024-05-12 21:57:11.000000 pylumos-0.0.2/lumos/examples/pulse.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1376 2024-05-12 21:56:59.000000 pylumos-0.0.2/lumos/examples/rainbow.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      479 2024-05-16 17:07:38.000000 pylumos-0.0.2/lumos/examples/random_bits.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      941 2024-05-12 21:57:05.000000 pylumos-0.0.2/lumos/examples/stream.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      736 2024-05-06 21:29:55.000000 pylumos-0.0.2/lumos/generator.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4632 2024-05-16 15:46:46.000000 pylumos-0.0.2/lumos/lumos.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-16 17:08:34.931721 pylumos-0.0.2/pylumos.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      318 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      534 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/entry_points.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       13 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-05-16 17:08:34.000000 pylumos-0.0.2/pylumos.egg-info/top_level.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2024-05-16 17:08:34.931721 pylumos-0.0.2/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      735 2024-05-16 17:08:04.000000 pylumos-0.0.2/setup.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     3078 2024-04-29 21:54:16.000000 pylumos-0.0.3/.gitignore
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1073 2024-03-29 15:32:32.000000 pylumos-0.0.3/LICENSE
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      318 2024-05-19 01:51:08.238320 pylumos-0.0.3/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        7 2024-03-29 15:34:56.000000 pylumos-0.0.3/README.md
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/drivers/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      304 2024-03-30 17:48:46.000000 pylumos-0.0.3/drivers/99-redhill.rules
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1334 2024-05-18 18:31:18.000000 pylumos-0.0.3/drivers/lumos.inf
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/lumos/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      108 2024-05-19 01:49:28.000000 pylumos-0.0.3/lumos/__init__.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      424 2024-03-29 15:34:56.000000 pylumos-0.0.3/lumos/__main__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/lumos/__pycache__/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      164 2024-05-16 15:22:28.000000 pylumos-0.0.3/lumos/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      650 2024-03-29 15:34:59.000000 pylumos-0.0.3/lumos/__pycache__/__main__.cpython-38.pyc
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4786 2024-05-16 15:54:58.000000 pylumos-0.0.3/lumos/__pycache__/cli.cpython-38.pyc
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     5287 2024-05-18 18:37:55.000000 pylumos-0.0.3/lumos/cli.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/lumos/examples/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      378 2024-05-12 21:57:11.000000 pylumos-0.0.3/lumos/examples/pulse.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1376 2024-05-12 21:56:59.000000 pylumos-0.0.3/lumos/examples/rainbow.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      479 2024-05-16 17:07:38.000000 pylumos-0.0.3/lumos/examples/random_bits.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      941 2024-05-12 21:57:05.000000 pylumos-0.0.3/lumos/examples/stream.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      736 2024-05-06 21:29:55.000000 pylumos-0.0.3/lumos/generator.py
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4632 2024-05-16 15:46:46.000000 pylumos-0.0.3/lumos/lumos.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-05-19 01:51:08.238320 pylumos-0.0.3/pylumos.egg-info/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      318 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      577 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       46 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       13 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        6 2024-05-19 01:51:08.000000 pylumos-0.0.3/pylumos.egg-info/top_level.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2024-05-19 01:51:08.238320 pylumos-0.0.3/setup.cfg
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      735 2024-05-19 01:49:23.000000 pylumos-0.0.3/setup.py
```

### Comparing `pylumos-0.0.2/.gitignore` & `pylumos-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/LICENSE` & `pylumos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/__pycache__/__main__.cpython-38.pyc` & `pylumos-0.0.3/lumos/__pycache__/__main__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/__pycache__/cli.cpython-38.pyc` & `pylumos-0.0.3/lumos/__pycache__/cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/cli.py` & `pylumos-0.0.3/lumos/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import argparse
 import os
 import shutil
+import platform
 
 from time import sleep
 
 import lumos
 from lumos.lumos import Lumos, LumosPowerState, LumosMode, LumosColor
 from recom import RecomDevice, RecomDeviceException
 from recom.backend.usb import get_vid_pid_on_port
-from recom.util import get_drive_mount_point_from_usb_port_path
+
+if platform.system() != 'Windows':
+    from recom.util import get_drive_mount_point_from_usb_port_path
 
 
 def print_info():
     board = Lumos()
     print(f"Number of LEDs = {board.interface.get_num_leds()}")
     print(f"Power state = {board.interface.get_power_state()}")
     print(f"Voltage = {board.interface.get_voltage_reading()}mV")
@@ -101,37 +104,41 @@
         if new_vp is not None:
             if new_vp[0] != old_vp[0] or new_vp[1] != old_vp[1]:
                 print("DONE")
                 print("Found device with VID=%04X, PID=%04X" % (new_vp[0], new_vp[1]))
                 break
         sleep(0.1)
 
-    print("Looking for mass storage device... ", end='')
-    for i in range(10):
-        mp = get_drive_mount_point_from_usb_port_path(port_path, new_vp)
-        if mp is not None:
-            break
-        sleep(1)
-    if mp == None:
-        print("\nERROR: Bootloader not found")
-        return False
+    if platform.system() != 'Windows':
+        print("Looking for mass storage device... ", end='')
+        for i in range(10):
+            mp = get_drive_mount_point_from_usb_port_path(port_path, new_vp)
+            if mp is not None:
+                break
+            sleep(1)
+        if mp == None:
+            print("\nERROR: Bootloader not found")
+            return False
+        else:
+            print(mp)
+        print(f"Updating device with {binary_file}")
+        if not os.path.exists(mp):
+            print(f"ERROR: Bootloader path does not exist ({mp})")
+            return False
+        dest_ref = os.path.join(mp, binary_file)
+        try:
+            shutil.copy(file_ref, dest_ref)
+        except IOError as exp:
+            print(f"ERROR: Failed to copy file {binary_file} ({exp})")
+            return False
+        print("DONE")
+        return True
     else:
-        print(mp)
-    print(f"Updating device with {binary_file}")
-    if not os.path.exists(mp):
-        print(f"ERROR: Bootloader path does not exist ({mp})")
-        return False
-    dest_ref = os.path.join(mp, binary_file)
-    try:
-        shutil.copy(file_ref, dest_ref)
-    except IOError as exp:
-        print(f"ERROR: Failed to copy file {binary_file} ({exp})")
-        return False
-    print("DONE")
-    return True
+        print(f"Please manually copy {binary_file} to the flash driver that just showd up!")
+        return True
 
 
 def cli(argv):
     parser = argparse.ArgumentParser(description="Lumos CLI to interract with an LED controller board.")
     parser.add_argument("cmd", type=str, help="Command/Action")
     parser.add_argument('--version', action='version', version=lumos.__version__,
                                                 help="Print package version")
```

### Comparing `pylumos-0.0.2/lumos/examples/rainbow.py` & `pylumos-0.0.3/lumos/examples/rainbow.py`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/examples/stream.py` & `pylumos-0.0.3/lumos/examples/stream.py`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/generator.py` & `pylumos-0.0.3/lumos/generator.py`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/lumos/lumos.py` & `pylumos-0.0.3/lumos/lumos.py`

 * *Files identical despite different names*

### Comparing `pylumos-0.0.2/pylumos.egg-info/SOURCES.txt` & `pylumos-0.0.3/pylumos.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 .gitignore
 LICENSE
 README.md
 setup.py
+drivers/99-redhill.rules
+drivers/lumos.inf
 lumos/__init__.py
 lumos/__main__.py
 lumos/cli.py
 lumos/generator.py
 lumos/lumos.py
 lumos/__pycache__/__init__.cpython-38.pyc
 lumos/__pycache__/__main__.cpython-38.pyc
```

### Comparing `pylumos-0.0.2/setup.py` & `pylumos-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='pylumos',
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     setup_requires=['setuptools_scm'],
     license='MIT',
     author='Adrian Rothenbuhler',
     author_email='adrian@redhill-embedded.com',
     description='Addressable LED interface tool',
     keywords='LED',
```

