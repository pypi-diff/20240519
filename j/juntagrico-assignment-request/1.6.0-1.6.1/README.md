# Comparing `tmp/juntagrico-assignment-request-1.6.0.tar.gz` & `tmp/juntagrico_assignment_request-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico-assignment-request-1.6.0.tar", last modified: Mon Jan  8 05:23:52 2024, max compression
+gzip compressed data, was "juntagrico_assignment_request-1.6.1.tar", last modified: Sat May 18 22:55:44 2024, max compression
```

## Comparing `juntagrico-assignment-request-1.6.0.tar` & `juntagrico_assignment_request-1.6.1.tar`

### file list

```diff
@@ -1,57 +1,72 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.581544 juntagrico-assignment-request-1.6.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     7651 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      228 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/MANIFEST.in
--rw-r--r--   0 dave      (1000) dave      (1000)    14762 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     4602 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.569543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/
--rw-rw-r--   0 dave      (1000) dave      (1000)       22 2024-01-08 05:23:29.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admin.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.569543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1480 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/assignment_request_admin.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1723 2024-01-08 05:08:09.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/apps.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2770 2024-01-08 05:04:55.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/forms.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1718 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/hack.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/
--rw-rw-r--   0 dave      (1000) dave      (1000)      696 2024-01-08 03:15:40.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1656 2024-01-08 04:43:28.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/adminnotification.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1105 2024-01-08 04:43:28.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/membernotification.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2587 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1676 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3229 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      775 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8794 2024-01-08 04:25:20.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/models.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.565543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/
--rwxrwxr-x   0 dave      (1000) dave      (1000)      772 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/edit.html
--rwxrwxr-x   0 dave      (1000) dave      (1000)     3750 2024-01-08 03:55:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/list.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.565543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/
--rw-rw-r--   0 dave      (1000) dave      (1000)      900 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      910 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      794 2024-01-08 04:08:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/
--rw-rw-r--   0 dave      (1000) dave      (1000)      603 2024-01-08 04:08:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      733 2024-01-08 04:08:45.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      652 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/
--rw-rw-r--   0 dave      (1000) dave      (1000)      310 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/summary.txt
--rwxrwxr-x   0 dave      (1000) dave      (1000)     4265 2024-01-08 03:54:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/request.html
--rwxrwxr-x   0 dave      (1000) dave      (1000)      805 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/respond.html
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/
--rw-rw-r--   0 dave      (1000) dave      (1000)      422 2024-01-08 04:47:19.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/admin_menu.html
--rw-rw-r--   0 dave      (1000) dave      (1000)      496 2024-01-08 04:52:43.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/user_menu.html
--rw-rw-r--   0 dave      (1000) dave      (1000)      910 2024-01-08 03:59:41.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/urls.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      570 2024-01-08 03:15:40.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/utils.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5577 2024-01-08 05:04:55.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/views.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/
--rw-r--r--   0 dave      (1000) dave      (1000)    14762 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2316 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       21 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       30 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1470 2024-01-08 05:16:43.000000 juntagrico-assignment-request-1.6.0/pyproject.toml
--rw-rw-r--   0 dave      (1000) dave      (1000)       42 2024-01-08 05:22:32.000000 juntagrico-assignment-request-1.6.0/requirements.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-01-08 05:23:52.581544 juntagrico-assignment-request-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.891114 juntagrico_assignment_request-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-18 22:55:44.891114 juntagrico_assignment_request-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.883114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.883114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/admins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/admins/assignment_request_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/hack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.883114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/adminnotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/membernotification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0005_alter_assignmentrequest_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0006_alter_assignmentrequest_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.879114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.879114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/static/juntagrico_assignment_request/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/static/juntagrico_assignment_request/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/static/juntagrico_assignment_request/js/request.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.879114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      998 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/edit.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3812 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.879114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/snippets/summary.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4679 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/request.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      805 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/respond.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/snippets/messages.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.879114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.887114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/juntagrico/menu/user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.891114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/test_assignment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/test_assignment_request_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/tests/test_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:55:44.891114 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-18 22:55:44.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-18 22:55:44.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:55:44.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 22:55:44.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 22:55:44.000000 juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 22:55:40.000000 juntagrico_assignment_request-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:55:44.891114 juntagrico_assignment_request-1.6.1/setup.cfg
```

### Comparing `juntagrico-assignment-request-1.6.0/LICENSE` & `juntagrico_assignment_request-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/PKG-INFO` & `juntagrico_assignment_request-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-assignment-request
-Version: 1.6.0
+Version: 1.6.1
 Summary: Allows members to request assignments for jobs they have done, that were not announced.
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -167,14 +167,15 @@
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://www.juntagrico.org
 Project-URL: Issues, https://github.com/juntagrico/juntagrico-assignment-request/issues
