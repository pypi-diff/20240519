# Comparing `tmp/coti_sdk-0.1.4.tar.gz` & `tmp/coti_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coti_sdk-0.1.4.tar", last modified: Sun May 19 17:33:03 2024, max compression
+gzip compressed data, was "coti_sdk-0.1.6.tar", last modified: Sun May 19 17:57:59 2024, max compression
```

## Comparing `coti_sdk-0.1.4.tar` & `coti_sdk-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:33:03.592741 coti_sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 17:33:03.592741 coti_sdk-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:33:03.588741 coti_sdk-0.1.4/coti_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:32:59.000000 coti_sdk-0.1.4/coti_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-19 17:32:59.000000 coti_sdk-0.1.4/coti_sdk/crypto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-19 17:32:59.000000 coti_sdk-0.1.4/coti_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:33:03.592741 coti_sdk-0.1.4/coti_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 17:33:03.000000 coti_sdk-0.1.4/coti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 17:33:03.000000 coti_sdk-0.1.4/coti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:33:03.000000 coti_sdk-0.1.4/coti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 17:33:03.000000 coti_sdk-0.1.4/coti_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 17:33:03.000000 coti_sdk-0.1.4/coti_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:33:03.592741 coti_sdk-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 17:32:59.000000 coti_sdk-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:57:59.810902 coti_sdk-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 17:57:59.810902 coti_sdk-0.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:57:59.810902 coti_sdk-0.1.6/coti/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:57:57.000000 coti_sdk-0.1.6/coti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-19 17:57:57.000000 coti_sdk-0.1.6/coti/crypto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-19 17:57:57.000000 coti_sdk-0.1.6/coti/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:57:59.810902 coti_sdk-0.1.6/coti_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-19 17:57:59.000000 coti_sdk-0.1.6/coti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-19 17:57:59.000000 coti_sdk-0.1.6/coti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:57:59.000000 coti_sdk-0.1.6/coti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 17:57:59.000000 coti_sdk-0.1.6/coti_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 17:57:59.000000 coti_sdk-0.1.6/coti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:57:59.810902 coti_sdk-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 17:57:57.000000 coti_sdk-0.1.6/setup.py
```

### Comparing `coti_sdk-0.1.4/coti_sdk/crypto_utils.py` & `coti_sdk-0.1.6/coti/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `coti_sdk-0.1.4/coti_sdk/utils.py` & `coti_sdk-0.1.6/coti/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from eth_account import Account
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 
-from crypto_utils import block_size, decrypt
+from coti.crypto_utils import block_size, decrypt
 
 SOLC_VERSION = '0.8.19'
 
 
 def web3_connected(web3):
     return web3.is_connected()
```

### Comparing `coti_sdk-0.1.4/setup.py` & `coti_sdk-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+
 from setuptools import setup
 
 setup(
     name='coti_sdk',
-    description='COTI SDK for Confidential Preserving network',
-    version='0.1.4',
+    description='COTI SDK for Privacy Preserving Network',
+    version='0.1.6',
     license='Apache2.0',
     author="gmesika-coti@COTI",
     author_email='support@coti.io',
     package_dir={'': '.'},
     url='https://github.com/coti-io/coti-sdk-python',
     keywords='COTI SDK Privacy',
     install_requires=[
```

