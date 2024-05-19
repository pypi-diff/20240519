# Comparing `tmp/langstory-0.0.0.tar.gz` & `tmp/langstory-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langstory-0.0.0.tar", last modified: Sun May 19 18:58:53 2024, max compression
+gzip compressed data, was "langstory-0.0.1.tar", last modified: Sun May 19 19:45:31 2024, max compression
```

## Comparing `langstory-0.0.0.tar` & `langstory-0.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.362146 langstory-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 18:58:53.361445 langstory-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3635 2024-05-18 19:57:49.000000 langstory-0.0.0/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.286171 langstory-0.0.0/app/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:50:47.000000 langstory-0.0.0/app/.gitkeep
--rw-r--r--   0 root         (0) root         (0)     1111 2024-05-19 18:14:19.000000 langstory-0.0.0/app/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.287782 langstory-0.0.0/app/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 18:14:19.000000 langstory-0.0.0/app/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1440 2024-05-19 18:14:19.000000 langstory-0.0.0/app/controllers/auth.py
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-19 18:14:19.000000 langstory-0.0.0/app/http_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.298546 langstory-0.0.0/app/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/base.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/event.py
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/journey.py
--rw-r--r--   0 root         (0) root         (0)      539 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/organization.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/persona.py
--rw-r--r--   0 root         (0) root         (0)      640 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/project.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/tool.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/tool_call.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-05-17 21:25:15.000000 langstory-0.0.0/app/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.324027 langstory-0.0.0/app/routers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 21:25:15.000000 langstory-0.0.0/app/routers/.gitkeep
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 21:25:15.000000 langstory-0.0.0/app/routers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.326825 langstory-0.0.0/app/routers/v1/
--rw-r--r--   0 root         (0) root         (0)      392 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.331372 langstory-0.0.0/app/routers/v1/auth/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/auth/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/auth/__Init__.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/auth/google.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/auth/jwt.py
--rw-r--r--   0 root         (0) root         (0)      548 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/auth/username_password.py
--rw-r--r--   0 root         (0) root         (0)      362 2024-05-19 18:14:19.000000 langstory-0.0.0/app/routers/v1/organizations.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-05-19 18:14:19.000000 langstory-0.0.0/app/settings.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-19 18:14:19.000000 langstory-0.0.0/app/tags_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.360551 langstory-0.0.0/langstory.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 18:58:53.000000 langstory-0.0.0/langstory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-05-19 18:58:53.000000 langstory-0.0.0/langstory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 18:58:53.000000 langstory-0.0.0/langstory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-19 18:58:53.000000 langstory-0.0.0/langstory.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.353627 langstory-0.0.0/migrations/
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 21:25:15.000000 langstory-0.0.0/migrations/README
--rw-r--r--   0 root         (0) root         (0)     2533 2024-05-17 21:25:15.000000 langstory-0.0.0/migrations/env.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-05-17 21:25:15.000000 langstory-0.0.0/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.357279 langstory-0.0.0/migrations/versions/
--rw-r--r--   0 root         (0) root         (0)     8995 2024-05-17 21:25:15.000000 langstory-0.0.0/migrations/versions/117f8dc64513_create_many_base_models.py
--rw-r--r--   0 root         (0) root         (0)     1192 2024-05-17 21:25:15.000000 langstory-0.0.0/migrations/versions/5fb191b116ed_init_with_organization.py
--rw-r--r--   0 root         (0) root         (0)      803 2024-05-19 18:58:50.000000 langstory-0.0.0/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 21:25:15.000000 langstory-0.0.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 18:58:53.359634 langstory-0.0.0/requirements/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-17 21:25:15.000000 langstory-0.0.0/requirements/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-19 18:14:19.000000 langstory-0.0.0/requirements/prod-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 18:58:53.362461 langstory-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.374787 langstory-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-19 19:45:31.374787 langstory-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-19 19:45:27.000000 langstory-0.0.1/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.366787 langstory-0.0.1/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-19 19:45:27.000000 langstory-0.0.1/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.366787 langstory-0.0.1/app/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-19 19:45:27.000000 langstory-0.0.1/app/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-19 19:45:27.000000 langstory-0.0.1/app/http_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.370787 langstory-0.0.1/app/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/tool_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-19 19:45:27.000000 langstory-0.0.1/app/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.370787 langstory-0.0.1/app/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.370787 langstory-0.0.1/app/routers/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.370787 langstory-0.0.1/app/routers/v1/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/auth/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/auth/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/auth/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/auth/username_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-19 19:45:27.000000 langstory-0.0.1/app/routers/v1/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-19 19:45:27.000000 langstory-0.0.1/app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 19:45:27.000000 langstory-0.0.1/app/tags_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.374787 langstory-0.0.1/langstory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-19 19:45:31.000000 langstory-0.0.1/langstory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 19:45:31.000000 langstory-0.0.1/langstory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:45:31.000000 langstory-0.0.1/langstory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 19:45:31.000000 langstory-0.0.1/langstory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.370787 langstory-0.0.1/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:45:27.000000 langstory-0.0.1/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-19 19:45:27.000000 langstory-0.0.1/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-19 19:45:27.000000 langstory-0.0.1/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.374787 langstory-0.0.1/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-19 19:45:27.000000 langstory-0.0.1/migrations/versions/117f8dc64513_create_many_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-19 19:45:27.000000 langstory-0.0.1/migrations/versions/5fb191b116ed_init_with_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 19:45:27.000000 langstory-0.0.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:27.000000 langstory-0.0.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:45:31.374787 langstory-0.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 19:45:27.000000 langstory-0.0.1/requirements/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-19 19:45:27.000000 langstory-0.0.1/requirements/prod-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:45:31.374787 langstory-0.0.1/setup.cfg
```

### Comparing `langstory-0.0.0/alembic.ini` & `langstory-0.0.1/alembic.ini`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # path to migration scripts
 script_location = migrations
 
 # template used to generate migration file names; The default value is %%(rev)s_%%(slug)s
 # Uncomment the line below if you want the files to be prepended with date and time
 # see https://alembic.sqlalchemy.org/en/latest/tutorial.html#editing-the-ini-file
 # for all available tokens
-# file_template = %%(year)d_%%(month).2d_%%(day).2d_%%(hour).2d%%(minute).2d-%%(rev)s_%%(slug)s
+file_template = %%(year)d_%%(month).2d_%%(day).2d_%%(hour).2d%%(minute).2d-%%(rev)s_%%(slug)s
 
 # sys.path path, will be prepended to sys.path if present.
 # defaults to the current working directory.
 prepend_sys_path = .
 
 # timezone to use when rendering the date within the migration file
 # as well as the filename.
```

