# Comparing `tmp/pyslth-0.3.6.tar.gz` & `tmp/pyslth-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.6.tar", last modified: Sun May 19 14:28:22 2024, max compression
+gzip compressed data, was "pyslth-0.3.7.tar", last modified: Sun May 19 19:48:10 2024, max compression
```

## Comparing `pyslth-0.3.6.tar` & `pyslth-0.3.7.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.123421 pyslth-0.3.6/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.6/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 14:28:22.123177 pyslth-0.3.6/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.075301 pyslth-0.3.6/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.6/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 14:28:22.123487 pyslth-0.3.6/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 14:27:50.000000 pyslth-0.3.6/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.084190 pyslth-0.3.6/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.6/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.6/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.084775 pyslth-0.3.6/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.6/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.6/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.6/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.6/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.6/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.085087 pyslth-0.3.6/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.085750 pyslth-0.3.6/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.6/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.6/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.093693 pyslth-0.3.6/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.6/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.6/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.6/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.6/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.6/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.6/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.6/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.6/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.094197 pyslth-0.3.6/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.6/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.6/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.6/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.094596 pyslth-0.3.6/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.105535 pyslth-0.3.6/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.6/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.109733 pyslth-0.3.6/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.6/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.6/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.6/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.6/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.112151 pyslth-0.3.6/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.6/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.6/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.6/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.6/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.6/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.122119 pyslth-0.3.6/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.6/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.6/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.6/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   101600 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.6/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.122761 pyslth-0.3.6/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-18 08:08:43.000000 pyslth-0.3.6/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.6/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.6/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.6/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.6/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.6/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.818979 pyslth-0.3.7/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.7/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 19:48:10.818745 pyslth-0.3.7/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.781910 pyslth-0.3.7/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.7/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 19:48:10.819054 pyslth-0.3.7/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 19:47:28.000000 pyslth-0.3.7/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.788920 pyslth-0.3.7/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.7/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.7/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.789532 pyslth-0.3.7/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.7/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.7/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.7/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.7/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.7/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.789858 pyslth-0.3.7/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.790533 pyslth-0.3.7/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.7/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.7/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.793629 pyslth-0.3.7/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.7/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.7/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.7/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.7/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.7/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.7/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.7/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.7/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.794121 pyslth-0.3.7/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.7/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.7/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.7/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.794432 pyslth-0.3.7/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.796832 pyslth-0.3.7/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.7/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.800836 pyslth-0.3.7/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.7/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.7/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.7/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.7/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.803312 pyslth-0.3.7/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.7/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.7/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.7/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.7/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.7/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.817436 pyslth-0.3.7/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.3.7/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.7/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.7/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.7/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102043 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.7/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.818302 pyslth-0.3.7/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.3.7/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.7/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.7/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.7/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.7/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.7/slth/views.py
```

### Comparing `pyslth-0.3.6/PKG-INFO` & `pyslth-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.6
+Version: 0.3.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.6/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.7/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.6
+Version: 0.3.7
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.6/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.7/pyslth.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 slth/static/css/fonts/rawline-400.woff
 slth/static/css/fonts/rawline-500i.woff
 slth/static/css/fonts/rawline-700.woff
 slth/static/images/logo.png
 slth/static/images/logo.svg
 slth/static/images/user.png
 slth/static/images/user.svg
+slth/static/js/default-passive-events.min.js
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
 slth/static/js/ios-splash.min.js
 slth/static/js/peerjs.min.js
 slth/static/js/qrcode.min.js
 slth/static/js/react-trigger-change.js
 slth/static/js/react.min.js
```

### Comparing `pyslth-0.3.6/setup.py` & `pyslth-0.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.6',
+    version='0.3.7',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.6/slth/__init__.py` & `pyslth-0.3.7/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/components.py` & `pyslth-0.3.7/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/db/models.py` & `pyslth-0.3.7/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/endpoints.py` & `pyslth-0.3.7/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/factory.py` & `pyslth-0.3.7/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/forms.py` & `pyslth-0.3.7/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/management/commands/integration_test.py` & `pyslth-0.3.7/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/management/commands/sync.py` & `pyslth-0.3.7/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/migrations/0001_initial.py` & `pyslth-0.3.7/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.7/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/migrations/0006_user.py` & `pyslth-0.3.7/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/models.py` & `pyslth-0.3.7/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/notifications.py` & `pyslth-0.3.7/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/oauth.py` & `pyslth-0.3.7/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/permissions.py` & `pyslth-0.3.7/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/queryset.py` & `pyslth-0.3.7/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/roles.py` & `pyslth-0.3.7/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/selenium/__init__.py` & `pyslth-0.3.7/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/selenium/browser.py` & `pyslth-0.3.7/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/serializer.py` & `pyslth-0.3.7/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/.DS_Store` & `pyslth-0.3.7/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fontawesome.min.css` & `pyslth-0.3.7/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.7/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.7/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.7/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.7/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.7/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/slth.css` & `pyslth-0.3.7/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/css/solid.min.css` & `pyslth-0.3.7/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/images/logo.png` & `pyslth-0.3.7/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/images/logo.svg` & `pyslth-0.3.7/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/images/user.png` & `pyslth-0.3.7/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/echarts.min.js` & `pyslth-0.3.7/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/index.min.js` & `pyslth-0.3.7/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/ios-splash.min.js` & `pyslth-0.3.7/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/peerjs.min.js` & `pyslth-0.3.7/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/qrcode.min.js` & `pyslth-0.3.7/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/react-trigger-change.js` & `pyslth-0.3.7/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/react.min.js` & `pyslth-0.3.7/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/slth.min.js` & `pyslth-0.3.7/slth/static/js/slth.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
     c as H,
     r as B,
     R as Te
 } from "./react.min.js";
