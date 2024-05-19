# Comparing `tmp/pyslth-0.3.4.tar.gz` & `tmp/pyslth-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.3.4.tar", last modified: Sat May 18 10:13:00 2024, max compression
+gzip compressed data, was "pyslth-0.3.6.tar", last modified: Sun May 19 14:28:22 2024, max compression
```

## Comparing `pyslth-0.3.4.tar` & `pyslth-0.3.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.740301 pyslth-0.3.4/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.4/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-18 10:13:00.740156 pyslth-0.3.4/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.714243 pyslth-0.3.4/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-18 10:13:00.000000 pyslth-0.3.4/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.4/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-18 10:13:00.740340 pyslth-0.3.4/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-18 10:12:36.000000 pyslth-0.3.4/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.719429 pyslth-0.3.4/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.4/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.4/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.719881 pyslth-0.3.4/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.4/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.4/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.4/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.4/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.4/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.720100 pyslth-0.3.4/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.720526 pyslth-0.3.4/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.4/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.4/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.722861 pyslth-0.3.4/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.4/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.4/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.4/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.4/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.4/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.4/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.3.4/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.4/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.4/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.723199 pyslth-0.3.4/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.4/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.4/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.4/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.723451 pyslth-0.3.4/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.724840 pyslth-0.3.4/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.4/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.728153 pyslth-0.3.4/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.4/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.4/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.4/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.4/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.4/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.730120 pyslth-0.3.4/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.4/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.4/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.4/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.4/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.4/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.739437 pyslth-0.3.4/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.4/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.4/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   100846 2024-05-18 10:12:29.000000 pyslth-0.3.4/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.4/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.4/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-18 10:13:00.739884 pyslth-0.3.4/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-18 08:08:43.000000 pyslth-0.3.4/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.4/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.4/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.4/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.4/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.4/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.123421 pyslth-0.3.6/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.3.6/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 14:28:22.123177 pyslth-0.3.6/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.075301 pyslth-0.3.6/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1859 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 14:28:22.000000 pyslth-0.3.6/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.3.6/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 14:28:22.123487 pyslth-0.3.6/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 14:27:50.000000 pyslth-0.3.6/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.084190 pyslth-0.3.6/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.3.6/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.3.6/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.084775 pyslth-0.3.6/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.3.6/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.3.6/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.3.6/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.3.6/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.3.6/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.085087 pyslth-0.3.6/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.085750 pyslth-0.3.6/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.3.6/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.3.6/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.093693 pyslth-0.3.6/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.3.6/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.3.6/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.3.6/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.3.6/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.3.6/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.3.6/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.3.6/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.3.6/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.3.6/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.3.6/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.094197 pyslth-0.3.6/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.3.6/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.3.6/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.3.6/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.094596 pyslth-0.3.6/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.105535 pyslth-0.3.6/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.3.6/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.109733 pyslth-0.3.6/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.3.6/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.3.6/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.3.6/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.3.6/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.3.6/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.112151 pyslth-0.3.6/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.3.6/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.3.6/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.3.6/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.3.6/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.3.6/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.122119 pyslth-0.3.6/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.3.6/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.3.6/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.3.6/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   101600 2024-05-19 14:27:59.000000 pyslth-0.3.6/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.3.6/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.3.6/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 14:28:22.122761 pyslth-0.3.6/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3146 2024-05-18 08:08:43.000000 pyslth-0.3.6/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.3.6/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.3.6/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.3.6/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.3.6/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.3.6/slth/views.py
```

### Comparing `pyslth-0.3.4/PKG-INFO` & `pyslth-0.3.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.4
+Version: 0.3.6
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.4/pyslth.egg-info/PKG-INFO` & `pyslth-0.3.6/pyslth.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.3.4
+Version: 0.3.6
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.3.4/pyslth.egg-info/SOURCES.txt` & `pyslth-0.3.6/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/setup.py` & `pyslth-0.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.3.4',
+    version='0.3.6',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.3.4/slth/__init__.py` & `pyslth-0.3.6/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/components.py` & `pyslth-0.3.6/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/db/models.py` & `pyslth-0.3.6/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/endpoints.py` & `pyslth-0.3.6/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/factory.py` & `pyslth-0.3.6/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/forms.py` & `pyslth-0.3.6/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/management/commands/integration_test.py` & `pyslth-0.3.6/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/management/commands/sync.py` & `pyslth-0.3.6/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/migrations/0001_initial.py` & `pyslth-0.3.6/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.3.6/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.3.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/migrations/0006_user.py` & `pyslth-0.3.6/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/models.py` & `pyslth-0.3.6/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/notifications.py` & `pyslth-0.3.6/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/oauth.py` & `pyslth-0.3.6/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/permissions.py` & `pyslth-0.3.6/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/queryset.py` & `pyslth-0.3.6/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/roles.py` & `pyslth-0.3.6/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/selenium/__init__.py` & `pyslth-0.3.6/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/selenium/browser.py` & `pyslth-0.3.6/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/serializer.py` & `pyslth-0.3.6/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/.DS_Store` & `pyslth-0.3.6/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fontawesome.min.css` & `pyslth-0.3.6/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fonts/.DS_Store` & `pyslth-0.3.6/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.3.6/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.3.6/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.3.6/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.3.6/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/slth.css` & `pyslth-0.3.6/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/css/solid.min.css` & `pyslth-0.3.6/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/images/logo.png` & `pyslth-0.3.6/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/images/logo.svg` & `pyslth-0.3.6/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/images/user.png` & `pyslth-0.3.6/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/echarts.min.js` & `pyslth-0.3.6/slth/static/js/echarts.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -33045,15 +33045,15 @@
                                 g = r.isHorizontal() ?
                                 ((v = g), (_ = s.y), (w = s.height), v + (x = m - v)) :
                                 ((v = s.x), (_ = g), (x = s.width), _ + (w = m - _)),
                                 m = l[d - 1].tickValue;
                             null != m && c.set(m, p),
                                 o.add(
                                     new Ns({
-                                        anid: null != m ? "area_" + m : null,
+                                        anid: null != m ? "area" + m : null,
                                         shape: {
                                             x: v,
                                             y: _,
                                             width: x,
                                             height: w
                                         },
                                         style: B({
```

### Comparing `pyslth-0.3.4/slth/static/js/index.min.js` & `pyslth-0.3.6/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/ios-splash.min.js` & `pyslth-0.3.6/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/peerjs.min.js` & `pyslth-0.3.6/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/qrcode.min.js` & `pyslth-0.3.6/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/react-trigger-change.js` & `pyslth-0.3.6/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/react.min.js` & `pyslth-0.3.6/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/slth.min.js` & `pyslth-0.3.6/slth/static/js/slth.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
-    c as W,
+    c as H,
     r as B,
     R as Te
 } from "./react.min.js";
-const k = {
+const S = {
     colors: {
         primary: "var(--primary-color)",
         success: "var(--success-color)",
         warning: "var(--warning-color)",
         info: "var(--info-color)",
         danger: "var(--danger-color)",
         highlight: "var(--highlight-color)",
@@ -36,15 +36,15 @@
         })
     }
     return n()
 }
 
 function De(e) {
     function n(r) {
-        navigator.clipboard.writeText(r), G('Icon "' + r + '" copied to clipboard!')
+        navigator.clipboard.writeText(r), z('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
@@ -72,15 +72,15 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function S(e) {
+function C(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
@@ -92,56 +92,56 @@
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: e.display || "block"
         };
-        return e.primary && (a.backgroundColor = k.colors.primary, a.color = "white"), e.default && (a.color = k.colors.primary, a.border = "solid 1px " + k.colors.primary), t.jsx("a", {
+        return e.primary && (a.backgroundColor = S.colors.primary, a.color = "white"), e.default && (a.color = S.colors.primary, a.border = "solid 1px " + S.colors.primary), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(S, {
+            children: t.jsx(C, {
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
-            backgroundColor: e.isError ? "#e52207" : k.colors.success,
+            backgroundColor: e.isError ? "#e52207" : S.colors.success,
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(S, {
+            children: [t.jsx(C, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
-function G(e, n = !1) {
+function z(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), W.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
+    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -150,16 +150,16 @@
         e.remove()
     })
 }
 
 function oe(e) {
     function n() {
         const a = {
-            color: k.colors.info,
-            backgroundColor: k.background.info,
+            color: S.colors.info,
+            backgroundColor: S.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
@@ -174,22 +174,22 @@
     return n()
 }
 
 function Le(e) {
     const n = e.data;
     n.store && Object.keys(n.store).map(function(a) {
         n.store[a] ? localStorage.setItem(a, n.store[a]) : localStorage.removeItem(a, n.store[a])
-    }), n.redirect && n.redirect.length > 2 ? (n.message && localStorage.setItem("message", n.message), document.location.href = H(n.redirect)) : n.message && G(n.message)
+    }), n.redirect && n.redirect.length > 2 ? (n.message && localStorage.setItem("message", n.message), document.location.href = U(n.redirect)) : n.message && z(n.message)
 }
 
 function A(e) {
     return e.replace("/app/", "/api/")
 }
 
-function H(e) {
+function U(e) {
     return e.replace("/api/", "/app/")
 }
 
 function q(e, n, a, r) {
     const i = localStorage.getItem("token");
     var l = {
         Accept: "application/json"
@@ -207,35 +207,35 @@
     fetch(d, c).then(function(o) {
         if (s = o, u = s.headers.get("Content-Type"), u == "application/json") return o.text();
         if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
         o.text()
     }).then(o => {
         if (u == "application/json") {
             var h = JSON.parse(o || "{}");
-            typeof h == "object" && h.type == "redirect" ? document.location.href = H(h.url) : a && a(h, s)
+            typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var g = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var f = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
                     type: u
                 })),
                 w = document.createElement("a");
-            w.href = g, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
+            w.href = f, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
         } else a && a(o, s)
     })
 }
 
-function z(e) {
+function W(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
     if (typeof e == "string") {
-        if (e.length == 7 && e[0] == "#") return t.jsx(y, {
+        if (e.length == 7 && e[0] == "#") return t.jsx(x, {
             data: {
                 type: "color",
                 value: e
             }
         });
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
@@ -247,19 +247,19 @@
 `).map(function(i, l) {
             return t.jsx("div", {
                 children: i
             }, Math.random())
         });
         return e
     }
-    return typeof e == "object" && e.type ? t.jsx(y, {
+    return typeof e == "object" && e.type ? t.jsx(x, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : typeof e[0] == "object" && e[0].type != null ? t.jsx(t.Fragment, {
         children: e.map(function(i) {
-            return t.jsx(y, {
+            return t.jsx(x, {
                 data: i
             }, Math.random())
         })
     }) : t.jsx("ul", {
         style: {
             padding: 0,
             marginLeft: 17
@@ -269,42 +269,42 @@
                 children: i
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function de() {
-    document.querySelector(".layer") == null && W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
+    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
 function pe(e, n) {
     le(), de(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function Ae(e) {
-    le(), de(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: A(e)
     }))
 }
 
 function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function Re(e) {
-    le(), de(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
 function Oe(e) {
     const n = {
         backgroundColor: "black",
@@ -346,19 +346,19 @@
                 cursor: "pointer",
                 marginTop: -15
             };
         if (n) return t.jsxs("div", {
             style: s,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(S, {
+                children: t.jsx(C, {
                     icon: "x",
                     onClick: () => V()
                 })
-            }), t.jsx(y, {
+            }), t.jsx(x, {
                 data: n
             })]
         })
     }
     const c = {
         minWidth: window.innerWidth < 800 ? "calc(100% - 60px)" : 800,
         display: n ? "block" : "none",
@@ -394,15 +394,15 @@
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: i,
-                children: t.jsx(S, {
+                children: t.jsx(C, {
                     icon: "x",
                     onClick: () => V()
                 })
             }), t.jsx("iframe", {
                 src: A(e.url),
                 width: "100%",
                 height: 500,
@@ -458,57 +458,59 @@
     return t.jsx("dialog", {
         id: n,
         style: i,
         children: a()
     })
 }
 
-function E(e) {
+function M(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function _(e) {
     const n = e.id || Math.random(),
         [a, r] = B.useState(e.data.name);
 
     function i(c) {
         c.preventDefault();
         var s = e.data.url;
-        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(H(s)) : pe(s)
+        e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
     }
 
     function l() {
-        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
+        return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(C, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(S, {
+            children: [t.jsx(C, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
     function d() {
         var c = {
             padding: 12,
             textDecoration: "none",
+            whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
-            minWidth: 50
+            minWidth: 50,
+            lineHeight: "4rem"
         };
-        return e.primary && (c.backgroundColor = k.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + k.colors.primary, c.color = k.colors.primary), e.style && Object.keys(e.style).map(function(s) {
+        return e.primary && (c.backgroundColor = S.colors.primary, c.color = "white"), e.default && (c.border = "solid 1px " + S.colors.primary, c.color = S.colors.primary), e.style && Object.keys(e.style).map(function(s) {
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
-            href: H(e.data.url) || "#",
+            href: U(e.data.url) || "#",
             onClick: i,
             style: c,
-            "data-label": E(e.data.name),
+            "data-label": M(e.data.name),
             children: l()
         })
     }
     return d()
 }
 
 function Z(e) {
@@ -548,15 +550,15 @@
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": E(e.dataLabel),
+                "data-label": M(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: l,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(c => t.jsx("li", {
                     style: d,
@@ -579,26 +581,26 @@
     modal: a,
     imodal: r,
     children: i,
     onClick: l,
     dataLabel: d,
     style: c
 }) {
-    const s = n && n.indexOf("/media/") < 0 ? H(n) : n;
+    const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
         s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
     }
 
     function o() {
         return t.jsx("a", {
             id: e,
             onClick: l || u,
             href: s || "#",
-            "data-label": E(d),
+            "data-label": M(d),
             style: c,
             children: i
         })
     }
     return o()
 }
 
@@ -648,22 +650,22 @@
         })
     }
 
     function a() {
         return e.data.url && e.data.url.indexOf("only=") < 0 ? t.jsx(O, {
             href: e.data.url,
             children: t.jsxs(t.Fragment, {
-                children: [z(e.data.value), t.jsx(S, {
+                children: [W(e.data.value), t.jsx(C, {
                     icon: "external-link",
                     style: {
                         marginLeft: 10
                     }
                 })]
             })
-        }) : z(e.data.value)
+        }) : W(e.data.value)
     }
 
     function r() {
         const i = {
             minWidth: e.width + "%",
             marginTop: 5,
             marginBottom: 5
@@ -737,15 +739,15 @@
                 })
             }, Math.random())
         })
     }
     return n()
 }
 
-function Pe(e) {
+function He(e) {
     function n() {
         const l = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
             style: l,
@@ -775,15 +777,15 @@
             style: l,
             children: [n(), a(), r()]
         })
     }
     return i()
 }
 
-function He(e) {
+function Pe(e) {
     F(`
     .cards{
       padding: 10px;
       box-shadow: 0 1px 6px rgba( 0, 0, 0 , 0.16 );
       margin: 10px;
     }
     .cards h3{
@@ -947,15 +949,15 @@
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
                 children: t.jsx($, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
-        }) : t.jsx(y, {
+        }) : t.jsx(x, {
             data: a.data
         })
     }
 
     function c(u) {
         q("GET", u, function(o) {
             r(o)
@@ -1011,23 +1013,31 @@
       .object-title {
         display: flex;
         justify-content: space-between;
         align-items: baseline;
       }
       .object-title h1 {
           margin: 0;
-          color: ${k.colors.primary};
+          color: ${S.colors.primary};
       }
     `), t.jsxs("div", {
             className: "object-title",
+            style: {
+                flexDirection: window.innerWidth > 800 ? "row" : "column"
+            },
             children: [e.data.title && t.jsx("h1", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
-            }), t.jsx(Ve, {
-                data: e.data
+            }), t.jsx("div", {
+                style: {
+                    margin: 10
+                },
+                children: t.jsx(Ve, {
+                    data: e.data
+                })
             })]
         })
     }
     return n()
 }
 
 function ke(e) {
@@ -1042,15 +1052,15 @@
       }
     `);
 
     function n() {
         return t.jsxs("div", {
             className: "fieldset-title",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), e.data.actions && e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(a) {
                     return t.jsx(_, {
                         data: a,
                         default: !0
                     }, Math.random())
@@ -1066,15 +1076,15 @@
         return t.jsx($e, {
             data: e.data
         })
     }
 
     function a() {
         return e.data.data.map(function(i, l) {
-            return t.jsx(y, {
+            return t.jsx(x, {
                 data: i
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs("div", {
@@ -1095,40 +1105,51 @@
     function a() {
         const i = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(l, d) {
             return t.jsx("div", {
                 style: i,
-                children: t.jsx(y, {
+                children: t.jsx(x, {
                     data: l
                 }, Math.random())
-            })
+            }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function Qe(e) {
+    F(`
+    .noscroll::-webkit-scrollbar {
+      display: none;
+    }
+    .noscroll {
+      -ms-overflow-style: none;  /* IE and Edge */
+      scrollbar-width: none;  /* Firefox */
+    }
+  `);
     const [n, a] = B.useState(0);
 
     function r() {
         return t.jsx("div", {
+            className: "noscroll",
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
-                marginBottom: 20
+                marginBottom: 20,
+                overflowX: "auto"
             },
             children: e.data.map(function(i, l) {
                 return t.jsx(O, {
                     href: i.url,
                     style: {
                         padding: 5,
                         fontWeight: n == l ? "bold" : "normal",
@@ -1136,30 +1157,30 @@
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
                         d.preventDefault(), a(l), e.loadContent(i.url)
                     },
-                    dataLabel: E(i.title),
+                    dataLabel: M(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Xe(e) {
     var n = Math.random();
     const [a, r] = B.useState(e.data.data[0]);
 
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": E(e.data.title),
+            "data-label": M(e.data.title),
             children: e.data.title
         })
     }
 
     function l() {
         return t.jsx(Qe, {
             data: e.data.data,
@@ -1173,15 +1194,15 @@
         };
         o.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
-            children: t.jsx(y, {
+            children: t.jsx(x, {
                 data: o
             }, Math.random())
         })
     }
 
     function c() {
         const o = {
@@ -1225,23 +1246,23 @@
     label: r,
     display: i,
     primary: l,
     compact: d,
     spin: c
 }) {
     function s() {
-        return a ? d || !r ? t.jsx(S, {
+        return a ? d || !r ? t.jsx(C, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Be, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(S, {
+            }), t.jsx(C, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
@@ -1254,18 +1275,18 @@
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return l ? (o.backgroundColor = k.colors.primary, o.color = "white") : (o.border = "solid 1px " + k.colors.primary, o.color = k.colors.primary), t.jsx("a", {
+        return l ? (o.backgroundColor = S.colors.primary, o.color = "white") : (o.border = "solid 1px " + S.colors.primary, o.color = S.colors.primary), t.jsx("a", {
             id: e,
             style: o,
-            "data-label": E(r || a),
+            "data-label": M(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
     return u()
@@ -1309,15 +1330,15 @@
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function nt(e) {
     function n(l) {
-        return e.data.icon ? l.done ? t.jsx(S, {
+        return e.data.icon ? l.done ? t.jsx(C, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -1326,18 +1347,18 @@
             },
             children: l.number
         })
     }
 
     function a(l) {
         return {
-            border: "3px solid " + k.colors.primary,
+            border: "3px solid " + S.colors.primary,
             borderRadius: "50%",
-            background: l.done ? k.colors.primary : "white",
-            color: l.done ? "white" : k.colors.primary,
+            background: l.done ? S.colors.primary : "white",
+            color: l.done ? "white" : S.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
@@ -1410,15 +1431,15 @@
             i = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: k.colors[e.data.style]
+                backgroundColor: S.colors[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
                 style: i,
                 children: t.jsxs("span", {
                     style: r,
@@ -1428,15 +1449,15 @@
         })
     }
     return n()
 }
 
 function rt(e) {
     function n() {
-        return e.data.color = k.colors[e.data.style], t.jsx(Se, {
+        return e.data.color = S.colors[e.data.style], t.jsx(Se, {
             data: e.data
         })
     }
     return n()
 }
 
 function Se(e) {
@@ -1450,15 +1471,15 @@
             whiteSpace: "nowrap",
             backgroundColor: e.data.color,
             display: "inline-flex",
             border: "solid 3px white"
         };
         return t.jsxs("div", {
             style: a,
-            children: [e.data.icon && t.jsx(S, {
+            children: [e.data.icon && t.jsx(C, {
                 icon: e.data.icon,
                 style: {
                     marginRight: 5
                 }
             }), e.data.label]
         })
     }
@@ -1484,39 +1505,39 @@
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
             i = {
                 marginTop: 30,
                 fontSize: "3rem",
-                color: k.colors.auxiliary
+                color: S.colors.auxiliary
             },
             l = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
-                color: k.colors.primary
+                color: S.colors.primary
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 style: {
-                    color: k.colors.primary
+                    color: S.colors.primary
                 },
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(d => t.jsxs(O, {
                     href: d.url,
                     style: r,
                     dataLabel: d.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             style: i,
                             icon: d.icon
                         })
                     }), t.jsx("div", {
                         style: l,
                         children: d.label
                     })]
@@ -1548,15 +1569,15 @@
 }
 
 function ot(e) {
     function n() {
         return e.data.url ? t.jsx(O, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(S, {
+            children: e.data.icon ? t.jsx(C, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
@@ -1597,15 +1618,15 @@
     return a()
 }
 
 function ct(e) {
     function n() {
         const a = {
                 color: "white",
-                backgroundColor: k.colors.highlight,
+                backgroundColor: S.colors.highlight,
                 margin: -20,
                 textAlign: "center",
                 paddingTop: 20,
                 paddingBottom: 70
             },
             r = {
                 fontSize: "4rem",
@@ -1617,22 +1638,22 @@
                 maxWidth: 200,
                 margin: "auto"
             };
         if (e.data) return t.jsxs("div", {
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
                 children: e.data.items.map(l => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
-                        children: z(l.value)
+                        children: W(l.value)
                     }), t.jsx("div", {
                         style: i,
                         children: l.name
                     })]
                 }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
@@ -1649,15 +1670,15 @@
 }
 
 function ut(e) {
     function n() {
         return t.jsx(P, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
-                children: t.jsx(y, {
+                children: t.jsx(x, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
@@ -1686,101 +1707,101 @@
     var a = !1;
     const r = "rgb(219, 237, 255)",
         i = "rgb(89, 154, 242)",
         l = "rgb(246, 123, 135)",
         d = [],
         c = [];
 
-    function s(v) {
-        return e.data.readonly ? v == null ? r : i : v == null ? r : v.text == null ? i : l
+    function s(y) {
+        return e.data.readonly ? y == null ? r : i : y == null ? r : y.text == null ? i : l
     }
 
-    function u(v) {
-        a = !0, v.preventDefault()
+    function u(y) {
+        a = !0, y.preventDefault()
     }
 
-    function o(v) {
+    function o(y) {
         a = !1, document.getElementById("input" + n).value = JSON.stringify({
             select: d,
             deselect: c
         })
     }
 
-    function h(v) {
-        e.data.readonly || e.data.single_selection && g().length > 0 && v.target.style.backgroundColor != i || a && v.target.style.backgroundColor != l && (v.target.style.backgroundColor == r ? (v.target.style.backgroundColor = i, console.log("MARCOU", v.target.dataset.day, v.target.dataset.time), d.push([v.target.dataset.day, v.target.dataset.time])) : (v.target.style.backgroundColor = r, console.log("DEMARCOU", v.target.dataset.day, v.target.dataset.time), c.push([v.target.dataset.day, v.target.dataset.time])))
+    function h(y) {
+        e.data.readonly || e.data.single_selection && f().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != l && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
     }
 
-    function g() {
-        const v = [];
+    function f() {
+        const y = [];
         return document.getElementById(n).querySelectorAll("td").forEach(function(D) {
-            D.style.backgroundColor == i && v.push(D.dataset.day, D.dataset.time)
-        }), v
+            D.style.backgroundColor == i && y.push(D.dataset.day, D.dataset.time)
+        }), y
     }
 
     function w() {
-        const v = {
+        const y = {
                 overflowX: "auto"
             },
             D = {
                 width: "100%",
                 borderSpacing: 0,
                 borderCollapse: "collapse",
                 marginTop: 15,
                 marginBottom: 15
             },
-            m = {
+            j = {
                 border: "solid 4px white"
             };
         return t.jsxs("div", {
             id: n,
-            style: v,
+            style: y,
             children: [t.jsx("input", {
                 id: "input" + n,
                 type: "hidden",
                 name: e.data.input_name
             }), t.jsxs("table", {
                 style: D,
                 onMouseDown: u,
                 onMouseUp: o,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: e.data.matrix[0].map(function(j) {
+                        children: e.data.matrix[0].map(function(v) {
                             return t.jsx("th", {
                                 className: "bold",
-                                style: m,
-                                children: j.text
+                                style: j,
+                                children: v.text
                             }, Math.random())
                         })
                     })
                 }), t.jsx("tbody", {
-                    children: e.data.matrix.map(function(j, x) {
-                        if (x > 0) return t.jsx("tr", {
-                            children: j.map(function(I, b) {
+                    children: e.data.matrix.map(function(v, g) {
+                        if (g > 0) return t.jsx("tr", {
+                            children: v.map(function(k, b) {
                                 if (b == 0) return t.jsx("th", {
                                     className: "bold",
                                     align: "center",
-                                    style: m,
-                                    children: I.text
+                                    style: j,
+                                    children: k.text
                                 }, Math.random());
                                 {
-                                    const C = {
-                                        backgroundColor: s(I),
+                                    const E = {
+                                        backgroundColor: s(k),
                                         border: "solid 4px white"
                                     };
                                     return t.jsx("td", {
                                         align: "center",
-                                        style: C,
+                                        style: E,
                                         onMouseDown: h,
                                         onMouseLeave: h,
                                         onMouseUp: h,
                                         "data-day": e.data.matrix[0][b].text,
-                                        "data-time": j[0].text,
-                                        children: I && I.text && t.jsx(mt, {
-                                            text: I.text,
-                                            children: t.jsx(S, {
+                                        "data-time": v[0].text,
+                                        children: k && k.text && t.jsx(mt, {
+                                            text: k.text,
+                                            children: t.jsx(C, {
                                                 icon: "stethoscope",
                                                 style: {
                                                     color: "white",
                                                     cursor: "help"
                                                 }
                                             })
                                         })
@@ -1802,15 +1823,15 @@
       .tooltip {
         position: relative;
         display: inline-block;
       }
       .tooltip .tooltiptext {
         visibility: hidden;
         width: 220px;
-        background-color: ${k.colors.highlight};
+        background-color: ${S.colors.highlight};
         color: #fff;
         text-align: center;
         border-radius: 6px;
         padding: 5px 0;
         position: absolute;
         z-index: 1;
         bottom: 150%;
@@ -1821,15 +1842,15 @@
       .tooltip:hover .tooltiptext {
         visibility: visible;
       }
     `), t.jsxs("div", {
             className: "tooltip",
             children: [e.children, t.jsx("div", {
                 className: "tooltiptext",
-                children: z(e.text)
+                children: W(e.text)
             })]
         })
     }
     return n()
 }
 const ft = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     J = {
@@ -1839,15 +1860,15 @@
         backgroundColor: "white"
     };
 
 function gt(e) {
     const n = new FormData(e);
     for (let [a, r] of Array.from(n.entries())) {
         const i = e[a];
-        (r === "" || !(i.tagName == "SELECT" || i.tagName == null)) && n.delete(a)
+        i.tagName == "SELECT" && r !== "" || i.tagName == null && r !== "" || i.type == "radio" && r !== "" || i.type == "checkbox" && r !== "" || n.delete(a)
     }
     return new URLSearchParams(n).toString()
 }
 
 function Q(e, n) {
     const a = e.indexOf("?") < 0 ? "?" : "&",
         r = gt(n);
@@ -1915,29 +1936,29 @@
         for (var a in e.set) bt(a, e.set[a])
     }
 }
 
 function wt(e) {
     function n() {
         const a = {
-            color: k.colors.info,
-            backgroundColor: k.background.info,
+            color: S.colors.info,
+            backgroundColor: S.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(S, {
+                children: [t.jsx(C, {
                     icon: "circle-check",
                     style: {
-                        color: k.colors.info,
+                        color: S.colors.info,
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
                 children: e.children
             })]
         })
@@ -1955,15 +1976,15 @@
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
             className: "error",
-            children: [t.jsx(S, {
+            children: [t.jsx(C, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -2071,18 +2092,18 @@
 }
 
 function ye(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), B.useEffect(() => {
         function d(u, o, h) {
-            var g = h.target,
-                w = g.value.replace(/\D/g, ""),
-                v = g.value.length > o ? 1 : 0;
-            VMasker(g).unMask(), VMasker(g).maskPattern(u[v]), g.value = VMasker.toPattern(w, u[v])
+            var f = h.target,
+                w = f.value.replace(/\D/g, ""),
+                y = f.value.length > o ? 1 : 0;
+            VMasker(f).unMask(), VMasker(f).maskPattern(u[y]), f.value = VMasker.toPattern(w, u[y])
         }
         if (e.data.mask) {
             var c = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
@@ -2102,32 +2123,32 @@
         if (e.data.type == "file" && d.target.files) {
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (re(s.name)) {
                     const w = "display" + a;
                     var o = document.createElement("img");
-                    o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(v) {
+                    o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(y) {
                         const D = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
-                        var m = document.createElement("canvas");
-                        const j = m.getContext("2d");
-                        m.height = m.width * (o.height / o.width);
-                        const x = document.createElement("canvas"),
-                            I = x.getContext("2d");
-                        x.width = o.width * D, x.height = o.height * D, I.drawImage(o, 0, 0, x.width, x.height), j.drawImage(x, 0, 0, x.width * D, x.height * D, 0, 0, m.width, m.height), x.toBlob(function(C) {
+                        var j = document.createElement("canvas");
+                        const v = j.getContext("2d");
+                        j.height = j.width * (o.height / o.width);
+                        const g = document.createElement("canvas"),
+                            k = g.getContext("2d");
+                        g.width = o.width * D, g.height = o.height * D, k.drawImage(o, 0, 0, g.width, g.height), v.drawImage(g, 0, 0, g.width * D, g.height * D, 0, 0, j.width, j.height), g.toBlob(function(E) {
                             const T = new DataTransfer;
-                            T.items.add(new File([C], s.name)), d.target.files = T.files
+                            T.items.add(new File([E], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
                         b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
                     }, o.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
-                var g = s.size / 1024;
-                g < 1024 ? g = parseInt(g) + " Kb" : g = (g / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + g, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + g + ". Por favor, adicione um arquivo menor.")
+                var f = s.size / 1024;
+                f < 1024 ? f = parseInt(f) + " Kb" : f = (f / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + f, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + f + ". Por favor, adicione um arquivo menor.")
             }, c.readAsDataURL(s)
         }
     }
 
     function l() {
         var d = e.data.type;
         if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
@@ -2147,19 +2168,19 @@
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
-                                color: k.colors.primary
+                                color: S.colors.primary
                             }
                         })
                     }), t.jsxs("div", {
                         style: u,
                         children: [e.data.value && re(e.data.value) && t.jsx("div", {
                             style: {
                                 textAlign: "center"
@@ -2187,15 +2208,15 @@
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: d,
                     name: e.data.name,
                     id: a,
-                    "data-label": E(e.data.label),
+                    "data-label": M(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: i,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
@@ -2208,28 +2229,28 @@
                 ...J
             }, s.width = "100%", s.backgroundColor = "white", s.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: d,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": E(e.data.label),
+                "data-label": M(e.data.label),
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
-    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, C) {
+    Array.isArray(e.data.value) ? e.data.value.forEach(function(b, E) {
         n.push({
             id: b.id,
             value: b.label
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
@@ -2238,60 +2259,60 @@
         r = e.data.id2,
         i = Array.isArray(e.data.value),
         [l, d] = B.useState(!1),
         [c, s] = B.useState(null);
     var u = !1;
     let o;
     B.useEffect(() => {
-        j(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
-            j(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+        v(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
+            v(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
         const b = document.getElementById(a);
         if (i) {
-            const C = {
+            const E = {
                     padding: 5,
                     display: "inline"
                 },
                 T = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                f = {
+                m = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [b == null && n.map((p, M) => t.jsxs("div", {
-                    style: C,
+                children: [b == null && n.map((p, I) => t.jsxs("div", {
+                    style: E,
                     children: [t.jsx("span", {
-                        onClick: () => x(M),
+                        onClick: () => g(I),
                         style: T,
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             icon: "trash-can",
-                            style: f
+                            style: m
                         })
                     }), p.value]
-                }, Math.random())), b != null && Array.from(b.options).map((p, M) => t.jsxs("div", {
-                    style: C,
+                }, Math.random())), b != null && Array.from(b.options).map((p, I) => t.jsxs("div", {
+                    style: E,
                     children: [t.jsx("span", {
-                        onClick: () => x(M),
+                        onClick: () => g(I),
                         style: T,
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             icon: "trash-can",
-                            style: f
+                            style: m
                         })
                     }), p.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
-    function g() {
+    function f() {
         return t.jsx("select", {
             id: a,
             name: e.data.name,
             multiple: i,
             readOnly: !0,
             style: {
                 display: "contents"
@@ -2300,143 +2321,143 @@
     }
 
     function w() {
         const b = {
                 ...J,
                 ...e.style || {}
             },
-            C = {
+            E = {
                 padding: 0,
                 margin: 0,
                 border: "solid 1px #d9d9d9",
                 marginTop: -1,
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto",
                 zIndex: 99999
             };
-        C.position = "absolute", C.backgroundColor = "white";
+        E.position = "absolute", E.backgroundColor = "white";
         const T = document.getElementById(r);
         if (e.data.icon && (b.paddingLeft = 30), T) {
             let N = null,
                 X = T,
                 ae = null;
             for (; !ae && (X = X.parentElement) instanceof HTMLElement;) X.matches("dialog") && (ae = X);
             N = ae;
             const K = T.getBoundingClientRect();
-            var f = K.top + K.height,
+            var m = K.top + K.height,
                 p = K.left;
             if (N) {
                 const fe = N.getBoundingClientRect();
-                f = f - fe.top, p = p - fe.left
-            } else f += window.scrollY, p += window.scrollX;
-            C.width = K.width, C.top = f, C.left = p
+                m = m - fe.top, p = p - fe.left
+            } else m += window.scrollY, p += window.scrollX;
+            E.width = K.width, E.top = m, E.left = p
         }
-        const M = {
+        const I = {
                 cursor: "pointer",
                 padding: 10
             },
             L = !i && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
-            children: [e.data.icon && t.jsx(S, {
+            children: [e.data.icon && t.jsx(C, {
                 icon: e.data.icon,
                 style: {
                     position: "absolute",
                     margin: 13,
                     color: "#d9d9d9"
                 }
             }), t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
                 onFocus: N => {
-                    N.target.select(), m(N)
+                    N.target.select(), j(N)
                 },
-                onChange: m,
-                onMouseLeave: v,
-                onBlur: v,
+                onChange: j,
+                onMouseLeave: y,
+                onBlur: y,
                 defaultValue: L,
                 style: b,
-                "data-label": E(e.data.label)
+                "data-label": M(e.data.label)
             }), c && l && t.jsxs("ul", {
-                style: C,
+                style: E,
                 onMouseLeave: D,
                 onMouseEnter: function(N) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
-                    style: M,
+                    style: I,
                     children: "Nenhuma opção encontrada."
                 }), c.map(N => t.jsx("li", {
                     onClick: () => {
-                        d(!1), e.onSelect ? e.onSelect(N) : j(N)
+                        d(!1), e.onSelect ? e.onSelect(N) : v(N)
                     },
-                    style: M,
+                    style: I,
                     className: "autocomplete-item",
-                    "data-label": E(N.value),
+                    "data-label": M(N.value),
                     children: N.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function v(b) {
+    function y(b) {
         u = !1, setTimeout(function() {
             u || D(b)
         }, 250)
     }
 
     function D(b) {
-        const C = document.getElementById(a);
-        if (C) {
+        const E = document.getElementById(a);
+        if (E) {
             const T = document.getElementById(r);
-            i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && Y(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
+            i || E.options.length > 0 && T.value != E.options[0].innerHTML && (E.innerHTML = "", T.value = "", d(!1), e.data.onchange && Y(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
-    function m(b) {
+    function j(b) {
         clearTimeout(o), o = setTimeout(function() {
-            const C = b.target.closest("form"),
+            const E = b.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            d(!0), q("GET", Q(e.data.choices + T + "term=" + b.target.value, C), function(p) {
+            d(!0), q("GET", Q(e.data.choices + T + "term=" + b.target.value, E), function(p) {
                 s(p)
             })
         }, 1e3)
     }
 
-    function j(b, C = !1) {
+    function v(b, E = !1) {
         const T = document.getElementById(a),
-            f = document.getElementById(r);
-        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, f.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, f.value = b.value), e.data.onchange && !C && Y(f, e.data.onchange)
+            m = document.getElementById(r);
+        T.innerHTML == null && (T.innerHTML = ""), Array.isArray(b) ? T.innerHTML = b.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : i ? (T.innerHTML += `<option selected value="${b.id}">${b.value}</option>`, m.value = "") : (T.innerHTML = `<option selected value="${b.id}">${b.value}</option>`, m.value = b.value), e.data.onchange && !E && Y(m, e.data.onchange)
     }
 
-    function x(b) {
-        const C = document.getElementById(a);
-        var T = Array.from(C.options);
-        C.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(f => `<option selected value="${f.value}">${f.innerHTML}</option>`).join(""), s([])
+    function g(b) {
+        const E = document.getElementById(a);
+        var T = Array.from(E.options);
+        E.innerHTML = T.slice(0, b).concat(T.slice(b + 1)).map(m => `<option selected value="${m.value}">${m.innerHTML}</option>`).join(""), s([])
     }
 
-    function I() {
+    function k() {
         return t.jsxs(t.Fragment, {
-            children: [h(), g(), w()]
+            children: [h(), f(), w()]
         })
     }
-    return I()
+    return k()
 }
 
 function kt(e) {
     function n() {
         var a = {
             ...J
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": E(e.data.label),
+            "data-label": M(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
@@ -2489,15 +2510,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + o,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
                     defaultChecked: l(u),
-                    "data-label": E(u.value),
+                    "data-label": M(u.value),
                     onClick: function() {
                         d(i.name + r + o)
                     },
                     onMouseEnter: function() {
                         c(i.name + r + o)
                     }
                 }), t.jsx("label", {
@@ -2551,15 +2572,15 @@
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
                     defaultChecked: l(s),
-                    "data-label": E(s.value)
+                    "data-label": M(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
             className: "checkbox-group " + i.name,
@@ -2574,15 +2595,15 @@
 function Ct(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": E(n.label),
+            "data-label": M(n.label),
             defaultValue: n.value,
             style: J,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
@@ -2618,16 +2639,16 @@
         })
     }
 
     function l(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
             o = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
-            g = document.getElementById("hide-" + n);
-        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", g.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+            f = document.getElementById("hide-" + n);
+        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", f.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function d() {
         const s = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
@@ -2646,91 +2667,91 @@
         const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: s,
-                "data-label": E(e.data.label),
+                "data-label": M(e.data.label),
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
-        const g = n;
+        const f = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
-            id: "form-" + g + "-" + a,
+            id: "form-" + f + "-" + a,
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
-                    id: "extra-add-" + g + "-",
+                    id: "extra-add-" + f + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => d(g),
+                    onClick: () => d(f),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function i() {
         const o = c(),
             h = o.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
-        for (var g = 0; g < n; g++) {
-            var w = document.getElementById("extra-add-" + g + "-");
+        for (var f = 0; f < n; f++) {
+            var w = document.getElementById("extra-add-" + f + "-");
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
-            h.fields.map(function(g) {
-                g.map(function(w) {
+            h.fields.map(function(f) {
+                f.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
-                }), g[0].value = 0
+                }), f[0].value = 0
             })
-        }), W.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
     }
 
     function d(o) {
         const h = e.data.template,
             w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
-            v = document.querySelector("input[name=" + w + "]");
-        parseInt(v.value) == 0 ? v.value = "" : v.value = -parseInt(v.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
+            y = document.querySelector("input[name=" + w + "]");
+        parseInt(y.value) == 0 ? y.value = "" : y.value = -parseInt(y.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
     }
 
     function c() {
         for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
         return o
     }
 
@@ -2756,23 +2777,23 @@
         const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: o,
-                "data-label": E(e.data.label),
+                "data-label": M(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
-                children: [s(), e.data.value.map(function(h, g) {
-                    return r(h, g == e.data.value.length - 1 ? "inline" : "none")
+                children: [s(), e.data.value.map(function(h, f) {
+                    return r(h, f == e.data.value.length - 1 ? "inline" : "none")
                 })]
             })]
         })
     }
     return u()
 }
 
@@ -2795,15 +2816,15 @@
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": E(r.title),
+                    "data-label": M(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
                     children: i.map(l => t.jsx("div", {
                         className: "form-group " + l.name,
@@ -2822,15 +2843,15 @@
 
 function Tt(e) {
     const n = Math.random();
 
     function a() {
         const h = {
             margin: 0,
-            color: k.colors.primary
+            color: S.colors.primary
         };
         return t.jsx("h1", {
             style: h,
             children: e.data.title
         })
     }
 
@@ -2840,15 +2861,15 @@
                 text: e.data.info
             }
         })
     }
 
     function i() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(h => t.jsx(y, {
+            children: [e.data.display.map(h => t.jsx(x, {
                 data: h
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
@@ -2914,41 +2935,41 @@
 
     function u() {
         V()
     }
 
     function o(h) {
         h.preventDefault();
-        var g = e.data.url,
+        var f = e.data.url,
             w = document.getElementById(n),
-            v = new FormData(w);
+            y = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
-            const D = g.indexOf("?") >= 0 ? "&" : "?";
-            g = g + D + "form=" + e.data.title + "&" + new URLSearchParams(v).toString(), v = null
+            const D = f.indexOf("?") >= 0 ? "&" : "?";
+            f = f + D + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
         }
-        q(w.method.toUpperCase(), g, function(m) {
-            if (w.querySelectorAll(".error").forEach(x => x.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), m.type == "response") m.store && Object.keys(m.store).map(function(x) {
-                m.store[x] ? localStorage.setItem(x, m.store[x]) : localStorage.removeItem(x, m.store[x])
-            }), m.redirect && m.redirect.length > 2 ? (m.message && localStorage.setItem("message", m.message), document.location.href = H(m.redirect)) : (m.message && G(m.message), m.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : V()), m.redirect == "." && w.reset(), m.dispose && (w.style.display = "none"), Ke());
-            else if (m.type == "error") {
-                var j = m.text;
-                console.log(m), Object.keys(m.errors).map(function(x) {
-                    if (x == "__all__") j = m.errors[x];
+        q(w.method.toUpperCase(), f, function(j) {
+            if (w.querySelectorAll(".error").forEach(g => g.style.display = "none"), h.target.dataset.spinning && (h.target.querySelector("i.fa-spin").style.display = "none", h.target.querySelector("i.fa-" + h.target.dataset.spinning).style.display = "inline-block"), j.type == "response") j.store && Object.keys(j.store).map(function(g) {
+                j.store[g] ? localStorage.setItem(g, j.store[g]) : localStorage.removeItem(g, j.store[g])
+            }), j.redirect && j.redirect.length > 2 ? (j.message && localStorage.setItem("message", j.message), document.location.href = U(j.redirect)) : (j.message && z(j.message), j.redirect == ".." && (document.getElementsByTagName("dialog").length == 0 ? history.back() : V()), j.redirect == "." && w.reset(), j.dispose && (w.style.display = "none"), Ke());
+            else if (j.type == "error") {
+                var v = j.text;
+                console.log(j), Object.keys(j.errors).map(function(g) {
+                    if (g == "__all__") v = j.errors[g];
                     else {
-                        const I = w.querySelector("#" + x + "_error");
-                        I.querySelector("span").innerHTML = m.errors[x], I.style.display = "block"
+                        const k = w.querySelector("#" + g + "_error");
+                        k.querySelector("span").innerHTML = j.errors[g], k.style.display = "block"
                     }
-                }), G(j, !0)
+                }), z(v, !0)
             } else {
-                const x = document.querySelector("#output");
-                x.innerHTML = "", W.createRoot(x.appendChild(document.createElement("div"))).render(t.jsx(y, {
-                    data: m
+                const g = document.querySelector("#output");
+                g.innerHTML = "", H.createRoot(g.appendChild(document.createElement("div"))).render(t.jsx(x, {
+                    data: j
                 }))
             }
-        }, v)
+        }, y)
     }
     return s()
 }
 
 function It(e) {
     F(`
         .calendar table{
@@ -3029,15 +3050,15 @@
                 }), t.jsxs("div", {
                     children: [t.jsxs("h3", {
                         align: "center",
                         children: [a[e.data.month - 1], " ", e.data.year]
                     }), e.data.day && t.jsxs("div", {
                         align: "center",
                         className: "day",
-                        children: [new Date(e.data.year, e.data.month - 1, e.data.day).toLocaleDateString("pt-BR"), t.jsx(S, {
+                        children: [new Date(e.data.year, e.data.month - 1, e.data.day).toLocaleDateString("pt-BR"), t.jsx(C, {
                             default: !0,
                             icon: "x",
                             onClick: () => e.onChange(null, e.data.month, e.data.year),
                             style: {
                                 marginLeft: 10,
                                 cursor: "pointer"
                             }
@@ -3070,15 +3091,15 @@
                                 }) : h.date + h.today
                             }), h.total && t.jsx("div", {
                                 className: "total",
                                 onClick: () => e.onChange(h.date, e.data.month, e.data.year),
                                 children: t.jsx("div", {
                                     className: "number",
                                     style: {
-                                        backgroundColor: k.colors.primary
+                                        backgroundColor: S.colors.primary
                                     },
                                     children: t.jsx("span", {
                                         style: {
                                             textDecoration: h.selected ? "underline" : "normal"
                                         },
                                         children: h.total
                                     })
@@ -3180,15 +3201,15 @@
     }
     return n()
 }
 
 function Bt(e) {
     function n() {
         const a = {
-            backgroundColor: k.colors.primary,
+            backgroundColor: S.colors.primary,
             color: "white",
             borderRadius: "50%",
             minWidth: 13,
             marginLeft: 2,
             padding: 4,
             fontSize: "70%",
             display: "inline-block",
@@ -3232,363 +3253,363 @@
         text-decoration: none;
     }
   `), e.data.id == null && (e.data.id = Math.random());
     const [n, a] = B.useState(e.data);
 
     function r() {
         return n.attrname ? t.jsx("h2", {
-            "data-label": E(n.title),
+            "data-label": M(n.title),
             children: n.title
         }) : t.jsxs("h1", {
-            "data-label": E(n.title),
+            "data-label": M(n.title),
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
 
-    function l(f) {
-        document.getElementById("loader-" + e.data.id).style.display = f ? "block" : "none"
+    function l(m) {
+        document.getElementById("loader-" + e.data.id).style.display = m ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
-            children: n.subsets.map(function(f, p) {
-                var M = n.subset === f.name || !n.subset && p == 0;
+            children: n.subsets.map(function(m, p) {
+                var I = n.subset === m.name || !n.subset && p == 0;
                 return t.jsxs(O, {
                     href: "#",
                     style: {
-                        borderBottom: M ? "solid 3px #2670e8" : 0,
+                        borderBottom: I ? "solid 3px #2670e8" : 0,
                         color: "#0c326f"
                     },
                     onClick: function(L) {
-                        L.preventDefault(), c(f.name)
+                        L.preventDefault(), c(m.name)
                     },
-                    dataLabel: E(f.label),
-                    children: [f.label, " ", t.jsx(Bt, {
-                        total: f.count
+                    dataLabel: M(m.label),
+                    children: [m.label, " ", t.jsx(Bt, {
+                        total: m.count
                     })]
                 }, Math.random())
             })
         })
     }
 
-    function c(f) {
+    function c(m) {
         const p = document.getElementById("subset-" + e.data.id);
-        p.value = f || "", I()
+        p.value = m || "", k()
     }
 
-    function s(f, p, M) {
+    function s(m, p, I) {
         const L = document.getElementById("form-" + e.data.id);
-        L.querySelector("input[name=" + n.calendar.field + "__day]").value = f || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = M || "", v(1)
+        L.querySelector("input[name=" + n.calendar.field + "__day]").value = m || "", L.querySelector("input[name=" + n.calendar.field + "__month]").value = p || "", L.querySelector("input[name=" + n.calendar.field + "__year]").value = I || "", y(1)
     }
 
     function u() {
         if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
-    function o(f) {
+    function o(m) {
         const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
-            color: k.colors.primary,
+            color: S.colors.primary,
             padding: 5
         };
         if (!(window.innerWidth < 800)) return t.jsxs("tr", {
-            children: [f.map(function(M) {
-                return M.label != "ID" && t.jsx("th", {
+            children: [m.map(function(I) {
+                return I.label != "ID" && t.jsx("th", {
                     style: p,
                     className: "bold",
-                    children: M.label
+                    children: I.label
                 }, Math.random())
             }), t.jsx("th", {
                 style: p
             })]
         })
     }
 
-    function h(f) {
+    function h(m) {
         const p = {
                 borderBottom: "solid 1px #DDD",
                 padding: 5
             },
-            M = {
+            I = {
                 borderBottom: "solid 1px #DDD",
                 lineHeight: "3rem",
                 textAlign: "right"
             };
         return window.innerWidth < 800 ? t.jsxs("tr", {
             children: [t.jsx("td", {
                 style: p,
-                children: f.title
+                children: m.title
             }, Math.random()), t.jsx("td", {
-                style: M,
+                style: I,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: t.jsx(S, {
+                    children: t.jsx(C, {
                         icon: "chevron-right",
-                        onClick: () => Re(f.actions),
+                        onClick: () => Re(m.actions),
                         style: {
                             cursor: "pointer",
                             marginRight: 20
                         }
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [f.data.map(function(L) {
+            children: [m.data.map(function(L) {
                 return L.label != "ID" && t.jsx("td", {
                     style: p,
-                    children: z(L.value)
+                    children: W(L.value)
                 }, Math.random())
             }), t.jsx("td", {
-                style: M,
+                style: I,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: f.actions.map(function(L) {
+                    children: m.actions.map(function(L) {
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
 
-    function g() {
+    function f() {
         return n.data.length > 0 ? (n.render == null && window.innerWidth < 800 && (n.renderer = "rows"), n.renderer ? n.renderer == "cards" ? t.jsx(P, {
             width: 300,
             alignItems: "start",
-            children: n.data.map(function(f) {
-                return f.type = n.renderer, t.jsx("div", {
-                    children: t.jsx(y, {
-                        data: f
+            children: n.data.map(function(m) {
+                return m.type = n.renderer, t.jsx("div", {
+                    children: t.jsx(x, {
+                        data: m
                     })
                 }, Math.random())
             })
         }) : t.jsx("div", {
             style: {
                 marginBottom: 15
             },
-            children: n.data.map(function(f) {
-                return f.type = n.renderer, t.jsx(y, {
-                    data: f
+            children: n.data.map(function(m) {
+                return m.type = n.renderer, t.jsx(x, {
+                    data: m
                 }, Math.random())
             })
         }) : w()) : t.jsx(oe, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
-        const f = {
+        const m = {
                 width: "100%",
                 overflowX: "auto"
             },
             p = {
                 width: "100%",
                 lineHeight: "2rem",
                 borderSpacing: 0
             };
         return t.jsx("div", {
-            style: f,
+            style: m,
             children: t.jsxs("table", {
                 style: p,
                 children: [t.jsx("thead", {
                     children: o(n.data[0].data)
                 }), t.jsx("tbody", {
-                    children: n.data.map(function(M) {
-                        return h(M)
+                    children: n.data.map(function(I) {
+                        return h(I)
                     })
                 })]
             })
         })
     }
 
-    function v(f) {
-        const M = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        M && (M.value = f), I(), j()
+    function y(m) {
+        const I = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
+        I && (I.value = m), k(), v()
     }
 
     function D() {
-        const f = document.getElementById("form-" + e.data.id);
-        if (f) {
-            const p = f.querySelector("input[name=page]");
+        const m = document.getElementById("form-" + e.data.id);
+        if (m) {
+            const p = m.querySelector("input[name=page]");
             p && (p.value = n.pagination.page.current)
         }
         return t.jsx(Dt, {
             data: n.pagination,
-            onChange: v,
+            onChange: y,
             total: n.total
         })
     }
 
-    function m() {
+    function j() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
-            children: n.actions.map(function(f) {
+            children: n.actions.map(function(m) {
                 return t.jsx(_, {
-                    data: f,
+                    data: m,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function j() {
-        const f = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
-        console.log(f), console.log(e.data.id), window.scrollTo({
-            top: f,
+    function v() {
+        const m = document.getElementById(e.data.id).getBoundingClientRect().top + window.scrollY;
+        console.log(m), console.log(e.data.id), window.scrollTo({
+            top: m,
             behavior: "smooth"
         })
     }
 
-    function x() {
-        const f = {
+    function g() {
+        const m = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             p = n.search.length > 0,
-            M = n.filters.length > 0;
-        if ((n.bi || n.data.length >= 0) && (p || M)) {
+            I = n.filters.length > 0;
+        if ((n.bi || n.data.length >= 0) && (p || I)) {
             const L = {
                 name: "q",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves",
                 value: n.q
             };
             return t.jsxs("div", {
-                style: f,
+                style: m,
                 children: [t.jsxs(P, {
                     width: 250,
                     children: [p && t.jsx("div", {
                         children: t.jsx(ee, {
                             data: L
                         })
-                    }), M && n.filters.map(function(N) {
+                    }), I && n.filters.map(function(N) {
                         return N.type != "hidden" && t.jsx("div", {
                             children: t.jsx(ee, {
                                 data: N
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         children: t.jsx(R, {
-                            onClick: I,
+                            onClick: k,
                             label: "Filtrar",
                             icon: "filter"
                         })
                     })]
-                }), M && n.filters.map(function(N) {
+                }), I && n.filters.map(function(N) {
                     return N.type == "hidden" && t.jsx("div", {
                         children: t.jsx(ee, {
                             data: N
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function I() {
+    function k() {
         l(!0);
-        var f;
+        var m;
         const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? f = e.data.url + "&" + p : f = e.data.url + "?" + p, q("GET", f, function(M) {
-            a(M), l(!1)
+        e.data.url.indexOf("?") > 0 ? m = e.data.url + "&" + p : m = e.data.url + "?" + p, q("GET", m, function(I) {
+            a(I), l(!1)
         })
     }
 
     function b() {
-        const f = {
-            color: k.colors.primary
+        const m = {
+            color: S.colors.primary
         };
         return e.data.reloadable && t.jsxs("div", {
             align: "center",
             children: [t.jsxs("i", {
                 children: ["Ultima atualização em ", new Date().toLocaleTimeString()]
             }), t.jsx("div", {
                 children: t.jsx(O, {
-                    style: f,
+                    style: m,
                     onClick: p => {
-                        p.preventDefault(), I()
+                        p.preventDefault(), k()
                     },
                     children: "Atualizar agora"
                 })
             })]
         })
     }
 
-    function C() {
+    function E() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [x(), n.bi.map(function(f) {
+            children: [g(), n.bi.map(function(m) {
                 return t.jsx(P, {
                     width: 300,
                     alignItems: "start",
-                    children: f.map(function(p) {
+                    children: m.map(function(p) {
                         return t.jsx("div", {
-                            children: t.jsx(y, {
+                            children: t.jsx(x, {
                                 data: p
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs("div", {
             className: "content",
-            children: [b(), m(), d(), x(), u(), g(), D()]
+            children: [b(), j(), d(), g(), u(), f(), D()]
         })
     }
 
     function T() {
-        window[e.data.id] = () => I();
-        const f = {
+        window[e.data.id] = () => k();
+        const m = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable queryset",
             id: e.data.id,
-            sytle: f,
+            sytle: m,
             children: t.jsxs("form", {
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), i(), C()]
+                }), i(), E()]
             })
         })
     }
     return T()
 }
 
 function ne(e) {
@@ -3703,15 +3724,15 @@
     return t.jsx(he, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function U(e) {
+function G(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         i = {
             type: "value"
         },
         l = {
@@ -3786,55 +3807,55 @@
             option: o
         })
     }
     return u()
 }
 
 function At(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Rt(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Ot(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function _t(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function Ft(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function zt(e) {
-    return t.jsx(U, {
+    return t.jsx(G, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
@@ -3886,15 +3907,15 @@
         return t.jsx(ne, {
             option: r
         })
     }
     return a()
 }
 
-function Pt(e) {
+function Ht(e) {
     function n() {
         var a = {
             series: [{
                 type: "gauge",
                 startAngle: 0,
                 endAngle: 360,
                 min: 0,
@@ -3989,20 +4010,20 @@
                 });
             case "area":
                 return t.jsx(Ot, {
                     headers: e.headers,
                     rows: e.rows
                 });
             case "progress":
-                return t.jsx(Pt, {
+                return t.jsx(Ht, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
-                return t.jsx(U, {
+                return t.jsx(G, {
                     headers: e.headers,
                     rows: e.rows
                 })
         }
     }
 
     function a() {
@@ -4016,15 +4037,15 @@
                 children: e.title
             }), n()]
         })
     }
     return a()
 }
 
-function Ht(e) {
+function Pt(e) {
     F(`
     .statistics .odd {
       background-color: #EEE;
     }
   `);
 
     function n() {
@@ -4032,15 +4053,15 @@
         return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
@@ -4051,15 +4072,15 @@
                                 lineHeight: "2rem",
                                 padding: 5
                             },
                             className: d % 2 == 0 ? "even" : "odd",
                             children: c
                         }, Math.random()) : t.jsx("td", {
                             className: d % 2 == 0 ? "even" : "odd",
-                            children: z(c)
+                            children: W(c)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
@@ -4076,51 +4097,51 @@
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: i
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": E(e.data.title),
+                "data-label": M(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: r.map(g => t.jsx("th", {
+                        children: r.map(f => t.jsx("th", {
                             className: "bold",
                             style: {
                                 textAlign: "left",
                                 padding: 5
                             },
-                            children: g
+                            children: f
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [i.map((g, w) => t.jsx("tr", {
-                        children: g.map((v, D) => D == 0 ? t.jsx("th", {
+                    children: [i.map((f, w) => t.jsx("tr", {
+                        children: f.map((y, D) => D == 0 ? t.jsx("th", {
                             className: w % 2 == 0 ? "even" : "odd",
                             style: {
                                 textAlign: "left",
                                 padding: 5
                             },
-                            children: v
+                            children: y
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
-                            className: (D == g.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (w % 2 == 0 ? "even" : "odd"),
-                            children: z(v)
+                            className: (D == f.length - 1 && r && r[r.length - 1] == "" ? "bold" : "") + " " + (w % 2 == 0 ? "even" : "odd"),
+                            children: W(y)
                         }, Math.random()))
                     }, Math.random())), d.length > 0 && t.jsxs("tr", {
-                        children: [t.jsx("th", {}), d.map(g => t.jsxs("td", {
+                        children: [t.jsx("th", {}), d.map(f => t.jsxs("td", {
                             align: "center",
                             className: "bold",
-                            children: [z(g), " "]
+                            children: [W(f), " "]
                         }, Math.random()))]
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
@@ -4129,15 +4150,15 @@
 function Ut() {
     function e() {
         const l = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
-            backgroundColor: k.colors.success
+            backgroundColor: S.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: l
@@ -4178,43 +4199,43 @@
                 display: d == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 15,
                 paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
-                color: k.colors.primary
+                color: S.colors.primary
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
-                dataLabel: E(l.label),
+                dataLabel: M(l.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [d == 0 && t.jsx(S, {
+                children: [d == 0 && t.jsx(C, {
                     icon: l.icon || "dot-circle",
                     style: s
                 }), l.label]
             })
         }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": E(l.label),
-            children: [d == 0 && t.jsx(S, {
+            "data-label": M(l.label),
+            children: [d == 0 && t.jsx(C, {
                 icon: l.icon || "dot-circle",
                 style: s
-            }), l.label, t.jsx(S, {
+            }), l.label, t.jsx(C, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
@@ -4291,35 +4312,35 @@
             } else console.log("No registered service worker.")
         }).catch(function(l) {
             alert("Erro"), console.error("Service Worker Error", l)
         }) : alert("Push messaging is not supported")
     }
 
     function i() {
-        return t.jsx(S, {
+        return t.jsx(C, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer",
-                color: k.colors.primary
+                color: S.colors.primary
             }
         })
     }
     return i()
 }
 
 function Vt(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
-                backgroundColor: k.colors.primary,
+                backgroundColor: S.colors.primary,
                 color: "white",
                 right: 10,
                 borderRadius: "50%",
                 cursor: "pointer"
             },
             r = {
                 paddingLeft: 14,
@@ -4329,28 +4350,28 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 100
                 },
                 onClick: () => history.back(),
-                children: t.jsx(S, {
+                children: t.jsx(C, {
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
-                children: t.jsx(S, {
+                children: t.jsx(C, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
@@ -4364,26 +4385,26 @@
         const i = {
             minHeight: 400,
             margin: window.innerWidth > 800 ? 20 : 5
         };
         return t.jsx("div", {
             style: i,
             id: "container",
-            children: t.jsx(y, {
+            children: t.jsx(x, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
 function Jt(e) {
     B.useEffect(() => {
         const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), G(o)), window.addEventListener("resize", () => {
+        o && (localStorage.removeItem("message"), z(o)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         })
     }, []);
 
     function a() {
         const o = document.querySelector("aside");
@@ -4415,15 +4436,15 @@
             };
         return e.data.navbar ? t.jsxs("div", {
             style: o,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [e.data.menu && t.jsx(S, {
+                children: [e.data.menu && t.jsx(C, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -4456,95 +4477,95 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Gt, {})
                 }), e.data.navbar.toolbar && window.innerWidth > 800 && e.data.navbar.toolbar.length > 0 && t.jsx("div", {
                     className: "toolbar",
-                    children: e.data.navbar.toolbar.map(function(g) {
+                    children: e.data.navbar.toolbar.map(function(f) {
                         return t.jsx(_, {
-                            data: g,
+                            data: f,
                             primary: !0,
                             compact: !0
                         }, Math.random())
                     })
-                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(g) {
-                    return g.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
+                }), e.data.navbar.actions && e.data.navbar.actions.length > 0 && e.data.navbar.actions.map(function(f) {
+                    return f.url == "/api/login/" && (e.data.navbar.user || document.location.pathname == "/app/login/") ? null : t.jsx("div", {
                         children: t.jsx(_, {
-                            data: g,
+                            data: f,
                             primary: !0
                         }, Math.random())
                     }, Math.random())
-                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(g) {
+                }), e.data.oauth && e.data.oauth.length > 0 && e.data.navbar.user == null && e.data.oauth.map(function(f) {
                     return t.jsx(O, {
-                        href: g.url,
+                        href: f.url,
                         style: {
                             marginRight: 10
                         },
-                        children: g.label
+                        children: f.label
                     }, Math.random())
                 }), e.data.navbar.tools.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
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
-                        children: t.jsx(S, {
+                        children: t.jsx(C, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && e.data.navbar.user && t.jsx("div", {
                     children: t.jsx(Me, {
                         data: h,
                         style: {
                             padding: 10
                         },
-                        onSelect: g => document.location.href = H(g.id)
+                        onSelect: f => document.location.href = U(f.id)
                     })
                 }), e.data.navbar.user && e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(Z, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: E(e.data.navbar.user),
+                        dataLabel: M(e.data.navbar.user),
                         children: t.jsx("img", {
                             src: "/static/images/user.svg",
                             style: {
                                 width: 30,
                                 height: 30,
                                 borderRadius: "50%",
                                 objectFit: "cover",
-                                backgroundColor: k.colors.primary
+                                backgroundColor: S.colors.primary
                             }
                         })
                     })
                 })]
             })]
         }) : null
     }
@@ -4559,38 +4580,44 @@
             },
             children: t.jsx(Ut, {})
         })
     }
 
     function d() {
         const o = {
-                margin: 15
+                margin: 15,
+                display: "flex",
+                justifyContent: "space-between"
             },
             h = {
-                color: k.colors.primary
+                color: S.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
             style: o,
-            children: [t.jsx(O, {
-                href: "/app/dashboard/",
-                style: {
-                    marginRight: 10
-                },
-                children: t.jsx(S, {
-                    icon: "home",
-                    style: h
-                })
-            }), "Área Administrativa"]
+            children: [t.jsxs("div", {
+                children: [t.jsx(O, {
+                    href: "/app/dashboard/",
+                    style: {
+                        marginRight: 10
+                    },
+                    children: t.jsx(C, {
+                        icon: "home",
+                        style: h
+                    })
+                }), "Área Administrativa"]
+            }), t.jsx("div", {
+                children: e.data.navbar.user
+            })]
         })
     }
 
     function c() {
         return t.jsxs("main", {
             style: {
-                flexGrow: 6
+                width: "100vw"
             },
             children: [d(), t.jsx($t, {
                 data: e.data.content
             }), t.jsx("footer", {
                 children: s()
             }), t.jsx(Vt, {})]
         })
@@ -4621,127 +4648,126 @@
 
     function u() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
                 children: i()
             }), t.jsxs("div", {
                 style: {
-                    overflowX: "hide",
                     width: "100%",
                     display: "flex",
-                    overflow: "hidden",
                     minHeight: window.innerHeight - 70
                 },
                 children: [l(), c()]
             })]
         })
     }
     return u()
 }
 
 function Yt(e) {
     var n = null,
         a = null,
         r = null,
-        i = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
-        l = {
+        i = !1,
+        l = null,
+        d = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
+        c = {
             constraints: {
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
                 offerToReceiveAudio: 1,
                 offerToReceiveVideo: 1
             },
-            sdpTransform: m => m.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+            sdpTransform: v => v.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
-    B.useEffect(() => {
-        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(m) {
-            document.getElementById("callerid").innerHTML = e.data.caller
-        }), n.on("call", function(m) {
-            i({
-                video: {
-                    width: {
-                        exact: 320
-                    },
-                    height: {
-                        exact: 240
-                    }
+    B.useEffect(() => (n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(v) {
+        document.getElementById("callerid").innerHTML = e.data.caller, D()
+    }), n.on("call", function(v) {
+        d({
+            video: {
+                width: {
+                    exact: 320
                 },
-                audio: !0
-            }, function(j) {
-                a = j;
-                var x = document.getElementById("video2");
-                x.addEventListener("loadedmetadata", function(I) {
-                    x.style.width = this.videoWidth / 4 + "px", x.style.height = this.videoHeight / 4 + "px", x.style.marginLeft = -this.videoWidth / 4 + "px", x.style.visibility = "visible"
-                }, !1), x.srcObject = a, m.answer(j), m.on("stream", function(I) {
-                    r = I, document.getElementById("video1").srcObject = r
-                }), m.on("close", function() {
-                    s()
-                }), n.on("error", function(I) {
-                    s()
-                })
-            }, function(j) {
-                console.log("Failed to get local stream", j)
+                height: {
+                    exact: 240
+                }
+            },
+            audio: !0
+        }, function(g) {
+            a = g;
+            var k = document.getElementById("video2");
+            k.addEventListener("loadedmetadata", function(b) {
+                k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
+            }, !1), k.srcObject = a, v.answer(g), v.on("stream", function(b) {
+                r = b, document.getElementById("video1").srcObject = r, i = !0
+            }), v.on("close", function() {
+                console.log("Closed!"), i = !1
+            }), n.on("error", function(b) {
+                console.log("Error!"), i = !1
             })
-        }), n.on("error", function(m) {
-            m.type == "browser-incompatible" ? alert("Navegador incompatível.") : m.type == "invalid-id" ? alert("Usuário inexistente.") : m.type == "network" ? alert("Problema na conexão do usuário.") : m.type == "peer-unavailable" && alert("Usuário indisponível.")
+        }, function(g) {
+            console.log("Failed to get local stream", g)
         })
-    }, []);
+    }), n.on("error", function(v) {
+        v.type == "browser-incompatible" ? alert("Navegador incompatível.") : v.type == "invalid-id" ? alert("Usuário inexistente.") : v.type == "network" ? alert("Problema na conexão do usuário.") : v.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
+    }), l = setInterval(function() {
+        i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), D())
+    }, 15e3), function() {
+        clearInterval(l), u(), z("Desconectado!")
+    }), []);
 
-    function d() {
-        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video")
-    }
-
-    function c() {
+    function s() {
         h(a, "audio"), h(a, "video"), h(r, "audio"), h(r, "video")
     }
 
-    function s() {
-        u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
+    function u() {
+        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video"), a = null, r = null;
+        const v = document.getElementById("video1"),
+            g = document.getElementById("video2");
+        v && (v.srcObject = null), g && (g.srcObject = null), console.log("Stopped!")
     }
 
-    function u(m, j) {
-        m != null && m.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && x.stop()
+    function o(v, g) {
+        v != null && v.getTracks().forEach(k => {
+            k.kind === g && k.stop()
         })
     }
 
-    function o(m, j) {
-        m != null && m.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && (x.enabled = !1)
+    function h(v, g) {
+        v != null && v.getTracks().forEach(k => {
+            k.readyState == "live" && k.kind === g && (k.enabled = !1)
         })
     }
 
-    function h(m, j) {
-        m != null && m.getTracks().forEach(x => {
-            x.readyState == "live" && x.kind === j && (x.enabled = !0)
-        })
+    function f() {
+        var v = document.getElementById("video1");
+        v.style.width = v.getClientRects()[0].width + 100 + "px"
     }
 
-    function g() {
-        var m = document.getElementById("video1");
-        m.style.width == "" ? m.style.width = "400px" : m.style.width = ""
+    function w() {
+        var v = document.getElementById("video1");
+        v.style.width = v.getClientRects()[0].width - 100 + "px"
     }
 
-    function w() {
-        var m = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, l);
-        m.on("stream", function(j) {
-            r = j, document.getElementById("video1").srcObject = r
-        }), m.on("close", function() {
-            s()
-        }), n.on("error", function(j) {
-            s()
+    function y() {
+        var v = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, c);
+        v.on("stream", function(g) {
+            r = g, document.getElementById("video1").srcObject = r, i = !0
+        }), v.on("close", function() {
+            console.log("Closed!"), i = !1
+        }), n.on("error", function(g) {
+            console.log("Error!"), i = !1
         })
     }
 
-    function v() {
-        if (a != null && r == null) return w();
-        if (a != null && r != null) return c();
-        i({
+    function D() {
+        if (a != null && !i) return y();
+        d({
             video: {
                 width: {
                     exact: 320
                 },
                 height: {
                     exact: 240
                 }
@@ -4752,89 +4778,89 @@
                 echoCancellation: !1,
                 latency: 0,
                 noiseSuppression: !1,
                 sampleRate: 48e3,
                 sampleSize: 16,
                 volume: 1
             }
-        }, function(m) {
-            a = m;
-            var j = document.getElementById("video2");
-            j.addEventListener("loadedmetadata", function(x) {
-                j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
-            }, !1), j.srcObject = a, w()
-        }, function(m) {
+        }, function(v) {
+            a = v;
+            var g = document.getElementById("video2");
+            g.addEventListener("loadedmetadata", function(k) {
+                g.style.width = this.videoWidth / 4 + "px", g.style.height = this.videoHeight / 4 + "px", g.style.marginLeft = -this.videoWidth / 4 + "px", g.style.visibility = "visible"
+            }, !1), g.srcObject = a, y()
+        }, function(v) {
             alert("Failed to get local stream.")
         })
     }
 
-    function D() {
-        var m = {
+    function j() {
+        var v = {
                 width: "fit-content",
                 margin: "auto"
             },
-            j = {
+            g = {
                 position: "absolute",
                 color: "white",
                 padding: "5px"
             },
-            x = {
+            k = {
                 color: "white",
                 backgroundColor: "black",
                 padding: 2
             },
-            I = {
+            b = {
                 position: "absolute",
                 marginTop: "-30px"
             },
-            b = {
+            E = {
                 backgroundColor: "black"
             },
-            C = {
+            T = {
                 visibility: "hidden",
                 width: "0px"
             };
         return t.jsxs("div", {
-            style: m,
+            style: v,
             children: [t.jsx("div", {
                 id: "callerid",
-                style: j
+                style: g
             }), t.jsx("video", {
                 id: "video1",
-                style: b,
+                style: E,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsx("video", {
                 id: "video2",
-                style: C,
+                style: T,
                 playsInline: !0,
                 autoPlay: !0
             }), t.jsxs("div", {
-                style: I,
-                children: [t.jsx(S, {
-                    style: x,
-                    onClick: v,
-                    icon: "play"
-                }), t.jsx(S, {
-                    style: x,
-                    onClick: d,
-                    icon: "pause"
-                }), t.jsx(S, {
-                    style: x,
+                style: b,
+                children: [t.jsx(C, {
+                    style: k,
                     onClick: s,
+                    icon: "pause"
+                }), t.jsx(C, {
+                    style: k,
+                    onClick: u,
                     icon: "stop"
-                }), t.jsx(S, {
-                    style: x,
-                    onClick: g,
-                    icon: "maximize"
+                }), t.jsx(C, {
+                    style: k,
+                    onClick: f,
+                    icon: "search-plus"
+                }), t.jsx(C, {
+                    style: k,
+                    onClick: w,
+                    icon: "search-minus"
                 })]
             })]
         })
     }
-    return D()
+    return j()
 }
 
 function Qt(e) {
     const n = {
         color: e.data.color
     };
 
@@ -4846,88 +4872,88 @@
     }
     return a()
 }
 var te, me = {};
 const Xt = "/api/application/",
     we = localStorage.getItem("application");
 
-function y(e) {
+function x(e) {
     const n = me[e.data.type];
     return n ? Te.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-y.register = function(e, n) {
+x.register = function(e, n) {
     me[n.toLowerCase()] = e
 };
-y.render = function(e) {
+x.render = function(e) {
     te = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/home/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-y.register(ht, "Counter");
-y.register(Tt, "Form");
-y.register(Nt, "QuerySet");
-y.register(Ge, "Fieldset");
-y.register($, "Field");
-y.register(Je, "Object");
-y.register(Ye, "Section");
-y.register(Xe, "Group");
-y.register(Ht, "Statistics");
-y.register(et, "Image");
-y.register(Ze, "Banner");
-y.register(tt, "Map");
-y.register(nt, "Steps");
-y.register(st, "QrCode");
-y.register(Se, "Badge");
-y.register(rt, "Status");
-y.register(at, "Progress");
-y.register(Ie, "Color");
-y.register(it, "Boxes");
-y.register(ct, "Indicators");
-y.register(lt, "Shell");
-y.register(ot, "FileLink");
-y.register(dt, "FilePreview");
-y.register(Le, "Response");
-y.register(Jt, "Application");
-y.register(De, "IconSet");
-y.register(ut, "Grid");
-y.register(Pe, "Rows");
-y.register(He, "Cards");
-y.register(Ue, "Timeline");
-y.register(Ce, "Scheduler");
-y.register(Yt, "WebConf");
-y.register(Qt, "Text");
+x.register(ht, "Counter");
+x.register(Tt, "Form");
+x.register(Nt, "QuerySet");
+x.register(Ge, "Fieldset");
+x.register($, "Field");
+x.register(Je, "Object");
+x.register(Ye, "Section");
+x.register(Xe, "Group");
+x.register(Pt, "Statistics");
+x.register(et, "Image");
+x.register(Ze, "Banner");
+x.register(tt, "Map");
+x.register(nt, "Steps");
+x.register(st, "QrCode");
+x.register(Se, "Badge");
+x.register(rt, "Status");
+x.register(at, "Progress");
+x.register(Ie, "Color");
+x.register(it, "Boxes");
+x.register(ct, "Indicators");
+x.register(lt, "Shell");
+x.register(ot, "FileLink");
+x.register(dt, "FilePreview");
+x.register(Le, "Response");
+x.register(Jt, "Application");
+x.register(De, "IconSet");
+x.register(ut, "Grid");
+x.register(He, "Rows");
+x.register(Pe, "Cards");
+x.register(Ue, "Timeline");
+x.register(Ce, "Scheduler");
+x.register(Yt, "WebConf");
+x.register(Qt, "Text");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
     me[n] ? q("GET", A(e), function(a) {
-        te.render(t.jsx(y, {
+        te.render(t.jsx(x, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
     }, "", e), we ? (window.application = JSON.parse(we), q("GET", A(e), function(a) {
-        window.application.content = a, te.render(t.jsx(y, {
+        window.application.content = a, te.render(t.jsx(x, {
             data: window.application
         }, Math.random()))
     })) : q("GET", Xt, function(r) {
         window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(i) {
-            window.application.content = i, te.render(t.jsx(y, {
+            window.application.content = i, te.render(t.jsx(x, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
     }, "", e), q("GET", A(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-y.render(W.createRoot(document.getElementById("root")));
+x.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.3.4/slth/static/js/vanilla-masker.js` & `pyslth-0.3.6/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/static/js/vanilla-masker.min.js` & `pyslth-0.3.6/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/statistics.py` & `pyslth-0.3.6/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/templates/index.html` & `pyslth-0.3.6/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/templates/service-worker.js` & `pyslth-0.3.6/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/tests.py` & `pyslth-0.3.6/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/urls.py` & `pyslth-0.3.6/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/utils.py` & `pyslth-0.3.6/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.3.4/slth/views.py` & `pyslth-0.3.6/slth/views.py`

 * *Files identical despite different names*