### Comparing `langstory-0.0.0/app/app.py` & `langstory-0.0.1/app/app.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/controllers/auth.py` & `langstory-0.0.1/app/controllers/auth.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/http_errors.py` & `langstory-0.0.1/app/http_errors.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/base.py` & `langstory-0.0.1/app/models/base.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/event.py` & `langstory-0.0.1/app/models/event.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/organization.py` & `langstory-0.0.1/app/models/organization.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/persona.py` & `langstory-0.0.1/app/models/persona.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/project.py` & `langstory-0.0.1/app/models/project.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/tool.py` & `langstory-0.0.1/app/models/tool.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/tool_call.py` & `langstory-0.0.1/app/models/tool_call.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/models/user.py` & `langstory-0.0.1/app/models/user.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/routers/v1/auth/README.md` & `langstory-0.0.1/app/routers/v1/auth/README.md`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/routers/v1/auth/google.py` & `langstory-0.0.1/app/routers/v1/auth/google.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/routers/v1/auth/username_password.py` & `langstory-0.0.1/app/routers/v1/auth/username_password.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/settings.py` & `langstory-0.0.1/app/settings.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/app/tags_metadata.py` & `langstory-0.0.1/app/tags_metadata.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/langstory.egg-info/SOURCES.txt` & `langstory-0.0.1/langstory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/migrations/env.py` & `langstory-0.0.1/migrations/env.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/migrations/script.py.mako` & `langstory-0.0.1/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/migrations/versions/117f8dc64513_create_many_base_models.py` & `langstory-0.0.1/migrations/versions/117f8dc64513_create_many_base_models.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/migrations/versions/5fb191b116ed_init_with_organization.py` & `langstory-0.0.1/migrations/versions/5fb191b116ed_init_with_organization.py`

 * *Files identical despite different names*

### Comparing `langstory-0.0.0/pyproject.toml` & `langstory-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langstory"
+version = "0.0.1"
 authors = [
     { name = "Ethan Knox", email = "ethan@langstory.org" },
     { name = "Yoaquim Cintron", email = "yoaquim@langstory.org" },
 ]
 description = "Adding the 'product' back to product design for AI Platforms"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["llm", "ai", "ux", "ux-design", "langfuse", "langchain"]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3", ]
-dynamic = ["version"]
 
 #dependencies = []
 
 #[project.optional-dependencies]
 #pdf = ["ReportLab>=1.2", "RXP"]
 #rest = ["docutils>=0.3", "pack ==1.1, ==1.3"]
```

