# Comparing `tmp/tahrir-1.0.0.tar.gz` & `tmp/tahrir-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir-1.0.0.tar", max compression
+gzip compressed data, was "tahrir-1.1.0.tar", max compression
```

## Comparing `tahrir-1.0.0.tar` & `tahrir-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    34917 2022-06-27 10:19:53.000000 tahrir-1.0.0/LICENSE
--rw-r--r--   0        0        0     2699 2024-04-22 10:23:44.598830 tahrir-1.0.0/README.md
--rw-r--r--   0        0        0     2073 2024-04-22 15:22:50.800616 tahrir-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6091 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/__init__.py
--rw-r--r--   0        0        0     1522 2024-04-11 08:06:57.238771 tahrir-1.0.0/tahrir/app.py
--rw-r--r--   0        0        0      828 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/auth/__init__.py
--rw-r--r--   0        0        0      251 2024-04-11 08:06:57.238771 tahrir-1.0.0/tahrir/auth/constants.py
--rw-r--r--   0        0        0     5775 2024-04-11 08:06:57.238771 tahrir-1.0.0/tahrir/auth/fedora.py
--rw-r--r--   0        0        0     2652 2024-04-11 08:06:57.239771 tahrir-1.0.0/tahrir/auth/oauth.py
--rw-r--r--   0        0        0     3598 2024-04-11 08:06:57.239771 tahrir-1.0.0/tahrir/auth/oauth_1.py
--rw-r--r--   0        0        0     2294 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/auth/utils.py
--rw-r--r--   0        0        0     1906 2024-04-11 08:06:57.239771 tahrir-1.0.0/tahrir/auth/views.py
--rw-r--r--   0        0        0     1506 2024-04-11 08:06:57.239771 tahrir-1.0.0/tahrir/events.py
--rw-r--r--   0        0        0     1061 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/notifications.py
--rw-r--r--   0        0        0      152 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/sitedocs/about.rst
--rw-r--r--   0        0        0      348 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/sitedocs/footer.rst
--rw-r--r--   0        0        0     2682 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/css/monokai.css
--rw-r--r--   0        0        0     6692 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/static/css/tahrir.css
--rw-r--r--   0        0        0    19275 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/css/unsemantic-grid-mobile.css
--rw-r--r--   0        0        0    64230 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css
--rw-r--r--   0        0        0    42765 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/css/unsemantic-grid-responsive.css
--rw-r--r--   0        0        0   337688 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/404.png
--rw-r--r--   0        0        0   353383 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/404.svg
--rw-r--r--   0        0        0   411482 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/500.png
--rw-r--r--   0        0        0   374146 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/500.svg
--rw-r--r--   0        0        0     9455 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/badge.png
--rw-r--r--   0        0        0     1695 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/badge_bullet.png
--rw-r--r--   0        0        0     3124 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/badge_bullet_fedora.png
--rw-r--r--   0        0        0    10473 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/badger_avatar.png
--rw-r--r--   0        0        0    21187 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/badger_avatar.svg
--rw-r--r--   0        0        0      645 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/favicon.ico
--rw-r--r--   0        0        0    71006 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/fedora_badges.png
--rw-r--r--   0        0        0    13083 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/fedora_badges_small.png
--rw-r--r--   0        0        0     9380 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/img/fedora_logo.png
--rw-r--r--   0        0        0     3534 2024-04-22 10:23:44.599830 tahrir-1.0.0/tahrir/static/js/builder.js
--rw-r--r--   0        0        0     8380 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/static/js/favico-0.3.4.min.js
--rw-r--r--   0        0        0    86927 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/js/jquery-3.3.1.min.js
--rw-r--r--   0        0        0      619 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/js/social.js
--rw-r--r--   0        0        0    95029 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/js/thingiview/Three.js
--rw-r--r--   0        0        0     3601 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/static/js/thingiview/binaryReader.js
--rw-r--r--   0        0        0     1457 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/js/thingiview/plane.js
--rw-r--r--   0        0        0     3801 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/static/js/thingiview/stats.js
--rw-r--r--   0        0        0    10202 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/static/js/thingiview/thingiloader.js
--rw-r--r--   0        0        0    26581 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/static/js/thingiview/thingiview.js
--rw-r--r--   0        0        0      610 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/404.mak
--rw-r--r--   0        0        0      616 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/500.mak
--rw-r--r--   0        0        0        0 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/__init__.py
--rw-r--r--   0        0        0      154 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/about.mak
--rw-r--r--   0        0        0    12097 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/admin.mak
--rw-r--r--   0        0        0      525 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/assertion_widget.mak
--rw-r--r--   0        0        0     7160 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/badge-base.mak
--rw-r--r--   0        0        0       96 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/badge.mak
--rw-r--r--   0        0        0      156 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/badge_full.mak
--rw-r--r--   0        0        0     3938 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/builder.mak
--rw-r--r--   0        0        0     3083 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/diff.mak
--rw-r--r--   0        0        0     5527 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/explore.mak
--rw-r--r--   0        0        0     2781 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/explore_badges.mak
--rw-r--r--   0        0        0     2596 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/functions.mak
--rw-r--r--   0        0        0     2680 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/index.mak
--rw-r--r--   0        0        0     3064 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/leaderboard.mak
--rw-r--r--   0        0        0      402 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/login.mak
--rw-r--r--   0        0        0     6654 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/master.mak
--rw-r--r--   0        0        0     1291 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/report.mak
--rw-r--r--   0        0        0      764 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/tags.mak
--rw-r--r--   0        0        0     1210 2022-06-27 10:19:53.000000 tahrir-1.0.0/tahrir/templates/thingiview.mak
--rw-r--r--   0        0        0     8867 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/templates/user.mak
--rw-r--r--   0        0        0     4199 2024-04-22 15:22:41.635537 tahrir-1.0.0/tahrir/utils.py
--rw-r--r--   0        0        0    53825 2024-04-22 10:23:44.600830 tahrir-1.0.0/tahrir/views.py
--rw-r--r--   0        0        0      652 2024-04-11 08:06:57.239771 tahrir-1.0.0/tahrir/widgets.py
--rw-r--r--   0        0        0        0 2022-06-27 10:19:53.000000 tahrir-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      758 2024-04-22 10:23:44.601830 tahrir-1.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 tahrir-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34917 2024-05-19 07:32:48.736635 tahrir-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2699 2024-05-19 07:32:48.736635 tahrir-1.1.0/README.md
+-rw-r--r--   0        0        0     2067 2024-05-19 07:32:48.740635 tahrir-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6089 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/app.py
+-rw-r--r--   0        0        0      828 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/constants.py
+-rw-r--r--   0        0        0     5775 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/fedora.py
+-rw-r--r--   0        0        0     2652 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/oauth.py
+-rw-r--r--   0        0        0     3598 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/oauth_1.py
+-rw-r--r--   0        0        0     2497 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/utils.py
+-rw-r--r--   0        0        0     1906 2024-05-19 07:32:48.740635 tahrir-1.1.0/tahrir/auth/views.py
+-rw-r--r--   0        0        0     1506 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/events.py
+-rw-r--r--   0        0        0     1061 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/notifications.py
+-rw-r--r--   0        0        0      152 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/sitedocs/about.rst
+-rw-r--r--   0        0        0      348 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/sitedocs/footer.rst
+-rw-r--r--   0        0        0     2682 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/monokai.css
+-rw-r--r--   0        0        0     6692 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/tahrir.css
+-rw-r--r--   0        0        0    19275 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-mobile.css
+-rw-r--r--   0        0        0    64230 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css
+-rw-r--r--   0        0        0    42765 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive.css
+-rw-r--r--   0        0        0   337688 2024-05-19 07:32:48.744635 tahrir-1.1.0/tahrir/static/img/404.png
+-rw-r--r--   0        0        0   353383 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/404.svg
+-rw-r--r--   0        0        0   411482 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/500.png
+-rw-r--r--   0        0        0   374146 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/500.svg
+-rw-r--r--   0        0        0     9455 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge.png
+-rw-r--r--   0        0        0     1695 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge_bullet.png
+-rw-r--r--   0        0        0     3124 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badge_bullet_fedora.png
+-rw-r--r--   0        0        0    10473 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badger_avatar.png
+-rw-r--r--   0        0        0    21187 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/badger_avatar.svg
+-rw-r--r--   0        0        0      645 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/favicon.ico
+-rw-r--r--   0        0        0    71006 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_badges.png
+-rw-r--r--   0        0        0    13083 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_badges_small.png
+-rw-r--r--   0        0        0     9380 2024-05-19 07:32:48.748635 tahrir-1.1.0/tahrir/static/img/fedora_logo.png
+-rw-r--r--   0        0        0     3534 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/builder.js
+-rw-r--r--   0        0        0     8380 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/favico-0.3.4.min.js
+-rw-r--r--   0        0        0    86927 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/jquery-3.3.1.min.js
+-rw-r--r--   0        0        0      619 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/social.js
+-rw-r--r--   0        0        0    95029 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/Three.js
+-rw-r--r--   0        0        0     3601 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/binaryReader.js
+-rw-r--r--   0        0        0     1457 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/plane.js
+-rw-r--r--   0        0        0     3801 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/stats.js
+-rw-r--r--   0        0        0    10202 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/thingiloader.js
+-rw-r--r--   0        0        0    26581 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/static/js/thingiview/thingiview.js
+-rw-r--r--   0        0        0      610 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/404.mak
+-rw-r--r--   0        0        0      616 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/500.mak
+-rw-r--r--   0        0        0        0 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/about.mak
+-rw-r--r--   0        0        0    12097 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/admin.mak
+-rw-r--r--   0        0        0      525 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/assertion_widget.mak
+-rw-r--r--   0        0        0     7160 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge-base.mak
+-rw-r--r--   0        0        0       96 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge.mak
+-rw-r--r--   0        0        0      156 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/badge_full.mak
+-rw-r--r--   0        0        0     3938 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/builder.mak
+-rw-r--r--   0        0        0     3083 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/diff.mak
+-rw-r--r--   0        0        0     5527 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/explore.mak
+-rw-r--r--   0        0        0     2781 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/explore_badges.mak
+-rw-r--r--   0        0        0     2597 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/functions.mak
+-rw-r--r--   0        0        0     2680 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/index.mak
+-rw-r--r--   0        0        0     3064 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/leaderboard.mak
+-rw-r--r--   0        0        0      402 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/login.mak
+-rw-r--r--   0        0        0     6654 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/master.mak
+-rw-r--r--   0        0        0     1291 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/report.mak
+-rw-r--r--   0        0        0      764 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/tags.mak
+-rw-r--r--   0        0        0     1210 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/thingiview.mak
+-rw-r--r--   0        0        0     8867 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/templates/user.mak
+-rw-r--r--   0        0        0     4199 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/utils.py
+-rw-r--r--   0        0        0    53811 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/views.py
+-rw-r--r--   0        0        0      652 2024-05-19 07:32:48.752635 tahrir-1.1.0/tahrir/widgets.py
+-rw-r--r--   0        0        0        0 2024-05-19 07:32:48.752635 tahrir-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-19 07:32:48.752635 tahrir-1.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4469 1970-01-01 00:00:00.000000 tahrir-1.1.0/PKG-INFO
```

### Comparing `tahrir-1.0.0/LICENSE` & `tahrir-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/README.md` & `tahrir-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/pyproject.toml` & `tahrir-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahrir"
-version = "1.0.0"
+version = "1.1.0"
 description = "A pyramid app for issuing your own Open Badges"
 
 license = "AGPLv3+ with additional permission"
 
 authors = [
   "Ralph Bean <rbean@redhat.com>",
   "Fedora Infrastructure <admin@fedoraproject.org>",
@@ -32,15 +32,15 @@
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 pyramid = "^2.0.2"
 pyramid-mako = "^1.1.0"
-tahrir-api = "^1.0.0"
+tahrir-api = "^1.1.0"
 sqlalchemy = "^2.0.29"
 pyramid-tm = "^2.5"
 qrcode = "^7.4.2"
 dogpile-cache = "^1.3.2"
 docutils = "^0.20.1 || ^0.21.0"
 python-dateutil = "^2.9.0.post0"
 feedgen = "^1.0.0"
@@ -92,10 +92,11 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
-select = ["E", "F", "W", "I", "B", "UP"]
 line-length = 100
-target-version = "py39"
+
+[tool.ruff.lint]
+select = ["E", "F", "W", "I", "B", "UP"]
```

### Comparing `tahrir-1.0.0/tahrir/__init__.py` & `tahrir-1.1.0/tahrir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,34 +39,34 @@
         "tahrir.title",
         "tahrir.base_url",
     ]
 
     # validate the config
     for key in required_keys:
         if key not in settings:
