# Comparing `tmp/zamino_fix-1.1.5.tar.gz` & `tmp/zamino_fix-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zamino_fix-1.1.5.tar", last modified: Mon May 13 11:07:42 2024, max compression
+gzip compressed data, was "zamino_fix-1.1.6.tar", last modified: Sun May 19 21:19:21 2024, max compression
```

## Comparing `zamino_fix-1.1.5.tar` & `zamino_fix-1.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.5/LICENSE
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/PKG-INFO
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.5/README.md
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAmino.fix.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/requires.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-13 11:07:42.000000 zamino_fix-1.1.5/ZAmino.fix.egg-info/top_level.txt
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-04-10 15:12:24.000000 zamino_fix-1.1.5/ZAminofix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.5/ZAminofix/acm.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/asyncfix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/acm.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.5/ZAminofix/asyncfix/sub_client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-12 08:17:35.000000 zamino_fix-1.1.5/ZAminofix/client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/lib/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/lib/__init__.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/ZAminofix/lib/util/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.5/ZAminofix/lib/util/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.5/ZAminofix/lib/util/exceptions.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.5/ZAminofix/lib/util/headers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.5/ZAminofix/lib/util/helpers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.5/ZAminofix/lib/util/objects.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 zamino_fix-1.1.5/ZAminofix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   107423 2024-05-13 10:55:56.000000 zamino_fix-1.1.5/ZAminofix/sub_client.py
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-13 11:07:42.516591 zamino_fix-1.1.5/setup.cfg
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      698 2024-05-13 11:06:36.000000 zamino_fix-1.1.5/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.728360 zamino_fix-1.1.6/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.6/LICENSE
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-19 21:19:21.718360 zamino_fix-1.1.6/PKG-INFO
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.6/README.md
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.718360 zamino_fix-1.1.6/ZAmino.fix.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-19 21:19:21.000000 zamino_fix-1.1.6/ZAmino.fix.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-19 21:19:21.000000 zamino_fix-1.1.6/ZAmino.fix.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-19 21:19:21.000000 zamino_fix-1.1.6/ZAmino.fix.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-19 21:19:21.000000 zamino_fix-1.1.6/ZAmino.fix.egg-info/requires.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-19 21:19:21.000000 zamino_fix-1.1.6/ZAmino.fix.egg-info/top_level.txt
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.698360 zamino_fix-1.1.6/ZAminofix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-05-19 21:18:39.000000 zamino_fix-1.1.6/ZAminofix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.6/ZAminofix/acm.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.708360 zamino_fix-1.1.6/ZAminofix/asyncfix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.6/ZAminofix/asyncfix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.6/ZAminofix/asyncfix/acm.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.6/ZAminofix/asyncfix/client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.6/ZAminofix/asyncfix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.6/ZAminofix/asyncfix/sub_client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    88977 2024-05-19 13:14:31.000000 zamino_fix-1.1.6/ZAminofix/client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.708360 zamino_fix-1.1.6/ZAminofix/lib/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.6/ZAminofix/lib/__init__.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:19:21.718360 zamino_fix-1.1.6/ZAminofix/lib/util/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.6/ZAminofix/lib/util/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.6/ZAminofix/lib/util/exceptions.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.6/ZAminofix/lib/util/headers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.6/ZAminofix/lib/util/helpers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.6/ZAminofix/lib/util/objects.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13852 2024-05-19 21:12:24.000000 zamino_fix-1.1.6/ZAminofix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   107423 2024-05-13 10:55:56.000000 zamino_fix-1.1.6/ZAminofix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-19 21:19:21.728360 zamino_fix-1.1.6/setup.cfg
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      698 2024-05-19 21:18:14.000000 zamino_fix-1.1.6/setup.py
```

### Comparing `zamino_fix-1.1.5/LICENSE` & `zamino_fix-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/PKG-INFO` & `zamino_fix-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.5
+Version: 1.1.6
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
 Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
```

### Comparing `zamino_fix-1.1.5/ZAmino.fix.egg-info/PKG-INFO` & `zamino_fix-1.1.6/ZAmino.fix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.5
+Version: 1.1.6
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
 Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
