# Comparing `tmp/lsx-0.3.4.tar.gz` & `tmp/lsx-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lsx-0.3.4.tar", last modified: Sat Apr  6 01:42:48 2024, max compression
+gzip compressed data, was "dist\lsx-0.3.5.tar", last modified: Sun May 19 12:16:21 2024, max compression
```

## Comparing `lsx-0.3.4.tar` & `lsx-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/
--rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lsx-0.3.4/.gitignore
--rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lsx-0.3.4/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/
--rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lsx-0.3.4/lsx/auto.py
--rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/c.py
--rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/cls.py
--rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/dec.py
--rw-rw-rw-   0        0        0     9816 2024-04-06 01:18:56.000000 lsx-0.3.4/lsx/doc.py
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/
--rw-rw-rw-   0        0        0     1125 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/LICENSE.txt
--rw-rw-rw-   0        0        0     5286 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/README.md
--rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/docs/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/gui.py
--rw-rw-rw-   0        0        0     2836 2024-04-06 00:49:11.000000 lsx-0.3.4/lsx/line.py
--rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lsx-0.3.4/lsx/new.py
--rw-rw-rw-   0        0        0      962 2024-04-06 00:54:55.000000 lsx-0.3.4/lsx/np.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/reg.py
--rw-rw-rw-   0        0        0     8725 2024-04-06 00:48:00.000000 lsx-0.3.4/lsx/util.py
--rw-rw-rw-   0        0        0       21 2024-04-06 01:35:33.000000 lsx-0.3.4/lsx/version.py
--rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/windll.py
--rw-rw-rw-   0        0        0     2608 2024-04-06 00:48:00.000000 lsx-0.3.4/lsx/__init__.py
--rw-rw-rw-   0        0        0     2040 2024-04-06 01:25:11.000000 lsx-0.3.4/lsx/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     7657 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lsx-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7657 2024-04-06 01:42:48.000000 lsx-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5286 2024-04-06 01:37:56.000000 lsx-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 01:42:48.000000 lsx-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lsx-0.3.4/setup.py
--rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lsx-0.3.4/__right_menu.reg
--rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lsx-0.3.4/__test_dist.bat
--rwxrwxrwx   0        0        0      556 2024-04-06 00:57:30.000000 lsx-0.3.4/__test_install_all.bat
--rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lsx-0.3.4/__test_upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:21.000000 lsx-0.3.5/
+-rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lsx-0.3.5/.gitignore
+-rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lsx-0.3.5/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx/
+-rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lsx-0.3.5/lsx/auto.py
+-rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/c.py
+-rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/cls.py
+-rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/dec.py
+-rw-rw-rw-   0        0        0     9816 2024-04-06 01:18:56.000000 lsx-0.3.5/lsx/doc.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx/docs/
+-rw-rw-rw-   0        0        0     1125 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx/docs/LICENSE.txt
+-rw-rw-rw-   0        0        0     5306 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx/docs/README.md
+-rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/docs/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/gui.py
+-rw-rw-rw-   0        0        0     2836 2024-04-06 00:49:11.000000 lsx-0.3.5/lsx/line.py
+-rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lsx-0.3.5/lsx/new.py
+-rw-rw-rw-   0        0        0      962 2024-04-06 00:54:55.000000 lsx-0.3.5/lsx/np.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/reg.py
+-rw-rw-rw-   0        0        0     8725 2024-04-06 00:48:00.000000 lsx-0.3.5/lsx/util.py
+-rw-rw-rw-   0        0        0       21 2024-05-19 09:18:59.000000 lsx-0.3.5/lsx/version.py
+-rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lsx-0.3.5/lsx/windll.py
+-rw-rw-rw-   0        0        0     2608 2024-04-06 00:48:00.000000 lsx-0.3.5/lsx/__init__.py
+-rw-rw-rw-   0        0        0     2456 2024-05-16 07:33:52.000000 lsx-0.3.5/lsx/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     7677 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        4 2024-05-19 12:16:21.000000 lsx-0.3.5/lsx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lsx-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7677 2024-05-19 12:16:21.000000 lsx-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5306 2024-05-19 09:14:45.000000 lsx-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:16:21.000000 lsx-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lsx-0.3.5/setup.py
+-rwxrwxrwx   0        0        0       91 2024-04-14 09:50:44.000000 lsx-0.3.5/__pip_config.bat
+-rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lsx-0.3.5/__right_menu.reg
+-rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lsx-0.3.5/__test_dist.bat
+-rwxrwxrwx   0        0        0      556 2024-04-06 00:57:30.000000 lsx-0.3.5/__test_install_all.bat
+-rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lsx-0.3.5/__test_upload_pypi.bat
```

### Comparing `lsx-0.3.4/LICENSE.txt` & `lsx-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/auto.py` & `lsx-0.3.5/lsx/auto.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/c.py` & `lsx-0.3.5/lsx/c.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/cls.py` & `lsx-0.3.5/lsx/cls.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/dec.py` & `lsx-0.3.5/lsx/dec.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/doc.py` & `lsx-0.3.5/lsx/doc.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/docs/LICENSE.txt` & `lsx-0.3.5/lsx/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/docs/README.md` & `lsx-0.3.5/lsx/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 Install on Github:
 
 ```bash
 git clone https://github.com/znsoooo/lishixian
 cd lishixian
-pip install -e .
+pip install .
 ```
 
 
 ## Usage
 
 Use it in Python script:
 
