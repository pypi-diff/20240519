# Comparing `tmp/ark-mainsail-1.2.0.tar.gz` & `tmp/ark-mainsail-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-mainsail-1.2.0.tar", last modified: Sat Apr 27 07:08:31 2024, max compression
+gzip compressed data, was "ark-mainsail-1.2.1.tar", last modified: Sun May 19 15:13:14 2024, max compression
```

## Comparing `ark-mainsail-1.2.0.tar` & `ark-mainsail-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.627492 ark-mainsail-1.2.0/
--rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4681 2024-04-27 07:08:31.625497 ark-mainsail-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3409 2024-04-27 06:46:21.000000 ark-mainsail-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.623507 ark-mainsail-1.2.0/ark_mainsail.egg-info/
--rw-rw-rw-   0        0        0     4681 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      616 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-27 07:08:30.000000 ark-mainsail-1.2.0/ark_mainsail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.314906 ark-mainsail-1.2.0/mainsail/
--rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.2.0/mainsail/__init__.py
--rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.2.0/mainsail/config.py
--rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.2.0/mainsail/deserializer.py
--rw-rw-rw-   0        0        0     9841 2024-04-24 20:18:46.000000 ark-mainsail-1.2.0/mainsail/identity.py
--rw-rw-rw-   0        0        0     5208 2024-04-27 05:59:41.000000 ark-mainsail-1.2.0/mainsail/rest.py
--rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.2.0/mainsail/serializer.py
--rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.2.0/mainsail/transaction.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.363258 ark-mainsail-1.2.0/mainsail/tx/
--rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.2.0/mainsail/tx/__init__.py
--rw-rw-rw-   0        0        0     7119 2024-04-25 06:54:53.000000 ark-mainsail-1.2.0/mainsail/tx/v1.py
--rw-rw-rw-   0        0        0     5052 2024-04-24 20:10:37.000000 ark-mainsail-1.2.0/mainsail/webhook.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.521772 ark-mainsail-1.2.0/mnsl_pool/
--rw-rw-rw-   0        0        0     5235 2024-04-26 07:11:22.000000 ark-mainsail-1.2.0/mnsl_pool/__init__.py
--rw-rw-rw-   0        0        0     5363 2024-04-26 07:11:10.000000 ark-mainsail-1.2.0/mnsl_pool/__main__.py
--rw-rw-rw-   0        0        0     1237 2024-04-26 07:11:15.000000 ark-mainsail-1.2.0/mnsl_pool/api.py
--rw-rw-rw-   0        0        0    12503 2024-04-27 05:24:23.000000 ark-mainsail-1.2.0/mnsl_pool/biom.py
--rw-rw-rw-   0        0        0     9468 2024-04-25 19:54:38.000000 ark-mainsail-1.2.0/mnsl_pool/tbw.py
--rw-rw-rw-   0        0        0       42 2024-04-27 07:08:31.627492 ark-mainsail-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1993 2024-04-26 17:46:53.000000 ark-mainsail-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 07:08:31.578691 ark-mainsail-1.2.0/test/
--rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.2.0/test/__init__.py
--rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.2.0/test/test_identity.py
--rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.2.0/test/test_v1_builders.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.276661 ark-mainsail-1.2.1/
+-rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4071 2024-05-19 15:13:14.274668 ark-mainsail-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2799 2024-05-19 15:11:55.000000 ark-mainsail-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.258709 ark-mainsail-1.2.1/ark_mainsail.egg-info/
+-rw-rw-rw-   0        0        0     4071 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-19 15:13:13.000000 ark-mainsail-1.2.1/ark_mainsail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.081776 ark-mainsail-1.2.1/mainsail/
+-rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.2.1/mainsail/__init__.py
+-rw-rw-rw-   0        0        0     1015 2024-05-12 19:42:22.000000 ark-mainsail-1.2.1/mainsail/config.py
+-rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.2.1/mainsail/deserializer.py
+-rw-rw-rw-   0        0        0     9841 2024-04-24 20:18:46.000000 ark-mainsail-1.2.1/mainsail/identity.py
+-rw-rw-rw-   0        0        0     6097 2024-05-19 06:30:07.000000 ark-mainsail-1.2.1/mainsail/rest.py
+-rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.2.1/mainsail/serializer.py
+-rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.2.1/mainsail/transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.131847 ark-mainsail-1.2.1/mainsail/tx/
+-rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.2.1/mainsail/tx/__init__.py
+-rw-rw-rw-   0        0        0     7119 2024-04-25 06:54:53.000000 ark-mainsail-1.2.1/mainsail/tx/v1.py
+-rw-rw-rw-   0        0        0     5052 2024-04-24 20:10:37.000000 ark-mainsail-1.2.1/mainsail/webhook.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.221781 ark-mainsail-1.2.1/mnsl_pool/
+-rw-rw-rw-   0        0        0     6269 2024-05-19 07:05:55.000000 ark-mainsail-1.2.1/mnsl_pool/__init__.py
+-rw-rw-rw-   0        0        0     4710 2024-05-16 20:01:52.000000 ark-mainsail-1.2.1/mnsl_pool/__main__.py
+-rw-rw-rw-   0        0        0     2042 2024-05-04 13:20:14.000000 ark-mainsail-1.2.1/mnsl_pool/api.py
+-rw-rw-rw-   0        0        0    17914 2024-05-19 07:06:31.000000 ark-mainsail-1.2.1/mnsl_pool/biom.py
+-rw-rw-rw-   0        0        0    11068 2024-05-18 15:37:44.000000 ark-mainsail-1.2.1/mnsl_pool/tbw.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:13:14.277660 ark-mainsail-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2044 2024-05-03 04:37:51.000000 ark-mainsail-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:13:14.237574 ark-mainsail-1.2.1/test/
+-rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.2.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.2.1/test/test_identity.py
+-rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.2.1/test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.2.0/LICENSE` & `ark-mainsail-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/README.md` & `ark-mainsail-1.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # python-mainsail
 
 This package provides a simple implementation to interact with `Ark` blockchain
