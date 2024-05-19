# Comparing `tmp/cabinet-2024.5.18.1.tar.gz` & `tmp/cabinet-2024.5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.5.18.1.tar", last modified: Sun May 19 00:50:43 2024, max compression
+gzip compressed data, was "cabinet-2024.5.7.1.tar", last modified: Wed May  8 04:43:54 2024, max compression
```

## Comparing `cabinet-2024.5.18.1.tar` & `cabinet-2024.5.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-19 00:50:43.691005 cabinet-2024.5.18.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.5.18.1/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7972 2024-05-19 00:50:43.691005 cabinet-2024.5.18.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7620 2024-05-19 00:50:09.000000 cabinet-2024.5.18.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.5.18.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-05-19 00:50:43.691005 cabinet-2024.5.18.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-19 00:50:43.687005 cabinet-2024.5.18.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-19 00:50:43.687005 cabinet-2024.5.18.1/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.5.18.1/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.5.18.1/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38351 2024-05-19 00:49:17.000000 cabinet-2024.5.18.1/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.5.18.1/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.5.18.1/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6528 2024-05-19 00:48:58.000000 cabinet-2024.5.18.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-19 00:50:43.691005 cabinet-2024.5.18.1/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7972 2024-05-19 00:50:43.000000 cabinet-2024.5.18.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-05-19 00:50:43.000000 cabinet-2024.5.18.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-19 00:50:43.000000 cabinet-2024.5.18.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-05-19 00:50:43.000000 cabinet-2024.5.18.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-05-19 00:50:43.000000 cabinet-2024.5.18.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.5.7.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38351 2024-05-08 04:41:54.000000 cabinet-2024.5.7.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.5.7.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.5.7.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.5.7.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.5.18.1/LICENSE` & `cabinet-2024.5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.5.18.1/PKG-INFO` & `cabinet-2024.5.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.5.18.1
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -126,15 +126,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

### Comparing `cabinet-2024.5.18.1/README.md` & `cabinet-2024.5.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

### Comparing `cabinet-2024.5.18.1/setup.cfg` & `cabinet-2024.5.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.05.18.1
+version = 2024.05.07.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.5.18.1/src/cabinet/cabinet.py` & `cabinet-2024.5.7.1/src/cabinet/cabinet.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.5.18.1/src/cabinet/constants.py` & `cabinet-2024.5.7.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.5.18.1/src/cabinet/mail.py` & `cabinet-2024.5.7.1/src/cabinet/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 Does not support Gmail.
 
 A throwaway email is highly recommended.
 """
 
 import smtplib
 from urllib.parse import unquote
-import subprocess
-import socket
-import shlex
-import pwd
 import sys
+import pwd
 import os
+import subprocess
+import shlex
 from typing import List
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 import cabinet
 
 class Mail:
     """
@@ -53,29 +52,29 @@
         Args:
         - subject (str): The subject of the email.
         - body (str): The body of the email.
         - signature (str): The signature to include at the end of the email.
         - to_addr (List): A list of email addresses to send the email to.
         - from_name (str, optional): The name to appear in the "From" field of the email.
             Reads from cabinet -> email -> from_name if unset.
-            If this is unset, defaults to machine's hostname or `Cabinet`
+            If this is unset, defaults to os.getenv("HOSTNAME") or `Cabinet`
         - logging_enabled (bool, optional): Whether to log the email send event.
             Defaults to True.
         - is_quiet: Whether to suppress log output.
             Defaults to False.
 
         Raises:
         - smtplib.SMTPAuthenticationError: If the SMTP server rejects the login credentials.
 
         Gmail will almost certainly not work.
         """
 
-        hostname = socket.gethostname()
+        hostname = os.getenv("HOSTNAME")
         if hostname:
-            hostname = hostname.capitalize().replace(".local", "")
+            hostname = hostname.capitalize()
 
         cab_from_name = self.cab.get("email", "from_name") or hostname or "Cabinet"
 
         # send IP if reminder came directly from outside of server
         client_name = os.getenv('SSH_CONNECTION')
 
         if client_name:
```

### Comparing `cabinet-2024.5.18.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.5.18.1
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -126,15 +126,15 @@
 
 file:
 ```
 {
     "email": {
         "from": "throwaway@example.com",
         "from_pw": "example",
-        "from_name": "Cabinet (or other name of your choice)",
+        "from_name": "Cabinet",
         "to": "destination@protonmail.com",
         "smtp_server": "example.com",
         "imap_server": "example.com",
         "port": 123
     }
 }
 ```
```