@@ -38,15 +38,15 @@
 lsx.help()
 ```
 
 The package can also be used in console, it takes one or zero parameter:
 
 ```bash
 $ lishixian help
-Commands: help version ip mac user crc md5 inv create delete detect half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote
+Commands: help version ip mac user crc md5 inv create delete detect hex2bin bin2hex half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote / \ \\
 
 $ lishixian float2hex 1.0
 3f800000
 ```
 
 ## Modules
```

### Comparing `lsx-0.3.4/lsx/gui.py` & `lsx-0.3.5/lsx/gui.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/line.py` & `lsx-0.3.5/lsx/line.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/new.py` & `lsx-0.3.5/lsx/new.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/np.py` & `lsx-0.3.5/lsx/np.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/reg.py` & `lsx-0.3.5/lsx/reg.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/util.py` & `lsx-0.3.5/lsx/util.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/windll.py` & `lsx-0.3.5/lsx/windll.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/__init__.py` & `lsx-0.3.5/lsx/__init__.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/lsx/__main__.py` & `lsx-0.3.5/lsx/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,29 +22,39 @@
     crc = lambda p: '0x%04X' % pkg('binascii').crc_hqx(open(p, 'rb').read(), 0)
     md5 = lambda p: pkg('hashlib').md5(open(p, 'rb').read()).hexdigest()
     inv = lambda p: open(p + '.inv', 'wb').write(bytes(255 - b for b in open(p, 'rb').read()))
     create = lambda p: os.path.dirname(p) and os.makedirs(os.path.dirname(p), exist_ok=True) or os.path.basename(p) and open(p, 'ab').close()
     delete = lambda p: os.remove(p) if os.path.isfile(p) else pkg('shutil').rmtree(p) if os.path.isdir(p) else None
     detect = lambda p: pkg('chardet').detect(open(p, 'rb').read())['encoding'] or 'utf-8'
 