-API and managment tools for validators aiming to run a pool.
+API and managment tools for validators aiming to [run a pool](https://moustikitos.github.io/python-mainsail/pool).
 
 ```python
 >>> from mainsail.tx.v1 import Transfer
 >>> from mainsail import rest
 >>> # http://xxx.xxx.xxx.xxx:4006/api/wallets/toons
 >>> wallet = rest.GET.api.wallets.toons()
 >>> wallet["address"]
 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv'
 >>> rest.GET.api.wallets()["meta"]["totalCount"]
 89
 >>> # use a custop peer
->>> custom_peer = {"ip": "49.13.30.19", "ports": {"api-development": 4003}}
+>>> custom_peer = rest.Peer("http://49.13.30.19:4006", port_name="api-development")
+>>> custom_peer
+{'ip': '49.13.30.19', 'ports': {'api-development': 4006}}
 >>> # http://49.13.30.19:4003/api/transactions?type=4
 >>> [t["blockId"] for t in rest.GET.api.transactions(type=4, peer=custom_peer)["data"]]
 ['41afebd995473aab76e8dd7415ab742a6882a08f4c0e0a7305d1a48c551c955c', 'aff37ad0288fadc9d5fdec584d1affab2df0021e86cde3ecb2ba263d6deba3cc']
 >>> t = Transfer(1, 'D5Ha4o3UTuTd59vjDw1F26mYhaRdXh7YPv', 'message \U0001f919')
 >>> t.sign()
 Type or paste your passphrase >
 >>> t.send()
 {'data': {'accept': [0], 'broadcast': [0], 'excess': [], 'invalid': []}}
 ```
 
 ## Linux distributions
 
-Due to [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994)
+Due to [RIPEMD160 issue with OpenSSL v>=3](https://github.com/openssl/openssl/issues/16994),
 `hashlib.ripemd160` is disabled within `python3`. To enable it back, get the
 installation folder...
 
 ```bash
 openssl version -d
 ```
 
@@ -49,74 +51,32 @@
 [default_sect]
 activate = 1
 
 [legacy_sect]
 activate = 1
 ```
 
-## Validator pool managment tools
-
-### Ubuntu installation
-
-First read [installation script](https://bit.ly/3U6BI8v), then:
-
-```bash
-~$ bash <(wget -qO- https://bit.ly/3U6BI8v)
-```
-
-### Deploy pool server
-
-```bash
-~$ mnsl_deploy # use ip address 0.0.0.0 with  port #5000
-```
-
-If you plan to deploy pool server behind a proxy, it is possible to customize
-`ip` and `port`:
-
-```bash
-~$ mnsl_deploy host=127.0.0.1 port=7542 # use localhost address with port #7542
-```
-
-Setup a pool using validator public key:
-
-```bash
-~$ add_pool puk=02968e862011738ac185e87f47dec61b32c842fd8e24fab625c02a15ad7e2d0f65
-```
-
-Configure pool options:
-
-```bash
-~$ set_pool ?key=value?
-```
-
-Check the logs:
-
-```bash
-~$ log_mnsl_pool
-~$ log_mnsl_bg
-```
-
 ## Available transactions
 
-* [x] Transfer
-* [x] ValidatorRegistration
-* [x] Vote
-* [x] MultiSignature
-* [x] MultiPayment
-* [x] ValidatorResignation
-* [x] UsernameRegistration
-* [x] UsernameResignation
+- [x] Transfer
+- [x] ValidatorRegistration
+- [x] Vote
+- [x] MultiSignature
+- [x] MultiPayment
+- [x] ValidatorResignation
+- [x] UsernameRegistration
+- [x] UsernameResignation
 
 ## Features
 
-* [x] secured private keys storage
-* [x] secured webhook subscriptions storage
-* [x] offline network configuration available
-* [x] pool server with remote managment tool
-* [x] `cmd` command line `set_validator` for windows platform
-* [x] pool installation and update using pip
+- [x] secured private keys storage
+- [x] secured webhook subscriptions storage
+- [x] offline network configuration available
+- [x] pool server with remote managment tool
+- [x] `cmd` command line `set_pool` and `dump_prk` for windows platform
+- [x] pool installation and update using pip
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
 [![Paypal me](https://img.shields.io/badge/PayPal-toons-00457C?logo=paypal&logoColor=white)](https://paypal.me/toons)
-[![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://github.com/Moustikitos/python-mainsail/blob/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
+[![Bitcoin](https://img.shields.io/badge/Donate-bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x-ff9900?logo=bitcoin)](https://raw.githubusercontent.com/Moustikitos/python-mainsail/master/docs/img/bc1q6aqr0hfq6shwlaux8a7ydvncw53lk2zynp277x.png)
```

### Comparing `ark-mainsail-1.2.0/ark_mainsail.egg-info/SOURCES.txt` & `ark-mainsail-1.2.1/ark_mainsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/__init__.py` & `ark-mainsail-1.2.1/mainsail/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/config.py` & `ark-mainsail-1.2.1/mainsail/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 DATA = os.path.join(os.getenv("HOME"), ".mainsail", ".networks")
 _track = []
 
 
 def _clear() -> None:
     for name in _track:
-        delattr(sys.modules[__name__], name)
+        if hasattr(sys.modules[__name__], name):
+            delattr(sys.modules[__name__], name)
     _track.clear()
 
 
 def _dump(name: str) -> None:
     path = os.path.join(DATA, f"{name}.net")
     os.makedirs(DATA, exist_ok=True)
     with open(path, "wb") as output:
```

### Comparing `ark-mainsail-1.2.0/mainsail/deserializer.py` & `ark-mainsail-1.2.1/mainsail/deserializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/identity.py` & `ark-mainsail-1.2.1/mainsail/identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/rest.py` & `ark-mainsail-1.2.1/mainsail/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Network endpoint managment module.
 """
 
+import re
 import requests
 
 from typing import Union
 from mainsail import config
 from urllib.parse import urlencode, urlparse, urlunparse
 from collections import namedtuple
 
@@ -18,14 +19,36 @@
 )
 
 
 class ApiError(Exception):
     pass
 
 
+class Peer(dict):
+
+    ip_port = r'([0-9]+(?:\.[0-9]+){3})(:[0-9]+)?'
+
+    def __init__(
+        self, url: str = "http://127.0.0.1", port_name: str = "requests"
+    ) -> None:
+        self.base_url = urlparse(url)
+        test = re.match(Peer.ip_port, self.base_url.netloc)
+        if test is not None:
+            ip, port = test.groups()
+            self["ip"] = ip
+            if port is not None:
+                self["ports"] = {port_name: int(port.replace(":", ""))}
+        else:
+            self["url"] = urlunparse(
+                self.base_url._replace(
+                    path="", params="", query="", fragment=""
+                )
+            )
+
+
 class EndPoint(object):
 
     def __init__(self, *path, **opt) -> None:
         self.headers = opt.pop("headers", {'Content-type': 'application/json'})
         self.ports = opt.pop("ports", "api-development")
         self.func = opt.pop("func", requests.get)
         self.path = "/".join(path)
@@ -65,24 +88,25 @@
                 f"no peer available with '{self.ports}' port enabled"
             )
         # else do HTTP request call
         # build an Urltuple to be updated according to needs
         if "url" in peer:
             base_url = urlparse(peer["url"])
         else:
+            peer_ports = peer.get("ports", {})
             # if peer == {} return the a default base_url
             # default -> ["requests"]
             ports = list(
-                ports or set(self.ports) & set(peer.get("ports", {}).keys())
+                ports or set(self.ports) & set(peer_ports.keys())
             ) or ["requests"]
             # default -> http://127.0.0.1:5000
             base_url = Urltuple(
                 'http',
                 f"{peer.get('ip', '127.0.0.1')}:" +
-                f"{peer.get('ports', {}).get(ports[0], 5000)}",
+                f"{peer_ports.get(ports[0], 5000)}",
                 None, None, None, None
             )
         base_url = base_url._replace(path='/'.join((self.path,) + path))
         if self.func in (requests.post, requests.delete):
             resp = self.func(urlunparse(base_url), headers=headers, json=data)
         else:
             base_url = base_url._replace(query=urlencode(data))
@@ -92,24 +116,25 @@
             return resp.json()
         except requests.exceptions.JSONDecodeError:
             return resp
 
 
 def use_network(peer: str) -> None:
     config._clear()
+    base_url = urlparse(peer)
 
     for key, value in requests.get(
-        f"{peer}/api/node/configuration",
+        urlunparse(base_url._replace(path="api/node/configuration")),
         headers={'Content-type': 'application/json'},
     ).json().get("data", {}).items():
         setattr(config, key, value)
         config._track.append(key)
 
     fees = requests.get(
-        f"{peer}/api/node/fees?days=30",
+        urlunparse(base_url._replace(path="api/node/fees", query="days=30")),
         headers={'Content-type': 'application/json'},
     ).json().get("data", {})
     setattr(config, "fees", fees)
     config._track.append("fees")
 
     get_peers(peer)
 
@@ -119,17 +144,19 @@
 
 
 def load_network(name: str) -> bool:
     return config._load(name)
 
 
 def get_peers(peer: str, latency: int = 500) -> None:
+    base_url = urlparse(peer)
     resp = sorted(
         requests.get(
-            f"{peer}/api/peers", headers={'Content-type': 'application/json'}
+            urlunparse(base_url._replace(path="api/peers")),
+            headers={'Content-type': 'application/json'}
         ).json().get("data", {}),
         key=lambda p: p["latency"]
     )
     setattr(config, "peers", [
         {
             "ip": peer["ip"],
             "ports": dict(
```

### Comparing `ark-mainsail-1.2.0/mainsail/serializer.py` & `ark-mainsail-1.2.1/mainsail/serializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/transaction.py` & `ark-mainsail-1.2.1/mainsail/transaction.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/tx/__init__.py` & `ark-mainsail-1.2.1/mainsail/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/tx/v1.py` & `ark-mainsail-1.2.1/mainsail/tx/v1.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mainsail/webhook.py` & `ark-mainsail-1.2.1/mainsail/webhook.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/mnsl_pool/__init__.py` & `ark-mainsail-1.2.1/mnsl_pool/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 
 """
 This package provides managment tools to run a pool on arkEcosystem mainsail
-framework. It computes a true block weight (TBW) distribution of block reward
+framework. It computes a true block weight (TBW) distribution of reward
 according to instant participant vote weight.
 
-## Install on Ubuntu
+### Ubuntu installation
+
+First read [installation script](https://bit.ly/3U6BI8v), then:
 
 ```bash
-wget https://bit.ly/3U6BI8v
-bash mnsl-pool.sh
+~$ bash <(wget -qO- https://bit.ly/3U6BI8v)
 ```
 
-Setup script creates 7 commands into `~/.bash_aliases` file:
+Setup script creates 9 commands into `~/.bash_aliases` file:
 
-* [x] `mnsl_deploy` takes broadcast ip address and port to create
+- [x] `mnsl_install` install a specific version
+- [x] `mnsl_deploy` takes broadcast ip address and port to create
   services managed by `systemd`.
-* [x] `add_pool` takes a validator public key to configure listening
+- [x] `dump_prk` secures validator private key to sign transactions
+- [x] `add_pool` takes a validator public key to configure listening
   subscription on blockchain.
-* [x] `set_pool` modifies validator TBW pool service parameters.
-* [x] `mnsl_venv` activates the virtual environment used to run
+- [x] `set_pool` modifies validator TBW pool service parameters.
+- [x] `mnsl_venv` activates the virtual environment used to run
   mainsail pool.
-* [x] `mnsl_restart` restarts pool tasks.
-* [x] `log_mnsl_pool` shows server logs.
-* [x] `log_mnsl_bg` shows background tasks logs.
+- [x] `mnsl_restart` restarts pool tasks.
+- [x] `log_mnsl_pool` shows server logs.
+- [x] `log_mnsl_bg` shows background tasks logs.
 """
 
 import os
 import json
 import queue
 import flask
 import logging
@@ -36,17 +39,17 @@
 from mnsl_pool import tbw, biom
 
 # set basic logging
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
-CONF_PARAMETERS = [
-    "sleep_time"
-]
+CONF_PARAMETERS = {
+    "sleep_time": int
+}
 
 
 # create worker and its queue
 JOB = queue.Queue()
 
 # create the application instance
 app = flask.Flask(__name__)
@@ -83,69 +86,84 @@
             return flask.jsonify({"status": 204}), 200
     else:
         return flask.jsonify({"status": 403}), 200
 
 
 @app.route("/pool/configure", methods=["POST"])
 def pool_configure() -> flask.Response:
-    """
-    Flask endpoint to configure validator pool parameters. Requests are secured
-    using validator signature on UTC-time-based nonce. Available parameters are
-    set in `pool.biom:DELEGATE_PARAMETERS` dict.
+    # Flask endpoint to configure validator pool parameters. Requests are
+    # secured # using validator signature on UTC-time-based nonce. Available
+    # parameters are set in `pool.biom:POOL_PARAMETERS` dict.
 
-    This end point is used by `set_pool` command.
-    """
+    # This endpoint is used by `set_pool` command.
 
     if biom.check_headers(flask.request.headers):
         puk = flask.request.headers["puk"]
         path = os.path.join(tbw.DATA, f"{puk}.json")
         data = json.loads(flask.request.data)
         # BUGFIX: when used directly on server where pool is runing, the
         # headers seem to be copied into request data...
         data.pop("headers", False)
         ##########################
         info = dict(
             loadJson(path), **dict(
                 [k, v] for k, v in data.items()
-                if k in biom.DELEGATE_PARAMETERS.keys()
+                if k in biom.POOL_PARAMETERS.keys()
             )
         )
+        # manage excludes:[add|pop]=... and exclusives:[add|pop]=...
+        for special_key in list(data.keys()):
+            if ("excludes" in special_key or "exclusives" in special_key) \
+               and ":" in special_key:
+                key, func = special_key.split(":")
+                former_value = set(info[key])
+                if func == "add":
+                    info[key] = list(former_value | set(data[special_key]))
+                elif func == "pop":
+                    info[key] = list(former_value - set(data[special_key]))
+                else:
+                    data.pop(special_key, False)
+                    LOGGER.info(
+                        f"{special_key} ignored, unknown action {func}"
+                    )
+
         if flask.request.method == "POST":
+            update = dict([k, v] for k, v in info.items() if k in data)
             LOGGER.debug(f"---- received> {data}")
-            LOGGER.info(f"updating {puk} info> {info}")
+            LOGGER.info(f"updating {puk} info> {update}")
             dumpJson(info, path, ensure_ascii=False)
-            return flask.jsonify({"status": 204, "updated": data})
+            os.makedirs(os.path.join(tbw.DATA, puk), exist_ok=True)
+            return flask.jsonify({"status": 204, "updated": update})
     else:
         return flask.jsonify({"status": 403})
 
 
 @app.route("/block/forged", methods=["POST", "GET"])
 def block_forged() -> flask.Response:
     check = False
     if flask.request.method == "POST":
         check = webhook.verify(
             flask.request.headers.get("Authorization", "")[:32]
         )
         LOGGER.info("webhook check> %s", check)
         if check is True and flask.request.data != b'':
             data = json.loads(flask.request.data)
-            block = data.get("data", {}).get("block", {}).get("data", {})
+            block = data.get("data", {})
             LOGGER.debug("block received> %s", block)
             JOB.put(block)
         else:
             check = False
     return flask.jsonify({"acknowledge": check})
 
 
 def main():
-    """
-    Server main loop ran as a `threading.Thread` target. It gets block
-    passed by `block_forged` (`/block/forged` endpoint) and update forgery
-    of validator issuing the block.
-    """
+    # Server main loop ran as a `threading.Thread` target. It gets block
+    # passed by `block_forged` (`/block/forged` endpoint) and update forgery
+    # of validator issuing the block.
+
     LOGGER.info("entering main loop")
     while True:
         block = JOB.get()
         if block not in [False, None]:
             lock = biom.acquireLock()
             try:
                 result = tbw.update_forgery(block)
```

### Comparing `ark-mainsail-1.2.0/mnsl_pool/__main__.py` & `ark-mainsail-1.2.1/mnsl_pool/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import queue
-import binascii
 import threading
 
-from mainsail import rest, identity
+from mainsail import rest
 from mnsl_pool import tbw, biom, loadJson, dumpJson, LOGGER
 
 TASK = queue.Queue()
 SLEEP = threading.Event()
 
 
 def payroll():
@@ -39,38 +38,26 @@
                 LOGGER.info(
                     f"{puk}: "
                     f"block delay<{block_delay}> - forged blocks<{blocks}>"
                 )
                 if blocks > block_delay:
                     lock = biom.acquireLock()
                     try:
-                        tbw.freeze_forgery(puk, **info)
+                        if "puk" in info:
+                            tbw.freeze_forgery(**info)
+                        else:
+                            tbw.freeze_forgery(puk, **info)
                     except Exception:
                         LOGGER.exception("---- error occured>")
                     else:
                         LOGGER.info(f"{puk} forgery frozen")
                     finally:
                         biom.releaseLock(lock)
                     tbw.bake_registry(puk)
-                    for registry in [
-                        reg for reg in os.listdir(os.path.join(tbw.DATA, puk))
-                        if reg.endswith(".registry")
-                    ]:
-                        tx = loadJson(os.path.join(tbw.DATA, puk, registry))
-                        LOGGER.info(
-                            rest.POST.api("transaction-pool", transactions=tx)
-                        )
-                        hash = identity.cSecp256k1.hash_sha256
-                        dumpJson(
-                            [
-                                hash(binascii.unhexlify(s)).decode("utf-8")
-                                for s in tx
-                            ],
-                            os.path.join(tbw.DATA, puk, f"{registry}.check")
-                        )
+                    tbw.broadcast_registry(puk)
     LOGGER.info("payroll loop exited")
 
 
 def accountant():
     while True:
         delay = TASK.get()
         if delay in [False, None]:
```

### Comparing `ark-mainsail-1.2.0/mnsl_pool/tbw.py` & `ark-mainsail-1.2.1/mnsl_pool/tbw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 # -*- coding: utf-8 -*-
 import os
 import math
 import time
+import random
 import logging
 import datetime
+import binascii
 
 from mainsail import rest, identity, loadJson, dumpJson, XTOSHI
 from mainsail.tx import Transfer, MultiPayment
 
 # Set basic logging.
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 DATA = os.path.join(os.getenv("HOME"), ".mainsail", ".pools")
-PEER = {"ip": "127.0.0.1", "ports": {"api-http": 4003}}
+PEER = rest.Peer("http://127.0.0.1:4003")  # {"ip": "127.0.0.1", "ports": {"api-http": 4003}}
 
 os.makedirs(DATA, exist_ok=True)
 
 
 class UnknownValidator(Exception):
     pass
 
 
 def update_forgery(block: dict) -> bool:
     # 1. GET GENERATOR PUBLIC KEY PARAMETERS
     publicKey = block["generatorPublicKey"]
     info = loadJson(os.path.join(DATA, f"{publicKey}.json"))
     if info == {}:
         raise UnknownValidator(f"{publicKey} has no subcription here")
-    excludes = info.get("excludes", [])
+    excludes = info.get("excludes", [])  # public pool
+    exclusives = info.get("exclusives", [])  # private pool
+    filter_addr = \
+        (lambda addr: addr in exclusives) if exclusives else \
+        (lambda addr: addr not in excludes)
     # Minimum vote and maximum vote have to be converted to Xtoshi.
     min_vote = info.get("min_vote", 1) * XTOSHI
     max_vote = info.get("max_vote", int(1e6)) * XTOSHI
     share = info.get("share", 1.0)
-    peer = info.get("peer", PEER)
+    peer = info.get("api_peer", PEER)
 
     # 2. GET FEES AND REWARDS SINCE LAST FORGED BLOCK
     last_block = loadJson(os.path.join(DATA, publicKey, "last.block"))
     # If no block found save the first one and exit.
     if last_block == {}:
         dumpJson(block, os.path.join(DATA, publicKey, "last.block"))
         return False
@@ -83,76 +89,92 @@
     voters, page = {}, 1
     while page > 0:  # infinite loop
         resp = rest.GET.api.delegates(
             publicKey, "voters", page=page, peer=peer
         )
         voters.update(
             (v["address"], int(v["balance"])) for v in resp.get("data", [])
-            if v["address"] not in excludes
+            if filter_addr(v["address"])  # not in excludes
         )
         if resp.get("meta", {}).get("next", None) is None:
             break  # -> exit infinite loop
         page += 1  # -> go to next API page
     # filter all voters using minimum and maximum votes
     voters = dict(
         [a, min(max_vote, b)] for a, b in voters.items() if b >= min_vote
     )
     LOGGER.debug(f"---- found {len(voters)} valid voters")
     # compute vote weight amongs fltered voters
     vote_weight = float(sum(voters.values()))
-    voters_weight = dict([a, b / vote_weight] for a, b in voters.items())
+    voter_weights = dict([a, b / vote_weight] for a, b in voters.items())
+    n_voters = len(voter_weights)
 
     # 4. UPDATE FORGERY ACCORDING TO REWARDS AND VOTER WEIGHT
     forgery = loadJson(os.path.join(DATA, publicKey, "forgery.json"))
     contributions = forgery.get("contributions", {})
     new_contributions = dict([
         address, int(
             math.floor(
                 contributions.get(address, 0) +
-                shared_reward * voters_weight[address]
+                shared_reward * voter_weights[address]
             )
         )
-    ] for address in voters_weight)
+    ] for address in voter_weights)
     forgery["reward"] = forgery.get("reward", 0) + generator_reward
     forgery["blocks"] = forgery.get("blocks", 0) + blocks
     forgery["fee"] = forgery.get("fee", 0) + fee
-    forgery["contributions"] = new_contributions
-    # compute checksum to determine XTOSHI
+    # compute checksum to determine lost XTOSHI due to roundings then
+    # redistribute XTOSHI if possible
     checksum = (sum(new_contributions.values()) + forgery["reward"])
     checksum -= int(rest.config.constants["reward"]) * forgery["blocks"]
     checksum -= forgery.get("undistributed", 0)
-    LOGGER.info(f"losed XTOSHI: {checksum}")
+    checksum = abs(checksum)
+    if checksum >= n_voters:  # can give n XTOSHI per voter
+        xtoshis = int(checksum // n_voters)
+        for k in new_contributions:
+            new_contributions[k] += xtoshis
+        checksum -= n_voters * xtoshis
+        LOGGER.info(f"lost XTOSHI redistributed: {n_voters * xtoshis}")
+    LOGGER.info(f"lost XTOSHI remaining: {checksum}")
+    forgery["contributions"] = new_contributions
+    forgery["lost XTOSHI"] = checksum
     # update true block weight state
     dumpJson(block, os.path.join(DATA, publicKey, "last.block"))
     dumpJson(forgery, os.path.join(DATA, publicKey, "forgery.json"))
     LOGGER.info(
-        f"{shared_reward / XTOSHI} token distributed to {len(voters)} voters "
-        f"- {generator_reward / XTOSHI} token plus {fee / XTOSHI} fee added "
+        f"{shared_reward / XTOSHI} coin distributed to {len(voters)} voters "
+        f"- {generator_reward / XTOSHI} coin plus {fee / XTOSHI} fee added "
         f"to {info.get('wallet', identity.get_wallet(publicKey))} share"
     )
 
     # 5. PRINT VOTE CHANGES
     for downvoter in list(set(contributions.keys()) - set(voters.keys())):
         LOGGER.info(
             f"{downvoter} downvoted {publicKey} : "
-            f"{contributions[downvoter] / XTOSHI:.8f} token leaved"
+            f"{contributions[downvoter] / XTOSHI:.8f} coin leaved"
         )
     for upvoters in list(set(voters.keys()) - set(contributions.keys())):
         LOGGER.info(
             f"{upvoters} upvoted validator - "
             f"{voters[upvoters] / XTOSHI:.8f} vote weight added"
         )
 
     # Exit with True means 5 steps gone straight.
     return True
 
 
 def freeze_forgery(puk: str, **options) -> None:
     min_share = options.get("min_share", 1.0) * XTOSHI
     forgery = loadJson(os.path.join(DATA, puk, "forgery.json"))
+    # give lost xtoshi to a random voter
+    lost_xtoshi = forgery.pop("lost XTOSHI", 0)
+    if lost_xtoshi > 0:
+        address = random.choice(list(forgery["contributions"].keys()))
+        forgery["contributions"][address] += lost_xtoshi
+        LOGGER.info(f"lucky {address} got {lost_xtoshi} XTOSHI")
     tbw = {
         "timestamp": f"{datetime.datetime.now()}",
         "validator-share": forgery.get("reward", 0) + forgery.get("fee", 0),
         "voter-shares": dict(
             [voter, amount]
             for voter, amount in forgery.get("contributions", {}).items()
             if amount >= min_share
@@ -228,7 +250,21 @@
                     tbw, os.path.join(DATA, puk, "forgery", f"{name}.forgery")
                 )
             except Exception:
                 pass
             else:
                 os.remove(os.path.join(DATA, puk, f"{name}.forgery"))
             LOGGER.info(f"{len(registry)} transactions baked")
+
+
+def broadcast_registry(puk: str) -> None:
+    for registry in [
+        reg for reg in os.listdir(os.path.join(DATA, puk))
+        if reg.endswith(".registry")
+    ]:
+        tx = loadJson(os.path.join(DATA, puk, registry))
+        LOGGER.info(rest.POST.api("transaction-pool", transactions=tx))
+        hash = identity.cSecp256k1.hash_sha256
+        dumpJson(
+            [hash(binascii.unhexlify(s)).decode("utf-8") for s in tx],
+            os.path.join(DATA, puk, f"{registry}.check")
+        )
```

### Comparing `ark-mainsail-1.2.0/setup.py` & `ark-mainsail-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 
 with open("README.md") as f2:
     LONG_DESCRIPTION = f2.read()
 
 kw = {
-    "version": "1.2.0",
+    "version": "1.2.1",
     "name": "ark-mainsail",
     "keywords": ["api", "ark", "blockchain"],
     "author": "Toons",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Toons",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://github.com/Moustikitos/python-mainsail",
@@ -50,14 +50,15 @@
     ],
     "package_dir": {
         "mainsail": "./mainsail",
         "mnsl_pool": "./mnsl_pool"
     },
     "entry_points": {
         'console_scripts': [
-            'set_pool = mnsl_pool.biom:set_pool'
+            'set_pool = mnsl_pool.biom:set_pool',
+            'dump_prk = mnsl_pool.biom:dump_prk'
         ]
     },
     "zip-safe": True
 }
 
 setup(**kw)
```

### Comparing `ark-mainsail-1.2.0/test/test_identity.py` & `ark-mainsail-1.2.1/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.2.0/test/test_v1_builders.py` & `ark-mainsail-1.2.1/test/test_v1_builders.py`

 * *Files identical despite different names*

