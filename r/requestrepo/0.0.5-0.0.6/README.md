# Comparing `tmp/requestrepo-0.0.5.tar.gz` & `tmp/requestrepo-0.0.6.tar.gz`

## Comparing `requestrepo-0.0.5.tar` & `requestrepo-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 requestrepo-0.0.5/requirements.txt
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 requestrepo-0.0.5/src/requestrepo/__init__.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 requestrepo-0.0.5/tests/dns.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 requestrepo-0.0.5/tests/request.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 requestrepo-0.0.5/tests/response.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 requestrepo-0.0.5/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.5/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 requestrepo-0.0.6/requirements.txt
+-rw-r--r--   0        0        0    10314 2020-02-02 00:00:00.000000 requestrepo-0.0.6/src/requestrepo/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 requestrepo-0.0.6/src/requestrepo/models/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 requestrepo-0.0.6/tests/dns.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 requestrepo-0.0.6/tests/request.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 requestrepo-0.0.6/tests/response.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 requestrepo-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.6/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.6/PKG-INFO
```

### Comparing `requestrepo-0.0.5/src/requestrepo/__init__.py` & `requestrepo-0.0.6/src/requestrepo/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import jwt
 import sys
 import json
 import base64
 import asyncio
 import requests
 from websockets.client import connect
-from typing import Union, Callable, Dict, List
+from typing import Union, Dict, List, Callable, Optional
 from jwt.exceptions import DecodeError
+from models import HttpRequest, DnsRequest, HttpResponse, DnsRecord
 
 class Requestrepo:
   """
   Class for interacting with the Requestrepo API. Provides real-time request monitoring,
   historical request retrieval, and the ability to delete requests.
   """
 
