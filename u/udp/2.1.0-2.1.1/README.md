# Comparing `tmp/udp-2.1.0.tar.gz` & `tmp/udp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udp-2.1.0.tar", last modified: Fri May 17 17:29:27 2024, max compression
+gzip compressed data, was "dist/udp-2.1.1.tar", last modified: Sun May 19 17:26:02 2024, max compression
```

## Comparing `udp-2.1.0.tar` & `udp-2.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-17 17:29:27.000000 udp-2.1.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-2.1.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:29:27.000000 udp-2.1.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      835 2024-05-17 10:41:38.000000 udp-2.1.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/
--rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-2.1.0/udp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5490 2024-05-17 11:58:03.000000 udp-2.1.0/udp/aio.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/ba/
--rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-2.1.0/udp/ba/array.py
--rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/convert.py
--rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-2.1.0/udp/ba/data.py
--rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-2.1.0/udp/ba/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/integer.py
--rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/mutable.py
--rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-2.1.0/udp/ba/utils.py
--rw-r--r--   0 moky       (501) staff       (20)    12515 2024-05-17 11:57:45.000000 udp-2.1.0/udp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     8271 2024-05-17 11:15:19.000000 udp-2.1.0/udp/hub.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/mtp/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-2.1.0/udp/mtp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/header.py
--rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/package.py
--rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-2.1.0/udp/mtp/protocol.py
--rw-r--r--   0 moky       (501) staff       (20)    11702 2024-05-07 15:14:23.000000 udp-2.1.0/udp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      453 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:02.000000 udp-2.1.1/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-19 17:26:02.000000 udp-2.1.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-2.1.1/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-19 17:26:02.000000 udp-2.1.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      835 2024-05-18 18:05:46.000000 udp-2.1.1/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:02.000000 udp-2.1.1/udp/
+-rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-2.1.1/udp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5490 2024-05-17 11:58:03.000000 udp-2.1.1/udp/aio.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:02.000000 udp-2.1.1/udp/ba/
+-rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-2.1.1/udp/ba/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-2.1.1/udp/ba/array.py
+-rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-2.1.1/udp/ba/convert.py
+-rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-2.1.1/udp/ba/data.py
+-rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-2.1.1/udp/ba/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-2.1.1/udp/ba/integer.py
+-rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-2.1.1/udp/ba/mutable.py
+-rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-2.1.1/udp/ba/utils.py
+-rw-r--r--   0 moky       (501) staff       (20)    12515 2024-05-17 11:57:45.000000 udp-2.1.1/udp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     8259 2024-05-18 18:06:16.000000 udp-2.1.1/udp/hub.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:02.000000 udp-2.1.1/udp/mtp/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-2.1.1/udp/mtp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-2.1.1/udp/mtp/header.py
+-rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-2.1.1/udp/mtp/package.py
+-rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-2.1.1/udp/mtp/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-2.1.1/udp/mtp/protocol.py
+-rw-r--r--   0 moky       (501) staff       (20)    11702 2024-05-07 15:14:23.000000 udp-2.1.1/udp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      453 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-19 17:26:02.000000 udp-2.1.1/udp.egg-info/top_level.txt
```

### Comparing `udp-2.1.0/setup.py` & `udp-2.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     User Datagram Protocol
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
@@ -30,10 +30,10 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'startrek>=2.1.0'
+        'startrek>=2.1.1'
     ]
 )
```

### Comparing `udp-2.1.0/udp/__init__.py` & `udp-2.1.1/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/aio.py` & `udp-2.1.1/udp/aio.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/__init__.py` & `udp-2.1.1/udp/ba/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/array.py` & `udp-2.1.1/udp/ba/array.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/convert.py` & `udp-2.1.1/udp/ba/convert.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/data.py` & `udp-2.1.1/udp/ba/data.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/helper.py` & `udp-2.1.1/udp/ba/helper.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/integer.py` & `udp-2.1.1/udp/ba/integer.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/mutable.py` & `udp-2.1.1/udp/ba/mutable.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/ba/utils.py` & `udp-2.1.1/udp/ba/utils.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/channel.py` & `udp-2.1.1/udp/channel.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/hub.py` & `udp-2.1.1/udp/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,28 +87,28 @@
 
     # Override
     def set(self, item: Optional[Channel],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
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
     def remove(self, item: Optional[Channel],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            Runner.async_run(coroutine=cached.close())
+            Runner.async_task(coro=cached.close())
         if item is not None:
-            Runner.async_run(coroutine=item.close())
+            Runner.async_task(coro=item.close())
         return cached
 
 
 # noinspection PyAbstractClass
 class PacketHub(BaseHub, ABC):
     """ Base Datagram Hub """
```

### Comparing `udp-2.1.0/udp/mtp/__init__.py` & `udp-2.1.1/udp/mtp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/mtp/header.py` & `udp-2.1.1/udp/mtp/header.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/mtp/package.py` & `udp-2.1.1/udp/mtp/package.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/mtp/packer.py` & `udp-2.1.1/udp/mtp/packer.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/mtp/protocol.py` & `udp-2.1.1/udp/mtp/protocol.py`

 * *Files identical despite different names*

### Comparing `udp-2.1.0/udp/startrek.py` & `udp-2.1.1/udp/startrek.py`

 * *Files identical despite different names*

