# Comparing `tmp/better_proxy-1.2.0.tar.gz` & `tmp/better_proxy-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_proxy-1.2.0.tar", max compression
+gzip compressed data, was "better_proxy-1.2.0b1.tar", max compression
```

## Comparing `better_proxy-1.2.0.tar` & `better_proxy-1.2.0b1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      101 2024-04-09 07:37:58.373466 better_proxy-1.2.0/better_proxy/__init__.py
--rw-r--r--   0        0        0     4374 2024-05-19 21:01:41.863775 better_proxy-1.2.0/better_proxy/proxy.py
--rw-r--r--   0        0        0      484 2024-05-19 21:01:58.959374 better_proxy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2587 2024-05-19 21:12:40.350796 better_proxy-1.2.0/README.md
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 better_proxy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-09 07:37:58.373466 better_proxy-1.2.0b1/better_proxy/__init__.py
+-rw-r--r--   0        0        0     3544 2024-04-09 07:36:49.254809 better_proxy-1.2.0b1/better_proxy/proxy.py
+-rw-r--r--   0        0        0      487 2024-04-09 07:38:59.657221 better_proxy-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1888 2024-02-24 09:09:36.593943 better_proxy-1.2.0b1/README.md
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 better_proxy-1.2.0b1/PKG-INFO
```

### Comparing `better_proxy-1.2.0/README.md` & `better_proxy-1.2.0b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,49 +24,21 @@
 pip install better-proxy
 ```
 
 More libraries of the family:
 - [tweepy-self](https://github.com/alenkimov/tweepy-self)
 - [better-web3](https://github.com/alenkimov/better_web3)
 
-## aiohttp
 ```python
 import aiohttp
 from better_proxy import Proxy
 from aiohttp_socks import ProxyConnector
 
-proxy = Proxy.from_str("socks5://user:password@127.0.0.1:1080")
 
 async def fetch(url):
+    proxy = Proxy.from_str('socks5://user:password@127.0.0.1:1080')
     connector = ProxyConnector.from_url(proxy.as_url)
     
     async with aiohttp.ClientSession(connector=connector) as session:
         async with session.get(url) as response:
             return await response.text()
 ```
-
-## requests
-```python
-import requests
-from better_proxy import Proxy
-
-proxy = Proxy.from_str("http://user:password@host:port")    
-
-def fetch(url):
-    response = requests.get(url, proxies=proxy.as_proxies_dict)    
-    return response.text
-```
-
-## playwright
-[Playwright: http proxy](https://playwright.dev/python/docs/network#http-proxy)
-
-```python
-from playwright.async_api import async_playwright, Playwright
-from better_proxy import Proxy
-
-proxy = Proxy.from_str("http://user:password@host:port")
-
-async def fetch(playwright: Playwright, url):
-    chromium = playwright.chromium
-    browser = await chromium.launch(proxy=proxy.as_playwright_proxy)
-    ...
-```
```

### Comparing `better_proxy-1.2.0/PKG-INFO` & `better_proxy-1.2.0b1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-proxy
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: Better proxy!
 Home-page: https://github.com/alenkimov/better_proxy
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -43,49 +43,22 @@
 pip install better-proxy
 ```
 
 More libraries of the family:
 - [tweepy-self](https://github.com/alenkimov/tweepy-self)
 - [better-web3](https://github.com/alenkimov/better_web3)
 
-## aiohttp
 ```python
 import aiohttp
 from better_proxy import Proxy
 from aiohttp_socks import ProxyConnector
 
-proxy = Proxy.from_str("socks5://user:password@127.0.0.1:1080")
 
 async def fetch(url):
+    proxy = Proxy.from_str('socks5://user:password@127.0.0.1:1080')
     connector = ProxyConnector.from_url(proxy.as_url)
     
     async with aiohttp.ClientSession(connector=connector) as session:
         async with session.get(url) as response:
             return await response.text()
 ```
 
-## requests
-```python
-import requests
-from better_proxy import Proxy
-
-proxy = Proxy.from_str("http://user:password@host:port")    
-
-def fetch(url):
-    response = requests.get(url, proxies=proxy.as_proxies_dict)    
-    return response.text
-```
-
-## playwright
-[Playwright: http proxy](https://playwright.dev/python/docs/network#http-proxy)
-
-```python
-from playwright.async_api import async_playwright, Playwright
-from better_proxy import Proxy
-
-proxy = Proxy.from_str("http://user:password@host:port")
-
-async def fetch(playwright: Playwright, url):
-    chromium = playwright.chromium
-    browser = await chromium.launch(proxy=proxy.as_playwright_proxy)
-    ...
-```
```