```

### Comparing `zamino_fix-1.1.5/ZAmino.fix.egg-info/SOURCES.txt` & `zamino_fix-1.1.6/ZAmino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/acm.py` & `zamino_fix-1.1.6/ZAminofix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/asyncfix/acm.py` & `zamino_fix-1.1.6/ZAminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/asyncfix/client.py` & `zamino_fix-1.1.6/ZAminofix/asyncfix/client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/asyncfix/socket.py` & `zamino_fix-1.1.6/ZAminofix/asyncfix/socket.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/asyncfix/sub_client.py` & `zamino_fix-1.1.6/ZAminofix/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/client.py` & `zamino_fix-1.1.6/ZAminofix/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -220,20 +220,18 @@
         """
 
         data = json.dumps({
             "email": email,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "clientType": 100
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/login", data=data)
         if response.status_code != 200: exceptions.CheckException(response.text)
         else:
             self.authenticated = True
             self.json = json.loads(response.text)
             self.sid = self.json["sid"]
             self.userId = self.json["account"]["uid"]
             self.account: objects.UserProfile = objects.UserProfile(self.json["account"]).UserProfile
@@ -262,20 +260,18 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "clientType": 100
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/login", data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response.text)
 
         else:
             self.authenticated = True
             self.json = json.loads(response.text)
             self.sid = self.json["sid"]
@@ -305,20 +301,18 @@
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "v": 2,
             "secret": secret,
             "deviceID": self.device_id,
-            "clientType": 100,
-            "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "clientType": 100
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/login", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/login", data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response.text)
 
         else:
             self.authenticated = True
             self.json = json.loads(response.text)
             self.sid = self.json["sid"]
@@ -368,19 +362,18 @@
                 "data": {
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "type": 1,
-            "identity": email,
-            "timestamp": int(timestamp() * 1000)
+            "identity": email
         })        
 
-        response = self.session.post(f"{self.api}/g/s/auth/register", data=data, headers=self.parse_headers(data=data), timeout=timeout)
+        response = self.session.post(f"{self.api}/g/s/auth/register", data=data, timeout=timeout)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)
 
     def restore(self, email: str, password: str):
         """
@@ -394,19 +387,18 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "email": email,
-            "timestamp": int(timestamp() * 1000)
+            "email": email
         })
 
-        response = self.session.post(f"{self.api}/g/s/account/delete-request/cancel", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/account/delete-request/cancel", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def logout(self):
         """
@@ -418,19 +410,18 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "deviceID": self.device_id,
-            "clientType": 100,
-            "timestamp": int(timestamp() * 1000)
+            "clientType": 100
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/logout", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/logout", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
 
             self.authenticated = False
             self.json = None
             self.sid = None
@@ -465,18 +456,18 @@
         else: raise exceptions.SpecifyType()
 
         if age <= 12: raise exceptions.AgeTooLow()
 
         data = json.dumps({
             "age": age,
             "gender": gender,
-            "timestamp": int(timestamp() * 1000)
+
         })
 
-        response = self.session.post(f"{self.api}/g/s/persona/profile/basic", data=data, headers=self.parse_headers(data=data))
+        response = self.session.post(f"{self.api}/g/s/persona/profile/basic", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def verify(self, email: str, code: str):
         """
@@ -492,19 +483,18 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
-            "deviceID": self.device_id,
-            "timestamp": int(timestamp() * 1000)
+            "deviceID": self.device_id
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/check-security-validation", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/check-security-validation", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def request_verify_code(self, email: str, resetPassword: bool = False, timeout: int = None):
         """
@@ -526,15 +516,15 @@
         }
 
         if resetPassword is True:
             data["level"] = 2
             data["purpose"] = "reset-password"
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/auth/request-security-validation", headers=self.parse_headers(data=data), data=data, timeout=timeout)
+        response = self.session.post(f"{self.api}/g/s/auth/request-security-validation", data=data, timeout=timeout)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def activate_account(self, email: str, code: str):
         """
@@ -553,15 +543,15 @@
         data = json.dumps({
             "type": 1,
             "identity": email,
             "data": {"code": code},
             "deviceID": self.device_id
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/activate-email", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/activate-email", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     # Provided by "𝑰 𝑵 𝑻 𝑬 𝑹 𝑳 𝑼 𝑫 𝑬#4082"
     def delete_account(self, password: str):
@@ -578,15 +568,15 @@
         """
 
         data = json.dumps({
             "deviceID": self.device_id,
             "secret": f"0 {password}"
         })
 
-        response = self.session.post(f"{self.api}/g/s/account/delete-request", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/account/delete-request", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def change_password(self, email: str, password: str, code: str):
         """
@@ -614,15 +604,15 @@
                 "level": 2,
                 "deviceID": self.device_id
             },
             "phoneNumberValidationContext": None,
             "deviceID": self.device_id
         })
 
