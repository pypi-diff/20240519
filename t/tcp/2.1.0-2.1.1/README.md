# Comparing `tmp/tcp-2.1.0.tar.gz` & `tmp/tcp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcp-2.1.0.tar", last modified: Fri May 17 17:30:07 2024, max compression
+gzip compressed data, was "dist/tcp-2.1.1.tar", last modified: Sun May 19 17:26:26 2024, max compression
```

## Comparing `tcp-2.1.0.tar` & `tcp-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-17 17:30:07.000000 tcp-2.1.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-2.1.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:30:07.000000 tcp-2.1.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      849 2024-05-17 03:47:56.000000 tcp-2.1.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp/
--rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-2.1.0/tcp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4945 2024-05-17 11:53:44.000000 tcp-2.1.0/tcp/aio.py
--rw-r--r--   0 moky       (501) staff       (20)     9327 2024-05-17 11:55:01.000000 tcp-2.1.0/tcp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10842 2024-05-17 09:40:31.000000 tcp-2.1.0/tcp/hub.py
--rw-r--r--   0 moky       (501) staff       (20)     4519 2024-05-07 14:35:33.000000 tcp-2.1.0/tcp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      221 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:26.000000 tcp-2.1.1/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-19 17:26:26.000000 tcp-2.1.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-2.1.1/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-19 17:26:26.000000 tcp-2.1.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      849 2024-05-18 18:03:22.000000 tcp-2.1.1/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:26.000000 tcp-2.1.1/tcp/
+-rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-2.1.1/tcp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4945 2024-05-17 11:53:44.000000 tcp-2.1.1/tcp/aio.py
+-rw-r--r--   0 moky       (501) staff       (20)     9327 2024-05-17 11:55:01.000000 tcp-2.1.1/tcp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10830 2024-05-18 18:04:04.000000 tcp-2.1.1/tcp/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4519 2024-05-07 14:35:33.000000 tcp-2.1.1/tcp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-19 17:26:26.000000 tcp-2.1.1/tcp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-19 17:26:25.000000 tcp-2.1.1/tcp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      221 2024-05-19 17:26:26.000000 tcp-2.1.1/tcp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-19 17:26:25.000000 tcp-2.1.1/tcp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-19 17:26:25.000000 tcp-2.1.1/tcp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-19 17:26:25.000000 tcp-2.1.1/tcp.egg-info/top_level.txt
```

### Comparing `tcp-2.1.0/setup.py` & `tcp-2.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     Transmission Control Protocol
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

### Comparing `tcp-2.1.0/tcp/__init__.py` & `tcp-2.1.1/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `tcp-2.1.0/tcp/aio.py` & `tcp-2.1.1/tcp/aio.py`

 * *Files identical despite different names*

### Comparing `tcp-2.1.0/tcp/channel.py` & `tcp-2.1.1/tcp/channel.py`

 * *Files identical despite different names*

### Comparing `tcp-2.1.0/tcp/hub.py` & `tcp-2.1.1/tcp/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 
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
 class StreamHub(BaseHub, ABC):
     """ Base Stream Hub """
```

### Comparing `tcp-2.1.0/tcp/startrek.py` & `tcp-2.1.1/tcp/startrek.py`

 * *Files identical despite different names*