-  __old_requests: List[Dict]
+  __old_requests: List[Union[HttpRequest, DnsRequest]] = []
+  __queue: List[Union[HttpRequest, DnsRequest]] = []
 
   def __init__(
         self,
         token: Union[str, None] = None,
         host: str = "requestrepo.com",
         port: int = 443,
         protocol: str = 'https',
@@ -73,62 +75,105 @@
 
     loop = asyncio.get_event_loop()
     self.__websocket = loop.run_until_complete(connect(f"{wsp}://{host}:{port}/api/ws"))
     loop.run_until_complete(self.__websocket.send(token))
 
     self.__old_requests = json.loads(loop.run_until_complete(self.__websocket.recv()))["data"]
 
-  def on_request(self, data: Dict):
+  def on_request(self, data: Union[HttpRequest, DnsRequest]):
     """
     Callback function for handling new incoming requests. **Override this in your code.**
 
     Args:
         data: Dictionary containing the request data.
     """
     raise NotImplementedError(f"You must implement the on_request method on {self} class")
 
-  def get_old_requests(self) -> List[Dict]:
+  def get_old_requests(self) -> List[Union[HttpRequest, DnsRequest]]:
     """
     Returns a list of previously received requests.
 
     Returns:
         List of dictionaries, each representing a past request.
     """
     return self.__old_requests
 
-  def get_request(self) -> Dict:
+  @staticmethod
+  def HTTP_FILTER(request: Union[HttpRequest, DnsRequest]) -> bool:
+    return isinstance(request, HttpRequest)
+
+  @staticmethod
+  def DNS_FILTER(request: Union[HttpRequest, DnsRequest]) -> bool:
+    return isinstance(request, DnsRequest)
+
+  def get_http_request(self) -> HttpRequest:
+    """
+    Synchronously gets a single new HTTP request (blocks the current thread).
+
+    Returns:
+        Dictionary containing the request data.
+    """
+    return self.get_request(Requestrepo.HTTP_FILTER)
+
+  def get_dns_request(self) -> DnsRequest:
+    """
+    Synchronously gets a single new DNS request (blocks the current thread).
+
+    Returns:
+        Dictionary containing the request data.
     """
+    return self.get_request(Requestrepo.DNS_FILTER)
+
+  def get_request(self, filter: Union[Callable[[Union[HttpRequest, DnsRequest]], bool], None] = None) -> Union[HttpRequest, DnsRequest]:
+    """ 
     Synchronously gets a single new request (blocks the current thread).
 
     Returns:
         Dictionary containing the request data.
     """
+    if filter and self.__queue:
+      for i, request in enumerate(self.__queue):
+        if filter(request):
+          return self.__queue.pop(i)
+
     loop = asyncio.get_event_loop()
-    return loop.run_until_complete(self.async_get_request())
+    request = loop.run_until_complete(self.async_get_request())
+    while filter and not filter(request):
+      self.__queue.append(request)
+      request = loop.run_until_complete(self.async_get_request())
 
-  async def async_get_request(self) -> Dict:
+    return request
+
+  async def async_get_request(self) -> Union[HttpRequest, DnsRequest]:
     """
     Asynchronously gets a single new request.
 
     Returns:
         Dictionary containing the request data.
     """
     data = json.loads(await self.__websocket.recv())["data"]
     data = json.loads(data)
     data["raw"] = base64.b64decode(data["raw"])
+    if data["type"] == "http":
+      data = HttpRequest(**data)
+    elif data["type"] == "dns":
+      data = DnsRequest(**data)
+    else:
+      raise ValueError(f"Invalid request type: {data['type']}")
+
     return data
 
   async def __process_requests(self):
       """
       Internal function to continuously receive and process requests asynchronously.
       """
       while True:
-          request_data = await self.async_get_request()
-          if self.__on_request_callback:
-              self.__on_request_callback(request_data)
+        request_data = await self.async_get_request()
+        if self.__on_request_callback:
+            self.__on_request_callback(request_data)
 
   def await_requests(self) -> None:
     """
     Starts listening for incoming requests indefinitely (doesn't return).
     """
     loop = asyncio.get_event_loop()
     loop.run_until_complete(self.__process_requests())
@@ -152,84 +197,85 @@
 
     Returns:
         True if deletion was successful, False otherwise.
     """
     r = requests.post(f"{self.__protocol}://{self.__host}:{self.__port}/api/delete_all_requests?token={self.__token}", verify=self.__verify)
     return r.status_code == 200
 
-  def response(self) -> Dict:
+  def response(self) -> HttpResponse:
     """
-    Returns a dictionary containing the response data.
+    Returns a dictionary containing the HTTP response data.
     """
     r = requests.get(f"{self.__protocol}://{self.__host}:{self.__port}/api/get_file?token={self.__token}", verify=self.__verify)
     data = r.json()
     data["raw"] = base64.b64decode(data["raw"])
     # normalize list of headers to dictionary
     data["headers"] = {h["header"]:h["value"] for h in data["headers"]}
 
-    return data
+    return HttpResponse(**data)
 
-  def update_response(self, headers: Union[Dict, None] = None, raw: Union[bytes, None] = None, status_code: Union[int, None] = None) -> bool:
+  def update_http(self, response: Optional[HttpResponse] = None, raw: Optional[bytes] = None, headers: Optional[Union[List[Dict[str, str]], Dict[str, str]]] = None, status_code: Optional[int] = None) -> bool:
     """
-    Updates the response data on remote.
+    Updates the HTTP response data on remote.
     If a value is not provided, it will not be updated.
     """
-    data = self.response()
+    data = response.model_dump() if response else self.response().model_dump()
 
     if headers:
       data["headers"] = headers
     if raw:
       data["raw"] = raw
     if status_code:
       data["status_code"] = status_code
 
     data["raw"] = base64.b64encode(data["raw"]).decode()
 
-    # normalize dictionary of headers to list
-    data["headers"] = [{"header":k, "value":v} for k,v in data["headers"].items()]
+    if type(data["headers"]) == dict: # normalize dictionary of headers to list, but only when needed
+      # this allows the user to pass a list of headers if needed
+      data["headers"] = [{"header":k, "value":v} for k,v in data["headers"].items()]
 
     r = requests.post(f"{self.__protocol}://{self.__host}:{self.__port}/api/update_file?token={self.__token}", json=data, verify=self.__verify)
     return r.status_code == 200
 
-  def dns(self) -> List[Dict]:
+  def dns(self) -> List[DnsRecord]:
     """
     Returns a dictionary containing the DNS data.
     """
     r = requests.get(f"{self.__protocol}://{self.__host}:{self.__port}/api/get_dns?token={self.__token}", verify=self.__verify)
-    return r.json()
+    return [DnsRecord(**d) for d in r.json()]
 
-  def update_dns(self, dns: List[Dict]) -> bool:
+  def update_dns(self, dns: List[DnsRecord]) -> bool:
     """
     Updates the DNS data on remote.
     """
-    r = requests.post(f"{self.__protocol}://{self.__host}:{self.__port}/api/update_dns?token={self.__token}", json={"records":dns}, verify=self.__verify)
+    r = requests.post(f"{self.__protocol}://{self.__host}:{self.__port}/api/update_dns?token={self.__token}", json={"records":[d.model_dump() for d in dns]}, verify=self.__verify)
     return r.status_code == 200
 
   def add_dns(self, subsubdomain: str, dnstype: Union[int, str], value: str) -> bool:
     """
     Adds a DNS record to the remote.
     """
     dns_types = ["A", "AAAA", "CNAME", "TXT"]
     records = self.dns()
 
     # if dns entry already exists for same subsubdomain and dnstype, update it
     # otherwise, add a new entry
     for record in records:
-      if record["domain"] == subsubdomain and record["type"] == dnstype:
-        record["value"] = value
+      if record.domain == subsubdomain and record.type == dnstype:
+        record.value = value
         return self.update_dns(records)
 
     if type(dnstype) == str:
       dnstype = dns_types.index(dnstype)
       if dnstype == -1:
         raise ValueError(f"Invalid DNS type: {dnstype}. Must be one of {dns_types}")
     elif type(dnstype) == int and (dnstype < 0 or dnstype > len(dns_types)):
       raise ValueError(f"Invalid DNS type: {dnstype}. Must be between 0 and {len(dns_types)-1}")
 
-    records.append({"domain":subsubdomain, "type":dnstype, "value":value})
+    records.append(DnsRecord(**{"domain":subsubdomain, "type":dnstype, "value":value}))
 
     return self.update_dns(records)
 
 
   def remove_dns(self, subsubdomain: str, dnstype: Union[int, str, None]) -> bool:
     """
     Removes a DNS record from the remote.
@@ -252,8 +298,8 @@
     if len(records) == prev_len:
       return False
 
     return self.update_dns(records)
 
 
 RequestRepo = Requestrepo
-requestrepo = Requestrepo
+requestrepo = Requestrepo
```

### Comparing `requestrepo-0.0.5/tests/request.py` & `requestrepo-0.0.6/tests/request.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.5/tests/response.py` & `requestrepo-0.0.6/tests/response.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.5/.gitignore` & `requestrepo-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.5/LICENSE` & `requestrepo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.5/README.md` & `requestrepo-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.5/pyproject.toml` & `requestrepo-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "requestrepo"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Dragos Albastroiu", email = "adragos@protonmail.com" }]
 description = "Python bindings to automate requestrepo.com"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `requestrepo-0.0.5/PKG-INFO` & `requestrepo-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: requestrepo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python bindings to automate requestrepo.com
 Project-URL: Homepage, https://github.com/adrgs/requestrepo-lib
 Project-URL: Issues, https://github.com/adrgs/requestrepo-lib/issues
 Author-email: Dragos Albastroiu <adragos@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

