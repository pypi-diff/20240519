# Comparing `tmp/pcmpdkyffzevgmdz-1.10000.10001.tar.gz` & `tmp/pcmpdkyffzevgmdz-1.10000.10002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun May 19 20:52:45 2024, max compression
+gzip compressed data, last modified: Sun May 19 20:53:20 2024, max compression
```

## Comparing `pcmpdkyffzevgmdz-1.10000.10001.tar` & `pcmpdkyffzevgmdz-1.10000.10002.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz/
-drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz.egg-info/
--rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/PKG-INFO
--rwxrwxrwx   0        0        0       38 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/setup.cfg
--rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz.egg-info/PKG-INFO
--rwxrwxrwx   0        0        0        1 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz.egg-info/dependency_links.txt
--rwxrwxrwx   0        0        0       17 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz.egg-info/top_level.txt
--rwxrwxrwx   0        0        0      262 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz.egg-info/SOURCES.txt
--rwxrwxrwx   0        0        0      245 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/setup.py
--rwxrwxrwx   0        0        0      101 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz/__init__.py
--rwxrwxrwx   0        0        0      379 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz/main.py
--rwxrwxrwx   0        0        0 95015176 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz/main_func_linux_x86.so
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz/
+drwxrwxrwx   0        0        0        0 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz.egg-info/
+-rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/PKG-INFO
+-rwxrwxrwx   0        0        0       38 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/setup.cfg
+-rwxrwxrwx   0        0        0      166 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz.egg-info/PKG-INFO
+-rwxrwxrwx   0        0        0        1 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz.egg-info/dependency_links.txt
+-rwxrwxrwx   0        0        0       17 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0      262 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz.egg-info/SOURCES.txt
+-rwxrwxrwx   0        0        0      245 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/setup.py
+-rwxrwxrwx   0        0        0      101 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz/__init__.py
+-rwxrwxrwx   0        0        0      379 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz/main.py
+-rwxrwxrwx   0        0        0 95015176 1970-01-01 00:00:00.000000 pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz/main_func_linux_x86.so
```

### Comparing `pcmpdkyffzevgmdz-1.10000.10001/pcmpdkyffzevgmdz/main_func_linux_x86.so` & `pcmpdkyffzevgmdz-1.10000.10002/pcmpdkyffzevgmdz/main_func_linux_x86.so`

 * *Files identical despite different names*

