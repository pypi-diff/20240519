# Comparing `tmp/MailMagician-0.5.0.tar.gz` & `tmp/MailMagician-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailMagician-0.5.0.tar", last modified: Sun May 19 13:35:48 2024, max compression
+gzip compressed data, was "MailMagician-0.6.0.tar", last modified: Sun May 19 13:36:29 2024, max compression
```

## Comparing `MailMagician-0.5.0.tar` & `MailMagician-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.528538 MailMagician-0.5.0/
--rw-r--r--   0 root         (0) staff       (20)     1066 2024-05-19 03:29:14.000000 MailMagician-0.5.0/LICENSE
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.527821 MailMagician-0.5.0/MailMagician.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      249 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2024-05-19 13:35:48.000000 MailMagician-0.5.0/MailMagician.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:35:48.528428 MailMagician-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       53 2024-05-19 03:29:14.000000 MailMagician-0.5.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:35:48.528171 MailMagician-0.5.0/mailmagician/
--rw-r--r--   0 root         (0) staff       (20)      111 2024-05-19 13:35:38.000000 MailMagician-0.5.0/mailmagician/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2153 2024-05-19 13:35:31.000000 MailMagician-0.5.0/mailmagician/_mailbot.py
--rw-r--r--   0 root         (0) staff       (20)      194 2024-05-19 03:29:14.000000 MailMagician-0.5.0/mailmagician/_smtp_server.py
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-19 13:35:48.528580 MailMagician-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      636 2024-05-19 13:35:43.000000 MailMagician-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:36:29.090750 MailMagician-0.6.0/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2024-05-19 03:29:14.000000 MailMagician-0.6.0/LICENSE
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:36:29.089924 MailMagician-0.6.0/MailMagician.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:36:29.000000 MailMagician-0.6.0/MailMagician.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      249 2024-05-19 13:36:29.000000 MailMagician-0.6.0/MailMagician.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-19 13:36:29.000000 MailMagician-0.6.0/MailMagician.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2024-05-19 13:36:29.000000 MailMagician-0.6.0/MailMagician.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 13:36:29.090623 MailMagician-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       53 2024-05-19 03:29:14.000000 MailMagician-0.6.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 13:36:29.090389 MailMagician-0.6.0/mailmagician/
+-rw-r--r--   0 root         (0) staff       (20)      111 2024-05-19 13:35:38.000000 MailMagician-0.6.0/mailmagician/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1686 2024-05-19 13:36:23.000000 MailMagician-0.6.0/mailmagician/_mailbot.py
+-rw-r--r--   0 root         (0) staff       (20)      194 2024-05-19 03:29:14.000000 MailMagician-0.6.0/mailmagician/_smtp_server.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-19 13:36:29.090798 MailMagician-0.6.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      636 2024-05-19 13:36:27.000000 MailMagician-0.6.0/setup.py
```

### Comparing `MailMagician-0.5.0/LICENSE` & `MailMagician-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MailMagician-0.5.0/mailmagician/_mailbot.py` & `MailMagician-0.6.0/mailmagician/_mailbot.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,28 +27,18 @@
         msg["Subject"] = Header(subject, charset='utf-8')
         msg["From"] = gmail_user
         msg["To"] = sentTo
 
         msg.attach(MIMEText(email_text, 'plain', 'utf-8'))
 
         if attachment:
-            if isinstance(attachment, UploadFile):
-                # 如果 attachment 是 UploadFile 类型
-                attachment_name = attachment.filename
-                payload = await attachment.read()  # 异步读取文件内容
-            else:
-                # 否则假设 attachment 是文件路径
-                attachment_name = os.path.basename(attachment)
-                with open(attachment, 'rb') as f:
-                    payload = f.read()
-            
             part = MIMEBase('application', 'octet-stream')
-            part.set_payload(payload)
+            part.set_payload(attachment.payload)
             encoders.encode_base64(part)
-            part.add_header('Content-Disposition', f'attachment; filename="{attachment_name}"')
+            part.add_header('Content-Disposition', f'attachment; filename="{attachment.filename}"')
             msg.attach(part)
 
         try:
             server = smtplib.SMTP_SSL(self.smtp_server)
             server.ehlo()
             server.login(gmail_user, gmail_password)
             server.sendmail(sent_from, sentTo, msg.as_string())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MailMagician-0.5.0/setup.py` & `MailMagician-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = [] 
 setup(
     name="MailMagician",
-    version="0.5.0",
+    version="0.6.0",
     author="Tao Xiang",
     author_email="tao.xiang@tum.de",
     description="A package of email robots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/leoxiang66/MailBot",
     packages=find_packages(),
```