-const S = {
+const k = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -72,15 +72,15 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function C(e) {
+function S(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
@@ -92,43 +92,43 @@
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = S.colors.primary, a.color = "white"), e.default && (a.color = S.colors.primary, a.border = "solid 1px " + S.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = k.colors.primary, a.color = "white"), e.default && (a.color = k.colors.primary, a.border = "solid 1px " + k.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(C, {
+            children: t.jsx(S, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const Ne = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
 function qe(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : S.colors.success,
+            backgroundColor: e.isError ? "#e52207" : k.colors.success,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(C, {
+            children: [t.jsx(S, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
@@ -141,25 +141,25 @@
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function le() {
+function oe() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function oe(e) {
+function le(e) {
     function n() {
         const a = {
-            color: S.colors.info,
-            backgroundColor: S.background.info,
+            color: k.colors.info,
+            backgroundColor: k.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -187,42 +187,42 @@
 
 function U(e) {
     return e.replace("/api/", "/app/")
 }
 
 function q(e, n, a, r) {
     const i = localStorage.getItem("token");
-    var l = {
+    var o = {
         Accept: "application/json"
     };
-    i && (l.Authorization = "Token " + i);
+    i && (o.Authorization = "Token " + i);
     const d = A(n);
     var c = {
         method: e,
-        headers: new Headers(l),
+        headers: new Headers(o),
         ajax: 1
     };
     r && (c.body = r);
     var s = null,
         u = null;
-    fetch(d, c).then(function(o) {
-        if (s = o, u = s.headers.get("Content-Type"), u == "application/json") return o.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
-        o.text()
-    }).then(o => {
+    fetch(d, c).then(function(l) {
+        if (s = l, u = s.headers.get("Content-Type"), u == "application/json") return l.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return l.arrayBuffer();
+        l.text()
+    }).then(l => {
         if (u == "application/json") {
-            var h = JSON.parse(o || "{}");
+            var h = JSON.parse(l || "{}");
             typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var f = window.URL.createObjectURL(new Blob([new Uint8Array(l)], {
                     type: u
                 })),
                 w = document.createElement("a");
             w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
-        } else a && a(o, s)
+        } else a && a(l, s)
     })
 }
 
 function W(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
@@ -240,15 +240,15 @@
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
                 a = n[0],
                 r = n[1];
             return r == "00:00:00" ? a : a + " " + r
         } else if (e.indexOf(`
 `) >= 0) return e.split(`
-`).map(function(i, l) {
+`).map(function(i, o) {
             return t.jsx("div", {
                 children: i
             }, Math.random())
         });
         return e
     }
     return typeof e == "object" && e.type ? t.jsx(x, {
@@ -273,38 +273,38 @@
 }
 
 function de() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
 function pe(e, n) {
-    le(), de(), window.reloader = n;
+    oe(), de(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function Ae(e) {
-    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: A(e)
     }))
 }
 
-function V(e) {
+function Y(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function Re(e) {
-    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
 function Oe(e) {
     const n = {
         backgroundColor: "black",
@@ -315,27 +315,27 @@
         top: 0,
         opacity: .7,
         display: "none"
     };
     return t.jsx("div", {
         className: "layer",
         onClick: function() {
-            V()
+            Y()
         },
         style: n
     })
 }
 
 function _e(e) {
     const [n, a] = B.useState(null), [r, i] = B.useState(0);
     B.useEffect(() => {
-        l(A(e.url)), document.querySelector(".layer").style.display = "block"
+        o(A(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
-    function l(s) {
+    function o(s) {
         q("GET", A(s), function(u) {
             a(u), i(r + 1)
         })
     }
 
     function d() {
         const s = {
@@ -346,17 +346,17 @@
                 cursor: "pointer",
                 marginTop: -15
             };
         if (n) return t.jsxs("div", {
             style: s,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(C, {
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => V()
+                    onClick: () => Y()
                 })
             }), t.jsx(x, {
                 data: n
             })]
         })
     }
     const c = {
@@ -394,17 +394,17 @@
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: i,
-                children: t.jsx(C, {
+                children: t.jsx(S, {
                     icon: "x",
-                    onClick: () => V()
+                    onClick: () => Y()
                 })
             }), t.jsx("iframe", {
                 src: A(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
@@ -418,38 +418,38 @@
 function ze(e) {
     const n = Math.random();
     B.useEffect(() => {
         document.querySelector(".layer").style.display = "block"
     }, []);
 
     function a() {
-        const l = {
+        const o = {
             width: "100%",
             borderBottom: "solid 1px #DDDD",
             padding: 20
         };
         return t.jsx("div", {
             align: "center",
             style: {},
             children: e.actions.map(function(d) {
                 return t.jsx("div", {
-                    style: l,
+                    style: o,
                     onClick: r,
                     children: t.jsx(_, {
                         data: d,
                         strech: !0
                     })
                 }, Math.random())
             })
         })
     }
 
     function r() {
-        const l = document.getElementById(n);
-        l.close(), l.classList.remove("opened"), l.remove(), document.querySelector(".layer").style.display = "none"
+        const o = document.getElementById(n);
+        o.close(), o.classList.remove("opened"), o.remove(), document.querySelector(".layer").style.display = "none"
     }
     const i = {
         width: "auto",
         display: "block",
         position: "fixed",
         bottom: 0,
         border: 0,
@@ -472,19 +472,19 @@
 
     function i(c) {
         c.preventDefault();
         var s = e.data.url;
         e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
     }
 
-    function l() {
-        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(C, {
+    function o() {
+        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(C, {
+            children: [t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
@@ -493,52 +493,52 @@
         var c = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             minWidth: 50,
-            lineHeight: "4rem"
+            lineHeight: e.data.icon ? "4rem" : "auto"
         };
-        return e.primary && (c.backgroundColor = S.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + S.colors.primary, c.color = S.colors.primary), e.style && Object.keys(e.style).map(function(s) {
+        return e.primary && (c.backgroundColor = k.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + k.colors.primary, c.color = k.colors.primary), e.style && Object.keys(e.style).map(function(s) {
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
             href: U(e.data.url) || "#",
             onClick: i,
             style: c,
             "data-label": M(e.data.name),
-            children: l()
+            children: o()
         })
     }
     return d()
 }
 
 function Z(e) {
-    function n(l) {
-        var d = l.target.parentNode.querySelector(".dropdown");
-        return d == null && (d = l.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = l.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
+    function n(o) {
+        var d = o.target.parentNode.querySelector(".dropdown");
+        return d == null && (d = o.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = o.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
     }
 
-    function a(l) {
-        const d = n(l);
+    function a(o) {
+        const d = n(o);
         if (d.style.display == "block") d.style.display = "none";
         else {
-            const c = l.target.getBoundingClientRect();
+            const c = o.target.getBoundingClientRect();
             document.querySelectorAll(".dropdown").forEach(s => s.style.display = "none"), d.style.left = c.left - 150 + c.width + "px", d.style.display = "block"
         }
     }
 
-    function r(l) {
-        const d = n(l);
+    function r(o) {
+        const d = n(o);
         d.style.display = "none"
     }
 
     function i() {
-        const l = {
+        const o = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
                 boxShadow: "15px 15px 10px -15px #DDD",
@@ -553,15 +553,15 @@
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
                 "data-label": M(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
-                style: l,
+                style: o,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(c => t.jsx("li", {
                     style: d,
                     children: t.jsx(_, {
                         data: c,
                         style: {
@@ -577,35 +577,35 @@
 
 function O({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: i,
-    onClick: l,
+    onClick: o,
     dataLabel: d,
     style: c
 }) {
     const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
         s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
     }
 
-    function o() {
+    function l() {
         return t.jsx("a", {
             id: e,
-            onClick: l || u,
+            onClick: o || u,
             href: s || "#",
             "data-label": M(d),
             style: c,
             children: i
         })
     }
-    return o()
+    return l()
 }
 
 function P(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
@@ -626,15 +626,15 @@
         a = window.document.styleSheets[0];
     e.split("}").forEach(r => {
         let i = (r + "}").replace(/\r?\n|\r/g, "");
         n = n === "" ? i : n + i, n.split("{").length === n.split("}").length && xe[n] == null && (a.insertRule(n, a.cssRules.length), n = "", xe[n] = !0)
     })
 }
 
-function $(e) {
+function X(e) {
     function n() {
         return e.data.url ? t.jsx(We, {
             data: e.data
         }) : t.jsx(je, {
             data: e.data
         })
     }
@@ -650,15 +650,15 @@
         })
     }
 
     function a() {
         return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(O, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
-                children: [W(e.data.value), t.jsx(C, {
+                children: [W(e.data.value), t.jsx(S, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
                 })]
             })
         }) : W(e.data.value)
@@ -684,25 +684,25 @@
 
     function i(d) {
         q("GET", d, function(c) {
             r(c)
         })
     }
 
-    function l() {
+    function o() {
         return window[n] = () => i(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
             children: t.jsx(je, {
                 data: a,
                 width: 100
             })
         })
     }
-    return l()
+    return o()
 }
 
 function se(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
@@ -723,38 +723,38 @@
 
 function ce(e) {
     function n() {
         return e.data.map(function(a) {
             if (Array.isArray(a)) return t.jsx(P, {
                 width: 300,
                 alignItems: "start",
-                children: a.map(r => t.jsx($, {
+                children: a.map(r => t.jsx(X, {
                     data: r,
                     width: 100 / a.length
                 }, Math.random()))
             }, Math.random());
             if (a.label != "ID" && (e.exclude == null || a.label != e.exclude)) return t.jsx("div", {
-                children: t.jsx($, {
+                children: t.jsx(X, {
                     data: a,
                     width: 100
                 })
             }, Math.random())
         })
     }
     return n()
 }
 
 function He(e) {
     function n() {
-        const l = {
+        const o = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
-            style: l,
+            style: o,
             children: e.data.title
         })
     }
 
     function a() {
         return t.jsx(ce, {
             data: e.data.data
@@ -764,21 +764,21 @@
     function r() {
         return t.jsx(se, {
             data: e.data.actions
         })
     }
 
     function i() {
-        const l = {
+        const o = {
             border: "solid 1px #DDD",
             padding: 10,
             borderStyle: "dashed"
         };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             children: [n(), a(), r()]
         })
     }
     return i()
 }
 
 function Pe(e) {
@@ -883,15 +883,15 @@
 
     function i() {
         return t.jsx(se, {
             data: e.data.actions
         })
     }
 
-    function l() {
+    function o() {
         const d = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
                 marginBottom: -10
@@ -903,15 +903,15 @@
             style: d,
             children: [r(), t.jsxs("div", {
                 style: c,
                 children: [n(), a(), i()]
             })]
         })
     }
-    return l()
+    return o()
 }
 
 function Ge(e) {
     const n = Math.random(),
         [a, r] = B.useState(e.data);
     F(`
     .object-fieldset{
@@ -921,15 +921,15 @@
 
     function i() {
         return t.jsx(ke, {
             data: a
         })
     }
 
-    function l() {
+    function o() {
         const u = {
             backgroundColor: "white",
             padding: 15,
             marginBottom: 15
         };
         return t.jsx("div", {
             style: u,
@@ -939,103 +939,103 @@
 
     function d() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
             return Array.isArray(u) ? t.jsx(P, {
                 width: 300,
-                children: u.map(o => t.jsx($, {
-                    data: o,
+                children: u.map(l => t.jsx(X, {
+                    data: l,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
-                children: t.jsx($, {
+                children: t.jsx(X, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
         }) : t.jsx(x, {
             data: a.data
         })
     }
 
     function c(u) {
-        q("GET", u, function(o) {
-            r(o)
+        q("GET", u, function(l) {
+            r(l)
         })
     }
 
     function s() {
         return e.data.url ? (window[n] = () => c(e.data.url), t.jsxs("div", {
             className: e.data.url ? "reloadable object-fieldset" : "object-fieldset",
             id: n,
-            children: [i(), l()]
+            children: [i(), o()]
         })) : t.jsxs("div", {
             className: "object-fieldset",
-            children: [i(), l()]
+            children: [i(), o()]
         })
     }
     return s()
 }
 
-function Ve(e) {
+function Ye(e) {
     const n = Math.random(),
         [a, r] = B.useState(e.data.actions);
 
     function i() {
         const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + c + "only=actions"
     }
 
-    function l() {
+    function o() {
         q("GET", i(), function(c) {
             r(c)
         })
     }
 
     function d() {
-        return window[n] = () => l(), t.jsx("div", {
+        return window[n] = () => o(), t.jsx("div", {
             className: "reloadable",
             id: n,
             children: a.map(function(c) {
                 return t.jsx(_, {
                     data: c,
                     default: !0
                 }, Math.random())
             })
         })
     }
     return d()
 }
 
-function $e(e) {
+function Xe(e) {
     function n() {
         return F(`
       .object-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .object-title h1 {
           margin: 0;
-          color: ${S.colors.primary};
+          color: ${k.colors.primary};
       }
     `), t.jsxs("div", {
             className: "object-title",
             style: {
                 flexDirection: window.innerWidth > 800 ? "row" : "column"
             },
             children: [e.data.title && t.jsx("h1", {
                 "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     margin: 10
                 },
-                children: t.jsx(Ve, {
+                children: t.jsx(Ye, {
                     data: e.data
                 })
             })]
         })
     }
     return n()
 }
@@ -1067,23 +1067,23 @@
                 })
             })]
         })
     }
     return n()
 }
 
-function Je(e) {
+function Ve(e) {
     function n() {
-        return t.jsx($e, {
+        return t.jsx(Xe, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(i, l) {
+        return e.data.data.map(function(i, o) {
             return t.jsx(x, {
                 data: i
             }, Math.random())
         })
     }
 
     function r() {
@@ -1091,44 +1091,44 @@
             className: "object-viewer",
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Ye(e) {
+function $e(e) {
     function n() {
         return t.jsx(ke, {
             data: e.data
         })
     }
 
     function a() {
         const i = {
             backgroundColor: "white"
         };
-        return e.data.data.map(function(l, d) {
+        return e.data.data.map(function(o, d) {
             return t.jsx("div", {
                 style: i,
                 children: t.jsx(x, {
-                    data: l
+                    data: o
                 }, Math.random())
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
-function Qe(e) {
+function Je(e) {
     F(`
     .noscroll::-webkit-scrollbar {
       display: none;
     }
     .noscroll {
       -ms-overflow-style: none;  /* IE and Edge */
       scrollbar-width: none;  /* Firefox */
@@ -1143,95 +1143,95 @@
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20,
                 overflowX: "auto"
             },
-            children: e.data.map(function(i, l) {
+            children: e.data.map(function(i, o) {
                 return t.jsx(O, {
                     href: i.url,
                     style: {
                         padding: 5,
-                        fontWeight: n == l ? "bold" : "normal",
-                        borderBottom: n == l ? "solid 3px #2670e8" : "solid 3px inherite",
+                        fontWeight: n == o ? "bold" : "normal",
+                        borderBottom: n == o ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
-                        d.preventDefault(), a(l), e.loadContent(i.url)
+                        d.preventDefault(), a(o), e.loadContent(i.url)
                     },
                     dataLabel: M(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
-function Xe(e) {
+function Qe(e) {
     var n = Math.random();
     const [a, r] = B.useState(e.data.data[0]);
 
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": M(e.data.title),
             children: e.data.title
         })
     }
 
-    function l() {
-        return t.jsx(Qe, {
+    function o() {
+        return t.jsx(Je, {
             data: e.data.data,
             loadContent: s
         })
     }
 
     function d() {
-        var o = {
+        var l = {
             ...a
         };
-        o.title = null;
+        l.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
             children: t.jsx(x, {
-                data: o
+                data: l
             }, Math.random())
         })
     }
 
     function c() {
-        const o = {
+        const l = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: o
+            style: l
         })
     }
 
-    function s(o) {
-        q("GET", o, function(h) {
+    function s(l) {
+        q("GET", l, function(h) {
             r(h)
         })
     }
 
     function u() {
         return window[n] = () => s(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [i(), l(), d(), c()]
+            children: [i(), o(), d(), c()]
         })
     }
     return u()
 }
 
 function Ke() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
@@ -1241,51 +1241,51 @@
 
 function R({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: i,
-    primary: l,
+    primary: o,
     compact: d,
     spin: c
 }) {
     function s() {
-        return a ? d || !r ? t.jsx(C, {
+        return a ? d || !r ? t.jsx(S, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Be, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(C, {
+            }), t.jsx(S, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const o = {
+        const l = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return l ? (o.backgroundColor = S.colors.primary, o.color = "white") : (o.border = "solid 1px " + S.colors.primary, o.color = S.colors.primary), t.jsx("a", {
+        return o ? (l.backgroundColor = k.colors.primary, l.color = "white") : (l.border = "solid 1px " + k.colors.primary, l.color = k.colors.primary), t.jsx("a", {
             id: e,
-            style: o,
+            style: l,
             "data-label": M(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
@@ -1329,55 +1329,55 @@
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function nt(e) {
-    function n(l) {
-        return e.data.icon ? l.done ? t.jsx(C, {
+    function n(o) {
+        return e.data.icon ? o.done ? t.jsx(S, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
             style: {
                 marginTop: 6
             },
-            children: l.number
+            children: o.number
         })
     }
 
-    function a(l) {
+    function a(o) {
         return {
-            border: "3px solid " + S.colors.primary,
+            border: "3px solid " + k.colors.primary,
             borderRadius: "50%",
-            background: l.done ? S.colors.primary : "white",
-            color: l.done ? "white" : S.colors.primary,
+            background: o.done ? k.colors.primary : "white",
+            color: o.done ? "white" : k.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
 
-    function r(l) {
+    function r(o) {
         return {
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
-            minWidth: l.length * 100
+            minWidth: o.length * 100
         }
     }
 
     function i() {
-        const l = {
+        const o = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
@@ -1391,15 +1391,15 @@
                 borderBottom: "2px solid #1151b3",
                 top: -28,
                 width: 45,
                 left: 77
             };
         return t.jsx("div", {
             children: t.jsx("div", {
-                style: l,
+                style: o,
                 children: t.jsx("ul", {
                     style: r(e.data.steps),
                     children: e.data.steps.map((s, u) => t.jsxs("li", {
                         style: d,
                         children: [t.jsx("div", {
                             style: a(s),
                             children: n(s)
@@ -1431,15 +1431,15 @@
             i = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: S.colors[e.data.style]
+                backgroundColor: k.colors[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
                 style: i,
                 children: t.jsxs("span", {
                     style: r,
@@ -1449,15 +1449,15 @@
         })
     }
     return n()
 }
 
 function rt(e) {
     function n() {
-        return e.data.color = S.colors[e.data.style], t.jsx(Se, {
+        return e.data.color = k.colors[e.data.style], t.jsx(Se, {
             data: e.data
         })
     }
     return n()
 }
 
 function Se(e) {
@@ -1471,15 +1471,15 @@
             whiteSpace: "nowrap",
             backgroundColor: e.data.color,
             display: "inline-flex",
             border: "solid 3px white"
         };
         return t.jsxs("div", {
             style: a,
-            children: [e.data.icon && t.jsx(C, {
+            children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     marginRight: 5
                 }
             }), e.data.label]
         })
     }
@@ -1505,54 +1505,54 @@
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
             i = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: S.colors.auxiliary
+                color: k.colors.auxiliary
             },
-            l = {
+            o = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: S.colors.primary
+                color: k.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
                 "data-label": M(e.data.title),
                 style: {
-                    color: S.colors.primary
+                    color: k.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(d => t.jsxs(O, {
                     href: d.url,
                     style: r,
                     dataLabel: d.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             style: i,
                             icon: d.icon
                         })
                     }), t.jsx("div", {
-                        style: l,
+                        style: o,
                         children: d.label
                     })]
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function lt(e) {
+function ot(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -1564,20 +1564,20 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function ot(e) {
+function lt(e) {
     function n() {
         return e.data.url ? t.jsx(O, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(C, {
+            children: e.data.icon ? t.jsx(S, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
@@ -1618,15 +1618,15 @@
     return a()
 }
 
 function ct(e) {
     function n() {
         const a = {
                 color: "white",
-                backgroundColor: S.colors.highlight,
+                backgroundColor: k.colors.highlight,
                 margin: -20,
                 textAlign: "center",
                 paddingTop: 20,
                 paddingBottom: 70
             },
             r = {
                 fontSize: "4rem",
@@ -1642,30 +1642,30 @@
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
                 "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
-                children: e.data.items.map(l => t.jsxs("div", {
+                children: e.data.items.map(o => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
-                        children: W(l.value)
+                        children: W(o.value)
                     }), t.jsx("div", {
                         style: i,
-                        children: l.name
+                        children: o.name
                     })]
                 }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
-                children: e.data.actions.map(l => t.jsx(O, {
-                    href: A(l.url),
-                    label: l.label,
-                    modal: l.modal,
-                    children: l.label
+                children: e.data.actions.map(o => t.jsx(O, {
+                    href: A(o.url),
+                    label: o.label,
+                    modal: o.modal,
+                    children: o.label
                 }, Math.random()))
             })]
         })
     }
     return n()
 }
 
@@ -1703,35 +1703,35 @@
 }
 
 function Ce(e) {
     const n = Math.random();
     var a = !1;
     const r = "rgb(219, 237, 255)",
         i = "rgb(89, 154, 242)",
-        l = "rgb(246, 123, 135)",
+        o = "rgb(246, 123, 135)",
         d = [],
         c = [];
 
     function s(y) {
-        return e.data.readonly ? y == null ? r : i : y == null ? r : y.text == null ? i : l
+        return e.data.readonly ? y == null ? r : i : y == null ? r : y.text == null ? i : o
     }
 
     function u(y) {
         a = !0, y.preventDefault()
     }
 
-    function o(y) {
+    function l(y) {
         a = !1, document.getElementById("input" + n).value = JSON.stringify({
             select: d,
             deselect: c
         })
     }
 
     function h(y) {
-        e.data.readonly || e.data.single_selection && f().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != l && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
+        e.data.readonly || e.data.single_selection && f().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != o && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
     }
 
     function f() {
         const y = [];
         return document.getElementById(n).querySelectorAll("td").forEach(function(D) {
             D.style.backgroundColor == i && y.push(D.dataset.day, D.dataset.time)
         }), y
@@ -1757,51 +1757,51 @@
             children: [t.jsx("input", {
                 id: "input" + n,
                 type: "hidden",
                 name: e.data.input_name
             }), t.jsxs("table", {
                 style: D,
                 onMouseDown: u,
-                onMouseUp: o,
+                onMouseUp: l,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: e.data.matrix[0].map(function(v) {
                             return t.jsx("th", {
                                 className: "bold",
                                 style: j,
                                 children: v.text
                             }, Math.random())
                         })
                     })
                 }), t.jsx("tbody", {
                     children: e.data.matrix.map(function(v, g) {
                         if (g > 0) return t.jsx("tr", {
-                            children: v.map(function(k, b) {
+                            children: v.map(function(C, b) {
                                 if (b == 0) return t.jsx("th", {
                                     className: "bold",
                                     align: "center",
                                     style: j,
-                                    children: k.text
+                                    children: C.text
                                 }, Math.random());
                                 {
                                     const E = {
-                                        backgroundColor: s(k),
+                                        backgroundColor: s(C),
                                         border: "solid 4px white"
                                     };
                                     return t.jsx("td", {
                                         align: "center",
                                         style: E,
                                         onMouseDown: h,
                                         onMouseLeave: h,
                                         onMouseUp: h,
                                         "data-day": e.data.matrix[0][b].text,
                                         "data-time": v[0].text,
-                                        children: k && k.text && t.jsx(mt, {
-                                            text: k.text,
-                                            children: t.jsx(C, {
+                                        children: C && C.text && t.jsx(mt, {
+                                            text: C.text,
+                                            children: t.jsx(S, {
                                                 icon: "stethoscope",
                                                 style: {
                                                     color: "white",
                                                     cursor: "help"
                                                 }
                                             })
                                         })
@@ -1823,15 +1823,15 @@
       .tooltip {
         position: relative;
         display: inline-block;
       }
       .tooltip .tooltiptext {
         visibility: hidden;
         width: 220px;
-        background-color: ${S.colors.highlight};
+        background-color: ${k.colors.highlight};
         color: #fff;
         text-align: center;
         border-radius: 6px;
         padding: 5px 0;
         position: absolute;
         z-index: 1;
         bottom: 150%;
@@ -1849,15 +1849,15 @@
                 children: W(e.text)
             })]
         })
     }
     return n()
 }
 const ft = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
-    J = {
+    V = {
         padding: 15,
         border: "solid 1px #d9d9d9",
         borderRadius: 5,
         backgroundColor: "white"
     };
 
 function gt(e) {
@@ -1865,30 +1865,30 @@
     for (let [a, r] of Array.from(n.entries())) {
         const i = e[a];
         i.tagName == "SELECT" && r !== "" || i.tagName == null && r !== "" || i.type == "radio" && r !== "" || i.type == "checkbox" && r !== "" || n.delete(a)
     }
     return new URLSearchParams(n).toString()
 }
 
-function Q(e, n) {
+function J(e, n) {
     const a = e.indexOf("?") < 0 ? "?" : "&",
         r = gt(n);
     return e = e + (r ? a + r : ""), e
 }
 
 function re(e) {
     if (e) {
         const a = [".png", ".jpeg", ".jpeg", ".gif"];
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
-function Y(e, n) {
-    q("GET", Q(n, e.closest("form")), Ee)
+function $(e, n) {
+    q("GET", J(n, e.closest("form")), Ee)
 }
 
 function xt(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -1936,29 +1936,29 @@
         for (var a in e.set) bt(a, e.set[a])
     }
 }
 
 function wt(e) {
     function n() {
         const a = {
-            color: S.colors.info,
-            backgroundColor: S.background.info,
+            color: k.colors.info,
+            backgroundColor: k.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(C, {
+                children: [t.jsx(S, {
                     icon: "circle-check",
                     style: {
-                        color: S.colors.info,
+                        color: k.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
@@ -1976,15 +1976,15 @@
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
             className: "error",
-            children: [t.jsx(C, {
+            children: [t.jsx(S, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -2014,15 +2014,15 @@
     function a() {
         const c = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.icon = null, e.data.action.modal = !0, e.data.action.urlfunc = function() {
-            return Q(e.data.action.url, document.getElementById(n).closest("form"))
+            return J(e.data.action.url, document.getElementById(n).closest("form"))
         }), t.jsxs("div", {
             style: c,
             children: [t.jsxs("label", {
                 className: "bold",
                 children: [e.data.label, " ", e.data.required ? "*" : ""]
             }), e.data.action && t.jsx(_, {
                 data: e.data.action,
@@ -2065,15 +2065,15 @@
         return t.jsx("div", {
             children: t.jsx(pt, {
                 id: e.data.name + "_error"
             })
         })
     }
 
-    function l() {
+    function o() {
         return e.data.help_text && t.jsx(jt, {
             text: e.data.help_text
         })
     }
 
     function d() {
         const c = {
@@ -2081,28 +2081,28 @@
             flexDirection: "column",
             padding: 5,
             width: "calc(100%-5px)"
         };
         return t.jsxs("div", {
             id: n,
             style: c,
-            children: [a(), r(), l(), i()]
+            children: [a(), r(), o(), i()]
         })
     }
     return d()
 }
 
 function ye(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), B.useEffect(() => {
-        function d(u, o, h) {
+        function d(u, l, h) {
             var f = h.target,
                 w = f.value.replace(/\D/g, ""),
-                y = f.value.length > o ? 1 : 0;
+                y = f.value.length > l ? 1 : 0;
             VMasker(f).unMask(), VMasker(f).maskPattern(u[y]), f.value = VMasker.toPattern(w, u[y])
         }
         if (e.data.mask) {
             var c = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
@@ -2112,75 +2112,75 @@
                 var s = e.data.mask.split("|");
                 VMasker(c).maskPattern(s[0]), c.addEventListener("input", d.bind(void 0, s, 14), !1)
             } else VMasker(c).maskPattern(e.data.mask)
         }
     }, []);
 
     function r(d) {
-        Y(d.target, e.data.onchange)
+        $(d.target, e.data.onchange)
     }
 
     function i(d) {
         if (e.data.type == "file" && d.target.files) {
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (re(s.name)) {
                     const w = "display" + a;
-                    var o = document.createElement("img");
-                    o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(y) {
-                        const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                    var l = document.createElement("img");
+                    l.id = d.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(y) {
+                        const D = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
                         var j = document.createElement("canvas");
                         const v = j.getContext("2d");
-                        j.height = j.width * (o.height / o.width);
+                        j.height = j.width * (l.height / l.width);
                         const g = document.createElement("canvas"),
-                            k = g.getContext("2d");
-                        g.width = o.width * D, g.height = o.height * D, k.drawImage(o, 0, 0, g.width, g.height), v.drawImage(g, 0, 0, g.width * D, g.height * D, 0, 0, j.width, j.height), g.toBlob(function(E) {
+                            C = g.getContext("2d");
+                        g.width = l.width * D, g.height = l.height * D, C.drawImage(l, 0, 0, g.width, g.height), v.drawImage(g, 0, 0, g.width * D, g.height * D, 0, 0, j.width, j.height), g.toBlob(function(E) {
                             const T = new DataTransfer;
                             T.items.add(new File([E], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
-                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
-                    }, o.src = u.target.result
+                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(l), d.target.parentNode.appendChild(b)
+                    }, l.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
                 var f = s.size / 1024;
                 f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + f, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
             }, c.readAsDataURL(s)
         }
     }
 
-    function l() {
+    function o() {
         var d = e.data.type;
         if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
             const u = {
                 alignContent: "center",
                 minHeight: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
             var c = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(o => "." + o).join(", ")), t.jsxs(t.Fragment, {
+            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(l => "." + l).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: S.colors.primary
+                                color: k.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
                         children: [e.data.value && re(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
@@ -2193,15 +2193,15 @@
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(o => "." + o).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
                         children: t.jsx(R, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
@@ -2220,32 +2220,32 @@
                         zIndex: "-1",
                         marginTop: -20
                     },
                     accept: c
                 })]
             })
         } else {
-            var s = J;
+            var s = V;
             return d == "color" && (s = {
-                ...J
+                ...V
             }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
                 "data-label": M(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: i,
                 style: s
             })
         }
     }
-    return l()
+    return o()
 }
 
 function Me(e) {
     var n = [];
     Array.isArray(e.data.value) ? e.data.value.forEach(function(b, E) {
         n.push({
             id: b.id,
@@ -2254,18 +2254,18 @@
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
         i = Array.isArray(e.data.value),
-        [l, d] = B.useState(!1),
+        [o, d] = B.useState(!1),
         [c, s] = B.useState(null);
     var u = !1;
-    let o;
+    let l;
     B.useEffect(() => {
         v(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
             v(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
@@ -2284,25 +2284,25 @@
                 };
             return t.jsxs("div", {
                 children: [b == null && n.map((p, I) => t.jsxs("div", {
                     style: E,
                     children: [t.jsx("span", {
                         onClick: () => g(I),
                         style: T,
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "trash-can",
                             style: m
                         })
                     }), p.value]
                 }, Math.random())), b != null && Array.from(b.options).map((p, I) => t.jsxs("div", {
                     style: E,
                     children: [t.jsx("span", {
                         onClick: () => g(I),
                         style: T,
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "trash-can",
                             style: m
                         })
                     }), p.innerHTML]
                 }, Math.random()))]
             })
         }
@@ -2318,15 +2318,15 @@
                 display: "contents"
             }
         })
     }
 
     function w() {
         const b = {
-                ...J,
+                ...V,
                 ...e.style || {}
             },
             E = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
@@ -2335,17 +2335,17 @@
                 overflowY: "auto",
                 zIndex: 99999
             };
         E.position = "absolute", E.backgroundColor = "white";
         const T = document.getElementById(r);
         if (e.data.icon && (b.paddingLeft = 30), T) {
             let N = null,
-                X = T,
+                Q = T,
                 ae = null;
-            for (; !ae && (X = X.parentElement) instanceof HTMLElement;) X.matches("dialog") && (ae = X);
+            for (; !ae && (Q = Q.parentElement) instanceof HTMLElement;) Q.matches("dialog") && (ae = Q);
             N = ae;
             const K = T.getBoundingClientRect();
             var m = K.top + K.height,
                 p = K.left;
             if (N) {
                 const fe = N.getBoundingClientRect();
                 m = m - fe.top, p = p - fe.left
@@ -2354,15 +2354,15 @@
         }
         const I = {
                 cursor: "pointer",
                 padding: 10
             },
             L = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
-            children: [e.data.icon && t.jsx(C, {
+            children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
@@ -2375,15 +2375,15 @@
                 },
                 onChange: j,
                 onMouseLeave: y,
                 onBlur: y,
                 defaultValue: L,
                 style: b,
                 "data-label": M(e.data.label)
-            }), c && l && t.jsxs("ul", {
+            }), c && o && t.jsxs("ul", {
                 style: E,
                 onMouseLeave: D,
                 onMouseEnter: function(N) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
                     style: I,
@@ -2407,52 +2407,52 @@
         }, 250)
     }
 
     function D(b) {
         const E = document.getElementById(a);
         if (E) {
             const T = document.getElementById(r);
-            i || E.options.length > 0 && T.value != E.options[0].innerHTML && (E.innerHTML = "", T.value = "", d(!1), e.data.onchange && Y(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
+            i || E.options.length > 0 && T.value != E.options[0].innerHTML && (E.innerHTML = "", T.value = "", d(!1), e.data.onchange && $(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
     function j(b) {
-        clearTimeout(o), o = setTimeout(function() {
+        clearTimeout(l), l = setTimeout(function() {
             const E = b.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), q("GET", Q(e.data.choices + T + "term=" + b.target.value, E), function(p) {
+            d(!0), q("GET", J(e.data.choices + T + "term=" + b.target.value, E), function(p) {
                 s(p)
             })
         }, 1e3)
     }
 
     function v(b, E = !1) {
         const T = document.getElementById(a),
             m = document.getElementById(r);
-        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !E && Y(m, e.data.onchange)
+        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !E && $(m, e.data.onchange)
     }
 
     function g(b) {
         const E = document.getElementById(a);
         var T = Array.from(E.options);
         E.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(m => `<option selected value="${m.value}">${m.innerHTML}</option>`).join(""), s([])
     }
 
-    function k() {
+    function C() {
         return t.jsxs(t.Fragment, {
             children: [h(), f(), w()]
         })
     }
-    return k()
+    return C()
 }
 
 function kt(e) {
     function n() {
         var a = {
-            ...J
+            ...V
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
             "data-label": M(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
@@ -2476,60 +2476,60 @@
 }
 
 function ie(e) {
     const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
-    function l(u) {
+    function o(u) {
         return i.value != null ? i.value == u.id ? !0 : i.value.id == u.id : !1
     }
 
     function d(u) {
-        var o = document.getElementById(u);
-        i.checked && (o.checked = !1), e.data.onchange && Y(o, e.data.onchange)
+        var l = document.getElementById(u);
+        i.checked && (l.checked = !1), e.data.onchange && $(l, e.data.onchange)
     }
 
     function c(u) {
-        var o = document.getElementById(u);
-        i.checked = o.checked
+        var l = document.getElementById(u);
+        i.checked = l.checked
     }
 
     function s() {
         return window["reload-" + i.name + "-field"] = function() {
-            q("GET", Q(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(o) {
-                a(o)
+            q("GET", J(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
+                a(l)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "radio-group " + i.name,
-            children: n.map((u, o) => (u.id || u.id === !1) && t.jsxs("div", {
+            children: n.map((u, l) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
                     display: "inline-block",
                     marginRight: 25,
                     width: window.innerWidth > 800 ? "auto" : "100%"
                 },
                 children: [t.jsx("input", {
-                    id: i.name + r + o,
+                    id: i.name + r + l,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
-                    defaultChecked: l(u),
+                    defaultChecked: o(u),
                     "data-label": M(u.value),
                     onClick: function() {
-                        d(i.name + r + o)
+                        d(i.name + r + l)
                     },
                     onMouseEnter: function() {
-                        c(i.name + r + o)
+                        c(i.name + r + l)
                     }
                 }), t.jsx("label", {
-                    htmlFor: i.name + r + o,
+                    htmlFor: i.name + r + l,
                     children: u.value
                 })]
-            }, r + o))
+            }, r + l))
         }) : t.jsx("div", {
             className: "radio-group " + i.name,
             children: t.jsx("i", {
                 children: "Nenhuma opção disponível para seleção."
             })
         })
     }
@@ -2537,31 +2537,31 @@
 }
 
 function ve(e) {
     const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
-    function l(s) {
+    function o(s) {
         var u = !1;
         if (i.value)
-            for (var o = 0; o < i.value.length; o++) {
-                var h = i.value[o];
+            for (var l = 0; l < i.value.length; l++) {
+                var h = i.value[l];
                 (h == s.id || h.id == s.id) && (u = !0)
             }
         return u
     }
 
     function d(s) {
-        e.data.onchange && Y(s.target, e.data.onchange)
+        e.data.onchange && $(s.target, e.data.onchange)
     }
 
     function c() {
         return window["reload-" + i.name + "-field"] = function() {
-            q("GET", Q(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
+            q("GET", J(e.data.pick, document.querySelector(".checkbox-group." + i.name).closest("form")), function(u) {
                 a(u)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "checkbox-group " + i.name,
             children: n.map((s, u) => (s.id || s.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
@@ -2571,15 +2571,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
-                    defaultChecked: l(s),
+                    defaultChecked: o(s),
                     "data-label": M(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
@@ -2597,15 +2597,15 @@
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
             "data-label": M(n.label),
             defaultValue: n.value,
-            style: J,
+            style: V,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
     })
 }
@@ -2614,41 +2614,41 @@
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(oe, {
+            children: t.jsxs(le, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
-                    onClick: () => l(!0),
+                    onClick: () => o(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => l(!1),
+                    onClick: () => o(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
-    function l(s) {
+    function o(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            o = document.getElementById("inline-form-" + n),
+            l = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
             f = document.getElementById("hide-" + n);
-        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+        l.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function d() {
         const s = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
@@ -2680,111 +2680,111 @@
 }
 
 function Mt(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(o, h) {
+    function r(l, h) {
         const f = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
             id: "form-" + f + "-" + a,
             children: [t.jsx(ue, {
-                data: o
+                data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
-                    onClick: () => l(),
+                    onClick: () => o(),
                     id: "extra-add-" + f + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => d(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function i() {
-        const o = c(),
-            h = o.length > 0 ? "none" : "inline";
+        const l = c(),
+            h = l.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
         for (var f = 0; f < n; f++) {
             var w = document.getElementById("extra-add-" + f + "-");
             w.style.display = "none"
         }
-        if (o.length > 0) {
-            var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
+        if (l.length > 0) {
+            var w = document.getElementById("extra-add-" + l[l.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
-    function l() {
+    function o() {
         i();
-        var o = JSON.parse(JSON.stringify(e.data.template));
-        o.fields ? (o.fields.map(function(h) {
+        var l = JSON.parse(JSON.stringify(e.data.template));
+        l.fields ? (l.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
-        }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
+        }), l.fields[0].value = 0) : l.fieldsets.map(function(h) {
             h.fields.map(function(f) {
                 f.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
                 }), f[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(i, 100)
     }
 
-    function d(o) {
+    function d(l) {
         const h = e.data.template,
-            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
+            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
             y = document.querySelector("input[name=" + w + "]");
-        parseInt(y.value) == 0 ? y.value = "" : y.value = -parseInt(y.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
+        parseInt(y.value) == 0 ? y.value = "" : y.value = -parseInt(y.value), document.getElementById("form-" + l + "-" + a).style.display = "none", i()
     }
 
     function c() {
-        for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
-        return o
+        for (var l = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && l.push(h);
+        return l
     }
 
     function s() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(oe, {
+            children: t.jsx(le, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
-                    onClick: () => l(),
+                    onClick: () => o(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const o = {
+        const l = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: o,
+                style: l,
                 "data-label": M(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
@@ -2822,36 +2822,36 @@
                 children: [t.jsx("h2", {
                     "data-label": M(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
-                    children: i.map(l => t.jsx("div", {
-                        className: "form-group " + l.name,
+                    children: i.map(o => t.jsx("div", {
+                        className: "form-group " + o.name,
                         style: {
                             width: 100 / i.length + "%",
-                            display: l.type == "hidden" ? "none" : "inline-block"
+                            display: o.type == "hidden" ? "none" : "inline-block"
                         },
-                        children: n(l)
+                        children: n(o)
                     }, Math.random()))
                 }, Math.random()))]
             })
         }, Math.random()))
     }
     return a()
 }
 
 function Tt(e) {
     const n = Math.random();
 
     function a() {
         const h = {
             margin: 0,
-            color: S.colors.primary
+            color: k.colors.primary
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
@@ -2871,15 +2871,15 @@
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
-    function l() {
+    function o() {
         return t.jsx(ue, {
             data: e.data
         })
     }
 
     function d() {
         return t.jsxs("div", {
@@ -2889,15 +2889,15 @@
             },
             children: [t.jsx(R, {
                 onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
             }), t.jsx(R, {
-                onClick: o,
+                onClick: l,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
@@ -2924,43 +2924,43 @@
             method: e.data.method,
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 5
                 },
-                children: [a(), r(), i(), l(), d(), c()]
+                children: [a(), r(), i(), o(), d(), c()]
             })]
         })
     }
 
     function u() {
-        V()
+        Y()
     }
 
-    function o(h) {
+    function l(h) {
         h.preventDefault();
         var f = e.data.url,
             w = document.getElementById(n),
             y = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
             const D = f.indexOf("?") >= 0 ? "&" : "?";
             f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
         }
         q(w.method.toUpperCase(), f, function(j) {
             if (w.querySelectorAll(".error").forEach(g => g.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), j.type == "response") j.store && Object.keys(j.store).map(function(g) {
                 j.store[g] ? localStorage.setItem(g, j.store[g]) : localStorage.removeItem(g, j.store[g])
-            }), j.redirect && j.redirect.length > 2 ? (j.message && localStorage.setItem("message", j.message), document.location.href = U(j.redirect)) : (j.message && z(j.message), j.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : V()), j.redirect == "." && w.reset(), j.dispose && (w.style.display = "none"), Ke());
+            }), j.redirect && j.redirect.length > 2 ? (j.message && localStorage.setItem("message", j.message), document.location.href = U(j.redirect)) : (j.message && z(j.message), j.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : Y()), j.redirect == "." && w.reset(), j.dispose && (w.style.display = "none"), Ke());
             else if (j.type == "error") {
                 var v = j.text;
                 console.log(j), Object.keys(j.errors).map(function(g) {
                     if (g == "__all__") v = j.errors[g];
                     else {
-                        const k = w.querySelector("#" + g + "_error");
-                        k.querySelector("span").innerHTML = j.errors[g], k.style.display = "block"
+                        const C = w.querySelector("#" + g + "_error");
+                        C.querySelector("span").innerHTML = j.errors[g], C.style.display = "block"
                     }
                 }), z(v, !0)
             } else {
                 const g = document.querySelector("#output");
                 g.innerHTML = "", H.createRoot(g.appendChild(document.createElement("div"))).render(t.jsx(x, {
                     data: j
                 }))
@@ -3016,24 +3016,24 @@
             margin: 0px;
         }       
     `);
     const n = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
         a = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
         r = new Date,
         i = e.data.day ? new Date(e.data.year, e.data.month - 1, e.data.day) : null;
-    for (var l = [
+    for (var o = [
             [],
             [],
             [],
             [],
             [],
             []
         ], d = e.data.month - 1, c = new Date(e.data.year, e.data.month - 1, 1); c.getDay() > 1;) c.setDate(c.getDate() - 1);
     for (var s = 0;
-        (c.getMonth() <= d || l[s].length < 7) && (l[s].length == 7 && (s += 1), s != 5);) l[s].push({
+        (c.getMonth() <= d || o[s].length < 7) && (o[s].length == 7 && (s += 1), s != 5);) o[s].push({
         date: c.getDate(),
         total: e.data.total[c.toLocaleDateString("pt-BR")],
         today: c.getDate() === r.getDate(),
         selected: i ? c.getDate() == i.getDate() : !1
     }), c.setDate(c.getDate() + 1);
 
     function u() {
@@ -3050,15 +3050,15 @@
                 }), t.jsxs("div", {
                     children: [t.jsxs("h3", {
                         align: "center",
                         children: [a[e.data.month - 1], " ", e.data.year]
                     }), e.data.day && t.jsxs("div", {
                         align: "center",
                         className: "day",
-                        children: [new Date(e.data.year, e.data.month - 1, e.data.day).toLocaleDateString("pt-BR"), t.jsx(C, {
+                        children: [new Date(e.data.year, e.data.month - 1, e.data.day).toLocaleDateString("pt-BR"), t.jsx(S, {
                             default: !0,
                             icon: "x",
                             onClick: () => e.onChange(null, e.data.month, e.data.year),
                             style: {
                                 marginLeft: 10,
                                 cursor: "pointer"
                             }
@@ -3070,36 +3070,36 @@
                         icon: "arrow-right",
                         onClick: () => e.onChange(null, e.data.next.month, e.data.next.year)
                     })
                 })]
             }), t.jsxs("table", {
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: n.map(o => t.jsx("th", {
-                            children: o
+                        children: n.map(l => t.jsx("th", {
+                            children: l
                         }, Math.random()))
                     })
                 }), t.jsx("tbody", {
-                    children: l.map(o => t.jsx("tr", {
-                        children: o.map(h => t.jsxs("td", {
+                    children: o.map(l => t.jsx("tr", {
+                        children: l.map(h => t.jsxs("td", {
                             children: [t.jsx("div", {
                                 className: "day",
                                 children: h.today ? t.jsx("span", {
                                     style: {
                                         textDecoration: "underline"
                                     },
                                     children: h.date
                                 }) : h.date + h.today
                             }), h.total && t.jsx("div", {
                                 className: "total",
                                 onClick: () => e.onChange(h.date, e.data.month, e.data.year),
                                 children: t.jsx("div", {
                                     className: "number",
                                     style: {
-                                        backgroundColor: S.colors.primary
+                                        backgroundColor: k.colors.primary
                                     },
                                     children: t.jsx("span", {
                                         style: {
                                             textDecoration: h.selected ? "underline" : "normal"
                                         },
                                         children: h.total
                                     })
@@ -3201,15 +3201,15 @@
     }
     return n()
 }
 
 function Bt(e) {
     function n() {
         const a = {
-            backgroundColor: S.colors.primary,
+            backgroundColor: k.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -3271,15 +3271,15 @@
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function l(m) {
+    function o(m) {
         document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
             children: n.subsets.map(function(m, p) {
@@ -3300,35 +3300,35 @@
                 }, Math.random())
             })
         })
     }
 
     function c(m) {
         const p = document.getElementById("subset-" + e.data.id);
-        p.value = m || "", k()
+        p.value = m || "", C()
     }
 
     function s(m, p, I) {
         const L = document.getElementById("form-" + e.data.id);
         L.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = I || "", y(1)
     }
 
     function u() {
         if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
-    function o(m) {
+    function l(m) {
         const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
-            color: S.colors.primary,
+            color: k.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
             children: [m.map(function(I) {
                 return I.label != "ID" && t.jsx("th", {
                     style: p,
                     className: "bold",
@@ -3356,15 +3356,15 @@
                 children: m.title
             }, Math.random()), t.jsx("td", {
                 style: I,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: t.jsx(C, {
+                    children: t.jsx(S, {
                         icon: "chevron-right",
                         onClick: () => Re(m.actions),
                         style: {
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
@@ -3410,15 +3410,15 @@
                 marginBottom: 15
             },
             children: n.data.map(function(m) {
                 return m.type = n.renderer, t.jsx(x, {
                     data: m
                 }, Math.random())
             })
-        }) : w()) : t.jsx(oe, {
+        }) : w()) : t.jsx(le, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
@@ -3432,27 +3432,27 @@
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: m,
             children: t.jsxs("table", {
                 style: p,
                 children: [t.jsx("thead", {
-                    children: o(n.data[0].data)
+                    children: l(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(I) {
                         return h(I)
                     })
                 })]
             })
         })
     }
 
     function y(m) {
         const I = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        I && (I.value = m), k(), v()
+        I && (I.value = m), C(), v()
     }
 
     function D() {
         const m = document.getElementById("form-" + e.data.id);
         if (m) {
             const p = m.querySelector("input[name=page]");
             p && (p.value = n.pagination.page.current)
@@ -3517,15 +3517,15 @@
                         return N.type != "hidden" && t.jsx("div", {
                             children: t.jsx(ee, {
                                 data: N
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: k,
+                            onClick: C,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
                 }), I && n.filters.map(function(N) {
                     return N.type == "hidden" && t.jsx("div", {
                         children: t.jsx(ee, {
@@ -3533,36 +3533,36 @@
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function k() {
-        l(!0);
+    function C() {
+        o(!0);
         var m;
         const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
         e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + p : m = e.data.url + "?" + p, q("GET", m, function(I) {
-            a(I), l(!1)
+            a(I), o(!1)
         })
     }
 
     function b() {
         const m = {
-            color: S.colors.primary
+            color: k.colors.primary
         };
         return e.data.reloadable && t.jsxs("div", {
             align: "center",
             children: [t.jsxs("i", {
                 children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
             }), t.jsx("div", {
                 children: t.jsx(O, {
                     style: m,
                     onClick: p => {
-                        p.preventDefault(), k()
+                        p.preventDefault(), C()
                     },
                     children: "Atualizar agora"
                 })
             })]
         })
     }
 
@@ -3584,15 +3584,15 @@
         }) : t.jsxs("div", {
             className: "content",
             children: [b(), j(), d(), g(), u(), f(), D()]
         })
     }
 
     function T() {
-        window[e.data.id] = () => k();
+        window[e.data.id] = () => C();
         const m = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable queryset",
             id: e.data.id,
@@ -3639,33 +3639,33 @@
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(i, l) {
+        return e.headers ? e.headers.slice(1).map(function(i, o) {
             return {
                 name: i,
                 type: "pie",
-                radius: n[l],
+                radius: n[o],
                 emphasis: {
                     label: {
                         show: !0,
                         formatter: function(d) {
                             return d.value.toLocaleString("pt-BR")
                         },
                         fontWeight: "bold"
                     }
                 },
                 roseType: null,
                 data: e.rows.map(function(d) {
                     return {
                         name: d[0],
-                        value: d[l + 1]
+                        value: d[o + 1]
                     }
                 })
             }
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
@@ -3675,36 +3675,36 @@
                     formatter: function(i) {
                         return i.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(i, l) {
+            data: e.rows.map(function(i, o) {
                 return {
                     name: i[0],
                     value: i[1]
                 }
             })
         }
     }
 
     function r() {
         var i = {
             tooltip: {
                 trigger: "item",
-                formatter: function(l) {
-                    return `${l.name}: <b>${l.data.value.toLocaleString("pt-BR")}</b> (${l.percent.toLocaleString("pt-BR")}%)`
+                formatter: function(o) {
+                    return `${o.name}: <b>${o.data.value.toLocaleString("pt-BR")}</b> (${o.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(l) {
-                    return l.name + " (" + l.percent.toLocaleString("pt-BR") + "%)"
+                formatter(o) {
+                    return o.name + " (" + o.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(ne, {
             option: i
         })
@@ -3731,15 +3731,15 @@
 function G(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         i = {
             type: "value"
         },
-        l = {
+        o = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
                 },
                 saveAsImage: {
                     show: !0
@@ -3750,43 +3750,43 @@
 
     function c() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(o) {
-                return o[0]
+            data: e.rows.map(function(l) {
+                return l[0]
             })
         }
     }
 
     function s() {
-        return e.headers ? e.rows.map(function(o) {
+        return e.headers ? e.rows.map(function(l) {
             return {
-                name: o[0],
-                data: o.slice(1),
+                name: l[0],
+                data: l.slice(1),
                 type: a,
                 stack: r,
                 areaStyle: d
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(o) {
-                return o[1]
+            data: e.rows.map(function(l) {
+                return l[1]
             }),
             type: a,
             stack: r,
             areaStyle: d
         }]
     }
 
     function u() {
-        var o = {
-            toolbox: l,
+        var l = {
+            toolbox: o,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(h) {
                     return `${h[0].name}: <b>${h[0].value.toLocaleString("pt-BR")}</b>`
@@ -3800,15 +3800,15 @@
                 }
             },
             xAxis: n ? i : c(),
             yAxis: n ? c() : i,
             series: s()
         };
         return t.jsx(ne, {
-            option: o
+            option: l
         })
     }
     return u()
 }
 
 function At(e) {
     return t.jsx(G, {
@@ -3865,18 +3865,18 @@
             type: "treemap",
             roam: "move",
             nodeClick: !0,
             data: e.headers.slice(1).map(function(r, i) {
                 return {
                     name: r,
                     type: "pie",
-                    children: e.rows.map(function(l) {
+                    children: e.rows.map(function(o) {
                         return {
-                            name: l[0],
-                            value: l[i + 1]
+                            name: o[0],
+                            value: o[i + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -4061,16 +4061,16 @@
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
-                    children: r.map((l, d) => t.jsx("tr", {
-                        children: l.map((c, s) => s == 0 ? t.jsx("th", {
+                    children: r.map((o, d) => t.jsx("tr", {
+                        children: o.map((c, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
                                 lineHeight: "2rem",
                                 padding: 5
                             },
                             className: d % 2 == 0 ? "even" : "odd",
                             children: c
@@ -4081,19 +4081,19 @@
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], i = [], l = Object.keys(e.data.series), d = [], c = 0; c < l.length; c++) {
+        for (var r = [], i = [], o = Object.keys(e.data.series), d = [], c = 0; c < o.length; c++) {
             c == 0 && r.push("");
-            for (var s = [l[c]], u = 0, o = 0; o < e.data.series[l[c]].length; o++) {
-                var h = e.data.series[l[c]];
-                c == 0 && r.push(h[o][0]), s.push(h[o][1]), u += h[o][1], l.length > 1 && (c == 0 ? d.push(h[o][1]) : d[o] += h[o][1], o > 0 && o == e.data.series[l[c]].length - 1 && (c == 0 ? d.push(u) : d[o + 1] += u))
+            for (var s = [o[c]], u = 0, l = 0; l < e.data.series[o[c]].length; l++) {
+                var h = e.data.series[o[c]];
+                c == 0 && r.push(h[l][0]), s.push(h[l][1]), u += h[l][1], o.length > 1 && (c == 0 ? d.push(h[l][1]) : d[l] += h[l][1], l > 0 && l == e.data.series[o[c]].length - 1 && (c == 0 ? d.push(u) : d[l + 1] += u))
             }
             s.length > 2 && (c == 0 && r.push(""), s.push(u)), i.push(s)
         }
         return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
@@ -4145,158 +4145,158 @@
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
 
 function Ut() {
     function e() {
-        const l = {
+        const o = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: S.colors.success
+            backgroundColor: k.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
-                    style: l
+                    style: o
                 })
             }), t.jsx("div", {
                 children: t.jsx(O, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
             })]
         })
     }
 
-    function n(l) {
-        var d = l.target;
+    function n(o) {
+        var d = o.target;
         const c = d.querySelector(":scope > ul, :scope > li");
         if (c) {
-            c.offsetParent === null ? d.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(o) {
-                o.style.display = "block"
-            }) : d.querySelectorAll(":scope > ul, :scope > li").forEach(function(o) {
-                o.style.display = "none"
+            c.offsetParent === null ? d.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(l) {
+                l.style.display = "block"
+            }) : d.querySelectorAll(":scope > ul, :scope > li").forEach(function(l) {
+                l.style.display = "none"
             });
             const s = d.querySelector(":scope > i.fa-solid.fa-chevron-right"),
                 u = d.querySelector(":scope > i.fa-solid.fa-chevron-up");
-            return s && (s.classList.remove("fa-chevron-right"), s.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), l.preventDefault(), l.stopPropagation(), l.cancelBubble = !0, !1
+            return s && (s.classList.remove("fa-chevron-right"), s.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), o.preventDefault(), o.stopPropagation(), o.cancelBubble = !0, !1
         } else {
             const s = document.querySelector("aside");
             s.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
-    function a(l, d) {
+    function a(o, d) {
         const c = {
                 display: d == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 15,
                 paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: S.colors.primary
+                color: k.colors.primary
             },
             s = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
-        return l.url ? t.jsx("li", {
+        return o.url ? t.jsx("li", {
             style: c,
             onClick: n,
             className: "item",
             children: t.jsxs(O, {
-                href: l.url,
-                dataLabel: M(l.label),
+                href: o.url,
+                dataLabel: M(o.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [d == 0 && t.jsx(C, {
-                    icon: l.icon || "dot-circle",
+                children: [d == 0 && t.jsx(S, {
+                    icon: o.icon || "dot-circle",
                     style: s
-                }), l.label]
+                }), o.label]
             })
-        }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
+        }, Math.random()) : o.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": M(l.label),
-            children: [d == 0 && t.jsx(C, {
-                icon: l.icon || "dot-circle",
+            "data-label": M(o.label),
+            children: [d == 0 && t.jsx(S, {
+                icon: o.icon || "dot-circle",
                 style: s
-            }), l.label, t.jsx(C, {
+            }), o.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
                     display: "none",
                     paddingLeft: 15
                 },
-                children: l.items.map(function(u) {
+                children: o.items.map(function(u) {
                     return a(u, d + 1)
                 })
             })]
         }, Math.random())
     }
 
     function r() {
-        const l = {
+        const o = {
             padding: 0
         };
         return window.application.menu.items.length > 0 && t.jsx("ul", {
-            style: l,
+            style: o,
             children: window.application.menu.items.map(function(d) {
                 return a(d, 0)
             })
         })
     }
 
     function i() {
-        const l = {
+        const o = {
             marginTop: 10,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             className: "menu",
             children: [e(), r()]
         })
     }
     return i()
 }
 
 function Gt(e) {
     var n;
 
-    function a(l) {
-        const d = "=".repeat((4 - l.length % 4) % 4),
-            c = (l + d).replace(/\-/g, "+").replace(/_/g, "/"),
+    function a(o) {
+        const d = "=".repeat((4 - o.length % 4) % 4),
+            c = (o + d).replace(/\-/g, "+").replace(/_/g, "/"),
             s = window.atob(c),
             u = new Uint8Array(s.length);
-        for (let o = 0; o < s.length; ++o) u[o] = s.charCodeAt(o);
+        for (let l = 0; l < s.length; ++l) u[l] = s.charCodeAt(l);
         return u
     }
 
     function r() {
-        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(l) {
-            if (l) {
+        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(o) {
+            if (o) {
                 const d = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
-                l.pushManager.subscribe({
+                o.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: d
                 }).then(function(c) {
                     if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
                         var s = new FormData;
                         s.append("subscription", n), q("POST", "/api/pushsubscribe/", function(u) {
@@ -4306,41 +4306,64 @@
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(c) {
                     alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", c)
                 })
             } else console.log("No registered service worker.")
-        }).catch(function(l) {
-            alert("Erro"), console.error("Service Worker Error", l)
+        }).catch(function(o) {
+            alert("Erro"), console.error("Service Worker Error", o)
         }) : alert("Push messaging is not supported")
     }
 
     function i() {
-        return t.jsx(C, {
+        return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: S.colors.primary
+                color: k.colors.primary
             }
         })
     }
     return i()
 }
 
-function Vt(e) {
+function Yt(e, n) {
+    var a = {
+            startX: 0,
+            startY: 0,
+            endX: 0,
+            endY: 0,
+            minX: 30,
+            maxX: 30,
+            minY: 50,
+            maxY: 60
+        },
+        r = null;
+    e.addEventListener("touchstart", function(i) {
+        var o = i.touches[0];
+        a.startX = o.screenX, a.startY = o.screenY
+    }), e.addEventListener("touchmove", function(i) {
+        var o = i.touches[0];
+        a.endX = o.screenX, a.endY = o.screenY
+    }), e.addEventListener("touchend", function(i) {
+        Math.abs(a.endX - a.startX) > a.minX && Math.abs(a.endY - a.startY) < a.maxY ? r = a.endX > a.startX ? "right" : "left" : Math.abs(a.endY - a.startY) > a.minY && Math.abs(a.endX - a.startX) < a.maxX && (r = a.endY > a.startY ? "down" : "up"), r !== null && typeof n == "function" && n(e, r)
+    })
+}
+
+function Xt(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: S.colors.primary,
+                backgroundColor: k.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -4350,38 +4373,38 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 100
                 },
                 onClick: () => history.back(),
-                children: t.jsx(C, {
+                children: t.jsx(S, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
                 onClick: () => window.scrollTo({
                     top: 0,
                     behavior: "smooth"
                 }),
-                children: t.jsx(C, {
+                children: t.jsx(S, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
-function $t(e) {
+function Vt(e) {
     const [n, a] = B.useState(e.data);
     window.loaddata = i => a(i);
 
     function r() {
         const i = {
             minHeight: 400,
             margin: window.innerWidth > 800 ? 20 : 5
@@ -4393,35 +4416,37 @@
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
-function Jt(e) {
+function $t(e) {
     B.useEffect(() => {
-        const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), z(o)), window.addEventListener("resize", () => {
+        const l = localStorage.getItem("message");
+        l && (localStorage.removeItem("message"), z(l)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
+        }), Yt(document.querySelector("main"), function(h, f) {
+            console.log(h, f)
         })
     }, []);
 
     function a() {
-        const o = document.querySelector("aside");
-        o.style.display = o.style.display == "none" ? "block" : "none"
+        const l = document.querySelector("aside");
+        l.style.display = l.style.display == "none" ? "block" : "none"
     }
 
-    function r(o) {
-        const h = o.target.tagName == "A" ? o.target : o.target.closest("a");
-        o.preventDefault(), window.load(h.href)
+    function r(l) {
+        const h = l.target.tagName == "A" ? l.target : l.target.closest("a");
+        l.preventDefault(), window.load(h.href)
     }
 
     function i() {
-        const o = {
+        const l = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
             h = {
@@ -4431,20 +4456,20 @@
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice",
                 icon: "search"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: o,
+            style: l,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [e.data.menu && t.jsx(C, {
+                children: [e.data.menu && t.jsx(S, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -4477,15 +4502,15 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
@@ -4518,27 +4543,27 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(C, {
+                        children: t.jsx(S, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
                     children: t.jsx(Me, {
                         data: h,
                         style: {
@@ -4557,84 +4582,85 @@
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: S.colors.primary
+                                backgroundColor: k.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
 
-    function l() {
+    function o() {
         return window.application.menu && window.application.menu.items.length > 0 && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
             children: t.jsx(Ut, {})
         })
     }
 
     function d() {
-        const o = {
+        const l = {
                 margin: 15,
                 display: "flex",
                 justifyContent: "space-between"
             },
             h = {
-                color: S.colors.primary
+                color: k.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
-            style: o,
+            style: l,
             children: [t.jsxs("div", {
                 children: [t.jsx(O, {
                     href: "/app/dashboard/",
                     style: {
                         marginRight: 10
                     },
-                    children: t.jsx(C, {
+                    children: t.jsx(S, {
                         icon: "home",
                         style: h
                     })
                 }), "Área Administrativa"]
             }), t.jsx("div", {
                 children: e.data.navbar.user
             })]
         })
     }
 
     function c() {
         return t.jsxs("main", {
+            id: "main",
             style: {
                 width: "100vw"
             },
-            children: [d(), t.jsx($t, {
+            children: [d(), t.jsx(Vt, {
                 data: e.data.content
             }), t.jsx("footer", {
                 children: s()
-            }), t.jsx(Vt, {})]
+            }), t.jsx(Xt, {})]
         })
     }
 
     function s() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
                 children: window.application.sponsors && window.application.sponsors.length > 0 && t.jsx("div", {
-                    children: window.application.sponsors.map(function(o) {
+                    children: window.application.sponsors.map(function(l) {
                         return t.jsx("img", {
-                            src: o,
+                            src: l,
                             style: {
                                 height: 30,
                                 padding: 5
                             }
                         }, Math.random())
                     })
                 })
@@ -4652,144 +4678,120 @@
                 children: i()
             }), t.jsxs("div", {
                 style: {
                     width: "100%",
                     display: "flex",
                     minHeight: window.innerHeight - 70
                 },
-                children: [l(), c()]
+                children: [o(), c()]
             })]
         })
     }
     return u()
 }
 
-function Yt(e) {
+function Jt(e) {
     var n = null,
         a = null,
         r = null,
         i = !1,
-        l = null,
+        o = null,
         d = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
         c = {
             constraints: {
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
             sdpTransform: v => v.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
-    B.useEffect(() => (n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(v) {
-        document.getElementById("callerid").innerHTML = e.data.caller, D()
-    }), n.on("call", function(v) {
-        d({
-            video: {
-                width: {
-                    exact: 320
-                },
-                height: {
-                    exact: 240
-                }
-            },
-            audio: !0
-        }, function(g) {
-            a = g;
-            var k = document.getElementById("video2");
-            k.addEventListener("loadedmetadata", function(b) {
-                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
-            }, !1), k.srcObject = a, v.answer(g), v.on("stream", function(b) {
-                r = b, document.getElementById("video1").srcObject = r, i = !0
-            }), v.on("close", function() {
-                console.log("Closed!"), i = !1
-            }), n.on("error", function(b) {
-                console.log("Error!"), i = !1
+    const s = {
+        video: {
+            width: {
+                exact: 320
+            },
+            height: {
+                exact: 240
+            },
+            frameRate: {
+                ideal: 5,
+                max: 10
+            }
+        },
+        audio: !0
+    };
+
+    function u() {
+        console.log("Trying to connect..."), n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(v) {
+            document.getElementById("callerid").innerHTML = e.data.caller, D(), o = setInterval(function() {
+                i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), D())
+            }, 15e3)
+        }), n.on("call", function(v) {
+            d(s, function(g) {
+                a = g;
+                var C = document.getElementById("video2");
+                C.addEventListener("loadedmetadata", function(b) {
+                    C.style.width = this.videoWidth / 4 + "px", C.style.height = this.videoHeight / 4 + "px", C.style.marginLeft = -this.videoWidth / 4 + "px", C.style.visibility = "visible"
+                }, !1), C.srcObject = a, v.answer(g), v.on("stream", function(b) {
+                    r = b, document.getElementById("video1").srcObject = r, i = !0
+                }), v.on("close", function() {
+                    console.log("Closed!"), i = !1
+                })
+            }, function(g) {
+                console.log("Failed to get local stream", g)
             })
-        }, function(g) {
-            console.log("Failed to get local stream", g)
+        }), n.on("error", function(v) {
+            v.type == "browser-incompatible" ? alert("Navegador incompatível.") : v.type == "invalid-id" ? alert("Usuário inexistente.") : v.type == "network" ? (i = !1, console.log("Problema na conexão do usuário. Tentando novamente em 5 segundos."), setTimeout(u, 5e3)) : v.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
         })
-    }), n.on("error", function(v) {
-        v.type == "browser-incompatible" ? alert("Navegador incompatível.") : v.type == "invalid-id" ? alert("Usuário inexistente.") : v.type == "network" ? alert("Problema na conexão do usuário.") : v.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
-    }), l = setInterval(function() {
-        i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), D())
-    }, 15e3), function() {
-        clearInterval(l), u(), z("Desconectado!")
-    }), []);
-
-    function s() {
-        h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
+    B.useEffect(() => (u(), function() {
+        clearInterval(o), l(), z("Desconectado!")
+    }), []);
 
-    function u() {
-        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video"), a = null, r = null;
+    function l() {
+        h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video"), a = null, r = null;
         const v = document.getElementById("video1"),
             g = document.getElementById("video2");
-        v && (v.srcObject = null), g && (g.srcObject = null), console.log("Stopped!")
-    }
-
-    function o(v, g) {
-        v != null && v.getTracks().forEach(k => {
-            k.kind === g && k.stop()
-        })
+        v && (v.srcObject = null), g && (g.srcObject = null), console.log("Stopped!"), i = !1
     }
 
     function h(v, g) {
-        v != null && v.getTracks().forEach(k => {
-            k.readyState == "live" && k.kind === g && (k.enabled = !1)
+        v != null && v.getTracks().forEach(C => {
+            C.kind === g && C.stop()
         })
     }
 
     function f() {
         var v = document.getElementById("video1");
         v.style.width = v.getClientRects()[0].width + 100 + "px"
     }
 
     function w() {
         var v = document.getElementById("video1");
         v.style.width = v.getClientRects()[0].width - 100 + "px"
     }
 
     function y() {
-        var v = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, c);
-        v.on("stream", function(g) {
+        var v = n.call("123456789" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
+        v && (v.on("stream", function(g) {
             r = g, document.getElementById("video1").srcObject = r, i = !0
         }), v.on("close", function() {
             console.log("Closed!"), i = !1
-        }), n.on("error", function(g) {
-            console.log("Error!"), i = !1
-        })
+        }))
     }
 
     function D() {
         if (a != null && !i) return y();
-        d({
-            video: {
-                width: {
-                    exact: 320
-                },
-                height: {
-                    exact: 240
-                }
-            },
-            audio: {
-                autoGainControl: !1,
-                channelCount: 2,
-                echoCancellation: !1,
-                latency: 0,
-                noiseSuppression: !1,
-                sampleRate: 48e3,
-                sampleSize: 16,
-                volume: 1
-            }
-        }, function(v) {
+        a == null && d(s, function(v) {
             a = v;
             var g = document.getElementById("video2");
-            g.addEventListener("loadedmetadata", function(k) {
+            g.addEventListener("loadedmetadata", function(C) {
                 g.style.width = this.videoWidth / 4 + "px", g.style.height = this.videoHeight / 4 + "px", g.style.marginLeft = -this.videoWidth / 4 + "px", g.style.visibility = "visible"
             }, !1), g.srcObject = a, y()
         }, function(v) {
             alert("Failed to get local stream.")
         })
     }
 
@@ -4799,18 +4801,19 @@
                 margin: "auto"
             },
             g = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            k = {
+            C = {
                 color: "white",
                 backgroundColor: "black",
-                padding: 2
+                paddingLeft: 15,
+                paddingRight: 15
             },
             b = {
                 position: "absolute",
                 marginTop: "-30px"
             },
             E = {
                 backgroundColor: "black"
@@ -4829,33 +4832,30 @@
                 style: E,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
                 style: T,
                 playsInline: !0,
-                autoPlay: !0
+                autoPlay: !0,
+                muted: "muted"
             }), t.jsxs("div", {
                 style: b,
-                children: [t.jsx(C, {
-                    style: k,
-                    onClick: s,
-                    icon: "pause"
-                }), t.jsx(C, {
-                    style: k,
-                    onClick: u,
-                    icon: "stop"
-                }), t.jsx(C, {
-                    style: k,
+                children: [t.jsx(S, {
+                    style: C,
                     onClick: f,
                     icon: "search-plus"
-                }), t.jsx(C, {
-                    style: k,
+                }), t.jsx(S, {
+                    style: C,
                     onClick: w,
                     icon: "search-minus"
+                }), t.jsx(S, {
+                    style: C,
+                    onClick: () => document.location.reload(),
+                    icon: "undo"
                 })]
             })]
         })
     }
     return j()
 }
 
@@ -4869,15 +4869,15 @@
             style: n,
             children: e.data.text
         })
     }
     return a()
 }
 var te, me = {};
-const Xt = "/api/application/",
+const Kt = "/api/application/",
     we = localStorage.getItem("application");
 
 function x(e) {
     const n = me[e.data.type];
     return n ? Te.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
@@ -4890,42 +4890,42 @@
 x.render = function(e) {
     te = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
 x.register(ht, "Counter");
 x.register(Tt, "Form");
 x.register(Nt, "QuerySet");
 x.register(Ge, "Fieldset");
-x.register($, "Field");
-x.register(Je, "Object");
-x.register(Ye, "Section");
-x.register(Xe, "Group");
+x.register(X, "Field");
+x.register(Ve, "Object");
+x.register($e, "Section");
+x.register(Qe, "Group");
 x.register(Pt, "Statistics");
 x.register(et, "Image");
 x.register(Ze, "Banner");
 x.register(tt, "Map");
 x.register(nt, "Steps");
 x.register(st, "QrCode");
 x.register(Se, "Badge");
 x.register(rt, "Status");
 x.register(at, "Progress");
 x.register(Ie, "Color");
 x.register(it, "Boxes");
 x.register(ct, "Indicators");
-x.register(lt, "Shell");
-x.register(ot, "FileLink");
+x.register(ot, "Shell");
+x.register(lt, "FileLink");
 x.register(dt, "FilePreview");
 x.register(Le, "Response");
-x.register(Jt, "Application");
+x.register($t, "Application");
 x.register(De, "IconSet");
 x.register(ut, "Grid");
 x.register(He, "Rows");
 x.register(Pe, "Cards");
 x.register(Ue, "Timeline");
 x.register(Ce, "Scheduler");
-x.register(Yt, "WebConf");
+x.register(Jt, "WebConf");
 x.register(Qt, "Text");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
     me[n] ? q("GET", A(e), function(a) {
@@ -4937,15 +4937,15 @@
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
     }, "", e), we ? (window.application = JSON.parse(we), q("GET", A(e), function(a) {
         window.application.content = a, te.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
-    })) : q("GET", Xt, function(r) {
+    })) : q("GET", Kt, function(r) {
         window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(i) {
             window.application.content = i, te.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
```

### Comparing `pyslth-0.3.6/slth/static/js/vanilla-masker.js` & `pyslth-0.3.7/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.7/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/statistics.py` & `pyslth-0.3.7/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/templates/index.html` & `pyslth-0.3.7/slth/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   <title>{{ application.version }} {{ application.title }}</title>
   <link rel="stylesheet" href="/static/css/style.css">
   <link rel="stylesheet" href="/static/css/slth.css">
   <link rel="stylesheet" href="/static/css/fontawesome.min.css">
   <link rel="stylesheet" href="/static/css/solid.min.css">
   <script type="module" src="/static/js/vanilla-masker.min.js"></script>
   <script type="module" src="/static/js/react-trigger-change.js"></script>
+  <script type="module" src="/static/js/default-passive-events.min.js"></script>
   <!-- <script type="module" src="/static/js/qrcode.min.js"></script> -->
   <script type="module" src="/static/js/peerjs.min.js"></script>
   <script type="module" src="/static/js/echarts.min.js"></script>
   <!-- <script src="/static/js/ios-splash.min.js"></script>
   <script>iosPWASplash('{{ application.icon }}', '#FFFFFF');</script>-->
 
   <link rel="manifest" href="/api/manifest/">
```

### Comparing `pyslth-0.3.6/slth/templates/service-worker.js` & `pyslth-0.3.7/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/tests.py` & `pyslth-0.3.7/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/urls.py` & `pyslth-0.3.7/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/utils.py` & `pyslth-0.3.7/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.6/slth/views.py` & `pyslth-0.3.7/slth/views.py`

 * *Files identical despite different names*