-        response = self.session.post(f"{self.api}/g/s/auth/reset-password", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/auth/reset-password", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def check_device(self, deviceId: str):
         """
@@ -638,26 +628,25 @@
         """
         data = json.dumps({
             "deviceID": deviceId,
             "bundleID": "com.narvii.amino.master",
             "clientType": 100,
             "timezone": -timezone // 1000,
             "systemPushEnabled": True,
-            "locale": locale()[0],
-            "timestamp": int(timestamp() * 1000)
+            "locale": locale()[0]
         })
 
-        response = self.session.post(f"{self.api}/g/s/device", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/device", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             self.configured = True; return response.status_code
 
     def get_account_info(self):
-        response = self.session.get(f"{self.api}/g/s/account", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/account")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfile(json.loads(response.text)["account"]).UserProfile
 
     def upload_media(self, file: BinaryIO, fileType: str):
         """
@@ -685,15 +674,15 @@
         else:
             return json.loads(response.text)["mediaValue"]
 
     def handle_socket_message(self, data):
         return self.resolve(data)
 
     def get_eventlog(self):
-        response = self.session.get(f"{self.api}/g/s/eventlog/profile?language=en", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/eventlog/profile?language=en")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)
 
     def sub_clients(self, start: int = 0, size: int = 25):
         """
@@ -705,23 +694,23 @@
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if not self.authenticated: raise exceptions.NotLoggedIn()
-        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
 
     def sub_clients_profile(self, start: int = 0, size: int = 25):
         if not self.authenticated: raise exceptions.NotLoggedIn()
-        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/community/joined?v=1&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)["userInfoInCommunities"]
 
     def get_user_info(self, userId: str):
         """
@@ -731,15 +720,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfile(json.loads(response.text)["userProfile"]).UserProfile
 
     def watch_ad(self, userId: str = None):
         data = json.dumps(headers.Tapjoy(userId if userId else self.userId).data) 
@@ -756,15 +745,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/chat/thread?type=joined-me&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.ThreadList(json.loads(response.text)["threadList"]).ThreadList
 
     def get_chat_thread(self, chatId: str):
         """
@@ -774,22 +763,22 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfileList(json.loads(response.text)["memberList"]).UserProfileList
 
     def join_chat(self, chatId: str):
         """
@@ -817,15 +806,15 @@
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.parse_headers())
+        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         """
@@ -848,28 +837,27 @@
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType()
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
-            "content": content,
-            "timestamp": int(timestamp() * 1000)
+            "content": content
         }
 
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
 
         data = json.dumps(data)
 
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread", data=data, headers=self.parse_headers(data=data))
+        response = self.session.post(f"{self.api}/g/s/chat/thread", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.Thread(json.loads(response.text)["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
         """
@@ -885,28 +873,27 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType
 
         data = json.dumps({
-            "uids": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "uids": userIds
         })
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/invite", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/invite", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
         if allowRejoin: allowRejoin = 1
         if not allowRejoin: allowRejoin = 0
-        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.parse_headers())
+        response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
         """
@@ -922,15 +909,15 @@
             - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if pageToken is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"{self.api}/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
-        response = self.session.get(url, headers=self.parse_headers())
+        response = self.session.get(url)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.GetMessages(json.loads(response.text)).GetMessages
 
     def get_message_info(self, chatId: str, messageId: str):
         """
@@ -941,15 +928,15 @@
             - **messageId** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.Message(json.loads(response.text)["message"]).Message
 
     def get_community_info(self, comId: str):
         """
@@ -959,15 +946,15 @@
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.Community(json.loads(response.text)["community"]).Community
 
     def search_community(self, aminoId: str):
         """
@@ -977,15 +964,15 @@
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/search/amino-id-and-link?q={aminoId}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/search/amino-id-and-link?q={aminoId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
 
             response = json.loads(response.text)["resultList"]
             if len(response) == 0: raise exceptions.CommunityNotFound(aminoId)
             else: return objects.CommunityList([com["refObject"] for com in response]).CommunityList
@@ -1000,15 +987,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/joined?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
         """
@@ -1020,15 +1007,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/member?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
         """
@@ -1040,15 +1027,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/visitors?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.VisitorsList(json.loads(response.text)).VisitorsList
 
     def get_blocked_users(self, start: int = 0, size: int = 25):
         """
@@ -1059,38 +1046,38 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/block?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/block?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfileList(json.loads(response.text)["userProfileList"]).UserProfileList
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
         if blogId or quizId:
             if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/g/s/blog/{blogId}", headers=self.parse_headers())
+            response = self.session.get(f"{self.api}/g/s/blog/{blogId}")
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else:
                 return objects.GetBlogInfo(json.loads(response.text)).GetBlogInfo
 
         elif wikiId:
-            response = self.session.get(f"{self.api}/g/s/item/{wikiId}", headers=self.parse_headers())
+            response = self.session.get(f"{self.api}/g/s/item/{wikiId}")
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else:
                 return objects.GetBlogInfo(json.loads(response.text)).GetWikiInfo
 
         elif fileId:
-            response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}", headers=self.parse_headers())
+            response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}")
             if response.status_code != 200: 
                 return exceptions.CheckException(response.text)
             else:
                 return objects.SharedFolderFile(json.loads(response.text)["file"]).SharedFolderFile
 
         else: raise exceptions.SpecifyType()
 
@@ -1098,17 +1085,17 @@
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         if blogId or quizId:
             if quizId is not None: blogId = quizId
-            response = self.session.get(f"{self.api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
-        elif wikiId: response = self.session.get(f"{self.api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
-        elif fileId: response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+            response = self.session.get(f"{self.api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}")
+        elif wikiId: response = self.session.get(f"{self.api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}")
+        elif fileId: response = self.session.get(f"{self.api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}")
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
@@ -1121,15 +1108,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <None>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/block/full-list?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/block/full-list?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)["blockerUidList"]
 
     def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
         """
@@ -1148,15 +1135,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommentList(json.loads(response.text)["commentList"]).CommentList
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
         """
@@ -1176,16 +1163,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
-            "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "message": reason
         }
 
         if userId:
             data["objectId"] = userId
             data["objectType"] = 0
 
         elif blogId:
@@ -1198,15 +1184,15 @@
 
         else: raise exceptions.SpecifyType
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/{flg}", data=data, headers=self.parse_headers(data=data))
+        response = self.session.post(f"{self.api}/g/s/{flg}", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
@@ -1253,16 +1239,15 @@
                 "objectId": embedId,
                 "objectType": embedType,
                 "link": embedLink,
                 "title": embedTitle,
                 "content": embedContent,
                 "mediaList": embedImage
             },
-            "extensions": {"mentionedArray": mentions},
-            "timestamp": int(timestamp() * 1000)
+            "extensions": {"mentionedArray": mentions}
         }
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
@@ -1286,15 +1271,15 @@
 
             else: raise exceptions.SpecifyType
 
             data["mediaUploadValue"] = base64.b64encode(file.read()).decode()
 
         data = json.dumps(data)
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
         """
@@ -1309,22 +1294,21 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "adminOpName": 102,
-            "adminOpNote": {"content": reason},
-            "timestamp": int(timestamp() * 1000)
+            "adminOpNote": {"content": reason}
         }
 
         data = json.dumps(data)
         
-        if not asStaff: response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.parse_headers())
-        else: response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.parse_headers(data=data), data=data)
+        if not asStaff: response = self.session.delete(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}")
+        else: response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/message/{messageId}/admin", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def mark_as_read(self, chatId: str, messageId: str):
         """
@@ -1336,19 +1320,18 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
-            "messageId": messageId,
-            "timestamp": int(timestamp() * 1000)
+            "messageId": messageId
         })
         
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/mark-as-read", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/mark-as-read", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def edit_chat(self, chatId: str, doNotDisturb: bool = None, pinChat: bool = None, title: str = None, icon: str = None, backgroundImage: str = None, content: str = None, announcement: str = None, coHosts: list = None, keywords: list = None, pinAnnouncement: bool = None, publishToGlobal: bool = None, canTip: bool = None, viewOnly: bool = None, canInvite: bool = None, fansOnly: bool = None):
         """
@@ -1373,15 +1356,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1390,49 +1373,49 @@
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
-                data = json.dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
+                data = json.dumps({"alertOption": 2})
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
-                data = json.dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
+                data = json.dumps({"alertOption": 1})
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/pin", data=data, headers=self.parse_headers())
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/pin", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not pinChat:
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/unpin", data=data, headers=self.parse_headers())
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/unpin", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
-            data = json.dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
+            data = json.dumps({"media": [100, backgroundImage, None]})
             
-            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data, headers=self.parse_headers(data=data))
+            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data)
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if coHosts is not None:
-            data = json.dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
+            data = json.dumps({"uidList": coHosts})
             
-            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/co-host", data=data, headers=self.parse_headers(data=data))
+            response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/co-host", data=data)
             if response.status_code != 200: res.append(exceptions.CheckException(response.text))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
                 
                 response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/enable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
@@ -1444,40 +1427,40 @@
                 response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/view-only/disable", headers=self.parse_headers(type="application/x-www-form-urlencoded"))
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canInvite is not None:
             if canInvite:
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/enable", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/enable", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canInvite:
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/disable", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/members-can-invite/disable", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         if canTip is not None:
             if canTip:
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/enable", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
             if not canTip:
                 
-                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data, headers=self.parse_headers(data=data))
+                response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/tipping-perm-status/disable", data=data)
                 if response.status_code != 200: res.append(exceptions.CheckException(response.text))
                 else: res.append(response.status_code)
 
         data = json.dumps(data)
         
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}", data=data)
         if response.status_code != 200: res.append(exceptions.CheckException(response.text))
         else: res.append(response.status_code)
 
         return res
 
     def visit(self, userId: str):
         """