+    hex2bin = lambda hex: bin(int(hex, 16))[2:].zfill(len(hex) * 4)
+    bin2hex = lambda bin: hex(int(bin, 2))[2:].zfill(len(bin) // 4)
     half2hex = lambda num: pkg('struct').pack('>e', float(num)).hex()
     hex2half = lambda hex: pkg('struct').unpack('>e', bytes.fromhex(hex))[0]
     float2hex = lambda num: pkg('struct').pack('>f', float(num)).hex()
     hex2float = lambda hex: pkg('struct').unpack('>f', bytes.fromhex(hex))[0]
     double2hex = lambda num: pkg('struct').pack('>d', float(num)).hex()
     hex2double = lambda hex: pkg('struct').unpack('>d', bytes.fromhex(hex))[0]
 
     escape = html.escape
     unescape = html.unescape
     quote = urllib.parse.quote_plus
     unquote = urllib.parse.unquote
 
-    funcs = [k for k, v in vars().copy().items() if inspect.isfunction(v)]
+    funcs = {k: v for k, v in vars().copy().items() if inspect.isfunction(v)}
 
-    if len(sys.argv) == 1:
-        sys.argv.append('help')
-    name, *args = sys.argv[1:]
-    print(vars()[name](*args) or '')
+    funcs['/']    = lambda s: pkg('re').sub(r'[\\/]+', r'/', s)
+    funcs['\\']   = lambda s: pkg('re').sub(r'[\\/]+', r'\\', s)
+    funcs['\\\\'] = lambda s: pkg('re').sub(r'[\\/]+', r'\\\\', s)
+
+    func = funcs[sys.argv[1]] if len(sys.argv) > 1 else help
+    args = sys.argv[2:]
+
+    if args:
+        for arg in args:
+            print(func(arg) or '')
+    else:
+        print(func() or '')
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `lsx-0.3.4/lsx.egg-info/PKG-INFO` & `lsx-0.3.5/lsx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsx
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Shixian Li (znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Description: # Lite Software eXtension
@@ -30,15 +30,15 @@
         ```
         
         Install on Github:
         
         ```bash
         git clone https://github.com/znsoooo/lishixian
         cd lishixian
-        pip install -e .
+        pip install .
         ```
         
         
         ## Usage
         
         Use it in Python script:
         
@@ -47,15 +47,15 @@
         lsx.help()
         ```
         
         The package can also be used in console, it takes one or zero parameter:
         
         ```bash
         $ lishixian help
-        Commands: help version ip mac user crc md5 inv create delete detect half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote
+        Commands: help version ip mac user crc md5 inv create delete detect hex2bin bin2hex half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote / \ \\
         
         $ lishixian float2hex 1.0
         3f800000
         ```
         
         ## Modules
```

### Comparing `lsx-0.3.4/lsx.egg-info/SOURCES.txt` & `lsx-0.3.5/lsx.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
+__pip_config.bat
 __right_menu.reg
 __test_dist.bat
 __test_install_all.bat
 __test_upload_pypi.bat
 setup.py
 lsx/__init__.py
 lsx/__main__.py
```

### Comparing `lsx-0.3.4/PKG-INFO` & `lsx-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsx
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Shixian Li (znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Description: # Lite Software eXtension
@@ -30,15 +30,15 @@
         ```
         
         Install on Github:
         
         ```bash
         git clone https://github.com/znsoooo/lishixian
         cd lishixian
-        pip install -e .
+        pip install .
         ```
         
         
         ## Usage
         
         Use it in Python script:
         
@@ -47,15 +47,15 @@
         lsx.help()
         ```
         
         The package can also be used in console, it takes one or zero parameter:
         
         ```bash
         $ lishixian help
-        Commands: help version ip mac user crc md5 inv create delete detect half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote
+        Commands: help version ip mac user crc md5 inv create delete detect hex2bin bin2hex half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote / \ \\
         
         $ lishixian float2hex 1.0
         3f800000
         ```
         
         ## Modules
```

### Comparing `lsx-0.3.4/README.md` & `lsx-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 Install on Github:
 
 ```bash
 git clone https://github.com/znsoooo/lishixian
 cd lishixian
-pip install -e .
+pip install .
 ```
 
 
 ## Usage
 
 Use it in Python script:
 
@@ -38,15 +38,15 @@
 lsx.help()
 ```
 
 The package can also be used in console, it takes one or zero parameter:
 
 ```bash
 $ lishixian help
-Commands: help version ip mac user crc md5 inv create delete detect half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote
+Commands: help version ip mac user crc md5 inv create delete detect hex2bin bin2hex half2hex hex2half float2hex hex2float double2hex hex2double escape unescape quote unquote / \ \\
 
 $ lishixian float2hex 1.0
 3f800000
 ```
 
 ## Modules
```

### Comparing `lsx-0.3.4/setup.py` & `lsx-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.4/__test_install_all.bat` & `lsx-0.3.5/__test_install_all.bat`

 * *Files identical despite different names*

