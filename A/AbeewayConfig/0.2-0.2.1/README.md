# Comparing `tmp/abeewayconfig-0.2.tar.gz` & `tmp/abeewayconfig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.tar", last modified: Thu May 16 14:02:40 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.1.tar", last modified: Sun May 19 01:51:44 2024, max compression
```

## Comparing `abeewayconfig-0.2.tar` & `abeewayconfig-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-16 14:02:40.787947 abeewayconfig-0.2/
--rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2/LICENSE
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1305 2024-05-16 14:02:40.787947 abeewayconfig-0.2/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      962 2024-05-15 19:16:13.000000 abeewayconfig-0.2/README.md
--rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-16 14:02:40.787947 abeewayconfig-0.2/setup.cfg
--rw-r--r--   0 lucas     (1001) lucas     (1001)      737 2024-05-16 14:01:17.000000 abeewayconfig-0.2/setup.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-16 14:02:40.781281 abeewayconfig-0.2/src/
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-16 14:02:40.784614 abeewayconfig-0.2/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1898 2024-05-16 13:41:49.000000 abeewayconfig-0.2/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2259 2024-05-16 13:41:49.000000 abeewayconfig-0.2/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4786 2024-05-16 13:59:40.000000 abeewayconfig-0.2/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-16 14:02:40.787947 abeewayconfig-0.2/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1305 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      434 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        9 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-16 14:02:40.000000 abeewayconfig-0.2/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)    35149 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/LICENSE
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1414 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1051 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/README.md
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/setup.cfg
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      753 2024-05-19 01:51:22.000000 abeewayconfig-0.2.1/setup.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.689399 abeewayconfig-0.2.1/src/
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.689399 abeewayconfig-0.2.1/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1881 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2259 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       32 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4769 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     4026 2024-05-19 01:48:12.000000 abeewayconfig-0.2.1/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-19 01:51:44.692732 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     1414 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) lucas     (1000)      434 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       67 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       12 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)       14 2024-05-19 01:51:44.000000 abeewayconfig-0.2.1/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2/LICENSE` & `abeewayconfig-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2/PKG-INFO` & `abeewayconfig-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1
-Name: AbeewayConfig
-Version: 0.2
-Summary: Abeeway configuration tool
-Home-page: https://github.com/jlabbude/AbeewayConfig
-Author: João Lucas
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyserial
-
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
 
+## Installation
+
+To install I recommend you use the package installer for Python - **pip**
+
+```bash
+  pip install abeewayconfig
+```
+
+Run the package using
+
+```bash
+  abeewayconfig
+```
+
 ## Compatibility
 
 ### Operating Systems
 - Linux
   - Arch
 - Windows
   - W11
@@ -31,14 +33,12 @@
 
 ### Firmware Version
 - 2.4.1
 
 ## Known issues
 - GUI doesn't stall user action when talking to devices properly, making it able to break communication with serial ports by forcing multiple calls to same serial port
   - (as far as I've looked, this doesn't kill the already established communication)
-- Line break (\n) characters are not being rendered properly at integrated terminal
-- For some 
 
 ## Future goals
 - [ ] Support for multiple firmware versions
 - [ ] Support for different types of devices
 - [ ] Support for flashing the firmware of these devices
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `abeewayconfig-0.2/setup.py` & `abeewayconfig-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2",
+    version="0.2.1",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
+        "tk",
     ],
     entry_points={
         "console_scripts": [
             "abeewayconfig = AbeewayConfig.abeewayconfig:main",
         ],
     },
     classifiers=[
```

### Comparing `abeewayconfig-0.2/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.1/src/AbeewayConfig/Config.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         match = p.search(line)
         if match:
             return int(match.group(1))
 
     def check_config_discrepancy(serial_port: str, br: int, console_output: Text) -> bool:
         device_config = Device.config_show_at_device(serial_port=serial_port, br=br)
         deveui = str(Device.get_deveui(serial_port=serial_port, br=br))
-        config_file = os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)), "config"), "config.cfg")
+        config_file = os.path.join(os.path.join(os.path.dirname(__file__), "config"), "config.cfg")
         with open(config_file, 'r') as config:
             for line in config:
                 config_parameter_cfg = Config.get_config_parameter_from_cfg(line)
                 config_value_cfg = Config.get_config_value_from_cfg(config_parameter_cfg, line)
                 config_name = config_dict.get(config_parameter_cfg)
                 if config_parameter_cfg is not None or config_value_cfg is not None:
                     config_value_dev = Device.get_config_value_from_dev(device_config, config_name)
```

### Comparing `abeewayconfig-0.2/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.1/src/AbeewayConfig/Device.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-0.2.1/src/AbeewayConfig/abeewayconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 def import_config(console_output):
     filename = filedialog.askopenfilename(initialdir=initialdir,
                                           filetypes=[("Text files", "*.txt"),
                                                      ("Config files", "*.cfg")])
     if filename:
-        destination_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "config")
+        destination_dir = os.path.join(os.path.dirname(__file__), "config")
         os.makedirs(destination_dir, exist_ok=True)
         destination_file = os.path.join(destination_dir, "config.cfg")
         try:
             shutil.copy(filename, destination_file)
             console_output.insert(tk.END, "Config file imported successfully.\n")
         except Exception as e:
             console_output.insert(tk.END, "Error:" + str(e) + "\n")
```

### Comparing `abeewayconfig-0.2/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.1/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2
+Version: 0.2.1
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
+Requires-Dist: tk
 
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
 
+## Installation
+
+To install I recommend you use the package installer for Python - **pip**
+
+```bash
+  pip install abeewayconfig
+```
+
+Run the package using
+
+```bash
+  abeewayconfig
+```
+
 ## Compatibility
 
 ### Operating Systems
 - Linux
   - Arch
 - Windows
   - W11
@@ -31,14 +46,12 @@
 
 ### Firmware Version
 - 2.4.1
 
 ## Known issues
 - GUI doesn't stall user action when talking to devices properly, making it able to break communication with serial ports by forcing multiple calls to same serial port
   - (as far as I've looked, this doesn't kill the already established communication)
-- Line break (\n) characters are not being rendered properly at integrated terminal
-- For some 
 
 ## Future goals
 - [ ] Support for multiple firmware versions
 - [ ] Support for different types of devices
 - [ ] Support for flashing the firmware of these devices
```