-            raise ValueError("%s required in settings." % key)
+            raise ValueError(f"{key} required in settings.")
 
     # Make data dir if it doesn't already exist.
     settings["tahrir.pngs.uri"] = os.path.abspath(settings["tahrir.pngs.uri"])
     if not os.path.exists(settings["tahrir.pngs.uri"]):
         os.makedirs(settings["tahrir.pngs.uri"])
 
     # Load secret stuff from secret.ini.
     try:
         default_path = os.path.abspath("secret.ini")
         secret_path = settings.get("tahrir.secret_config_path", default_path)
         # TODO: There is a better way to log this message than print.
-        print("Reading secrets from %r" % secret_path)
+        print(f"Reading secrets from {secret_path!r}")
         parser = ConfigParser()
         parser.read(secret_path)
         secret_config = dict(parser.items("tahrir"))
         settings.update(secret_config)
     except Exception as e:
         # TODO: There is a better way to log this message than print.
-        print("Failed to load secret.ini.  Reason: %r" % str(e))
+        print(f"Failed to load secret.ini.  Reason: {str(e)!r}")
 
     authn_policy = AuthTktAuthenticationPolicy(
         secret=settings["authnsecret"],
         callback=groupfinder,  # groupfinder callback checks for admin privs
         hashalg="sha512",  # because md5 is deprecated
         secure=asbool(settings.get("tahrir.secure_cookies", True)),
         http_only=asbool(settings.get("tahrir.httponly_cookies", True)),
```

### Comparing `tahrir-1.0.0/tahrir/app.py` & `tahrir-1.1.0/tahrir/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __getitem__(self, key):
         for assertion in self.badge.assertions:
             if assertion.recipient == key:
                 assertion.__parent__ = self
                 assertion.__name__ = assertion.recipient
                 return assertion
         else:
-            raise KeyError("Assertion %r not found." % key)
+            raise KeyError(f"Assertion {key!r} not found.")
 
 
 class InvitationApp:
     __name__ = "invitations"
 
     def __init__(self, request):
         self.request = request
@@ -50,15 +50,15 @@
             resource.__parent__ = self
             return resource
 
         # else
 
         badge = self.request.db.get_badge(key)
         if not badge:
-            raise KeyError("No such badge %r" % key)
+            raise KeyError(f"No such badge {key!r}")
         resource = AssertionApp(badge=badge)
         resource.__parent__ = self
         return resource
 
 
 def get_root(request):
     return RootApp(request=request)
```

### Comparing `tahrir-1.0.0/tahrir/auth/__init__.py` & `tahrir-1.1.0/tahrir/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/auth/fedora.py` & `tahrir-1.1.0/tahrir/auth/fedora.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/auth/oauth.py` & `tahrir-1.1.0/tahrir/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/auth/oauth_1.py` & `tahrir-1.1.0/tahrir/auth/oauth_1.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/auth/utils.py` & `tahrir-1.1.0/tahrir/auth/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,30 @@
     userinfo = request.registry.oidc.fedora.userinfo(token={"access_token": access_token})
     if "error" in userinfo:
         raise InvalidTokenError(description=userinfo["error_description"])
 
     nickname = userinfo["nickname"]
     if asbool(settings.get("tahrir.use_openid_email")):
         email = userinfo["email"]
+        avatar = None
     else:
         email = nickname + settings.get("tahrir.email_domain")
+        avatar = userinfo["email"]
 
     # Keep adding underscores until we get a default nickname
     # that isn't already used.
     while request.db.get_person(nickname=nickname):
         nickname += "_"
 
-    if not request.db.get_person(person_email=email):
-        request.db.add_person(email=email, nickname=nickname)
+    existing = request.db.get_person(person_email=email)
+    if not existing:
+        request.db.add_person(email=email, nickname=nickname, avatar=avatar)
+    elif existing._avatar != avatar:
+        existing._avatar = avatar
+        request.db.session.commit()
 
     # Note that they have logged in if we are installed with a newer version of
     # the db API that supports this.
     if hasattr(request.db, "note_login"):
         request.db.note_login(person_email=email)
 
     headers = remember(request, email)
```

### Comparing `tahrir-1.0.0/tahrir/auth/views.py` & `tahrir-1.1.0/tahrir/auth/views.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/events.py` & `tahrir-1.1.0/tahrir/events.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/notifications.py` & `tahrir-1.1.0/tahrir/notifications.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/css/monokai.css` & `tahrir-1.1.0/tahrir/static/css/monokai.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/css/tahrir.css` & `tahrir-1.1.0/tahrir/static/css/tahrir.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/css/unsemantic-grid-mobile.css` & `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-mobile.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css` & `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive-tablet.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/css/unsemantic-grid-responsive.css` & `tahrir-1.1.0/tahrir/static/css/unsemantic-grid-responsive.css`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/404.png` & `tahrir-1.1.0/tahrir/static/img/404.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/404.svg` & `tahrir-1.1.0/tahrir/static/img/404.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/500.png` & `tahrir-1.1.0/tahrir/static/img/500.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/500.svg` & `tahrir-1.1.0/tahrir/static/img/500.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/badge.png` & `tahrir-1.1.0/tahrir/static/img/badge.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/badge_bullet.png` & `tahrir-1.1.0/tahrir/static/img/badge_bullet.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/badge_bullet_fedora.png` & `tahrir-1.1.0/tahrir/static/img/badge_bullet_fedora.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/badger_avatar.png` & `tahrir-1.1.0/tahrir/static/img/badger_avatar.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/badger_avatar.svg` & `tahrir-1.1.0/tahrir/static/img/badger_avatar.svg`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/favicon.ico` & `tahrir-1.1.0/tahrir/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/fedora_badges.png` & `tahrir-1.1.0/tahrir/static/img/fedora_badges.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/fedora_badges_small.png` & `tahrir-1.1.0/tahrir/static/img/fedora_badges_small.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/img/fedora_logo.png` & `tahrir-1.1.0/tahrir/static/img/fedora_logo.png`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/builder.js` & `tahrir-1.1.0/tahrir/static/js/builder.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/favico-0.3.4.min.js` & `tahrir-1.1.0/tahrir/static/js/favico-0.3.4.min.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/jquery-3.3.1.min.js` & `tahrir-1.1.0/tahrir/static/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/social.js` & `tahrir-1.1.0/tahrir/static/js/social.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/Three.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/Three.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/binaryReader.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/binaryReader.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/plane.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/plane.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/stats.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/stats.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/thingiloader.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/thingiloader.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/static/js/thingiview/thingiview.js` & `tahrir-1.1.0/tahrir/static/js/thingiview/thingiview.js`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/404.mak` & `tahrir-1.1.0/tahrir/templates/404.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/500.mak` & `tahrir-1.1.0/tahrir/templates/500.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/admin.mak` & `tahrir-1.1.0/tahrir/templates/admin.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/assertion_widget.mak` & `tahrir-1.1.0/tahrir/templates/assertion_widget.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/badge-base.mak` & `tahrir-1.1.0/tahrir/templates/badge-base.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/builder.mak` & `tahrir-1.1.0/tahrir/templates/builder.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/diff.mak` & `tahrir-1.1.0/tahrir/templates/diff.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/explore.mak` & `tahrir-1.1.0/tahrir/templates/explore.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/explore_badges.mak` & `tahrir-1.1.0/tahrir/templates/explore_badges.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/functions.mak` & `tahrir-1.1.0/tahrir/templates/functions.mak`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <%def name="avatar_thumbnail(person, size, cell_width, tooltip=True)">
 	<div class="grid-${cell_width} thumbnail-container">
 		<div class="thumbnail thumbnail-${size}">
       % if tooltip:
 			<span class="tooltip tooltip-${size}" data-tooltip="${person.nickname}">
       % endif
 				<a href="${request.route_url('user', id=person.nickname or person.id)}">
-					<img property="foaf:img schema:image" src="${person.email | as_avatar(size)}" />
+					<img property="foaf:img schema:image" src="${person.avatar | as_avatar(size)}" />
 				</a>
       % if tooltip:
 			</span>
       % endif
 		</div>
 	</div>
 </%def>
```

### Comparing `tahrir-1.0.0/tahrir/templates/index.mak` & `tahrir-1.1.0/tahrir/templates/index.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/leaderboard.mak` & `tahrir-1.1.0/tahrir/templates/leaderboard.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/master.mak` & `tahrir-1.1.0/tahrir/templates/master.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/report.mak` & `tahrir-1.1.0/tahrir/templates/report.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/tags.mak` & `tahrir-1.1.0/tahrir/templates/tags.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/thingiview.mak` & `tahrir-1.1.0/tahrir/templates/thingiview.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/templates/user.mak` & `tahrir-1.1.0/tahrir/templates/user.mak`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/utils.py` & `tahrir-1.1.0/tahrir/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tahrir/views.py` & `tahrir-1.1.0/tahrir/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import os
 import random
 import types
 from datetime import date, datetime, timedelta, timezone
 from decimal import ROUND_UP, Decimal
-from io import StringIO
+from io import BytesIO
 
 import docutils.examples
 import markupsafe
 import qrcode as qrcode_module
 import sqlalchemy as sa
 import tahrir_api.model as m
 from feedgen.feed import FeedGenerator
@@ -102,26 +102,26 @@
     agent = request.db.get_person(request.authenticated_userid)
     if not agent:
         raise HTTPForbidden()
 
     badge_id = request.POST.get("badge_id")
     badge = request.db.get_badge(badge_id)
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     if not badge.authorized(agent):
-        raise HTTPForbidden("Unauthorized for %r" % badge_id)
+        raise HTTPForbidden(f"Unauthorized for {badge_id!r}")
 
     nickname = request.POST.get("nickname")
     user = request.db.get_person(nickname=nickname)
     if not user:
-        raise HTTPNotFound("No such user %r" % nickname)
+        raise HTTPNotFound(f"No such user {nickname!r}")
 
     if user.opt_out:
-        raise HTTPNotFound("No such user %r" % nickname)
+        raise HTTPNotFound(f"No such user {nickname!r}")
 
     # OK
     request.db.add_assertion(badge.id, user.email, None)
 
     return HTTPFound(location=request.route_url("badge_rss", id=badge.id))
 
 
@@ -137,18 +137,18 @@
     agent = request.db.get_person(request.authenticated_userid)
     if not agent:
         raise HTTPForbidden()
 
     badge_id = request.POST.get("badge_id")
     badge = request.db.get_badge(badge_id)
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     if not badge.authorized(agent):
-        raise HTTPForbidden("Unauthorized for %r" % badge_id)
+        raise HTTPForbidden(f"Unauthorized for {badge_id!r}")
 
     try:
         fmt = "%Y-%m-%d %H:%M"
         expires_on = datetime.strptime(request.POST.get("expires-on"), fmt)
     except ValueError:
         expires_on = None  # Will default to 1 hour from now
 
@@ -170,15 +170,15 @@
     agent = request.db.get_person(request.authenticated_userid)
     if not agent:
         raise HTTPForbidden()
 
     badge_id = request.POST.get("badge_id")
     badge = request.db.get_badge(badge_id)
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     tags = request.POST.get("tags", "")
     new_tags = [tag.strip() for tag in tags.strip().split(",") if tag.strip()]
     originals = [tag.strip() for tag in badge.tags.split(",") if tag.strip()]
     badge.tags = ",".join(set(originals + new_tags)) + ","
     request.db.session.flush()
 
@@ -256,15 +256,15 @@
             email = request.POST.get("person-email")
             if not request.db.person_exists(email=email):
                 request.db.add_person(
                     email,
                     nickname=request.POST.get("person-nickname"),
                 )
                 request.session.flash(
-                    "You added a person with email %s" % request.POST.get("person-email")
+                    "You added a person with email {}".format(request.POST.get("person-email"))
                 )
             else:
                 request.session.flash(f"Person with email {email} already exists.")
         elif request.POST.get("add-badge"):
             name = request.POST.get("badge-name")
             idx = convert_name_to_id(name)
             if not request.db.badge_exists(idx):
@@ -273,15 +273,15 @@
                     name,
                     request.POST.get("badge-image"),
                     request.POST.get("badge-description"),
                     request.POST.get("badge-criteria"),
                     request.POST.get("badge-issuer"),
                     request.POST.get("badge-tags"),
                 )