+Project-URL: Changelog, https://github.com/juntagrico/juntagrico-assignment-request/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -184,53 +185,71 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: juntagrico==1.6.0rc3
+Requires-Dist: juntagrico>=1.6.0
 
 # juntagrico_assignment_request
 
 [![juntagrico-ci](https://github.com/juntagrico/juntagrico-assignment-request/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-assignment-request/actions/workflows/juntagrico-ci.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/6c1a453b157b9395a858/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-assignment-request/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/6c1a453b157b9395a858/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-assignment-request/test_coverage)
 [![image](https://img.shields.io/pypi/v/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/l/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/pyversions/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/status/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/dm/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request/)
 [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-assignment-request.svg)](https://github.com/juntagrico/juntagrico-assignment-request)
 [![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-assignment-request)](https://github.com/juntagrico/juntagrico-assignment-request)
-[![Requirements Status](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements/?branch=main)
 
 This is an extension for juntagrico. You can find more information about juntagrico here
 (https://github.com/juntagrico/juntagrico)
 
 It allows members to request assignments for jobs they have done, that were not announced.
 
 ## Installation
 
 1. Add `juntagrico-assignment-request` to your `requirements.txt`
-2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py`
+2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py` **above** `juntagrico`
 3. Add `path(r'', include('juntagrico_assignment_request.urls')),` at the end of your `urls.py`
-4. Redeploy your project
+4. Redeploy your project (and apply migrations)
 
 ## Configuration
 
-When requesting an assignment, members can select the person that can confirm that they did a job.
+When requesting an assignment, members can select the person (confirmer) that can confirm that they did a job.
 To add people to this selection you will have to add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze bestätigen`
 
+If you want to allow an activity area coordinator to confirm requests, but only on the areas they coordinate,
+add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze im eigenen Tätigkeitsbereich bestätigen`
+
 Only the selected confirmer, will be informed about the request by email and can see the request.
 
 If members don't select any confirmer all users with the following permission will receive a notification and can see the request: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Wird über nicht abgesprochene Arbeitseinsätze informiert`
 
 The [ASSIGNMENT_UNIT](https://juntagrico.readthedocs.io/en/latest/settings.html?highlight=ASSIGNMENT_UNIT#assignment-unit) setting is respected.
 
+### ASSIGNMENT_REQUEST_AREAS
+
+If you need to limit the activity areas that can be selected in the requests,
+set this setting to a function, that takes an `ActivityArea` queryset as the first argument
+and returns a filtered queryset.
+By default, all activity areas can be selected.
+
+Example: Include only visible activity areas:
+
+```python
+def only_visible(queryset):
+    return queryset.filter(hidden=False)
+
+ASSIGNMENT_REQUEST_AREAS = only_visible
+```
+
 ## Usage
 
 1. Members will see a new entry in the menu to request assignments
 2. They are presented with a form to fill out the details of the job they did
 3. Below the form, they see a list of assignments that they already sent with the option to edit or delete them
 4. Upon sending the form, the selected confirmer (or the fallback users) will be informed by email
 5. The confirmer can modify the assignment amount, accept, deny or just send a message to the member
@@ -239,29 +258,32 @@
 
 ## Admin modifications
 
 The extension creates job types and jobs on the fly behind the scenes as they are needed to create the assignments and show them to the member that made them.
 In order to not clutter the admin views with automatically generated content, these jobs and job types are hidden.
 As a side effect there will be assignments that have a valid job link, but when you follow that job, you will be told that no job with the given id exists.
 
-## Release Notes
+## Screenshots
+
+New menu entry
+
+![New menu entry](doc/01_menu_entry.png)
 
-## 1.5
+Request Form
 
-Upgrade to Juntagrico 1.5
+![Request Form](doc/02_request_form)
 
-## 1.4
+Overview about reported assignments
 
-Upgrade to Juntagrico 1.4
+![Overview](doc/03_overview.png)
 
-### 1.4.1
+Form to accept/deny the request
 
-* Fix error when deleting selected jobs in the django admin
+![Accept/Deny Form](doc/04_accept_deny.png)
 
-### 1.4.2
+Confirmation by mail for the requester
 
-* Consistently use vocabulary for the word "assignment(s)"
-* Support for assignment unit HOURS
+![Mail Confirmation](doc/05_mail_confirmation.png)
 
-### 1.4.3
+The assignment appears in the list
 
-* Compatibility to juntagrico>=1.4.6
+![New menu entry](doc/06_assignment_list.png)
```

### Comparing `juntagrico-assignment-request-1.6.0/README.md` & `juntagrico_assignment_request-1.6.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,39 +6,57 @@
 [![image](https://img.shields.io/pypi/v/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/l/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/pyversions/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/status/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/dm/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request/)
 [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-assignment-request.svg)](https://github.com/juntagrico/juntagrico-assignment-request)
 [![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-assignment-request)](https://github.com/juntagrico/juntagrico-assignment-request)
-[![Requirements Status](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements/?branch=main)
 
 This is an extension for juntagrico. You can find more information about juntagrico here
 (https://github.com/juntagrico/juntagrico)
 
 It allows members to request assignments for jobs they have done, that were not announced.
 
 ## Installation
 
 1. Add `juntagrico-assignment-request` to your `requirements.txt`
-2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py`
+2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py` **above** `juntagrico`
 3. Add `path(r'', include('juntagrico_assignment_request.urls')),` at the end of your `urls.py`
-4. Redeploy your project
+4. Redeploy your project (and apply migrations)
 
 ## Configuration
 
-When requesting an assignment, members can select the person that can confirm that they did a job.
+When requesting an assignment, members can select the person (confirmer) that can confirm that they did a job.
 To add people to this selection you will have to add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze bestätigen`
 
+If you want to allow an activity area coordinator to confirm requests, but only on the areas they coordinate,
+add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze im eigenen Tätigkeitsbereich bestätigen`
+
 Only the selected confirmer, will be informed about the request by email and can see the request.
 
 If members don't select any confirmer all users with the following permission will receive a notification and can see the request: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Wird über nicht abgesprochene Arbeitseinsätze informiert`
 
 The [ASSIGNMENT_UNIT](https://juntagrico.readthedocs.io/en/latest/settings.html?highlight=ASSIGNMENT_UNIT#assignment-unit) setting is respected.
 
+### ASSIGNMENT_REQUEST_AREAS
+
+If you need to limit the activity areas that can be selected in the requests,
+set this setting to a function, that takes an `ActivityArea` queryset as the first argument
+and returns a filtered queryset.
+By default, all activity areas can be selected.
+
+Example: Include only visible activity areas:
+
+```python
+def only_visible(queryset):
+    return queryset.filter(hidden=False)
+
+ASSIGNMENT_REQUEST_AREAS = only_visible
+```
+
 ## Usage
 
 1. Members will see a new entry in the menu to request assignments
 2. They are presented with a form to fill out the details of the job they did
 3. Below the form, they see a list of assignments that they already sent with the option to edit or delete them
 4. Upon sending the form, the selected confirmer (or the fallback users) will be informed by email
 5. The confirmer can modify the assignment amount, accept, deny or just send a message to the member
@@ -47,29 +65,32 @@
 
 ## Admin modifications
 
 The extension creates job types and jobs on the fly behind the scenes as they are needed to create the assignments and show them to the member that made them.
 In order to not clutter the admin views with automatically generated content, these jobs and job types are hidden.
 As a side effect there will be assignments that have a valid job link, but when you follow that job, you will be told that no job with the given id exists.
 
-## Release Notes
+## Screenshots
+
+New menu entry
+
+![New menu entry](doc/01_menu_entry.png)
 
-## 1.5
+Request Form
 
-Upgrade to Juntagrico 1.5
+![Request Form](doc/02_request_form)
 
-## 1.4
+Overview about reported assignments
 
-Upgrade to Juntagrico 1.4
+![Overview](doc/03_overview.png)
 
-### 1.4.1
+Form to accept/deny the request
 
-* Fix error when deleting selected jobs in the django admin
+![Accept/Deny Form](doc/04_accept_deny.png)
 
-### 1.4.2
+Confirmation by mail for the requester
 
-* Consistently use vocabulary for the word "assignment(s)"
-* Support for assignment unit HOURS
+![Mail Confirmation](doc/05_mail_confirmation.png)
 
-### 1.4.3
+The assignment appears in the list
 
-* Compatibility to juntagrico>=1.4.6
+![New menu entry](doc/06_assignment_list.png)
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/assignment_request_admin.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/admins/assignment_request_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from django.urls import reverse
 
 from juntagrico.admins import BaseAdmin
 from juntagrico.util.admin import MyHTMLWidget
 from juntagrico.config import Config
 
 from juntagrico_assignment_request.models import AssignmentRequest
-from juntagrico_assignment_request.utils import all_approvers
+from juntagrico_assignment_request.utils import get_approvers
 
 
 class AssignmentRequestAdminForm(ModelForm):
     class Meta:
         model = AssignmentRequest
         fields = '__all__'
 
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
-        self.fields['approver'].queryset = all_approvers()
+        self.fields['approver'].queryset = get_approvers()
         instance = k.get('instance')
         self.fields['assignment_link'].initial = self.get_assignment_link(instance)
 
     @staticmethod
     def get_assignment_link(instance):
         if instance is None:
             return ''
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/apps.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/apps.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/hack.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/hack.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/__init__.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/__init__.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/adminnotification.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/adminnotification.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/membernotification.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/mailer/membernotification.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/models.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     ]
 
     member = models.ForeignKey(Member, verbose_name=Config.vocabulary('member'), on_delete=models.CASCADE,
                                help_text=_("Beantragt von"))
     assignment = models.OneToOneField(Assignment, verbose_name=Config.vocabulary('assignment'),
                                       blank=True, null=True, on_delete=models.PROTECT)
 
-    amount = models.PositiveIntegerField(
-        _('Wert'), default=1, validators=[MinValueValidator(1)],
+    amount = models.FloatField(
+        _('Wert'), default=1, validators=[MinValueValidator(0)],
         help_text=_("Wie viele " + Config.vocabulary('assignment_pl') + "?") + _(
             " Wird mit 'Dauer in Stunden' multipliziert.") if Config.assignment_unit() == 'HOURS' else ''
     )
 
     job_time = models.DateTimeField(_('Geleistet am'), default=datetime.now)
     request_date = models.DateField(_('Beantragt am'), default=date.today, blank=True, null=True)
     response_date = models.DateField(_('Beantwortet am'), blank=True, null=True,
@@ -90,15 +90,15 @@
         return self.status == self.REJECTED
 
     def get_amount(self):
         """
         :return: amount taking into account the assignment unit setting
         """
         if Config.assignment_unit() == 'HOURS':
-            return self.amount * self.duration
+            return self.amount * float(self.duration)
         return self.amount
 
     def save(self, **kwargs):
         old_assignment = self.assignment
         super().save(**kwargs)
         # delete assignment object, if request is unconfirmed again
         # this must be done after fully saving the request,
@@ -191,9 +191,11 @@
             job.slots -= 1
 
     class Meta:
         verbose_name = _('%s Anfrage') % Config.vocabulary('assignment')
         verbose_name_plural = _('%s Anfragen') % Config.vocabulary('assignment')
         permissions = (
             ('can_confirm_assignments', _('Kann selbständige Arbeitseinsätze bestätigen')),
+            ('can_confirm_assignments_for_area',
+             _('Kann selbständige Arbeitseinsätze im eigenen Tätigkeitsbereich bestätigen')),
             ('notified_on_unapproved_assignments', _('Wird über nicht abgesprochene Arbeitseinsätze informiert')),
         )
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/list.html` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
             {% else %}
                 {% blocktrans %}Angemeldete {{ v_assignment_pl }}{% endblocktrans %}
             {% endif %}
         </h3>
     </div>
 {% endblock %}
 {% block content %}
+    {% include "assignment_request/snippets/messages.html" %}
     {% if archive %}
     <div class="col-md-12 mb-4">
         <a href="{% url 'juntagrico-assignment-request:list' %}">{% trans "Zurück zu den offenen Anfragen" %}</a>
     </div>
     {% endif %}
     <div class="col-md-12 mb-4">
         {% if assignment_requests %}
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends "base.html" %} {% load i18n %} {% load juntagrico.config %} {% load
 crispy_forms_tags %} {% block page_title %} {% vocabulary "assignment_pl" as
 v_assignment_pl %}
 ******** {{%% iiff aarrcchhiivvee %%}} {{%% bblloocckkttrraannss %%}}BBeeaannttwwoorrtteettee AAnnffrraaggeenn{{%% eennddbblloocckkttrraannss %%}}
 {{%% eellssee %%}} {{%% bblloocckkttrraannss %%}}AAnnggeemmeellddeettee {{{{ vv__aassssiiggnnmmeenntt__ppll }}}}{{%% eennddbblloocckkttrraannss %%}}
 {{%% eennddiiff %%}} ********
-{% endblock %} {% block content %} {% if archive %}
+{% endblock %} {% block content %} {% include "assignment_request/snippets/
+messages.html" %} {% if archive %}
 _{_%_ _t_r_a_n_s_ _"_Z_u_r_Ã_¼_c_k_ _z_u_ _d_e_n_ _o_f_f_e_n_e_n_ _A_n_f_r_a_g_e_n_"_ _%_}
 {% endif %}
 {% if assignment_requests %}
 {{%% ttrraannss ""EEiinnssaattzz vvoomm"" %%}}         {{%% ttrraannss ""VVoonn"" %%}}         {{%% ttrraannss ""AAbbggeesspprroocchheenn mmiitt"" %%}}       {{%% ttrraannss ""SSttaattuuss"" %%}}
                                                                                                  {% if
                                                                                                  assignment_request.assignment.job %}
 {                                 {                         {                                    _{                                     {% if not
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Soeben hat {{ new_approver }} die {{ v_assignment }}-Anfrage von {{ assignment_request.member }} beantwortet und dir die Arbeit abgenommen.
 {% if assignment_request.response %}
 Entscheidung: {{ assignment_request.get_status_display }}
 Antwort: "{{ assignment_request.response }}"{% endif %}
 
 {{ assignment_request.member }} hatte zuletzt dich als Referenzperson angegeben.
 
-Es geht um folgende/n/s {% vocabulary 'assignment' %}:
+Es geht um folgende/n/s {{ v_assignment }}:
 {% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Beschreibung:
 "{{ assignment_request.description }}"
 {% endif %}
 
 {% endblock %}
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends "mails/email.txt" %}
 {% load juntagrico.config %}
-{% block content %}
+{% block content %}{% vocabulary 'assignment' as v_assignment %}
 Soeben hat {{ assignment_request.approver }} deine Anfrage angenommen.
 {% if assignment_request.response %}
 Antwort: "{{ assignment_request.response }}"
 {% endif %}
 
-Es geht um folgende/n/s {% vocabulary 'assignment' %}:
+Es geht um folgende/n/s {{ v_assignment }}:
     {{ serverurl }}{% url 'job' assignment_request.assignment.job.id %}
 {% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 {% endblock %}
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "mails/email.txt" %}
 {% load juntagrico.config %}
-{% block content %}
+{% block content %}{% vocabulary 'assignment' as v_assignment %}
 Soeben hat {{ assignment_request.approver }} deine Anfrage mit folgender Begründung abgelehnt:
 "{{ assignment_request.response }}"
 
-Es geht um folgende/n/s {% vocabulary 'assignment' %}:
+Es geht um folgende/n/s {{ v_assignment }}:
 {% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 
 Du kannst hier deine Anfrage anpassen:
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "mails/email.txt" %}
 {% load juntagrico.config %}
-{% block content %}
+{% block content %}{% vocabulary 'assignment' as v_assignment %}
 Soeben hat {{ assignment_request.approver }} eine Rückfrage auf deine Anfrage verfasst:
 "{{ assignment_request.response }}"
 
-Es geht um folgende/n/s {% vocabulary 'assignment' %}:
+Es geht um folgende/n/s {{ v_assignment }}:
 {% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 
 Du kannst auf die Rückfrage antworten, indem du hier die Anfrage anpasst:
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/request.html` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/request.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "base.html" %}
+{% load static %}
 {% load i18n %}
 {% load juntagrico.config %}
 {% load crispy_forms_tags %}
 
 {% block page_title %}
    {% vocabulary "assignment" as v_assignment %}
     <div class="page-title col-md-12">
@@ -10,32 +11,45 @@
             {% blocktrans %}{{ v_assignment }} melden{% endblocktrans %}
         </h3>
     </div>
 {% endblock %}
 {% block content %}  
     {% vocabulary "assignment" as v_assignment %}
     {% vocabulary "assignment_pl" as v_assignment_pl %}
+    {% include "assignment_request/snippets/messages.html" %}
+    
     <div class="col-md-12 mb-4">
-        {% blocktrans %}Hier kannst du deine {{ v_assignment_pl }} melden. Dies gilt für Termine, die nicht mit einer festgelegten Arbeitszeit buchbar sind aber auch für selbständige Einsätze. Bitte sprich dich vorgängig mit einer Gartenfachkraft oder einer/m Arbeitsgruppen-KoordinatorIn ab, wenn du selbständige Einsätze machen willst.{% endblocktrans %}
+        {% block instructions %}
+            {% blocktrans %}
+                Hier kannst du deine {{ v_assignment_pl }} melden. 
+                Dies gilt für Termine, die nicht mit einer festgelegten Arbeitszeit buchbar sind aber auch
+                für selbständige Einsätze. Bitte sprich dich vorgängig mit einer Gartenfachkraft
+                oder einer/m Arbeitsgruppen-KoordinatorIn ab, wenn du selbständige Einsätze machen willst.
+            {% endblocktrans %}
+        {% endblock %}
+    </div>
+
+    <div class="col-md-12 mb-4">
+        <h4>
+            {% blocktrans %}Neue Anfrage erstellen{% endblocktrans %}
+        </h4>
     </div>
     <div class="col-md-12 mb-4">
-        {% if sent %}
-        <div class="alert alert-success">
-            {% blocktrans %} 
-                Deine Anfrage wurde erfolgreich verschickt. 
-                <br> Du wirst per E-Mail benachrichtigt, sobald diese bestätigt wurde.
-            {% endblocktrans %}
-        </div>
-        {% endif %}
         <form action="" method="post" id="request_assignment">
             {% crispy form %}
         </form>
     </div>
+
     {% if assignment_requests %}
     <div class="col-md-12 mb-4">
+        <h4>
+            {% blocktrans %}Gemeldete {{ v_assignment_pl }}{% endblocktrans %}
+        </h4>
+    </div>
+    <div class="col-md-12 mb-4">
         {% blocktrans %}Diese {{ v_assignment_pl }} hast du schon gemeldet{% endblocktrans %}
 
         <table id="filter-table" class="list table" style="display: table;">
             <thead>
                 <tr>
                     <th class="align-top">
                         {% trans "Einsatz vom" %}
@@ -86,7 +100,11 @@
             </tbody>
         </table>
         {% blocktrans %}Es werden nur erledigte Anfragen von dieser Saison und alle offenen Anfragen angezeigt.{% endblocktrans %}
     </div>
     {% endif %}
 {% endblock %}
 
+{% block scripts %}
+    {{ form.approvers_by_area|json_script:'approvers_data' }}
+    <script type="text/javascript" src="{% static 'juntagrico_assignment_request/js/request.js' %}"></script>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-{% extends "base.html" %} {% load i18n %} {% load juntagrico.config %} {% load
-crispy_forms_tags %} {% block page_title %} {% vocabulary "assignment" as
-v_assignment %}
+{% extends "base.html" %} {% load static %} {% load i18n %} {% load
+juntagrico.config %} {% load crispy_forms_tags %} {% block page_title %} {%
+vocabulary "assignment" as v_assignment %}
 ******** {{%% bblloocckkttrraannss %%}}{{{{ vv__aassssiiggnnmmeenntt }}}} mmeellddeenn{{%% eennddbblloocckkttrraannss %%}} ********
 {% endblock %} {% block content %} {% vocabulary "assignment" as v_assignment
-%} {% vocabulary "assignment_pl" as v_assignment_pl %}
-{% blocktrans %}Hier kannst du deine {{ v_assignment_pl }} melden. Dies gilt
-fÃ¼r Termine, die nicht mit einer festgelegten Arbeitszeit buchbar sind aber
-auch fÃ¼r selbstÃ¤ndige EinsÃ¤tze. Bitte sprich dich vorgÃ¤ngig mit einer
-Gartenfachkraft oder einer/m Arbeitsgruppen-KoordinatorIn ab, wenn du
-selbstÃ¤ndige EinsÃ¤tze machen willst.{% endblocktrans %}
-{% if sent %}
-{% blocktrans %} Deine Anfrage wurde erfolgreich verschickt.
-Du wirst per E-Mail benachrichtigt, sobald diese bestÃ¤tigt wurde. {%
-endblocktrans %}
-{% endif %}
+%} {% vocabulary "assignment_pl" as v_assignment_pl %} {% include
+"assignment_request/snippets/messages.html" %}
+{% block instructions %} {% blocktrans %} Hier kannst du deine {
+{ v_assignment_pl }} melden. Dies gilt fÃ¼r Termine, die nicht mit einer
+festgelegten Arbeitszeit buchbar sind aber auch fÃ¼r selbstÃ¤ndige EinsÃ¤tze.
+Bitte sprich dich vorgÃ¤ngig mit einer Gartenfachkraft oder einer/
+m Arbeitsgruppen-KoordinatorIn ab, wenn du selbstÃ¤ndige EinsÃ¤tze machen
+willst. {% endblocktrans %} {% endblock %}
+****** {{%% bblloocckkttrraannss %%}}NNeeuuee AAnnffrraaggee eerrsstteelllleenn{{%% eennddbblloocckkttrraannss %%}} ******
 {% crispy form %}
 {% if assignment_requests %}
+****** {{%% bblloocckkttrraannss %%}}GGeemmeellddeettee {{{{ vv__aassssiiggnnmmeenntt__ppll }}}}{{%% eennddbblloocckkttrraannss %%}} ******
 {% blocktrans %}Diese {{ v_assignment_pl }} hast du schon gemeldet{%
 endblocktrans %}
 {{%% ttrraannss ""EEiinnssaattzz vvoomm"" %%}}         {{%% ttrraannss ""AAbbggeesspprroocchheenn mmiitt"" %%}}       {{%% ttrraannss ""SSttaattuuss"" %%}}
                                                                        {% if
                                                                        assignment_request.assignment.job %}
 {                                 {                                    _{
 {                                 {                                    _{                                     {% if not
@@ -30,8 +29,10 @@
                                                                        }} {% endif %}
 {% trans "Beschreibung" %}: {{ assignment_request.description }}
 {% if assignment_request.response %}
 {% trans "Antwort" %}: {{ assignment_request.response }}
 {% endif %}
 {% blocktrans %}Es werden nur erledigte Anfragen von dieser Saison und alle
 offenen Anfragen angezeigt.{% endblocktrans %}
-{% endif %} {% endblock %}
+{% endif %} {% endblock %} {% block scripts %} {
+{ form.approvers_by_area|json_script:'approvers_data' }}
+{% endblock %}
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/respond.html` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/templates/assignment_request/respond.html`

 * *Files identical despite different names*

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/urls.py` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 from django.urls import path
 from juntagrico_assignment_request import views
 
 app_name = 'juntagrico-assignment-request'
 urlpatterns = [
     path('ar/assignment/request', views.request_assignment, name='request'),
-    path('ar/assignment/requested', views.request_assignment, {'sent': True}, name='requested'),
     path('ar/assignment/delete/<int:request_id>/', views.delete_request_assignment, name='delete'),
     path('ar/assignment/edit/<int:request_id>/', views.edit_request_assignment, name='edit'),
     path('ar/assignment/list', views.list_assignment_requests, name='list'),
     path('ar/assignment/archive', views.list_archive, name='archive'),
     path('ar/assignment/respond/<int:request_id>/', views.respond_assignment_request, name='respond'),
     path('ar/assignment/confirm/<int:request_id>/', views.confirm_assignment_request, name='confirm'),
 ]
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/PKG-INFO` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-assignment-request
-Version: 1.6.0
+Version: 1.6.1
 Summary: Allows members to request assignments for jobs they have done, that were not announced.
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -167,14 +167,15 @@
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://www.juntagrico.org
 Project-URL: Issues, https://github.com/juntagrico/juntagrico-assignment-request/issues
+Project-URL: Changelog, https://github.com/juntagrico/juntagrico-assignment-request/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -184,53 +185,71 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: juntagrico==1.6.0rc3
+Requires-Dist: juntagrico>=1.6.0
 
 # juntagrico_assignment_request
 
 [![juntagrico-ci](https://github.com/juntagrico/juntagrico-assignment-request/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-assignment-request/actions/workflows/juntagrico-ci.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/6c1a453b157b9395a858/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-assignment-request/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/6c1a453b157b9395a858/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-assignment-request/test_coverage)
 [![image](https://img.shields.io/pypi/v/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/l/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/pyversions/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/status/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request)
 [![image](https://img.shields.io/pypi/dm/juntagrico_assignment_request.svg)](https://pypi.python.org/pypi/juntagrico_assignment_request/)
 [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-assignment-request.svg)](https://github.com/juntagrico/juntagrico-assignment-request)
 [![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-assignment-request)](https://github.com/juntagrico/juntagrico-assignment-request)
-[![Requirements Status](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-assignment-request/requirements/?branch=main)
 
 This is an extension for juntagrico. You can find more information about juntagrico here
 (https://github.com/juntagrico/juntagrico)
 
 It allows members to request assignments for jobs they have done, that were not announced.
 
 ## Installation
 
 1. Add `juntagrico-assignment-request` to your `requirements.txt`
-2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py`
+2. Add `'juntagrico_assignment_request',` to the `INSTALLED_APPS` in your `settings.py` **above** `juntagrico`
 3. Add `path(r'', include('juntagrico_assignment_request.urls')),` at the end of your `urls.py`
-4. Redeploy your project
+4. Redeploy your project (and apply migrations)
 
 ## Configuration
 
-When requesting an assignment, members can select the person that can confirm that they did a job.
+When requesting an assignment, members can select the person (confirmer) that can confirm that they did a job.
 To add people to this selection you will have to add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze bestätigen`
 
+If you want to allow an activity area coordinator to confirm requests, but only on the areas they coordinate,
+add this permission to that user: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Kann selbständige Arbeitseinsätze im eigenen Tätigkeitsbereich bestätigen`
+
 Only the selected confirmer, will be informed about the request by email and can see the request.
 
 If members don't select any confirmer all users with the following permission will receive a notification and can see the request: `juntagrico_assignment_request | Arbeitseinsatz Anfrage | Wird über nicht abgesprochene Arbeitseinsätze informiert`
 
 The [ASSIGNMENT_UNIT](https://juntagrico.readthedocs.io/en/latest/settings.html?highlight=ASSIGNMENT_UNIT#assignment-unit) setting is respected.
 
+### ASSIGNMENT_REQUEST_AREAS
+
+If you need to limit the activity areas that can be selected in the requests,
+set this setting to a function, that takes an `ActivityArea` queryset as the first argument
+and returns a filtered queryset.
+By default, all activity areas can be selected.
+
+Example: Include only visible activity areas:
+
+```python
+def only_visible(queryset):
+    return queryset.filter(hidden=False)
+
+ASSIGNMENT_REQUEST_AREAS = only_visible
+```
+
 ## Usage
 
 1. Members will see a new entry in the menu to request assignments
 2. They are presented with a form to fill out the details of the job they did
 3. Below the form, they see a list of assignments that they already sent with the option to edit or delete them
 4. Upon sending the form, the selected confirmer (or the fallback users) will be informed by email
 5. The confirmer can modify the assignment amount, accept, deny or just send a message to the member
@@ -239,29 +258,32 @@
 
 ## Admin modifications
 
 The extension creates job types and jobs on the fly behind the scenes as they are needed to create the assignments and show them to the member that made them.
 In order to not clutter the admin views with automatically generated content, these jobs and job types are hidden.
 As a side effect there will be assignments that have a valid job link, but when you follow that job, you will be told that no job with the given id exists.
 
-## Release Notes
+## Screenshots
+
+New menu entry
+
+![New menu entry](doc/01_menu_entry.png)
 
-## 1.5
+Request Form
 
-Upgrade to Juntagrico 1.5
+![Request Form](doc/02_request_form)
 
-## 1.4
+Overview about reported assignments
 
-Upgrade to Juntagrico 1.4
+![Overview](doc/03_overview.png)
 
-### 1.4.1
+Form to accept/deny the request
 
-* Fix error when deleting selected jobs in the django admin
+![Accept/Deny Form](doc/04_accept_deny.png)
 
-### 1.4.2
+Confirmation by mail for the requester
 
-* Consistently use vocabulary for the word "assignment(s)"
-* Support for assignment unit HOURS
+![Mail Confirmation](doc/05_mail_confirmation.png)
 
-### 1.4.3
+The assignment appears in the list
 
-* Compatibility to juntagrico>=1.4.6
+![New menu entry](doc/06_assignment_list.png)
```

### Comparing `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/SOURCES.txt` & `juntagrico_assignment_request-1.6.1/juntagrico_assignment_request.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,30 @@
 juntagrico_assignment_request/mailer/__init__.py
 juntagrico_assignment_request/mailer/adminnotification.py
 juntagrico_assignment_request/mailer/membernotification.py
 juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
 juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
 juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
 juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
+juntagrico_assignment_request/migrations/0005_alter_assignmentrequest_amount.py
+juntagrico_assignment_request/migrations/0006_alter_assignmentrequest_options.py
 juntagrico_assignment_request/migrations/__init__.py
+juntagrico_assignment_request/static/juntagrico_assignment_request/js/request.js
 juntagrico_assignment_request/templates/assignment_request/edit.html
 juntagrico_assignment_request/templates/assignment_request/list.html
 juntagrico_assignment_request/templates/assignment_request/request.html
 juntagrico_assignment_request/templates/assignment_request/respond.html
 juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt
 juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt
 juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt
 juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt
 juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt
 juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt
 juntagrico_assignment_request/templates/assignment_request/mails/snippets/summary.txt
-juntagrico_assignment_request/templates/menu/admin_menu.html
-juntagrico_assignment_request/templates/menu/user_menu.html
+juntagrico_assignment_request/templates/assignment_request/snippets/messages.html
+juntagrico_assignment_request/templates/juntagrico/menu/admin.html
+juntagrico_assignment_request/templates/juntagrico/menu/user.html
+juntagrico_assignment_request/tests/__init__.py
+juntagrico_assignment_request/tests/test_admin.py
+juntagrico_assignment_request/tests/test_assignment_request.py
+juntagrico_assignment_request/tests/test_assignment_request_hours.py
+juntagrico_assignment_request/tests/test_manipulation.py
```

### Comparing `juntagrico-assignment-request-1.6.0/pyproject.toml` & `juntagrico_assignment_request-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
     {name = "juntagrico", email = "python@juntagrico.org"},
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
-    "juntagrico==1.6.0rc3",
+    "juntagrico>=1.6.0",
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
     'Framework :: Django :: 4.2',
     'Intended Audience :: Developers',
@@ -31,14 +31,15 @@
     'Topic :: Internet :: WWW/HTTP :: Site Management',
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://www.juntagrico.org"
 Issues = "https://github.com/juntagrico/juntagrico-assignment-request/issues"
+Changelog = "https://github.com/juntagrico/juntagrico-assignment-request/releases"
 
 [tool.setuptools.packages.find]
 include = ["juntagrico_assignment_request*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "juntagrico_assignment_request.__version__"}
```

