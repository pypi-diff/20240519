# Comparing `tmp/lishixian-0.3.4.tar.gz` & `tmp/lishixian-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lishixian-0.3.4.tar", last modified: Sat Apr  6 01:42:46 2024, max compression
+gzip compressed data, was "dist\lishixian-0.3.5.tar", last modified: Sun May 19 12:16:16 2024, max compression
```

## Comparing `lishixian-0.3.4.tar` & `lishixian-0.3.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:46.000000 lishixian-0.3.4/
--rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lishixian-0.3.4/.gitignore
--rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lishixian-0.3.4/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:46.000000 lishixian-0.3.4/lishixian/
--rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lishixian-0.3.4/lishixian/auto.py
--rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/c.py
--rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/cls.py
--rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/dec.py
--rw-rw-rw-   0        0        0     9816 2024-04-06 01:18:56.000000 lishixian-0.3.4/lishixian/doc.py
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:46.000000 lishixian-0.3.4/lishixian/docs/
--rw-rw-rw-   0        0        0     1125 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian/docs/LICENSE.txt
--rw-rw-rw-   0        0        0     5286 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian/docs/README.md
--rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/docs/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/gui.py
--rw-rw-rw-   0        0        0     2836 2024-04-06 00:49:11.000000 lishixian-0.3.4/lishixian/line.py
--rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lishixian-0.3.4/lishixian/new.py
--rw-rw-rw-   0        0        0      962 2024-04-06 00:54:55.000000 lishixian-0.3.4/lishixian/np.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/reg.py
--rw-rw-rw-   0        0        0     8725 2024-04-06 00:48:00.000000 lishixian-0.3.4/lishixian/util.py
--rw-rw-rw-   0        0        0       21 2024-04-06 01:35:33.000000 lishixian-0.3.4/lishixian/version.py
--rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lishixian-0.3.4/lishixian/windll.py
--rw-rw-rw-   0        0        0     2608 2024-04-06 00:48:00.000000 lishixian-0.3.4/lishixian/__init__.py
--rw-rw-rw-   0        0        0     2040 2024-04-06 01:25:11.000000 lishixian-0.3.4/lishixian/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 01:42:46.000000 lishixian-0.3.4/lishixian.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     7663 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-04-06 01:42:45.000000 lishixian-0.3.4/lishixian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lishixian-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7663 2024-04-06 01:42:46.000000 lishixian-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     5286 2024-04-06 01:37:56.000000 lishixian-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 01:42:46.000000 lishixian-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lishixian-0.3.4/setup.py
--rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lishixian-0.3.4/__right_menu.reg
--rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lishixian-0.3.4/__test_dist.bat
--rwxrwxrwx   0        0        0      556 2024-04-06 00:57:30.000000 lishixian-0.3.4/__test_install_all.bat
--rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lishixian-0.3.4/__test_upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:16.000000 lishixian-0.3.5/
+-rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lishixian-0.3.5/.gitignore
+-rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lishixian-0.3.5/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:16.000000 lishixian-0.3.5/lishixian/
+-rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lishixian-0.3.5/lishixian/auto.py
+-rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/c.py
+-rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/cls.py
+-rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/dec.py
+-rw-rw-rw-   0        0        0     9816 2024-04-06 01:18:56.000000 lishixian-0.3.5/lishixian/doc.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:16.000000 lishixian-0.3.5/lishixian/docs/
+-rw-rw-rw-   0        0        0     1125 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian/docs/LICENSE.txt
+-rw-rw-rw-   0        0        0     5306 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian/docs/README.md
+-rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/docs/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/gui.py
+-rw-rw-rw-   0        0        0     2836 2024-04-06 00:49:11.000000 lishixian-0.3.5/lishixian/line.py
+-rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lishixian-0.3.5/lishixian/new.py
+-rw-rw-rw-   0        0        0      962 2024-04-06 00:54:55.000000 lishixian-0.3.5/lishixian/np.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/reg.py
+-rw-rw-rw-   0        0        0     8725 2024-04-06 00:48:00.000000 lishixian-0.3.5/lishixian/util.py
+-rw-rw-rw-   0        0        0       21 2024-05-19 09:18:59.000000 lishixian-0.3.5/lishixian/version.py
+-rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lishixian-0.3.5/lishixian/windll.py
+-rw-rw-rw-   0        0        0     2608 2024-04-06 00:48:00.000000 lishixian-0.3.5/lishixian/__init__.py
+-rw-rw-rw-   0        0        0     2456 2024-05-16 07:33:52.000000 lishixian-0.3.5/lishixian/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:16:16.000000 lishixian-0.3.5/lishixian.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     7683 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 12:16:15.000000 lishixian-0.3.5/lishixian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lishixian-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7683 2024-05-19 12:16:16.000000 lishixian-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5306 2024-05-19 09:14:45.000000 lishixian-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:16:16.000000 lishixian-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lishixian-0.3.5/setup.py
+-rwxrwxrwx   0        0        0       91 2024-04-14 09:50:44.000000 lishixian-0.3.5/__pip_config.bat
+-rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lishixian-0.3.5/__right_menu.reg
+-rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lishixian-0.3.5/__test_dist.bat
+-rwxrwxrwx   0        0        0      556 2024-04-06 00:57:30.000000 lishixian-0.3.5/__test_install_all.bat
+-rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lishixian-0.3.5/__test_upload_pypi.bat
```

### Comparing `lishixian-0.3.4/LICENSE.txt` & `lishixian-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/auto.py` & `lishixian-0.3.5/lishixian/auto.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/c.py` & `lishixian-0.3.5/lishixian/c.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/cls.py` & `lishixian-0.3.5/lishixian/cls.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/dec.py` & `lishixian-0.3.5/lishixian/dec.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/doc.py` & `lishixian-0.3.5/lishixian/doc.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/docs/LICENSE.txt` & `lishixian-0.3.5/lishixian/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/docs/README.md` & `lishixian-0.3.5/lishixian/docs/README.md`

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

### Comparing `lishixian-0.3.4/lishixian/gui.py` & `lishixian-0.3.5/lishixian/gui.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/line.py` & `lishixian-0.3.5/lishixian/line.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/new.py` & `lishixian-0.3.5/lishixian/new.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/np.py` & `lishixian-0.3.5/lishixian/np.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/reg.py` & `lishixian-0.3.5/lishixian/reg.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/util.py` & `lishixian-0.3.5/lishixian/util.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/windll.py` & `lishixian-0.3.5/lishixian/windll.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/__init__.py` & `lishixian-0.3.5/lishixian/__init__.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/lishixian/__main__.py` & `lishixian-0.3.5/lishixian/__main__.py`

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

### Comparing `lishixian-0.3.4/lishixian.egg-info/PKG-INFO` & `lishixian-0.3.5/lishixian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lishixian
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

### Comparing `lishixian-0.3.4/lishixian.egg-info/SOURCES.txt` & `lishixian-0.3.5/lishixian.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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
 lishixian/__init__.py
 lishixian/__main__.py
```

### Comparing `lishixian-0.3.4/PKG-INFO` & `lishixian-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lishixian
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

### Comparing `lishixian-0.3.4/README.md` & `lishixian-0.3.5/README.md`

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

### Comparing `lishixian-0.3.4/setup.py` & `lishixian-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `lishixian-0.3.4/__test_install_all.bat` & `lishixian-0.3.5/__test_install_all.bat`

 * *Files identical despite different names*