-                request.session.flash("You added a badge with name %s" % name)
+                request.session.flash(f"You added a badge with name {name}")
             else:
                 request.session.flash(f"Badge with id {idx} already exists.")
 
         elif request.POST.get("add-invitation"):
             # Add an Invitation to the DB.
             try:
                 created_on = datetime.strptime(
@@ -300,26 +300,28 @@
             request.db.add_invitation(
                 request.POST.get("invitation-badge-id"),
                 created_on=created_on,
                 expires_on=expires_on,
                 created_by_email=request.POST.get("invitation-issuer-email"),
             )
             request.session.flash(
-                "You added an invitation for badge %s" % request.POST.get("invitation-badge-id")
+                "You added an invitation for badge {}".format(
+                    request.POST.get("invitation-badge-id")
+                )
             )
         elif request.POST.get("add-issuer"):
             origin = request.POST.get("issuer-origin")
             name = request.POST.get("issuer-name")
             if not request.db.issuer_exists(origin, name):
                 # Add an Issuer to the DB.
                 request.db.add_issuer(
                     origin, name, request.POST.get("issuer-org"), request.POST.get("issuer-contact")
                 )
                 request.session.flash(
-                    "You added an issuer with the name %s" % request.POST.get("issuer-name")
+                    "You added an issuer with the name {}".format(request.POST.get("issuer-name"))
                 )
             else:
                 request.session.flash(
                     f"Issuer with origin {origin} and name {name} already exists."
                 )
 
         elif request.POST.get("add-assertion"):
@@ -425,15 +427,15 @@
 
 @view_config(context=m.Invitation, name="claim")
 def invitation_claim(request):
     """Action that awards a person a badge after scanning a qrcode."""
 
     # settings = request.registry.settings
 
-    if request.context.expires_on < datetime.now(timezone.utc):
+    if request.context.expires_on < datetime.now():
         return HTTPGone("That invitation is expired.")
 
     if not request.authenticated_userid:
         request.session["came_from"] = request.resource_url(request.context, "claim")
         return HTTPFound(location=request.route_url("login"))
 
     person = request.db.get_person(person_email=request.authenticated_userid)
@@ -452,23 +454,23 @@
     return HTTPFound(location=request.route_url("home"))
 
 
 @view_config(context=m.Invitation, name="qrcode")
 def invitation_qrcode(request):
     """Returns a raw dummy qrcode through to the user."""
 
-    if request.context.expires_on < datetime.now(timezone.utc):
+    if request.context.expires_on < datetime.now():
         return HTTPGone("That invitation is expired.")
 
     target = request.resource_url(request.context, "claim")
     img = qrcode_module.make(target)
-    stringstream = StringIO()
-    img.save(stringstream)
+    bytestream = BytesIO()
+    img.save(bytestream)
     return Response(
-        body=stringstream.getvalue(),
+        body=bytestream.getvalue(),
         content_type="image/png",
     )
 
 
 @view_config(route_name="leaderboard", renderer="leaderboard.mak")
 def leaderboard(request):
     """Render a top users view."""
@@ -693,15 +695,15 @@
     feed.language = "en"
 
     description_template = "<img src='%s' alt='%s' />%s"
 
     for badge in newest_badges:
         url = request.route_url("badge", id=badge.id)
         entry = feed.add_entry()
-        entry.title("New badge: %s !" % badge.name)
+        entry.title(f"New badge: {badge.name} !")
         entry.link(href=url)
         pubdate = badge.created_on.replace(tzinfo=timezone.utc)
         entry.published(pubdate)
         entry.description(
             description_template
             % (
                 badge.image,
@@ -723,15 +725,15 @@
     """Render badge info page."""
     # Get the badge to render info about.
     badge_id = request.matchdict.get("id")
     badge = request.db.get_badge(badge_id)
 
     # if the badge isn't found, raise a 404
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     # Get awarded assertions.
     if request.authenticated_userid:
         awarded_assertions = request.db.get_assertions_by_email(request.authenticated_userid)
     else:
         awarded_assertions = []
 
@@ -880,41 +882,41 @@
 def badge_rss(request):
     """Render per-badge rss."""
 
     badge_id = request.matchdict.get("id")
     badge = request.db.get_badge(badge_id)
 
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     # this gives us the assertions sorted *earliest first*. feedgen's
     # default when adding entries is to prepend - put the new item at
     # the top of the feed. so as we iterate over this and add items to
     # the feed, we add each newer assertion to the front of the feed
     sorted_assertions = sorted(badge.assertions, key=lambda x: x.issued_on)
 
     feed = FeedGenerator()
-    feed.title("Badges Feed for %s" % badge.name)
+    feed.title(f"Badges Feed for {badge.name}")
     feed.link(href=request.route_url("badge", id=badge.id), rel="self")
-    feed.subtitle("Latest recipients of the badge %s" % badge.name)
+    feed.subtitle(f"Latest recipients of the badge {badge.name}")
     feed.language("en")
 
     description_template = "<img src='%s' alt='%s' />%s"
 
     for assertion in sorted_assertions:
         url = request.route_url("user", id=assertion.person.nickname or assertion.person.id)
         entry = feed.add_entry()
         entry.title(assertion.person.nickname)
         entry.link(href=url)
         pubdate = assertion.issued_on.replace(tzinfo=timezone.utc)
         entry.published(pubdate)
         entry.description(
             description_template
             % (
-                get_avatar(assertion.person.email, 128),
+                get_avatar(assertion.person.avatar, 128),
                 assertion.person.nickname,
                 assertion.person.nickname,
             )
         )
 
     return Response(
         body=feed.rss_str(pretty=True),
@@ -927,15 +929,15 @@
 def badge_stl(request):
     """Render per-badge stl."""
 
     badge_id = request.matchdict.get("id")
     badge = request.db.get_badge(badge_id)
 
     if not badge:
-        raise HTTPNotFound("No such badge %r" % badge_id)
+        raise HTTPNotFound(f"No such badge {badge_id!r}")
 
     if not badge.stl:
         raise HTTPNotFound("Badge has no stl file.")
 
     return dict(
         badge=badge,
         auth_principals=request.effective_principals,
@@ -946,29 +948,29 @@
 def user_rss(request):
     """Render per-user rss."""
 
     user_id = request.matchdict.get("id")
     user = _get_user(request, user_id)
 
     if not user:
-        raise HTTPNotFound("No such user %r" % user_id)
+        raise HTTPNotFound(f"No such user {user_id!r}")
 
     if user.opt_out and user.email != request.authenticated_userid:
-        raise HTTPNotFound("User %r has opted out." % user_id)
+        raise HTTPNotFound(f"User {user_id!r} has opted out.")
 
     # this gives us the assertions sorted *earliest first*. feedgen's
     # default when adding entries is to prepend - put the new item at
     # the top of the feed. so as we iterate over this and add items to
     # the feed, we add each newer assertion to the front of the feed
     sorted_assertions = sorted(user.assertions, key=lambda x: x.issued_on)
 
     feed = FeedGenerator()
-    feed.title("Badges Feed for %s" % user.nickname)
+    feed.title(f"Badges Feed for {user.nickname}")
     feed.link(href=request.route_url("user", id=user.nickname or user.id), rel="self")
-    feed.subtitle("The latest Fedora Badges obtained by %s" % user.nickname)
+    feed.subtitle(f"The latest Fedora Badges obtained by {user.nickname}")
     feed.language("en")
 
     description_template = "<img src='%s' alt='%s'/>%s -- %s"
 
     for assertion in sorted_assertions:
         entry = feed.add_entry()
         entry.title(assertion.badge.name)
@@ -1007,18 +1009,18 @@
 
     user_id = request.matchdict.get("id")
     user = _get_user(request, user_id)
 
     history_limit = int(request.params.get("history_limit", 10))
 
     if not user:
-        raise HTTPNotFound("No such user %r" % user_id)
+        raise HTTPNotFound(f"No such user {user_id!r}")
 
     if user.opt_out and user.email != request.authenticated_userid:
-        raise HTTPNotFound("User %r has opted out." % user_id)
+        raise HTTPNotFound(f"User {user_id!r} has opted out.")
 
     if request.POST:
 
         token = request.session.get_csrf_token()
         if token != request.POST["csrf_token"]:
             raise HTTPForbidden("CSRF token did not match")
 
@@ -1032,17 +1034,15 @@
 
         if request.POST.get("deactivate-account"):
             person.opt_out = True
         elif request.POST.get("reactivate-account"):
             person.opt_out = False
 
     # Get invitations the user has created.
-    invitations = [
-        i for i in request.db.get_invitations(user.id) if i.expires_on > datetime.now(timezone.utc)
-    ]
+    invitations = [i for i in request.db.get_invitations(user.id) if i.expires_on > datetime.now()]
 
     user_info = dict(
         user=user,
         invitations=invitations,
         auth_principals=request.effective_principals,
         awarded_assertions=awarded_assertions,
         history_limit=history_limit,
@@ -1061,15 +1061,15 @@
     for assertion in user.assertions:
         issued = {"issued": float(assertion.issued_on.strftime("%s"))}
         _badged = _badge_json_generator(request, assertion.badge, withasserts=False)
         assertions.append({**issued, **_badged})
 
     return {
         "user": user.nickname,
-        "avatar": get_avatar(user.email, int(request.GET.get("size", 100))),
+        "avatar": get_avatar(user.avatar, int(request.GET.get("size", 100))),
         "percent_earned": user_info["percent_earned"],
         "assertions": assertions,
         "percentile": str(user_info["percentile"]),
         "rank": user_info["rank"],
         "user_count": user_info["user_count"],
     }
 
@@ -1113,22 +1113,22 @@
 
     user_a_id = request.matchdict.get("id_a")
     user_b_id = request.matchdict.get("id_b")
     user_a = _get_user(request, user_a_id)
     user_b = _get_user(request, user_b_id)
 
     if not user_a:
-        raise HTTPNotFound("No such user %r" % user_a_id)
+        raise HTTPNotFound(f"No such user {user_a_id!r}")
     if not user_b:
-        raise HTTPNotFound("No such user %r" % user_b_id)
+        raise HTTPNotFound(f"No such user {user_b_id!r}")
 
     if user_a.opt_out and user_a.email != request.authenticated_userid:
-        raise HTTPNotFound("User %r has opted out." % user_a_id)
+        raise HTTPNotFound(f"User {user_a_id!r} has opted out.")
     if user_b.opt_out and user_b.email != request.authenticated_userid:
-        raise HTTPNotFound("User %r has opted out." % user_b_id)
+        raise HTTPNotFound(f"User {user_b_id!r} has opted out.")
 
     # Get user badges.
     user_a_badges = [a.badge for a in user_a.assertions]
     user_b_badges = [a.badge for a in user_b.assertions]
 
     # Sort user badges by id.
     user_a_badges = sorted(user_a_badges, key=lambda badge: badge.id)
@@ -1471,15 +1471,15 @@
         # to be awarded it, give it to them.
         if request.db.badge_exists(badge_id):
             if not request.db.assertion_exists(badge_id, email):
                 # The None will default to datetime.now().
                 request.db.add_assertion(badge_id, email, None)
                 successful_awards += 1
 
-    request.session.flash("Successfully awarded %s badges." % successful_awards)
+    request.session.flash(f"Successfully awarded {successful_awards} badges.")
     return HTTPFound(location=request.route_url("admin"))
 
 
 @view_config(context=str)
 def html(context, request):
     return Response(context)
 
@@ -1503,15 +1503,15 @@
 
 @view_config(route_name="assertion_widget", renderer="assertion_widget.mak")
 def assertion_widget(request):
     person_id = request.matchdict.get("person")
     badge_id = request.matchdict.get("badge")
     user = request.db.get_person(id=person_id)
     if not user:
-        raise HTTPNotFound("No such person %r" % person_id)
+        raise HTTPNotFound(f"No such person {person_id!r}")
 
     def get_assertion():
         for assertion in user.assertions:
             if assertion.badge.id == badge_id:
                 return assertion
         raise HTTPNotFound("User does not have that badge")
 
@@ -1586,15 +1586,15 @@
         here = os.path.dirname(os.path.abspath(__file__))
         dflt = os.path.join(here, "sitedocs")
         directory = request.registry.settings.get("tahrir.sitedocs_dir", dflt)
         for k in possible_keys:
             htmldocs[k] = _load_docs(directory, k)
 
     if key not in htmldocs:
-        raise KeyError("%r is not permitted." % key)
+        raise KeyError(f"{key!r} is not permitted.")
 
     return htmldocs[key]
 
 
 def get_start_week(year=None, month=None, day=None):
     """For a given date, retrieve the day the week started.
     For any missing parameters (ie: None), use the value of the current
```

### Comparing `tahrir-1.0.0/tahrir/widgets.py` & `tahrir-1.1.0/tahrir/widgets.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/tests/test_utils.py` & `tahrir-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tahrir-1.0.0/PKG-INFO` & `tahrir-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir
-Version: 1.0.0
+Version: 1.1.0
 Summary: A pyramid app for issuing your own Open Badges
 Home-page: https://github.com/fedora-infra/tahrir
 License: AGPLv3+ with additional permission
 Author: Ralph Bean
 Author-email: rbean@redhat.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Environment :: Web Environment
@@ -32,15 +32,15 @@
 Requires-Dist: pyramid-tm (>=2.5,<3.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
-Requires-Dist: tahrir-api (>=1.0.0,<2.0.0)
+Requires-Dist: tahrir-api (>=1.1.0,<2.0.0)
 Requires-Dist: tahrir-messages (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/fedora-infra/tahrir
 Description-Content-Type: text/markdown
 
 # Tahrir
 > fedora-badges https://badges.fedoraproject.org/
```

