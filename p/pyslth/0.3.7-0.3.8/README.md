# Comparing `tmp/pyslth-0.3.7.tar.gz` & `tmp/pyslth-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.7.tar", last modified: Sun May 19 19:48:10 2024, max compression
+gzip compressed data, was "pyslth-0.3.8.tar", last modified: Sun May 19 20:17:27 2024, max compression
```

## Comparing `pyslth-0.3.7.tar` & `pyslth-0.3.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.818979 pyslth-0.3.7/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.7/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 19:48:10.818745 pyslth-0.3.7/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.781910 pyslth-0.3.7/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 19:48:10.000000 pyslth-0.3.7/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.7/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 19:48:10.819054 pyslth-0.3.7/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 19:47:28.000000 pyslth-0.3.7/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.788920 pyslth-0.3.7/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.7/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.7/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.789532 pyslth-0.3.7/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.7/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.7/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.7/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.7/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.7/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.789858 pyslth-0.3.7/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.790533 pyslth-0.3.7/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.7/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.7/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.793629 pyslth-0.3.7/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.7/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.7/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.7/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.7/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.7/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.7/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.7/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.7/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.7/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.7/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.794121 pyslth-0.3.7/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.7/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.7/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.7/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.794432 pyslth-0.3.7/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.796832 pyslth-0.3.7/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.7/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.800836 pyslth-0.3.7/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.7/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.7/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.7/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.7/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.7/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.803312 pyslth-0.3.7/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.7/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.7/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.7/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.7/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.7/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.817436 pyslth-0.3.7/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.3.7/slth/static/js/default-passive-events.min.js
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.7/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.7/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.7/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102043 2024-05-19 19:47:51.000000 pyslth-0.3.7/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.7/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.7/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 19:48:10.818302 pyslth-0.3.7/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.3.7/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.7/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.7/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.7/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.7/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.7/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.539356 pyslth-0.3.8/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.8/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 20:17:27.539142 pyslth-0.3.8/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.507151 pyslth-0.3.8/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 20:17:27.000000 pyslth-0.3.8/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 20:17:27.000000 pyslth-0.3.8/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 20:17:27.000000 pyslth-0.3.8/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 20:17:27.000000 pyslth-0.3.8/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 20:17:27.000000 pyslth-0.3.8/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.8/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 20:17:27.539420 pyslth-0.3.8/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 20:17:20.000000 pyslth-0.3.8/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.514097 pyslth-0.3.8/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.8/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.8/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.514794 pyslth-0.3.8/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.8/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.8/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.8/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.8/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.8/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.8/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.515088 pyslth-0.3.8/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.8/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.515897 pyslth-0.3.8/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.8/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.8/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.8/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.518890 pyslth-0.3.8/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.8/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.8/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.8/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.8/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.8/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.8/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.8/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.8/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.8/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.8/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.8/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.8/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.519388 pyslth-0.3.8/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.8/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.8/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.8/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.519709 pyslth-0.3.8/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.521754 pyslth-0.3.8/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.8/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.526113 pyslth-0.3.8/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.8/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.8/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.8/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.8/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.8/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.8/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.8/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.528588 pyslth-0.3.8/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.8/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.8/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.8/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.8/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.8/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.538078 pyslth-0.3.8/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.3.8/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.8/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 20:16:47.000000 pyslth-0.3.8/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.8/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.8/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 20:16:47.000000 pyslth-0.3.8/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102040 2024-05-19 20:16:47.000000 pyslth-0.3.8/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.8/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.8/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:17:27.538735 pyslth-0.3.8/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.3.8/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.8/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.8/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.8/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.8/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.8/slth/views.py
```

### Comparing `pyslth-0.3.7/PKG-INFO` & `pyslth-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.7
+Version: 0.3.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.7/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.8/pyslth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.7
+Version: 0.3.8
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.7/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.8/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/setup.py` & `pyslth-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.7',
+    version='0.3.8',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.7/slth/__init__.py` & `pyslth-0.3.8/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/components.py` & `pyslth-0.3.8/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/db/models.py` & `pyslth-0.3.8/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/endpoints.py` & `pyslth-0.3.8/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/factory.py` & `pyslth-0.3.8/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/forms.py` & `pyslth-0.3.8/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/management/commands/integration_test.py` & `pyslth-0.3.8/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/management/commands/sync.py` & `pyslth-0.3.8/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/migrations/0001_initial.py` & `pyslth-0.3.8/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.8/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/migrations/0006_user.py` & `pyslth-0.3.8/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/models.py` & `pyslth-0.3.8/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/notifications.py` & `pyslth-0.3.8/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/oauth.py` & `pyslth-0.3.8/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/permissions.py` & `pyslth-0.3.8/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/queryset.py` & `pyslth-0.3.8/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/roles.py` & `pyslth-0.3.8/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/selenium/__init__.py` & `pyslth-0.3.8/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/selenium/browser.py` & `pyslth-0.3.8/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/serializer.py` & `pyslth-0.3.8/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/.DS_Store` & `pyslth-0.3.8/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fontawesome.min.css` & `pyslth-0.3.8/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.8/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.8/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.8/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.8/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.8/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/slth.css` & `pyslth-0.3.8/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/css/solid.min.css` & `pyslth-0.3.8/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/images/logo.png` & `pyslth-0.3.8/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/images/logo.svg` & `pyslth-0.3.8/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/images/user.png` & `pyslth-0.3.8/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/default-passive-events.min.js` & `pyslth-0.3.8/slth/static/js/default-passive-events.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/echarts.min.js` & `pyslth-0.3.8/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/index.min.js` & `pyslth-0.3.8/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/ios-splash.min.js` & `pyslth-0.3.8/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/peerjs.min.js` & `pyslth-0.3.8/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/qrcode.min.js` & `pyslth-0.3.8/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/react-trigger-change.js` & `pyslth-0.3.8/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/react.min.js` & `pyslth-0.3.8/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/slth.min.js` & `pyslth-0.3.8/slth/static/js/slth.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4720,15 +4720,15 @@
                 max: 10
             }
         },
         audio: !0
     };
 
     function u() {
-        console.log("Trying to connect..."), n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(v) {
+        console.log("Trying to connect..."), n = new Peer("999123" + e.data.caller.replaceAll(".", "")), n.on("open", function(v) {
             document.getElementById("callerid").innerHTML = e.data.caller, D(), o = setInterval(function() {
                 i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), D())
             }, 15e3)
         }), n.on("call", function(v) {
             d(s, function(g) {
                 a = g;
                 var C = document.getElementById("video2");
@@ -4770,15 +4770,15 @@
 
     function w() {
         var v = document.getElementById("video1");
         v.style.width = v.getClientRects()[0].width - 100 + "px"
     }
 
     function y() {
-        var v = n.call("123456789" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
+        var v = n.call("999123" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
         v && (v.on("stream", function(g) {
             r = g, document.getElementById("video1").srcObject = r, i = !0
         }), v.on("close", function() {
             console.log("Closed!"), i = !1
         }))
     }
```

### Comparing `pyslth-0.3.7/slth/static/js/vanilla-masker.js` & `pyslth-0.3.8/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.8/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/statistics.py` & `pyslth-0.3.8/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/templates/index.html` & `pyslth-0.3.8/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/templates/service-worker.js` & `pyslth-0.3.8/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/tests.py` & `pyslth-0.3.8/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/urls.py` & `pyslth-0.3.8/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/utils.py` & `pyslth-0.3.8/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.7/slth/views.py` & `pyslth-0.3.8/slth/views.py`

 * *Files identical despite different names*

