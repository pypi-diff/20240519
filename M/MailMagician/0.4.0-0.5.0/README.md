# Comparing `tmp/MailMagician-0.4.0.tar.gz` & `tmp/MailMagician-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailMagician-0.4.0.tar", last modified: Sun May 19 13:29:17 2024, max compression
+gzip compressed data, was "MailMagician-0.5.0.tar", last modified: Sun May 19 13:35:48 2024, max compression
```

## Comparing `MailMagician-0.4.0.tar` & `MailMagician-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:29:17.733554 MailMagician-0.4.0/
--rw-r--r--   0 root         (0) staff       (20)     1066 2024-05-19 03:29:14.000000 MailMagician-0.4.0/LICENSE
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:29:17.732255 MailMagician-0.4.0/MailMagician.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:29:17.000000 MailMagician-0.4.0/MailMagician.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      249 2024-05-19 13:29:17.000000 MailMagician-0.4.0/MailMagician.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-19 13:29:17.000000 MailMagician-0.4.0/MailMagician.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2024-05-19 13:29:17.000000 MailMagician-0.4.0/MailMagician.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:29:17.733447 MailMagician-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       53 2024-05-19 03:29:14.000000 MailMagician-0.4.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:29:17.733261 MailMagician-0.4.0/mailmagician/
--rw-r--r--   0 root         (0) staff       (20)      100 2024-05-19 03:29:14.000000 MailMagician-0.4.0/mailmagician/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1602 2024-05-19 13:25:53.000000 MailMagician-0.4.0/mailmagician/_mailbot.py
--rw-r--r--   0 root         (0) staff       (20)      194 2024-05-19 03:29:14.000000 MailMagician-0.4.0/mailmagician/_smtp_server.py
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-19 13:29:17.733596 MailMagician-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      636 2024-05-19 13:25:58.000000 MailMagician-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.528538 MailMagician-0.5.0/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2024-05-19 03:29:14.000000 MailMagician-0.5.0/LICENSE
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.527821 MailMagician-0.5.0/MailMagician.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      249 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:35:48.528428 MailMagician-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       53 2024-05-19 03:29:14.000000 MailMagician-0.5.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.528171 MailMagician-0.5.0/mailmagician/
+-rw-r--r--   0 root         (0) staff       (20)      111 2024-05-19 13:35:38.000000 MailMagician-0.5.0/mailmagician/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     2153 2024-05-19 13:35:31.000000 MailMagician-0.5.0/mailmagician/_mailbot.py
+-rw-r--r--   0 root         (0) staff       (20)      194 2024-05-19 03:29:14.000000 MailMagician-0.5.0/mailmagician/_smtp_server.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-19 13:35:48.528580 MailMagician-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      636 2024-05-19 13:35:43.000000 MailMagician-0.5.0/setup.py
```

### Comparing `MailMagician-0.4.0/LICENSE` & `MailMagician-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MailMagician-0.4.0/mailmagician/_mailbot.py` & `MailMagician-0.5.0/mailmagician/_mailbot.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,48 +2,59 @@
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email import encoders
 from email.header import Header
 import os
 
+class Attachment:
+    def __init__(self,filename:str, payload:bytes) -> None:
+        self.filename = filename
+        self.payload = payload
 
 class Mailbot():
     def __init__(self, email_account: str, password: str, smtp_server: str = 'smtp.126.com'):
         self.gmail_user = email_account
         self.gmail_password = password
         self.smtp_server = smtp_server
 
-    def send(self, sentTo, subject, msgBody, attachment=None):
+    async def send(self, sentTo, subject, msgBody, attachment:Attachment=None):
         gmail_user = self.gmail_user
         sent_from = self.gmail_user
         gmail_password = self.gmail_password
         email_text = msgBody
-        
 
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, charset='utf-8')
         msg["From"] = gmail_user
         msg["To"] = sentTo
 
         msg.attach(MIMEText(email_text, 'plain', 'utf-8'))
 
         if attachment:
-            attachment_name = os.path.basename(attachment)
+            if isinstance(attachment, UploadFile):
+                # 如果 attachment 是 UploadFile 类型
+                attachment_name = attachment.filename
+                payload = await attachment.read()  # 异步读取文件内容
+            else:
+                # 否则假设 attachment 是文件路径
+                attachment_name = os.path.basename(attachment)
+                with open(attachment, 'rb') as f:
+                    payload = f.read()
+            
             part = MIMEBase('application', 'octet-stream')
-            part.set_payload(open(attachment, 'rb').read())
+            part.set_payload(payload)
             encoders.encode_base64(part)
-            part.add_header('Content-Disposition', f'attachment; filename= {attachment_name}')
+            part.add_header('Content-Disposition', f'attachment; filename="{attachment_name}"')
             msg.attach(part)
 
         try:
             server = smtplib.SMTP_SSL(self.smtp_server)
             server.ehlo()
             server.login(gmail_user, gmail_password)
-
             server.sendmail(sent_from, sentTo, msg.as_string())
             server.close()
 
             print('Email sent!')
         except Exception as e:
             print('Something went wrong...')
             raise e
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `MailMagician-0.4.0/setup.py` & `MailMagician-0.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = [] 
 setup(
     name="MailMagician",
-    version="0.4.0",
+    version="0.5.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of email robots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/MailBot",
     packages=find_packages(),
```