@@ -1487,41 +1470,40 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}?action=visit", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}?action=visit")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         url = None
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
         data = {
             "coins": coins,
-            "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "tippingContext": {"transactionId": transactionId}
         }
 
         if blogId is not None: url = f"{self.api}/g/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"{self.api}/g/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
             url = f"{self.api}/g/s/tipping"
 
         if url is None: raise exceptions.SpecifyType()
 
         data = json.dumps(data)
-        response = self.session.post(url, headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(url, data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
@@ -1532,20 +1514,20 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str):
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/member", headers=self.parse_headers())
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/member")
 
         elif isinstance(userId, list):
-            data = json.dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            data = json.dumps({"targetUidList": userId})
             
-            response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/joined", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/joined", data=data)
 
         else: raise exceptions.WrongType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
@@ -1558,15 +1540,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/member/{self.userId}", headers=self.parse_headers())
+        response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/member/{self.userId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def block(self, userId: str):
         """
@@ -1576,15 +1558,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers())
+        response = self.session.post(f"{self.api}/g/s/block/{userId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def unblock(self, userId: str):
         """
@@ -1594,15 +1576,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/block/{userId}", headers=self.parse_headers())
+        response = self.session.delete(f"{self.api}/g/s/block/{userId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def join_community(self, comId: str, invitationId: str = None):
         """
@@ -1613,19 +1595,19 @@
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {}
         if invitationId: data["invitationId"] = invitationId
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/x{comId}/s/community/join", data=data, headers=self.parse_headers(data=data))
+        response = self.session.post(f"{self.api}/x{comId}/s/community/join", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def request_join_community(self, comId: str, message: str = None):
         """
@@ -1636,16 +1618,16 @@
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({"message": message, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/x{comId}/s/community/membership-request", data=data, headers=self.parse_headers(data=data))
+        data = json.dumps({"message": message})
+        response = self.session.post(f"{self.api}/x{comId}/s/community/membership-request", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def leave_community(self, comId: str):
         """
@@ -1655,15 +1637,15 @@
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/x{comId}/s/community/leave", headers=self.parse_headers())
+        response = self.session.post(f"{self.api}/x{comId}/s/community/leave")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def flag_community(self, comId: str, reason: str, flagType: int, isGuest: bool = False):
         """
@@ -1682,22 +1664,21 @@
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = json.dumps({
             "objectId": comId,
             "objectType": 16,
             "flagType": flagType,
-            "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "message": reason
         })
 
         if isGuest: flg = "g-flag"
         else: flg = "flag"
         
-        response = self.session.post(f"{self.api}/x{comId}/s/{flg}", data=data, headers=self.parse_headers(data=data))
+        response = self.session.post(f"{self.api}/x{comId}/s/{flg}", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, backgroundColor: str = None, backgroundImage: str = None, defaultBubbleId: str = None):
         """
@@ -1717,27 +1698,26 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
-            "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
+            "eventSource": "UserProfileView"
         }
 
         if nickname: data["nickname"] = nickname
         if icon: data["icon"] = self.upload_media(icon, "image")
         if content: data["content"] = content
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
         if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def set_privacy_status(self, isAnonymous: bool = False, getNotifications: bool = False):
         """
@@ -1749,23 +1729,23 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {}
 
         if not isAnonymous: data["privacyMode"] = 1
         if isAnonymous: data["privacyMode"] = 2
         if not getNotifications: data["notificationStatus"] = 2
         if getNotifications: data["privacyMode"] = 1
 
         data = json.dumps(data)
-        response = self.session.post(f"{self.api}/g/s/account/visit-settings", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/account/visit-settings", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def set_amino_id(self, aminoId: str):
         """
@@ -1775,16 +1755,16 @@
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/g/s/account/change-amino-id", headers=self.parse_headers(data=data), data=data)
+        data = json.dumps({"aminoId": aminoId})
+        response = self.session.post(f"{self.api}/g/s/account/change-amino-id", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def get_linked_communities(self, userId: str):
         """
@@ -1794,15 +1774,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommunityList(json.loads(response.text)["linkedCommunityList"]).CommunityList
 
     def get_unlinked_communities(self, userId: str):
         """
@@ -1812,15 +1792,15 @@
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile/{userId}/linked-community")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommunityList(json.loads(response.text)["unlinkedCommunityList"]).CommunityList
 
     def reorder_linked_communities(self, comIds: list):
         """
@@ -1830,16 +1810,16 @@
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = json.dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.parse_headers(data=data), data=data)
+        data = json.dumps({"ndcIds": comIds})
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/reorder", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def add_linked_community(self, comId: str):
         """
@@ -1849,15 +1829,15 @@
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers())
+        response = self.session.post(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def remove_linked_community(self, comId: str):
         """
@@ -1867,15 +1847,15 @@
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.delete(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.parse_headers())
+        response = self.session.delete(f"{self.api}/g/s/user-profile/{self.userId}/linked-community/{comId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None):
         """
@@ -1894,37 +1874,36 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if message is None: raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
-            "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "type": 0
         }
 
         if replyTo: data["respondTo"] = replyTo
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/g-comment", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/g-comment", data=data)
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-comment", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-comment", data=data)
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-comment", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-comment", data=data)
 
         else: raise exceptions.SpecifyType
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
@@ -1939,17 +1918,17 @@
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/g-comment/{commentId}", headers=self.parse_headers())
-        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-comment/{commentId}", headers=self.parse_headers())
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-comment/{commentId}", headers=self.parse_headers())
+        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/g-comment/{commentId}")
+        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-comment/{commentId}")
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-comment/{commentId}")
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
@@ -1963,38 +1942,37 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
-            "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "value": 4
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = json.dumps(data)
                 
-                response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
+                response = self.session.post(f"{self.api}/g/s/blog/{blogId}/g-vote?cv=1.2", data=data)
 
             elif isinstance(blogId, list):
                 data["targetIdList"] = blogId
                 data = json.dumps(data)
                 
-                response = self.session.post(f"{self.api}/g/s/feed/g-vote", headers=self.parse_headers(data=data), data=data)
+                response = self.session.post(f"{self.api}/g/s/feed/g-vote", data=data)
 
             else: raise exceptions.WrongType(type(blogId))
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-vote?cv=1.2", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/g-vote?cv=1.2", data=data)
 
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
@@ -2008,16 +1986,16 @@
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers())
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        if blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView")
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView")
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
@@ -2033,35 +2011,34 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = {
-            "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "value": 4
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", data=data)
 
         elif blogId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?cv=1.2&value=1", data=data)
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             data = json.dumps(data)
             
-            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.parse_headers(data=data), data=data)
+            response = self.session.post(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?cv=1.2&value=1", data=data)
 
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
@@ -2077,17 +2054,17 @@
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.parse_headers())
-        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
-        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.parse_headers())
+        if userId: response = self.session.delete(f"{self.api}/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView")
+        elif blogId: response = self.session.delete(f"{self.api}/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView")
+        elif wikiId: response = self.session.delete(f"{self.api}/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView")
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
@@ -2099,15 +2076,15 @@
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/membership?force=true", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/membership?force=true")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.Membership(json.loads(response.text)).Membership
 
     def get_ta_announcements(self, language: str = "en", start: int = 0, size: int = 25):
         """
@@ -2121,15 +2098,15 @@
 
         **Returns**
             - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
-        response = self.session.get(f"{self.api}/g/s/announcement?language={language}&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/announcement?language={language}&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
 
     def get_wallet_info(self):
         """
@@ -2139,15 +2116,15 @@
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/wallet", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/wallet")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.WalletInfo(json.loads(response.text)["wallet"]).WalletInfo
 
     def get_wallet_history(self, start: int = 0, size: int = 25):
         """
@@ -2158,15 +2135,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/wallet/coin/history?start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/wallet/coin/history?start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.WalletHistory(json.loads(response.text)["coinHistoryList"]).WalletHistory
 
     def get_from_deviceid(self, deviceId: str):
         """
@@ -2195,15 +2172,15 @@
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/link-resolution?q={code}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/link-resolution?q={code}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
 
     def get_from_id(self, objectId: str, objectType: int, comId: str = None):
         """
@@ -2218,20 +2195,19 @@
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         data = json.dumps({
             "objectId": objectId,
             "targetCode": 1,
-            "objectType": objectType,
-            "timestamp": int(timestamp() * 1000)
+            "objectType": objectType
         })
         
-        if comId: response = self.session.post(f"{self.api}/g/s-x{comId}/link-resolution", headers=self.parse_headers(data=data), data=data)
-        else: response = self.session.post(f"{self.api}/g/s/link-resolution", headers=self.parse_headers(data=data), data=data)
+        if comId: response = self.session.post(f"{self.api}/g/s-x{comId}/link-resolution", data=data)
+        else: response = self.session.post(f"{self.api}/g/s/link-resolution", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.FromCode(json.loads(response.text)["linkInfoV2"]).FromCode
 
     def get_supported_languages(self):
         """
@@ -2241,15 +2217,15 @@
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`List of Supported Languages <List>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/community-collection/supported-languages?start=0&size=100", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/community-collection/supported-languages?start=0&size=100")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)["supportedLanguages"]
 
     def claim_new_user_coupon(self):
         """
@@ -2259,15 +2235,15 @@
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.post(f"{self.api}/g/s/coupon/new-user-coupon/claim", headers=self.parse_headers())
+        response = self.session.post(f"{self.api}/g/s/coupon/new-user-coupon/claim")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def get_subscriptions(self, start: int = 0, size: int = 25):
         """
@@ -2278,15 +2254,15 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List <List>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/store/subscription?objectType=122&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/store/subscription?objectType=122&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return json.loads(response.text)["storeSubscriptionItemList"]
 
     def get_all_users(self, start: int = 0, size: int = 25):
         """
@@ -2297,34 +2273,34 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        response = self.session.get(f"{self.api}/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/user-profile?type=recent&start={start}&size={size}")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
 
     def accept_host(self, chatId: str, requestId: str):
         data = json.dumps({})
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
         self.accept_host(chatId, requestId)
 
     # Contributed by 'https://github.com/LynxN1'
     def link_identify(self, code: str):
-        response = self.session.get(f"{self.api}/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}")
         return json.loads(response.text)
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
 
         **Parameters**
@@ -2337,15 +2313,15 @@
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = json.dumps({
             "uid": userId
         })
 
-        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/vvchat-presenter/invite", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/chat/thread/{chatId}/vvchat-presenter/invite", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def wallet_config(self, level: int):
         """
@@ -2358,38 +2334,36 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = json.dumps({
-            "adsLevel": level,
-            "timestamp": int(timestamp() * 1000)
+            "adsLevel": level
         })
 
-        response = self.session.post(f"{self.api}/g/s/wallet/ads/config", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/wallet/ads/config", data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return response.status_code
 
     def purchase(self, objectId: str, isAutoRenew: bool = False):
         data = json.dumps({
             "objectId": objectId,
             "objectType": 114,
             "v": 1,
             "paymentContext":
             {
                 "discountStatus": 0,
                 "isAutoRenew": isAutoRenew
-            },
-            "timestamp": timestamp()
+            }
         })
 
-        response = self.session.post(f"{self.api}/g/s/store/purchase", headers=self.parse_headers(data=data), data=data)
+        response = self.session.post(f"{self.api}/g/s/store/purchase", data=data)
         if response.status_code != 200: return exceptions.CheckException(json.loads(response.text()))
         else: return response.status_code
 
     def get_public_communities(self, language: str = "en", size: int = 25):
         """
         Get public communites
 
@@ -2398,12 +2372,12 @@
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        response = self.session.get(f"{self.api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.parse_headers())
+        response = self.session.get(f"{self.api}/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t")
         if response.status_code != 200: 
             return exceptions.CheckException(response.text)
         else:
             return objects.CommunityList(json.loads(response.text)["communityList"]).CommunityList
```

### Comparing `zamino_fix-1.1.5/ZAminofix/lib/util/exceptions.py` & `zamino_fix-1.1.6/ZAminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/lib/util/headers.py` & `zamino_fix-1.1.6/ZAminofix/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/lib/util/helpers.py` & `zamino_fix-1.1.6/ZAminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/lib/util/objects.py` & `zamino_fix-1.1.6/ZAminofix/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/ZAminofix/socket.py` & `zamino_fix-1.1.6/ZAminofix/socket.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,105 +6,116 @@
 from threading import Thread
 from sys import _getframe as getframe
 
 from .lib.util.helpers import gen_deviceId
 from .lib.util import objects, helpers
 
 class SocketHandler:
-    def __init__(self, client, socket_trace = False, debug = False):
-        self.socket_url = "wss://ws1.aminoapps.com"
+    SOCKET_URL = "wss://ws1.aminoapps.com"
+    RECONNECT_TIME = 180
+
+    def __init__(self, client, socket_trace=False, debug=False):
+        self.socket_url = self.SOCKET_URL
         self.client = client
         self.debug = debug
         self.active = False
         self.headers = None
         self.socket = None
         self.socket_thread = None
-        self.reconnectTime = 180
-        self.socket_thread = None
-
-        if self.socket_enabled:
-            self.reconnect_thread = Thread(target=self.reconnect_handler)
-            self.reconnect_thread.start()
+        self.reconnect_thread = None
+        self.previous_socket = None  # Added to keep track of the previous socket
 
         websocket.enableTrace(socket_trace)
+        self.run_amino_socket()
 
     def reconnect_handler(self):
-        # Made by enchart#3410 thx
-        # Fixed by The_Phoenix#3967
         while True:
-            time.sleep(self.reconnectTime)
-
+            time.sleep(self.RECONNECT_TIME)
             if self.active:
-                if self.debug is True:
+                if self.debug:
                     print(f"[socket][reconnect_handler] Reconnecting Socket")
-
                 self.close()
                 self.run_amino_socket()
 
     def handle_message(self, ws, data):
         self.client.handle_socket_message(data)
-        return
+
+    def handle_close(self, ws, close_status_code, close_msg):
+        if self.debug:
+            print(f"[socket][close] Socket closed: {close_status_code} - {close_msg}")
+        self.active = False
+
+    def handle_error(self, ws, error):
+        if self.debug:
+            print(f"[socket][error] Socket error: {error}")
+        self.active = False
 
     def send(self, data):
-        if self.debug is True:
-            print(f"[socket][send] Sending Data : {data}")
+        if self.debug:
+            print(f"[socket][send] Sending Data: {data}")
         
-        if not self.socket_thread:
+        if not self.socket_thread or not self.socket_thread.is_alive():
             self.run_amino_socket()
             time.sleep(5)
-
-        self.socket.send(data)
+        try:
+            self.socket.send(data)
+        except Exception as e:
+            if self.debug:
+                print(f"[socket][send] Error sending data: {e}")
+            self.run_amino_socket()
 
     def run_amino_socket(self):
         try:
-            if self.debug is True:
+            if self.debug:
                 print(f"[socket][start] Starting Socket")
 
-            if self.client.sid is None:
+            if not self.client.sid:
                 return
 
             final = f"{self.client.device_id}|{int(time.time() * 1000)}"
-
             self.headers = {
                 "NDCDEVICEID": gen_deviceId() if self.client.autoDevice else self.client.device_id,
                 "NDCAUTH": f"sid={self.client.sid}",
                 "NDC-MSG-SIG": helpers.signature(final)
             }
 
             self.socket = websocket.WebSocketApp(
                 f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
-                on_message = self.handle_message,
-                header = self.headers
+                on_message=self.handle_message,
+                on_close=self.handle_close,
+                on_error=self.handle_error,
+                header=self.headers
             )
 
             self.active = True
+            self.previous_socket = self.socket
             self.socket_thread = Thread(target=self.socket.run_forever)
             self.socket_thread.start()
 
-            if self.reconnect_thread is None:
+            if not self.reconnect_thread:
                 self.reconnect_thread = Thread(target=self.reconnect_handler)
                 self.reconnect_thread.start()
             
-            if self.debug is True:
+            if self.debug:
                 print(f"[socket][start] Socket Started")
         except Exception as e:
-            print(e)
+            if self.debug:
+                print(f"[socket][start] Error starting socket: {e}")
 
     def close(self):
-        if self.debug is True:
+        if self.debug:
             print(f"[socket][close] Closing Socket")
-
         self.active = False
         try:
-            self.socket.close()
+            if self.previous_socket:
+                self.previous_socket.close()
         except Exception as closeError:
-            if self.debug is True:
-                print(f"[socket][close] Error while closing Socket : {closeError}")
+            if self.debug:
+                print(f"[socket][close] Error while closing Socket: {closeError}")
 
-        return
 
 class Callbacks:
     def __init__(self, client):
         self.client = client
         self.handlers = {}
 
         self.methods = {
```

### Comparing `zamino_fix-1.1.5/ZAminofix/sub_client.py` & `zamino_fix-1.1.6/ZAminofix/sub_client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.5/setup.py` & `zamino_fix-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="ZAmino.fix",
     author="ZOOM",
-    version="1.1.5",
+    version="1.1.6",
     description="Aminofix update. https://t.me/ZAminoZ",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
     	'ZAmino'
     	'ZAmino.fix'
```

