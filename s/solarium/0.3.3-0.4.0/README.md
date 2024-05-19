# Comparing `tmp/solarium-0.3.3.tar.gz` & `tmp/solarium-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarium-0.3.3.tar", last modified: Sun Dec  5 13:00:50 2021, max compression
+gzip compressed data, was "solarium-0.4.0.tar", last modified: Sun May 19 15:39:14 2024, max compression
```

## Comparing `solarium-0.3.3.tar` & `solarium-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 13:00:50.680773 solarium-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-12-05 13:00:26.000000 solarium-0.3.3/.bandit
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-12-05 13:00:26.000000 solarium-0.3.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-05 13:00:26.000000 solarium-0.3.3/.fussyfox.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 13:00:50.676773 solarium-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 13:00:50.680773 solarium-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2021-12-05 13:00:26.000000 solarium-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-12-05 13:00:26.000000 solarium-0.3.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2021-12-05 13:00:26.000000 solarium-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-05 13:00:26.000000 solarium-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-05 13:00:26.000000 solarium-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-12-05 13:00:50.680773 solarium-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-12-05 13:00:26.000000 solarium-0.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-12-05 13:00:50.680773 solarium-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       80 2021-12-05 13:00:26.000000 solarium-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 13:00:50.680773 solarium-0.3.3/solarium/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-05 13:00:26.000000 solarium-0.3.3/solarium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-12-05 13:00:26.000000 solarium-0.3.3/solarium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2021-12-05 13:00:26.000000 solarium-0.3.3/solarium/led.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-12-05 13:00:26.000000 solarium-0.3.3/solarium/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-12-05 13:00:26.000000 solarium-0.3.3/solarium/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-05 13:00:50.680773 solarium-0.3.3/solarium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-05 13:00:50.000000 solarium-0.3.3/solarium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:39:14.496834 solarium-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 15:38:55.000000 solarium-0.4.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-19 15:38:55.000000 solarium-0.4.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 15:38:55.000000 solarium-0.4.0/.fussyfox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:39:14.492834 solarium-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:39:14.492834 solarium-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 15:38:55.000000 solarium-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-19 15:38:55.000000 solarium-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 15:38:55.000000 solarium-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 15:38:55.000000 solarium-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 15:38:55.000000 solarium-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-19 15:39:14.496834 solarium-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-19 15:38:55.000000 solarium-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-19 15:39:14.496834 solarium-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-19 15:38:55.000000 solarium-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:39:14.496834 solarium-0.4.0/solarium/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 15:38:55.000000 solarium-0.4.0/solarium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-19 15:38:55.000000 solarium-0.4.0/solarium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-19 15:38:55.000000 solarium-0.4.0/solarium/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-19 15:38:55.000000 solarium-0.4.0/solarium/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-19 15:38:55.000000 solarium-0.4.0/solarium/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:39:14.496834 solarium-0.4.0/solarium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 15:39:14.000000 solarium-0.4.0/solarium.egg-info/top_level.txt
```

### Comparing `solarium-0.3.3/.github/workflows/ci.yml` & `solarium-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/.github/workflows/release.yml` & `solarium-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/.gitignore` & `solarium-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/LICENSE` & `solarium-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/PKG-INFO` & `solarium-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: solarium
-Version: 0.3.3
+Version: 0.4.0
 Summary: RaspberryPi based LED controller for artificial sunlight
 Home-page: https://github.com/codingjoe/solarium
 Author: Johannes Maron
 Author-email: info@johanneshoppe.com
 License: MIT
 Keywords: led,raspberrypi
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: pysolar
+Requires-Dist: gpiozero
+Requires-Dist: pigpio
 
 solarium
 ===============================================================================
 
 **RaspberryPi based LED controller for artificial sunlight.**
 
 Setup
@@ -78,9 +81,7 @@
 
 .. _ffplay: https://ffmpeg.org/ffplay.html
 
 Should you be using an Inter-IC Sound (I2S) board, make sure to run pigpiod's clock
 in PMW mode, to ensure PCM is available for audio::
 
     sudo pygpiod -t 0
-
-
```

### Comparing `solarium-0.3.3/README.rst` & `solarium-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/setup.cfg` & `solarium-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/solarium/__main__.py` & `solarium-0.4.0/solarium/__main__.py`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/solarium/led.py` & `solarium-0.4.0/solarium/led.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,22 +33,24 @@
         while transition > i:
             self.value = max(min(1, self.value + increments), 0)
             await asyncio.sleep(interval)
             i += interval
 
 
 class PowerToggleMixin:
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, power_led=None, **kwargs):
         super().__init__(*args, **kwargs)
         self.power = 1
+        self.power_led = power_led
         self.callbacks = []
 
     def toggle(self):
         logger.info("Toggle: %i -> %i", self.power, not self.power)
         self.power ^= 1
+        self.power_led.value = not self.power
         for func in self.callbacks:
             func(self)
 
     def __bool__(self):
         return bool(self.power)
 
     def __int__(self):
@@ -66,20 +68,28 @@
             await asyncio.sleep(1)
 
 
 class PowerToggle(PowerToggleMixin, gpiozero.Button):
     pass
 
 
-def init(host="localhost", warm_pin=12, cold_pin=13, power_pin=17, frequency=100):
+def init(
+    host="localhost",
+    warm_pin=12,
+    cold_pin=13,
+    power_pin=17,
+    power_led_pin=26,
+    frequency=100,
+):
     logger.debug("warm LED: %s:%d@%dHz", host, warm_pin, frequency)
     logger.debug("cold LED: %s:%d@%dHz", host, cold_pin, frequency)
     factory = PiGPIOFactory(host=host)
 
-    power_button = PowerToggle(power_pin, pin_factory=factory)
+    power_led = gpiozero.LED(power_led_pin, pin_factory=factory)
+    power_button = PowerToggle(power_pin, pin_factory=factory, power_led=power_led)
     power_button.when_pressed = lambda: power_button.toggle()
     warm = PWMLED(warm_pin, name="warm", power_state=power_button, pin_factory=factory)
     cold = PWMLED(cold_pin, name="cold", power_state=power_button, pin_factory=factory)
     warm.frequency = frequency
     cold.frequency = frequency
 
     return warm, cold, power_button
```

### Comparing `solarium-0.3.3/solarium/player.py` & `solarium-0.4.0/solarium/player.py`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/solarium/utils.py` & `solarium-0.4.0/solarium/utils.py`

 * *Files identical despite different names*

### Comparing `solarium-0.3.3/solarium.egg-info/PKG-INFO` & `solarium-0.4.0/solarium.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: solarium
-Version: 0.3.3
+Version: 0.4.0
 Summary: RaspberryPi based LED controller for artificial sunlight
 Home-page: https://github.com/codingjoe/solarium
 Author: Johannes Maron
 Author-email: info@johanneshoppe.com
 License: MIT
 Keywords: led,raspberrypi
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: pysolar
+Requires-Dist: gpiozero
+Requires-Dist: pigpio
 
 solarium
 ===============================================================================
 
 **RaspberryPi based LED controller for artificial sunlight.**
 
 Setup
@@ -78,9 +81,7 @@
 
 .. _ffplay: https://ffmpeg.org/ffplay.html
 
 Should you be using an Inter-IC Sound (I2S) board, make sure to run pigpiod's clock
 in PMW mode, to ensure PCM is available for audio::
 
     sudo pygpiod -t 0
-
-
```

