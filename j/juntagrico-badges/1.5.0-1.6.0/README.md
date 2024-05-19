# Comparing `tmp/juntagrico-badges-1.5.0.tar.gz` & `tmp/juntagrico_badges-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico-badges-1.5.0.tar", last modified: Wed Jan 10 05:06:41 2024, max compression
+gzip compressed data, was "juntagrico_badges-1.6.0.tar", last modified: Sun May 19 13:18:15 2024, max compression
```

## Comparing `juntagrico-badges-1.5.0.tar` & `juntagrico_badges-1.6.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.780287 juntagrico-badges-1.5.0/juntagrico_badges/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.780287 juntagrico-badges-1.5.0/juntagrico_badges/entity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/entity/badges.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/juntagricoapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/juntagrico_badges/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.776287 juntagrico-badges-1.5.0/juntagrico_badges/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/admin_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/home.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/management_lists/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/management_lists/badges.html
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/snippets/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/juntagrico_badges/views_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-01-10 05:06:41.000000 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-10 05:06:41.000000 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 05:06:41.000000 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-10 05:06:41.000000 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-10 05:06:41.000000 juntagrico-badges-1.5.0/juntagrico_badges.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-10 05:06:41.784287 juntagrico-badges-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-10 05:06:34.000000 juntagrico-badges-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/entity/badges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.632534 juntagrico_badges-1.6.0/juntagrico_badges/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/home.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/management_lists/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/management_lists/badges.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.636534 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/snippets/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.632534 juntagrico_badges-1.6.0/juntagrico_badges/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/juntagrico_badges/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/templates/juntagrico/menu/user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/juntagrico_badges/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/tests/test_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/juntagrico_badges/views_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-19 13:18:15.000000 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-19 13:18:15.000000 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:18:15.000000 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 13:18:15.000000 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 13:18:15.000000 juntagrico_badges-1.6.0/juntagrico_badges.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 13:18:11.000000 juntagrico_badges-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 13:18:15.640534 juntagrico_badges-1.6.0/setup.cfg
```

### Comparing `juntagrico-badges-1.5.0/LICENSE` & `juntagrico_badges-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/README.md` & `juntagrico_badges-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 Install juntagrico-badge via `pip`
 
     $ pip install juntagrico-badges
 
 or add it in your projects `requirements.txt`
 
-In `settings.py` add `'juntagrico_badges',`.
+In `settings.py` add `'juntagrico_badges',`, **above** `'juntagrico''`.
 
 ```python
 INSTALLED_APPS = [
     ...
-    'juntagrico',
     'juntagrico_badges',
+    'juntagrico',
 ]
 ```
 
 In your `urls.py` you also need to extend the pattern:
 
 ```python
 urlpatterns = [
```

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/entity/badges.py` & `juntagrico_badges-1.6.0/juntagrico_badges/entity/badges.py`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/migrations/0001_initial.py` & `juntagrico_badges-1.6.0/juntagrico_badges/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/home.html` & `juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/home.html`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/management_lists/badges.html` & `juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/management_lists/badges.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 {% load juntagrico.common %}
 {% load juntagrico.config %}
 {% block page_title %}
     <h3>
         {% trans "Abzeichen" %}
     </h3>
 {% endblock %}
+{% block management_cmd %}
+    {% include 'management_lists/snippets/email_sender.html' %}
+{% endblock %}
 {% block list %}
     <table id="filter-table" class="list table" style="display: table;">
         <thead>
             <tr>
                 <th class="filter">
                     {% trans "Mitglied" %}
                 </th>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends "management_lists/man_list_base.html" %} {% load i18n %} {% load
 juntagrico.common %} {% load juntagrico.config %} {% block page_title %}
 ******** {{%% ttrraannss ""AAbbzzeeiicchheenn"" %%}} ********
-{% endblock %} {% block list %}
+{% endblock %} {% block management_cmd %} {% include 'management_lists/
+snippets/email_sender.html' %} {% endblock %} {% block list %}
 {{%% ttrraannss ""MMiittgglliieedd"" %%}} {{%% ttrraannss ""AAbbzzeeiicchheenn"" %%}}           {{%% ttrraannss ""EEmmaaiillss"" %%}}
                        {% for badge in member.badges.all
 {{ member }}           %} {{ badge.name }}{% if not      {{ member.email }}
                        forloop.last %},{% endif %} {%
                        endfor %}
 {% endblock %}
```

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/templates/jbg/snippets/badge.html` & `juntagrico_badges-1.6.0/juntagrico_badges/templates/jbg/snippets/badge.html`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges/views.py` & `juntagrico_badges-1.6.0/juntagrico_badges/views.py`

 * *Files identical despite different names*

### Comparing `juntagrico-badges-1.5.0/juntagrico_badges.egg-info/SOURCES.txt` & `juntagrico_badges-1.6.0/juntagrico_badges.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
-setup.py
 juntagrico_badges/__init__.py
 juntagrico_badges/admin.py
 juntagrico_badges/apps.py
-juntagrico_badges/juntagricoapp.py
 juntagrico_badges/urls.py
 juntagrico_badges/views.py
 juntagrico_badges/views_admin.py
 juntagrico_badges.egg-info/PKG-INFO
 juntagrico_badges.egg-info/SOURCES.txt
 juntagrico_badges.egg-info/dependency_links.txt
 juntagrico_badges.egg-info/requires.txt
 juntagrico_badges.egg-info/top_level.txt
 juntagrico_badges/entity/__init__.py
 juntagrico_badges/entity/badges.py
 juntagrico_badges/migrations/0001_initial.py
 juntagrico_badges/migrations/__init__.py
-juntagrico_badges/templates/jbg/admin_menu.html
 juntagrico_badges/templates/jbg/home.html
-juntagrico_badges/templates/jbg/menu.html
 juntagrico_badges/templates/jbg/management_lists/badges.html
-juntagrico_badges/templates/jbg/snippets/badge.html
+juntagrico_badges/templates/jbg/snippets/badge.html
+juntagrico_badges/templates/juntagrico/menu/admin.html
+juntagrico_badges/templates/juntagrico/menu/user.html
+juntagrico_badges/tests/__init__.py
+juntagrico_badges/tests/test_badges.py
```

