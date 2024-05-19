# Comparing `tmp/pyslth-0.3.9.tar.gz` & `tmp/pyslth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.9.tar", last modified: Sun May 19 20:28:57 2024, max compression
+gzip compressed data, was "pyslth-0.4.0.tar", last modified: Sun May 19 21:09:05 2024, max compression
```

## Comparing `pyslth-0.3.9.tar` & `pyslth-0.4.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.359127 pyslth-0.3.9/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.9/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 20:28:57.358900 pyslth-0.3.9/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.323008 pyslth-0.3.9/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 20:28:57.000000 pyslth-0.3.9/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 20:28:57.000000 pyslth-0.3.9/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 20:28:57.000000 pyslth-0.3.9/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 20:28:57.000000 pyslth-0.3.9/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 20:28:57.000000 pyslth-0.3.9/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.9/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 20:28:57.359188 pyslth-0.3.9/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 20:28:53.000000 pyslth-0.3.9/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.332963 pyslth-0.3.9/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.9/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.9/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.333590 pyslth-0.3.9/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.9/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.9/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.9/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.9/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.9/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.9/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.333876 pyslth-0.3.9/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.9/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.334499 pyslth-0.3.9/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.9/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.9/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.9/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.337437 pyslth-0.3.9/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.9/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.9/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.9/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.9/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.9/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.9/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.9/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.9/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.9/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.9/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.9/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.9/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.337932 pyslth-0.3.9/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.9/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.9/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.9/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.338264 pyslth-0.3.9/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.340375 pyslth-0.3.9/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.9/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.345199 pyslth-0.3.9/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.9/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.9/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.9/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.9/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.9/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.9/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.9/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.347718 pyslth-0.3.9/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.9/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.9/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.9/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.9/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.9/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.357886 pyslth-0.3.9/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.3.9/slth/static/js/default-passive-events.min.js
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.9/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 20:28:35.000000 pyslth-0.3.9/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.9/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.9/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 20:28:35.000000 pyslth-0.3.9/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102059 2024-05-19 20:28:35.000000 pyslth-0.3.9/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.9/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.9/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 20:28:57.358512 pyslth-0.3.9/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.3.9/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.9/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.9/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.9/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.9/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.9/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.699151 pyslth-0.4.0/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.0/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:09:05.698912 pyslth-0.4.0/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.665763 pyslth-0.4.0/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.0/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 21:09:05.699212 pyslth-0.4.0/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 21:08:17.000000 pyslth-0.4.0/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.672954 pyslth-0.4.0/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.0/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.4.0/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.673620 pyslth-0.4.0/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.0/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.0/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.4.0/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.0/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.4.0/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.673910 pyslth-0.4.0/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.674588 pyslth-0.4.0/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.0/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.0/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.677395 pyslth-0.4.0/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.0/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.0/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.0/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.0/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.0/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.0/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.0/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.0/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.677859 pyslth-0.4.0/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.0/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.0/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.4.0/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.678162 pyslth-0.4.0/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.680299 pyslth-0.4.0/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.0/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.684548 pyslth-0.4.0/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.0/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.0/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.0/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.0/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.687106 pyslth-0.4.0/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.0/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.0/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.0/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.0/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.0/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.697823 pyslth-0.4.0/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.0/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.0/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.0/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.0/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102225 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.0/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.698467 pyslth-0.4.0/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.4.0/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.0/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.0/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.0/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.0/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.0/slth/views.py
```

### Comparing `pyslth-0.3.9/PKG-INFO` & `pyslth-0.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.9
+Version: 0.4.0
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.9/pyslth.egg-info/PKG-INFO` & `pyslth-0.4.0/pyslth.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.9
+Version: 0.4.0
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.9/pyslth.egg-info/SOURCES.txt` & `pyslth-0.4.0/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/setup.py` & `pyslth-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.9',
+    version='0.4.0',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.9/slth/__init__.py` & `pyslth-0.4.0/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/components.py` & `pyslth-0.4.0/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/db/models.py` & `pyslth-0.4.0/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/endpoints.py` & `pyslth-0.4.0/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/factory.py` & `pyslth-0.4.0/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/forms.py` & `pyslth-0.4.0/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/management/commands/integration_test.py` & `pyslth-0.4.0/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/management/commands/sync.py` & `pyslth-0.4.0/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/migrations/0001_initial.py` & `pyslth-0.4.0/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.4.0/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.4.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/migrations/0006_user.py` & `pyslth-0.4.0/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/models.py` & `pyslth-0.4.0/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/notifications.py` & `pyslth-0.4.0/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/oauth.py` & `pyslth-0.4.0/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/permissions.py` & `pyslth-0.4.0/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/queryset.py` & `pyslth-0.4.0/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/roles.py` & `pyslth-0.4.0/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/selenium/__init__.py` & `pyslth-0.4.0/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/selenium/browser.py` & `pyslth-0.4.0/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/serializer.py` & `pyslth-0.4.0/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/.DS_Store` & `pyslth-0.4.0/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fontawesome.min.css` & `pyslth-0.4.0/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fonts/.DS_Store` & `pyslth-0.4.0/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.4.0/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.4.0/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.4.0/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.4.0/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/slth.css` & `pyslth-0.4.0/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/css/solid.min.css` & `pyslth-0.4.0/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/images/logo.png` & `pyslth-0.4.0/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/images/logo.svg` & `pyslth-0.4.0/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/images/user.png` & `pyslth-0.4.0/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/default-passive-events.min.js` & `pyslth-0.4.0/slth/static/js/default-passive-events.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/echarts.min.js` & `pyslth-0.4.0/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/index.min.js` & `pyslth-0.4.0/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/ios-splash.min.js` & `pyslth-0.4.0/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/peerjs.min.js` & `pyslth-0.4.0/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/qrcode.min.js` & `pyslth-0.4.0/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/react-trigger-change.js` & `pyslth-0.4.0/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/react.min.js` & `pyslth-0.4.0/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/slth.min.js` & `pyslth-0.4.0/slth/static/js/slth.min.js`

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
-const k = {
+const j = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -92,15 +92,15 @@
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = k.colors.primary, a.color = "white"), e.default && (a.color = k.colors.primary, a.border = "solid 1px " + k.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = j.colors.primary, a.color = "white"), e.default && (a.color = j.colors.primary, a.border = "solid 1px " + j.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
             children: t.jsx(S, {
                 icon: e.icon
@@ -112,15 +112,15 @@
 const Ne = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
 function qe(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
-            backgroundColor: e.isError ? "#e52207" : k.colors.success,
+            backgroundColor: e.isError ? "#e52207" : j.colors.success,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
@@ -150,16 +150,16 @@
         e.remove()
     })
 }
 
 function oe(e) {
     function n() {
         const a = {
-            color: k.colors.info,
-            backgroundColor: k.background.info,
+            color: j.colors.info,
+            backgroundColor: j.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -209,19 +209,19 @@
         if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
         o.text()
     }).then(o => {
         if (u == "application/json") {
             var h = JSON.parse(o || "{}");
             typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var g = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
                     type: u
                 })),
                 w = document.createElement("a");
-            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
+            w.href = g, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
         } else a && a(o, s)
     })
 }
 
 function W(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
@@ -458,15 +458,15 @@
     return t.jsx("dialog", {
         id: n,
         style: i,
         children: a()
     })
 }
 
-function M(e) {
+function E(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function _(e) {
     const n = e.id || Math.random(),
         [a, r] = B.useState(e.data.name);
 
@@ -495,22 +495,22 @@
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             minWidth: 50,
             lineHeight: e.data.icon ? "4rem" : "auto"
         };
-        return e.primary && (c.backgroundColor = k.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + k.colors.primary, c.color = k.colors.primary), e.style && Object.keys(e.style).map(function(s) {
+        return e.primary && (c.backgroundColor = j.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + j.colors.primary, c.color = j.colors.primary), e.style && Object.keys(e.style).map(function(s) {
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
             href: U(e.data.url) || "#",
             onClick: i,
             style: c,
-            "data-label": M(e.data.name),
+            "data-label": E(e.data.name),
             children: l()
         })
     }
     return d()
 }
 
 function Z(e) {
@@ -550,15 +550,15 @@
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": M(e.dataLabel),
+                "data-label": E(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: l,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(c => t.jsx("li", {
                     style: d,
@@ -592,15 +592,15 @@
     }
 
     function o() {
         return t.jsx("a", {
             id: e,
             onClick: l || u,
             href: s || "#",
-            "data-label": M(d),
+            "data-label": E(d),
             style: c,
             children: i
         })
     }
     return o()
 }
 
@@ -1013,23 +1013,23 @@
       .object-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .object-title h1 {
           margin: 0;
-          color: ${k.colors.primary};
+          color: ${j.colors.primary};
       }
     `), t.jsxs("div", {
             className: "object-title",
             style: {
                 flexDirection: window.innerWidth > 800 ? "row" : "column"
             },
             children: [e.data.title && t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     margin: 10
                 },
                 children: t.jsx(Ye, {
                     data: e.data
@@ -1052,15 +1052,15 @@
       }
     `);
 
     function n() {
         return t.jsxs("div", {
             className: "fieldset-title",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(a) {
                     return t.jsx(_, {
                         data: a,
                         default: !0
                     }, Math.random())
@@ -1157,30 +1157,30 @@
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
                         d.preventDefault(), a(l), e.loadContent(i.url)
                     },
-                    dataLabel: M(i.title),
+                    dataLabel: E(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Qe(e) {
     var n = Math.random();
     const [a, r] = B.useState(e.data.data[0]);
 
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": M(e.data.title),
+            "data-label": E(e.data.title),
             children: e.data.title
         })
     }
 
     function l() {
         return t.jsx(Je, {
             data: e.data.data,
@@ -1275,18 +1275,18 @@
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return l ? (o.backgroundColor = k.colors.primary, o.color = "white") : (o.border = "solid 1px " + k.colors.primary, o.color = k.colors.primary), t.jsx("a", {
+        return l ? (o.backgroundColor = j.colors.primary, o.color = "white") : (o.border = "solid 1px " + j.colors.primary, o.color = j.colors.primary), t.jsx("a", {
             id: e,
             style: o,
-            "data-label": M(r || a),
+            "data-label": E(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
     return u()
@@ -1347,18 +1347,18 @@
             },
             children: l.number
         })
     }
 
     function a(l) {
         return {
-            border: "3px solid " + k.colors.primary,
+            border: "3px solid " + j.colors.primary,
             borderRadius: "50%",
-            background: l.done ? k.colors.primary : "white",
-            color: l.done ? "white" : k.colors.primary,
+            background: l.done ? j.colors.primary : "white",
+            color: l.done ? "white" : j.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -1431,15 +1431,15 @@
             i = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: k.colors[e.data.style]
+                backgroundColor: j.colors[e.data.style]
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
-        return e.data.color = k.colors[e.data.style], t.jsx(Se, {
+        return e.data.color = j.colors[e.data.style], t.jsx(Se, {
             data: e.data
         })
     }
     return n()
 }
 
 function Se(e) {
@@ -1505,30 +1505,30 @@
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
             i = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: k.colors.auxiliary
+                color: j.colors.auxiliary
             },
             l = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: k.colors.primary
+                color: j.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 style: {
-                    color: k.colors.primary
+                    color: j.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(d => t.jsxs(O, {
                     href: d.url,
                     style: r,
                     dataLabel: d.label,
@@ -1618,15 +1618,15 @@
     return a()
 }
 
 function ct(e) {
     function n() {
         const a = {
                 color: "white",
-                backgroundColor: k.colors.highlight,
+                backgroundColor: j.colors.highlight,
                 margin: -20,
                 textAlign: "center",
                 paddingTop: 20,
                 paddingBottom: 70
             },
             r = {
                 fontSize: "4rem",
@@ -1638,15 +1638,15 @@
                 maxWidth: 200,
                 margin: "auto"
             };
         if (e.data) return t.jsxs("div", {
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
                 children: e.data.items.map(l => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
                         children: W(l.value)
@@ -1723,84 +1723,84 @@
         a = !1, document.getElementById("input" + n).value = JSON.stringify({
             select: d,
             deselect: c
         })
     }
 
     function h(y) {
-        e.data.readonly || e.data.single_selection && f().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != l && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
+        e.data.readonly || e.data.single_selection && g().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != l && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
     }
 
-    function f() {
+    function g() {
         const y = [];
-        return document.getElementById(n).querySelectorAll("td").forEach(function(D) {
-            D.style.backgroundColor == i && y.push(D.dataset.day, D.dataset.time)
+        return document.getElementById(n).querySelectorAll("td").forEach(function(I) {
+            I.style.backgroundColor == i && y.push(I.dataset.day, I.dataset.time)
         }), y
     }
 
     function w() {
         const y = {
                 overflowX: "auto"
             },
-            D = {
+            I = {
                 width: "100%",
                 borderSpacing: 0,
                 borderCollapse: "collapse",
                 marginTop: 15,
                 marginBottom: 15
             },
-            j = {
+            m = {
                 border: "solid 4px white"
             };
         return t.jsxs("div", {
             id: n,
             style: y,
             children: [t.jsx("input", {
                 id: "input" + n,
                 type: "hidden",
                 name: e.data.input_name
             }), t.jsxs("table", {
-                style: D,
+                style: I,
                 onMouseDown: u,
                 onMouseUp: o,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: e.data.matrix[0].map(function(v) {
+                        children: e.data.matrix[0].map(function(k) {
                             return t.jsx("th", {
                                 className: "bold",
-                                style: j,
-                                children: v.text
+                                style: m,
+                                children: k.text
                             }, Math.random())
                         })
                     })
                 }), t.jsx("tbody", {
-                    children: e.data.matrix.map(function(v, g) {
-                        if (g > 0) return t.jsx("tr", {
-                            children: v.map(function(C, b) {
+                    children: e.data.matrix.map(function(k, v) {
+                        if (v > 0) return t.jsx("tr", {
+                            children: k.map(function(D, b) {
                                 if (b == 0) return t.jsx("th", {
                                     className: "bold",
                                     align: "center",
-                                    style: j,
-                                    children: C.text
+                                    style: m,
+                                    children: D.text
                                 }, Math.random());
                                 {
-                                    const E = {
-                                        backgroundColor: s(C),
+                                    const C = {
+                                        backgroundColor: s(D),
                                         border: "solid 4px white"
                                     };
                                     return t.jsx("td", {
                                         align: "center",
-                                        style: E,
+                                        style: C,
                                         onMouseDown: h,
                                         onMouseLeave: h,
                                         onMouseUp: h,
                                         "data-day": e.data.matrix[0][b].text,
-                                        "data-time": v[0].text,
-                                        children: C && C.text && t.jsx(mt, {
-                                            text: C.text,
+                                        "data-time": k[0].text,
+                                        children: D && D.text && t.jsx(mt, {
+                                            text: D.text,
                                             children: t.jsx(S, {
                                                 icon: "stethoscope",
                                                 style: {
                                                     color: "white",
                                                     cursor: "help"
                                                 }
                                             })
@@ -1823,15 +1823,15 @@
       .tooltip {
         position: relative;
         display: inline-block;
       }
       .tooltip .tooltiptext {
         visibility: hidden;
         width: 220px;
-        background-color: ${k.colors.highlight};
+        background-color: ${j.colors.highlight};
         color: #fff;
         text-align: center;
         border-radius: 6px;
         padding: 5px 0;
         position: absolute;
         z-index: 1;
         bottom: 150%;
@@ -1936,29 +1936,29 @@
         for (var a in e.set) bt(a, e.set[a])
     }
 }
 
 function wt(e) {
     function n() {
         const a = {
-            color: k.colors.info,
-            backgroundColor: k.background.info,
+            color: j.colors.info,
+            backgroundColor: j.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
                 children: [t.jsx(S, {
                     icon: "circle-check",
                     style: {
-                        color: k.colors.info,
+                        color: j.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
@@ -2092,18 +2092,18 @@
 }
 
 function ye(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), B.useEffect(() => {
         function d(u, o, h) {
-            var f = h.target,
-                w = f.value.replace(/\D/g, ""),
-                y = f.value.length > o ? 1 : 0;
-            VMasker(f).unMask(), VMasker(f).maskPattern(u[y]), f.value = VMasker.toPattern(w, u[y])
+            var g = h.target,
+                w = g.value.replace(/\D/g, ""),
+                y = g.value.length > o ? 1 : 0;
+            VMasker(g).unMask(), VMasker(g).maskPattern(u[y]), g.value = VMasker.toPattern(w, u[y])
         }
         if (e.data.mask) {
             var c = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
@@ -2124,31 +2124,31 @@
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (re(s.name)) {
                     const w = "display" + a;
                     var o = document.createElement("img");
                     o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(y) {
-                        const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
-                        var j = document.createElement("canvas");
-                        const v = j.getContext("2d");
-                        j.height = j.width * (o.height / o.width);
-                        const g = document.createElement("canvas"),
-                            C = g.getContext("2d");
-                        g.width = o.width * D, g.height = o.height * D, C.drawImage(o, 0, 0, g.width, g.height), v.drawImage(g, 0, 0, g.width * D, g.height * D, 0, 0, j.width, j.height), g.toBlob(function(E) {
+                        const I = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                        var m = document.createElement("canvas");
+                        const k = m.getContext("2d");
+                        m.height = m.width * (o.height / o.width);
+                        const v = document.createElement("canvas"),
+                            D = v.getContext("2d");
+                        v.width = o.width * I, v.height = o.height * I, D.drawImage(o, 0, 0, v.width, v.height), k.drawImage(v, 0, 0, v.width * I, v.height * I, 0, 0, m.width, m.height), v.toBlob(function(C) {
                             const T = new DataTransfer;
-                            T.items.add(new File([E], s.name)), d.target.files = T.files
+                            T.items.add(new File([C], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
                         b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
                     }, o.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
-                var f = s.size / 1024;
-                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + f, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
+                var g = s.size / 1024;
+                g < 1024 ? g = parseInt(g) + " Kb" : g = (g / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + g, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + g + ". Por favor, adicione um arquivo menor.")
             }, c.readAsDataURL(s)
         }
     }
 
     function l() {
         var d = e.data.type;
         if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
@@ -2172,15 +2172,15 @@
                     },
                     children: [t.jsx("div", {
                         style: u,
                         children: t.jsx(S, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: k.colors.primary
+                                color: j.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
                         children: [e.data.value && re(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
@@ -2208,15 +2208,15 @@
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: d,
                     name: e.data.name,
                     id: a,
-                    "data-label": M(e.data.label),
+                    "data-label": E(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: i,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
@@ -2229,28 +2229,28 @@
                 ...V
             }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: i,
                 style: s
             })
         }
     }
     return l()
 }
 
 function Me(e) {
     var n = [];
-    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, E) {
+    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, C) {
         n.push({
             id: b.id,
             value: b.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
@@ -2259,60 +2259,60 @@
         r = e.data.id2,
         i = Array.isArray(e.data.value),
         [l, d] = B.useState(!1),
         [c, s] = B.useState(null);
     var u = !1;
     let o;
     B.useEffect(() => {
-        v(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
-            v(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+        k(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
+            k(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
         const b = document.getElementById(a);
         if (i) {
-            const E = {
+            const C = {
                     padding: 5,
                     display: "inline"
                 },
                 T = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                m = {
+                f = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((p, I) => t.jsxs("div", {
-                    style: E,
+                children: [b == null && n.map((p, M) => t.jsxs("div", {
+                    style: C,
                     children: [t.jsx("span", {
-                        onClick: () => g(I),
+                        onClick: () => v(M),
                         style: T,
                         children: t.jsx(S, {
                             icon: "trash-can",
-                            style: m
+                            style: f
                         })
                     }), p.value]
-                }, Math.random())), b != null && Array.from(b.options).map((p, I) => t.jsxs("div", {
-                    style: E,
+                }, Math.random())), b != null && Array.from(b.options).map((p, M) => t.jsxs("div", {
+                    style: C,
                     children: [t.jsx("span", {
-                        onClick: () => g(I),
+                        onClick: () => v(M),
                         style: T,
                         children: t.jsx(S, {
                             icon: "trash-can",
-                            style: m
+                            style: f
                         })
                     }), p.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
-    function f() {
+    function g() {
         return t.jsx("select", {
             id: a,
             name: e.data.name,
             multiple: i,
             readOnly: !0,
             style: {
                 display: "contents"
@@ -2321,42 +2321,42 @@
     }
 
     function w() {
         const b = {
                 ...V,
                 ...e.style || {}
             },
-            E = {
+            C = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto",
                 zIndex: 99999
             };
-        E.position = "absolute", E.backgroundColor = "white";
+        C.position = "absolute", C.backgroundColor = "white";
         const T = document.getElementById(r);
         if (e.data.icon && (b.paddingLeft = 30), T) {
             let N = null,
                 Q = T,
                 ae = null;
             for (; !ae && (Q = Q.parentElement) instanceof HTMLElement;) Q.matches("dialog") && (ae = Q);
             N = ae;
             const K = T.getBoundingClientRect();
-            var m = K.top + K.height,
+            var f = K.top + K.height,
                 p = K.left;
             if (N) {
                 const fe = N.getBoundingClientRect();
-                m = m - fe.top, p = p - fe.left
-            } else m += window.scrollY, p += window.scrollX;
-            E.width = K.width, E.top = m, E.left = p
+                f = f - fe.top, p = p - fe.left
+            } else f += window.scrollY, p += window.scrollX;
+            C.width = K.width, C.top = f, C.left = p
         }
-        const I = {
+        const M = {
                 cursor: "pointer",
                 padding: 10
             },
             L = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
@@ -2367,97 +2367,97 @@
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
                 onFocus: N => {
-                    N.target.select(), j(N)
+                    N.target.select(), m(N)
                 },
-                onChange: j,
+                onChange: m,
                 onMouseLeave: y,
                 onBlur: y,
                 defaultValue: L,
                 style: b,
-                "data-label": M(e.data.label)
+                "data-label": E(e.data.label)
             }), c && l && t.jsxs("ul", {
-                style: E,
-                onMouseLeave: D,
+                style: C,
+                onMouseLeave: I,
                 onMouseEnter: function(N) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
-                    style: I,
+                    style: M,
                     children: "Nenhuma opção encontrada."
                 }), c.map(N => t.jsx("li", {
                     onClick: () => {
-                        d(!1), e.onSelect ? e.onSelect(N) : v(N)
+                        d(!1), e.onSelect ? e.onSelect(N) : k(N)
                     },
-                    style: I,
+                    style: M,
                     className: "autocomplete-item",
-                    "data-label": M(N.value),
+                    "data-label": E(N.value),
                     children: N.value
                 }, Math.random()))]
             })]
         })
     }
 
     function y(b) {
         u = !1, setTimeout(function() {
-            u || D(b)
+            u || I(b)
         }, 250)
     }
 
-    function D(b) {
-        const E = document.getElementById(a);
-        if (E) {
+    function I(b) {
+        const C = document.getElementById(a);
+        if (C) {
             const T = document.getElementById(r);
-            i || E.options.length > 0 && T.value != E.options[0].innerHTML && (E.innerHTML = "", T.value = "", d(!1), e.data.onchange && $(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
+            i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && $(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
-    function j(b) {
+    function m(b) {
         clearTimeout(o), o = setTimeout(function() {
-            const E = b.target.closest("form"),
+            const C = b.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), q("GET", J(e.data.choices + T + "term=" + b.target.value, E), function(p) {
+            d(!0), q("GET", J(e.data.choices + T + "term=" + b.target.value, C), function(p) {
                 s(p)
             })
         }, 1e3)
     }
 
-    function v(b, E = !1) {
+    function k(b, C = !1) {
         const T = document.getElementById(a),
-            m = document.getElementById(r);
-        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !E && $(m, e.data.onchange)
+            f = document.getElementById(r);
+        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, f.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, f.value = b.value), e.data.onchange && !C && $(f, e.data.onchange)
     }
 
-    function g(b) {
-        const E = document.getElementById(a);
-        var T = Array.from(E.options);
-        E.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(m => `<option selected value="${m.value}">${m.innerHTML}</option>`).join(""), s([])
+    function v(b) {
+        const C = document.getElementById(a);
+        var T = Array.from(C.options);
+        C.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), s([])
     }
 
-    function C() {
+    function D() {
         return t.jsxs(t.Fragment, {
-            children: [h(), f(), w()]
+            children: [h(), g(), w()]
         })
     }
-    return C()
+    return D()
 }
 
 function kt(e) {
     function n() {
         var a = {
             ...V
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": M(e.data.label),
+            "data-label": E(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
@@ -2510,15 +2510,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + o,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
                     defaultChecked: l(u),
-                    "data-label": M(u.value),
+                    "data-label": E(u.value),
                     onClick: function() {
                         d(i.name + r + o)
                     },
                     onMouseEnter: function() {
                         c(i.name + r + o)
                     }
                 }), t.jsx("label", {
@@ -2572,15 +2572,15 @@
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
                     defaultChecked: l(s),
-                    "data-label": M(s.value)
+                    "data-label": E(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
             className: "checkbox-group " + i.name,
@@ -2595,15 +2595,15 @@
 function Ct(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": M(n.label),
+            "data-label": E(n.label),
             defaultValue: n.value,
             style: V,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
@@ -2639,16 +2639,16 @@
         })
     }
 
     function l(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
             o = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
-            f = document.getElementById("hide-" + n);
-        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+            g = document.getElementById("hide-" + n);
+        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", g.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function d() {
         const s = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
@@ -2667,82 +2667,82 @@
         const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: s,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), i(), d()]
         })
     }
     return c()
 }
 
 function Mt(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
     function r(o, h) {
-        const f = n;
+        const g = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
-            id: "form-" + f + "-" + a,
+            id: "form-" + g + "-" + a,
             children: [t.jsx(ue, {
                 data: o
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => l(),
-                    id: "extra-add-" + f + "-",
+                    id: "extra-add-" + g + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => d(f),
+                    onClick: () => d(g),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function i() {
         const o = c(),
             h = o.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
-        for (var f = 0; f < n; f++) {
-            var w = document.getElementById("extra-add-" + f + "-");
+        for (var g = 0; g < n; g++) {
+            var w = document.getElementById("extra-add-" + g + "-");
             w.style.display = "none"
         }
         if (o.length > 0) {
             var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
     function l() {
         i();
         var o = JSON.parse(JSON.stringify(e.data.template));
         o.fields ? (o.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
         }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
-            h.fields.map(function(f) {
-                f.map(function(w) {
+            h.fields.map(function(g) {
+                g.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
-                }), f[0].value = 0
+                }), g[0].value = 0
             })
         }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
     }
 
     function d(o) {
         const h = e.data.template,
             w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
@@ -2777,23 +2777,23 @@
         const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: o,
-                "data-label": M(e.data.label),
+                "data-label": E(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [s(), e.data.value.map(function(h, f) {
-                    return r(h, f == e.data.value.length - 1 ? "inline" : "none")
+                children: [s(), e.data.value.map(function(h, g) {
+                    return r(h, g == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
@@ -2816,15 +2816,15 @@
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": M(r.title),
+                    "data-label": E(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
                     children: i.map(l => t.jsx("div", {
                         className: "form-group " + l.name,
@@ -2843,15 +2843,15 @@
 
 function Tt(e) {
     const n = Math.random();
 
     function a() {
         const h = {
             margin: 0,
-            color: k.colors.primary
+            color: j.colors.primary
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
@@ -2935,38 +2935,38 @@
 
     function u() {
         Y()
     }
 
     function o(h) {
         h.preventDefault();
-        var f = e.data.url,
+        var g = e.data.url,
             w = document.getElementById(n),
             y = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
-            const D = f.indexOf("?") >= 0 ? "&" : "?";
-            f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
+            const I = g.indexOf("?") >= 0 ? "&" : "?";
+            g = g + I + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
         }
-        q(w.method.toUpperCase(), f, function(j) {
-            if (w.querySelectorAll(".error").forEach(g => g.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), j.type == "response") j.store && Object.keys(j.store).map(function(g) {
-                j.store[g] ? localStorage.setItem(g, j.store[g]) : localStorage.removeItem(g, j.store[g])
-            }), j.redirect && j.redirect.length > 2 ? (j.message && localStorage.setItem("message", j.message), document.location.href = U(j.redirect)) : (j.message && z(j.message), j.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : Y()), j.redirect == "." && w.reset(), j.dispose && (w.style.display = "none"), Ke());
-            else if (j.type == "error") {
-                var v = j.text;
-                console.log(j), Object.keys(j.errors).map(function(g) {
-                    if (g == "__all__") v = j.errors[g];
+        q(w.method.toUpperCase(), g, function(m) {
+            if (w.querySelectorAll(".error").forEach(v => v.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), m.type == "response") m.store && Object.keys(m.store).map(function(v) {
+                m.store[v] ? localStorage.setItem(v, m.store[v]) : localStorage.removeItem(v, m.store[v])
+            }), m.redirect && m.redirect.length > 2 ? (m.message && localStorage.setItem("message", m.message), document.location.href = U(m.redirect)) : (m.message && z(m.message), m.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : Y()), m.redirect == "." && w.reset(), m.dispose && (w.style.display = "none"), Ke());
+            else if (m.type == "error") {
+                var k = m.text;
+                console.log(m), Object.keys(m.errors).map(function(v) {
+                    if (v == "__all__") k = m.errors[v];
                     else {
-                        const C = w.querySelector("#" + g + "_error");
-                        C.querySelector("span").innerHTML = j.errors[g], C.style.display = "block"
+                        const D = w.querySelector("#" + v + "_error");
+                        D.querySelector("span").innerHTML = m.errors[v], D.style.display = "block"
                     }
-                }), z(v, !0)
+                }), z(k, !0)
             } else {
-                const g = document.querySelector("#output");
-                g.innerHTML = "", H.createRoot(g.appendChild(document.createElement("div"))).render(t.jsx(x, {
-                    data: j
+                const v = document.querySelector("#output");
+                v.innerHTML = "", H.createRoot(v.appendChild(document.createElement("div"))).render(t.jsx(x, {
+                    data: m
                 }))
             }
         }, y)
     }
     return s()
 }
 
@@ -3091,15 +3091,15 @@
                                 }) : h.date + h.today
                             }), h.total && t.jsx("div", {
                                 className: "total",
                                 onClick: () => e.onChange(h.date, e.data.month, e.data.year),
                                 children: t.jsx("div", {
                                     className: "number",
                                     style: {
-                                        backgroundColor: k.colors.primary
+                                        backgroundColor: j.colors.primary
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
-            backgroundColor: k.colors.primary,
+            backgroundColor: j.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -3253,363 +3253,363 @@
         text-decoration: none;
     }
   `), e.data.id == null && (e.data.id = Math.random());
     const [n, a] = B.useState(e.data);
 
     function r() {
         return n.attrname ? t.jsx("h2", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: n.title
         }) : t.jsxs("h1", {
-            "data-label": M(n.title),
+            "data-label": E(n.title),
             children: [n.title, " ", n.total > 10 && "(" + n.total + ")"]
         })
     }
 
     function i() {
         return t.jsxs("div", {
             className: "title",
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function l(m) {
-        document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
+    function l(f) {
+        document.getElementById("loader-" + e.data.id).style.display = f ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
-            children: n.subsets.map(function(m, p) {
-                var I = n.subset === m.name || !n.subset && p == 0;
+            children: n.subsets.map(function(f, p) {
+                var M = n.subset === f.name || !n.subset && p == 0;
                 return t.jsxs(O, {
                     href: "#",
                     style: {
-                        borderBottom: I ? "solid 3px #2670e8" : 0,
+                        borderBottom: M ? "solid 3px #2670e8" : 0,
                         color: "#0c326f"
                     },
                     onClick: function(L) {
-                        L.preventDefault(), c(m.name)
+                        L.preventDefault(), c(f.name)
                     },
-                    dataLabel: M(m.label),
-                    children: [m.label, " ", t.jsx(Bt, {
-                        total: m.count
+                    dataLabel: E(f.label),
+                    children: [f.label, " ", t.jsx(Bt, {
+                        total: f.count
                     })]
                 }, Math.random())
             })
         })
     }
 
-    function c(m) {
+    function c(f) {
         const p = document.getElementById("subset-" + e.data.id);
-        p.value = m || "", C()
+        p.value = f || "", D()
     }
 
-    function s(m, p, I) {
+    function s(f, p, M) {
         const L = document.getElementById("form-" + e.data.id);
-        L.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = I || "", y(1)
+        L.querySelector("input[name=" + n.calendar.field + "__day]").value = f || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = M || "", y(1)
     }
 
     function u() {
         if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
-    function o(m) {
+    function o(f) {
         const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
-            color: k.colors.primary,
+            color: j.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [m.map(function(I) {
-                return I.label != "ID" && t.jsx("th", {
+            children: [f.map(function(M) {
+                return M.label != "ID" && t.jsx("th", {
                     style: p,
                     className: "bold",
-                    children: I.label
+                    children: M.label
                 }, Math.random())
             }), t.jsx("th", {
                 style: p
             })]
         })
     }
 
-    function h(m) {
+    function h(f) {
         const p = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
-            I = {
+            M = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
                 style: p,
-                children: m.title
+                children: f.title
             }, Math.random()), t.jsx("td", {
-                style: I,
+                style: M,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
                     children: t.jsx(S, {
                         icon: "chevron-right",
-                        onClick: () => Re(m.actions),
+                        onClick: () => Re(f.actions),
                         style: {
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [m.data.map(function(L) {
+            children: [f.data.map(function(L) {
                 return L.label != "ID" && t.jsx("td", {
                     style: p,
                     children: W(L.value)
                 }, Math.random())
             }), t.jsx("td", {
-                style: I,
+                style: M,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: m.actions.map(function(L) {
+                    children: f.actions.map(function(L) {
                         return t.jsx(_, {
                             data: L,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
     }
 
-    function f() {
+    function g() {
         return n.data.length > 0 ? (n.render == null && window.innerWidth < 800 && (n.renderer = "rows"), n.renderer ? n.renderer == "cards" ? t.jsx(P, {
             width: 300,
             alignItems: "start",
-            children: n.data.map(function(m) {
-                return m.type = n.renderer, t.jsx("div", {
+            children: n.data.map(function(f) {
+                return f.type = n.renderer, t.jsx("div", {
                     children: t.jsx(x, {
-                        data: m
+                        data: f
                     })
                 }, Math.random())
             })
         }) : t.jsx("div", {
             style: {
                 marginBottom: 15
             },
-            children: n.data.map(function(m) {
-                return m.type = n.renderer, t.jsx(x, {
-                    data: m
+            children: n.data.map(function(f) {
+                return f.type = n.renderer, t.jsx(x, {
+                    data: f
                 }, Math.random())
             })
         }) : w()) : t.jsx(oe, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
-        const m = {
+        const f = {
                 width: "100%",
                 overflowX: "auto"
             },
             p = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
-            style: m,
+            style: f,
             children: t.jsxs("table", {
                 style: p,
                 children: [t.jsx("thead", {
                     children: o(n.data[0].data)
                 }), t.jsx("tbody", {
-                    children: n.data.map(function(I) {
-                        return h(I)
+                    children: n.data.map(function(M) {
+                        return h(M)
                     })
                 })]
             })
         })
     }
 
-    function y(m) {
-        const I = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        I && (I.value = m), C(), v()
+    function y(f) {
+        const M = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
+        M && (M.value = f), D(), k()
     }
 
-    function D() {
-        const m = document.getElementById("form-" + e.data.id);
-        if (m) {
-            const p = m.querySelector("input[name=page]");
+    function I() {
+        const f = document.getElementById("form-" + e.data.id);
+        if (f) {
+            const p = f.querySelector("input[name=page]");
             p && (p.value = n.pagination.page.current)
         }
         return t.jsx(Dt, {
             data: n.pagination,
             onChange: y,
             total: n.total
         })
     }
 
-    function j() {
+    function m() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
-            children: n.actions.map(function(m) {
+            children: n.actions.map(function(f) {
                 return t.jsx(_, {
-                    data: m,
+                    data: f,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function v() {
-        const m = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
-        console.log(m), console.log(e.data.id), window.scrollTo({
-            top: m,
+    function k() {
+        const f = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
+        console.log(f), console.log(e.data.id), window.scrollTo({
+            top: f,
             behavior: "smooth"
         })
     }
 
-    function g() {
-        const m = {
+    function v() {
+        const f = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             p = n.search.length > 0,
-            I = n.filters.length > 0;
-        if ((n.bi || n.data.length >= 0) && (p || I)) {
+            M = n.filters.length > 0;
+        if ((n.bi || n.data.length >= 0) && (p || M)) {
             const L = {
                 name: "q",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves",
                 value: n.q
             };
             return t.jsxs("div", {
-                style: m,
+                style: f,
                 children: [t.jsxs(P, {
                     width: 250,
                     children: [p && t.jsx("div", {
                         children: t.jsx(ee, {
                             data: L
                         })
-                    }), I && n.filters.map(function(N) {
+                    }), M && n.filters.map(function(N) {
                         return N.type != "hidden" && t.jsx("div", {
                             children: t.jsx(ee, {
                                 data: N
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: C,
+                            onClick: D,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
-                }), I && n.filters.map(function(N) {
+                }), M && n.filters.map(function(N) {
                     return N.type == "hidden" && t.jsx("div", {
                         children: t.jsx(ee, {
                             data: N
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function C() {
+    function D() {
         l(!0);
-        var m;
+        var f;
         const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + p : m = e.data.url + "?" + p, q("GET", m, function(I) {
-            a(I), l(!1)
+        e.data.url.indexOf("?") > 0 ? f = e.data.url + "&" + p : f = e.data.url + "?" + p, q("GET", f, function(M) {
+            a(M), l(!1)
         })
     }
 
     function b() {
-        const m = {
-            color: k.colors.primary
+        const f = {
+            color: j.colors.primary
         };
         return e.data.reloadable && t.jsxs("div", {
             align: "center",
             children: [t.jsxs("i", {
                 children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
             }), t.jsx("div", {
                 children: t.jsx(O, {
-                    style: m,
+                    style: f,
                     onClick: p => {
-                        p.preventDefault(), C()
+                        p.preventDefault(), D()
                     },
                     children: "Atualizar agora"
                 })
             })]
         })
     }
 
-    function E() {
+    function C() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [g(), n.bi.map(function(m) {
+            children: [v(), n.bi.map(function(f) {
                 return t.jsx(P, {
                     width: 300,
                     alignItems: "start",
-                    children: m.map(function(p) {
+                    children: f.map(function(p) {
                         return t.jsx("div", {
                             children: t.jsx(x, {
                                 data: p
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs("div", {
             className: "content",
-            children: [b(), j(), d(), g(), u(), f(), D()]
+            children: [b(), m(), d(), v(), u(), g(), I()]
         })
     }
 
     function T() {
-        window[e.data.id] = () => C();
-        const m = {
+        window[e.data.id] = () => D();
+        const f = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable queryset",
             id: e.data.id,
-            sytle: m,
+            sytle: f,
             children: t.jsxs("form", {
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), i(), E()]
+                }), i(), C()]
             })
         })
     }
     return T()
 }
 
 function ne(e) {
@@ -4053,15 +4053,15 @@
         return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
@@ -4097,51 +4097,51 @@
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: i
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": M(e.data.title),
+                "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: r.map(f => t.jsx("th", {
+                        children: r.map(g => t.jsx("th", {
                             className: "bold",
                             style: {
                                 textAlign: "left",
                                 padding: 5
                             },
-                            children: f
+                            children: g
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [i.map((f, w) => t.jsx("tr", {
-                        children: f.map((y, D) => D == 0 ? t.jsx("th", {
+                    children: [i.map((g, w) => t.jsx("tr", {
+                        children: g.map((y, I) => I == 0 ? t.jsx("th", {
                             className: w % 2 == 0 ? "even" : "odd",
                             style: {
                                 textAlign: "left",
                                 padding: 5
                             },
                             children: y
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
-                            className: (D == f.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (w % 2 == 0 ? "even" : "odd"),
+                            className: (I == g.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (w % 2 == 0 ? "even" : "odd"),
                             children: W(y)
                         }, Math.random()))
                     }, Math.random())), d.length > 0 && t.jsxs("tr", {
-                        children: [t.jsx("th", {}), d.map(f => t.jsxs("td", {
+                        children: [t.jsx("th", {}), d.map(g => t.jsxs("td", {
                             align: "center",
                             className: "bold",
-                            children: [W(f), " "]
+                            children: [W(g), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
@@ -4150,15 +4150,15 @@
 function Ut() {
     function e() {
         const l = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: k.colors.success
+            backgroundColor: j.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: l
@@ -4199,39 +4199,39 @@
                 display: d == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 15,
                 paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: k.colors.primary
+                color: j.colors.primary
             },
             s = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return l.url ? t.jsx("li", {
             style: c,
             onClick: n,
             className: "item",
             children: t.jsxs(O, {
                 href: l.url,
-                dataLabel: M(l.label),
+                dataLabel: E(l.label),
                 style: {
                     textDecoration: "none"
                 },
                 children: [d == 0 && t.jsx(S, {
                     icon: l.icon || "dot-circle",
                     style: s
                 }), l.label]
             })
         }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": M(l.label),
+            "data-label": E(l.label),
             children: [d == 0 && t.jsx(S, {
                 icon: l.icon || "dot-circle",
                 style: s
             }), l.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
@@ -4317,15 +4317,15 @@
 
     function i() {
         return t.jsx(S, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: k.colors.primary
+                color: j.colors.primary
             }
         })
     }
     return i()
 }
 
 function Yt(e, n) {
@@ -4355,15 +4355,15 @@
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: k.colors.primary,
+                backgroundColor: j.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -4422,16 +4422,16 @@
 
 function $t(e) {
     B.useEffect(() => {
         const o = localStorage.getItem("message");
         o && (localStorage.removeItem("message"), z(o)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
-        }), Yt(document.querySelector("main"), function(h, f) {
-            console.log(h, f)
+        }), Yt(document.querySelector("main"), function(h, g) {
+            console.log(h, g)
         })
     }, []);
 
     function a() {
         const o = document.querySelector("aside");
         o.style.display = o.style.display == "none" ? "block" : "none"
     }
@@ -4513,35 +4513,35 @@
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Gt, {})
                 }), e.data.navbar.toolbar && window.innerWidth > 800 && e.data.navbar.toolbar.length > 0 && t.jsx("div", {
                     className: "toolbar",
-                    children: e.data.navbar.toolbar.map(function(f) {
+                    children: e.data.navbar.toolbar.map(function(g) {
                         return t.jsx(_, {
-                            data: f,
+                            data: g,
                             primary: !0,
                             compact: !0
                         }, Math.random())
                     })
-                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
-                    return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
+                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(g) {
+                    return g.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(_, {
-                            data: f,
+                            data: g,
                             primary: !0
                         }, Math.random())
                     }, Math.random())
-                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
+                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(g) {
                     return t.jsx(O, {
-                        href: f.url,
+                        href: g.url,
                         style: {
                             marginRight: 10
                         },
-                        children: f.label
+                        children: g.label
                     }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.tools,
@@ -4565,32 +4565,32 @@
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
                     children: t.jsx(Me, {
                         data: h,
                         style: {
                             padding: 10
                         },
-                        onSelect: f => document.location.href = U(f.id)
+                        onSelect: g => document.location.href = U(g.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: M(e.data.navbar.user),
+                        dataLabel: E(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: k.colors.primary
+                                backgroundColor: j.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
@@ -4610,15 +4610,15 @@
     function d() {
         const o = {
                 margin: 15,
                 display: "flex",
                 justifyContent: "space-between"
             },
             h = {
-                color: k.colors.primary
+                color: j.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
             style: o,
             children: [t.jsxs("div", {
                 children: [t.jsx(O, {
                     href: "/app/dashboard/",
                     style: {
@@ -4701,166 +4701,184 @@
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: v => v.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: m => m.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
-    const s = {
-        video: {
-            width: {
-                exact: 320
-            },
-            height: {
-                exact: 240
-            },
-            frameRate: {
-                ideal: 5,
-                max: 10
-            }
-        },
-        audio: !0
-    };
 
-    function u() {
-        console.log("Trying to connect..."), n = new Peer("999123" + e.data.caller.replaceAll(".", "").replaceAll("-", "")), n.on("open", function(v) {
-            document.getElementById("callerid").innerHTML = e.data.caller, D(), l = setInterval(function() {
-                i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), D())
+    function s() {
+        console.log("Trying to connect..."), n = new Peer("999123" + e.data.caller.replaceAll(".", "").replaceAll("-", "")), n.on("open", function(m) {
+            document.getElementById("callerid").innerHTML = e.data.caller, y(), l = setInterval(function() {
+                i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), y())
             }, 15e3)
-        }), n.on("call", function(v) {
-            d(s, function(g) {
-                a = g;
-                var C = document.getElementById("video2");
-                C.addEventListener("loadedmetadata", function(b) {
-                    C.style.width = this.videoWidth / 4 + "px", C.style.height = this.videoHeight / 4 + "px", C.style.marginLeft = -this.videoWidth / 4 + "px", C.style.visibility = "visible"
-                }, !1), C.srcObject = a, v.answer(g), v.on("stream", function(b) {
-                    r = b, document.getElementById("video1").srcObject = r, i = !0
-                }), v.on("close", function() {
+        }), n.on("call", function(m) {
+            d({
+                video: {
+                    width: {
+                        exact: 320
+                    },
+                    height: {
+                        exact: 240
+                    }
+                },
+                audio: !0
+            }, function(k) {
+                a = k;
+                var v = document.getElementById("video2");
+                v.addEventListener("loadedmetadata", function(D) {
+                    v.style.width = this.videoWidth / 4 + "px", v.style.height = this.videoHeight / 4 + "px", v.style.marginLeft = -this.videoWidth / 4 + "px", v.style.visibility = "visible"
+                }, !1), v.srcObject = a, m.answer(k), m.on("stream", function(D) {
+                    r = D, document.getElementById("video1").srcObject = r, i = !0
+                }), m.on("close", function() {
                     console.log("Closed!"), i = !1
                 })
-            }, function(g) {
-                console.log("Failed to get local stream", g)
+            }, function(k) {
+                console.log("Failed to get local stream", k)
             })
-        }), n.on("error", function(v) {
-            v.type == "browser-incompatible" ? alert("Navegador incompatível.") : v.type == "invalid-id" ? alert("Usuário inexistente.") : v.type == "network" ? (i = !1, console.log("Problema na conexão do usuário. Tentando novamente em 5 segundos."), setTimeout(u, 5e3)) : v.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
+        }), n.on("error", function(m) {
+            m.type == "browser-incompatible" ? alert("Navegador incompatível.") : m.type == "invalid-id" ? alert("Usuário inexistente.") : m.type == "network" ? (i = !1, console.log("Problema na conexão do usuário. Tentando novamente em 5 segundos."), setTimeout(s, 5e3)) : m.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
         })
     }
-    B.useEffect(() => (u(), function() {
-        clearInterval(l), o(), z("Desconectado!")
+    B.useEffect(() => (s(), function() {
+        clearInterval(l), u(), z("Desconectado!")
     }), []);
 
-    function o() {
-        h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video"), a = null, r = null;
-        const v = document.getElementById("video1"),
-            g = document.getElementById("video2");
-        v && (v.srcObject = null), g && (g.srcObject = null), console.log("Stopped!"), i = !1
+    function u() {
+        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video"), a = null, r = null;
+        const m = document.getElementById("video1"),
+            k = document.getElementById("video2");
+        m && (m.srcObject = null), k && (k.srcObject = null), console.log("Stopped!"), i = !1
     }
 
-    function h(v, g) {
-        v != null && v.getTracks().forEach(C => {
-            C.kind === g && C.stop()
+    function o(m, k) {
+        m != null && m.getTracks().forEach(v => {
+            v.kind === k && v.stop()
         })
     }
 
-    function f() {
-        var v = document.getElementById("video1");
-        v.style.width = v.getClientRects()[0].width + 100 + "px"
+    function h() {
+        var m = document.getElementById("video1");
+        m.style.width = m.getClientRects()[0].width + 100 + "px"
     }
 
-    function w() {
-        var v = document.getElementById("video1");
-        v.style.width = v.getClientRects()[0].width - 100 + "px"
+    function g() {
+        var m = document.getElementById("video1");
+        m.style.width = m.getClientRects()[0].width - 100 + "px"
     }
 
-    function y() {
-        var v = n.call("999123" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
-        v && (v.on("stream", function(g) {
-            r = g, document.getElementById("video1").srcObject = r, i = !0
-        }), v.on("close", function() {
+    function w() {
+        var m = n.call("999123" + e.data.receiver.replaceAll(".", "").replaceAll("-", ""), a, c);
+        m && (m.on("stream", function(k) {
+            r = k, document.getElementById("video1").srcObject = r, i = !0
+        }), m.on("close", function() {
             console.log("Closed!"), i = !1
         }))
     }
 
-    function D() {
-        if (a != null && !i) return y();
-        a == null && d(s, function(v) {
-            a = v;
-            var g = document.getElementById("video2");
-            g.addEventListener("loadedmetadata", function(C) {
-                g.style.width = this.videoWidth / 4 + "px", g.style.height = this.videoHeight / 4 + "px", g.style.marginLeft = -this.videoWidth / 4 + "px", g.style.visibility = "visible"
-            }, !1), g.srcObject = a, y()
-        }, function(v) {
+    function y() {
+        if (a != null && !i) return w();
+        a == null && d({
+            video: {
+                width: {
+                    exact: 320
+                },
+                height: {
+                    exact: 240
+                },
+                frameRate: {
+                    ideal: 5,
+                    max: 10
+                }
+            },
+            audio: {
+                autoGainControl: !1,
+                channelCount: 2,
+                echoCancellation: !1,
+                latency: 0,
+                noiseSuppression: !1,
+                sampleRate: 48e3,
+                sampleSize: 16,
+                volume: 1
+            }
+        }, function(m) {
+            a = m;
+            var k = document.getElementById("video2");
+            k.addEventListener("loadedmetadata", function(v) {
+                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
+            }, !1), k.srcObject = a, w()
+        }, function(m) {
             alert("Failed to get local stream.")
         })
     }
 
-    function j() {
-        var v = {
+    function I() {
+        var m = {
                 width: "fit-content",
                 margin: "auto"
             },
-            g = {
+            k = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            C = {
+            v = {
                 color: "white",
-                backgroundColor: "black",
                 paddingLeft: 15,
                 paddingRight: 15
             },
-            b = {
+            D = {
                 position: "absolute",
-                marginTop: "-30px"
+                marginTop: "-26px",
+                backgroundColor: "black"
             },
-            E = {
+            b = {
                 backgroundColor: "black"
             },
-            T = {
+            C = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: v,
+            style: m,
             children: [t.jsx("div", {
                 id: "callerid",
-                style: g
+                style: k
             }), t.jsx("video", {
                 id: "video1",
-                style: E,
+                style: b,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
-                style: T,
+                style: C,
                 playsInline: !0,
                 autoPlay: !0,
                 muted: "muted"
             }), t.jsxs("div", {
-                style: b,
+                style: D,
                 children: [t.jsx(S, {
-                    style: C,
-                    onClick: f,
+                    style: v,
+                    onClick: h,
                     icon: "search-plus"
                 }), t.jsx(S, {
-                    style: C,
-                    onClick: w,
+                    style: v,
+                    onClick: g,
                     icon: "search-minus"
                 }), t.jsx(S, {
-                    style: C,
+                    style: v,
                     onClick: () => document.location.reload(),
                     icon: "undo"
                 })]
             })]
         })
     }
-    return j()
+    return I()
 }
 
 function Qt(e) {
     const n = {
         color: e.data.color
     };
```

### Comparing `pyslth-0.3.9/slth/static/js/vanilla-masker.js` & `pyslth-0.4.0/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/static/js/vanilla-masker.min.js` & `pyslth-0.4.0/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/statistics.py` & `pyslth-0.4.0/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/templates/index.html` & `pyslth-0.4.0/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/templates/service-worker.js` & `pyslth-0.4.0/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/tests.py` & `pyslth-0.4.0/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/urls.py` & `pyslth-0.4.0/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/utils.py` & `pyslth-0.4.0/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.9/slth/views.py` & `pyslth-0.4.0/slth/views.py`

 * *Files identical despite different names*

