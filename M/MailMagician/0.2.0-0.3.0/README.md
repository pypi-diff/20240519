# Comparing `tmp/MailMagician-0.2.0.tar.gz` & `tmp/MailMagician-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MailMagician-0.2.0.tar", last modified: Tue Apr 11 08:21:44 2023, max compression
+gzip compressed data, was "MailMagician-0.3.0.tar", last modified: Sun May 19 03:41:09 2024, max compression
```

## Comparing `MailMagician-0.2.0.tar` & `MailMagician-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:21:44.007055 MailMagician-0.2.0/
--rw-rw-rw-   0        0        0     1087 2023-04-11 07:52:28.000000 MailMagician-0.2.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-11 08:21:43.993052 MailMagician-0.2.0/MailMagician.egg-info/
--rw-rw-rw-   0        0        0      420 2023-04-11 08:21:43.000000 MailMagician-0.2.0/MailMagician.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-11 08:21:43.000000 MailMagician-0.2.0/MailMagician.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:21:43.000000 MailMagician-0.2.0/MailMagician.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 08:21:43.000000 MailMagician-0.2.0/MailMagician.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      420 2023-04-11 08:21:44.006054 MailMagician-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-04-11 07:52:28.000000 MailMagician-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:21:44.002054 MailMagician-0.2.0/mailmagician/
--rw-rw-rw-   0        0        0      102 2023-04-11 08:18:07.000000 MailMagician-0.2.0/mailmagician/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-04-11 07:53:33.000000 MailMagician-0.2.0/mailmagician/_mailbot.py
--rw-rw-rw-   0        0        0      203 2023-04-11 08:17:38.000000 MailMagician-0.2.0/mailmagician/_smtp_server.py
--rw-rw-rw-   0        0        0       42 2023-04-11 08:21:44.008055 MailMagician-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      659 2023-04-11 08:19:06.000000 MailMagician-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 03:41:09.804179 MailMagician-0.3.0/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2024-05-19 03:29:14.000000 MailMagician-0.3.0/LICENSE
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 03:41:09.803333 MailMagician-0.3.0/MailMagician.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 03:41:09.000000 MailMagician-0.3.0/MailMagician.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      249 2024-05-19 03:41:09.000000 MailMagician-0.3.0/MailMagician.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-19 03:41:09.000000 MailMagician-0.3.0/MailMagician.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2024-05-19 03:41:09.000000 MailMagician-0.3.0/MailMagician.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      443 2024-05-19 03:41:09.804052 MailMagician-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)       53 2024-05-19 03:29:14.000000 MailMagician-0.3.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-19 03:41:09.803833 MailMagician-0.3.0/mailmagician/
+-rw-r--r--   0 root         (0) staff       (20)      100 2024-05-19 03:29:14.000000 MailMagician-0.3.0/mailmagician/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1593 2024-05-19 03:32:04.000000 MailMagician-0.3.0/mailmagician/_mailbot.py
+-rw-r--r--   0 root         (0) staff       (20)      194 2024-05-19 03:29:14.000000 MailMagician-0.3.0/mailmagician/_smtp_server.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-19 03:41:09.804245 MailMagician-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      636 2024-05-19 03:35:09.000000 MailMagician-0.3.0/setup.py
```

