# Comparing `tmp/pymdg-1.1.0.tar.gz` & `tmp/pymdg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymdg-1.1.0.tar", last modified: Sun Apr 28 21:01:24 2024, max compression
+gzip compressed data, was "pymdg-1.2.0.tar", last modified: Sun May 19 00:39:09 2024, max compression
```

## Comparing `pymdg-1.1.0.tar` & `pymdg-1.2.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.637621 pymdg-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-28 21:01:21.000000 pymdg-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 21:01:21.000000 pymdg-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-28 21:01:24.637621 pymdg-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-28 21:01:21.000000 pymdg-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/generate/
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.625620 pymdg-1.1.0/mdg/generate/confluence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/content_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/image_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/confluence/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/generate/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/parse/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/bouml_xmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/drawio_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/erwin_xmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_db_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    21487 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/parse/sparx_xmi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Arango/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Arango/models.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/.azure/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/.azure/config.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/.azure/setup.ps1.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/admin.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/apps.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/serializers.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/urls.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/app/views.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/manage.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.629621 pymdg-1.1.0/mdg/templates/Django/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/asgi.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/settings.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/urls.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/validators.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/project/wsgi.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Django/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/Java/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/entities.jdl.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/enums.java.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Java/pojos.java.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/SQLAlchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/SQLAlchemy/models.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/SQLAlchemy/schemas.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/templates/Schema/
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Schema/avro.avsc.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/Schema/openapi.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/base.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/hasura-abac.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/hasura.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/templates/postgresql.sql.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_uml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tests/test_xmi_model_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/DrawIO MDG UML Library.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/mdg_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    46970 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/tools/sparx_db_models_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.633621 pymdg-1.1.0/mdg/uml/
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/uml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-28 21:01:21.000000 pymdg-1.1.0/mdg/uml/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:01:24.637621 pymdg-1.1.0/pymdg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 21:01:24.000000 pymdg-1.1.0/pymdg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-28 21:01:21.000000 pymdg-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:01:24.637621 pymdg-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-28 21:01:21.000000 pymdg-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.694990 pymdg-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-19 00:39:06.000000 pymdg-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-19 00:39:06.000000 pymdg-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-19 00:39:09.690990 pymdg-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-19 00:39:06.000000 pymdg-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.678990 pymdg-1.2.0/mdg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.678990 pymdg-1.2.0/mdg/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/generate/confluence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/confluence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/confluence/content_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/confluence/image_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/confluence/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/generate/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/bouml_xmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/drawio_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/erwin_xmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17926 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/sparx_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/sparx_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21491 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/parse/sparx_xmi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/templates/Arango/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Arango/models.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/templates/Django/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.682990 pymdg-1.2.0/mdg/templates/Django/.azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/.azure/config.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/.azure/setup.ps1.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/Django/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/admin.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/apps.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/serializers.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/urls.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/app/views.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/manage.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/Django/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/asgi.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/settings.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/urls.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/validators.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/project/wsgi.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Django/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/Java/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Java/entities.jdl.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Java/enums.java.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Java/pojos.java.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/Python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Python/dataclass_avro.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/SQLAlchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/SQLAlchemy/models.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/SQLAlchemy/schemas.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.686990 pymdg-1.2.0/mdg/templates/Schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Schema/avro.avsc.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/Schema/openapi.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/base.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/hasura-abac.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/hasura.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/templates/postgresql.sql.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.690990 pymdg-1.2.0/mdg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_uml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tests/test_xmi_model_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.690990 pymdg-1.2.0/mdg/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/DrawIO MDG UML Library.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/mdg_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46970 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/tools/sparx_db_models_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.690990 pymdg-1.2.0/mdg/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/uml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-19 00:39:06.000000 pymdg-1.2.0/mdg/uml/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:39:09.690990 pymdg-1.2.0/pymdg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 00:39:09.000000 pymdg-1.2.0/pymdg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 00:39:06.000000 pymdg-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:39:09.694990 pymdg-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-19 00:39:06.000000 pymdg-1.2.0/setup.py
```

### Comparing `pymdg-1.1.0/LICENSE` & `pymdg-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/PKG-INFO` & `pymdg-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymdg
-Version: 1.1.0
+Version: 1.2.0
 Summary: Model driven genration - from UML to Code & Docs
 Home-page: https://github.com/semprini/pyMDG
 Author: Semprini
 Author-email: dont@contact.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -78,15 +78,15 @@
 ![Nomenclature](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_9100ADB5_EFF8_4ded_BA61_E8564C8134AC.png)
 
 ## Sample model
 ![Sample model](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_96AC850E_2FD0_4e6c_B00E_C030EDA89F42.png)
 
 ## Metamodel
 This diagram shows the internal classes which are passed to the templates during generation.
-![Metamodel](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_B080F856_9EFB_46f2_8D69_1C79956D714A.png)
+![Metamodel](https://raw.githubusercontent.com/Semprini/pyMDG/master/docs/_static/image/metamodel.png)
 
 ## Build the docs
 Install sphinx
 ```
  > cd pyMDG
  > sphinx-apidoc -o docs\source mdg
  > cd docs
```

### Comparing `pymdg-1.1.0/README.md` & `pymdg-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ![Nomenclature](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_9100ADB5_EFF8_4ded_BA61_E8564C8134AC.png)
 
 ## Sample model
 ![Sample model](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_96AC850E_2FD0_4e6c_B00E_C030EDA89F42.png)
 
 ## Metamodel
 This diagram shows the internal classes which are passed to the templates during generation.
-![Metamodel](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_B080F856_9EFB_46f2_8D69_1C79956D714A.png)
+![Metamodel](https://raw.githubusercontent.com/Semprini/pyMDG/master/docs/_static/image/metamodel.png)
 
 ## Build the docs
 Install sphinx
 ```
  > cd pyMDG
  > sphinx-apidoc -o docs\source mdg
  > cd docs
```

### Comparing `pymdg-1.1.0/mdg/__init__.py` & `pymdg-1.2.0/mdg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         "duration": "DurationField",
         "file": "FileField",
         "float": "FloatField",
         "date": "DateField",
         "dateTime": "DateTimeField",
         "datetime": "DateTimeField",
         "date_time": "DateTimeField",
+        "Timestamp": "DateTimeField",
+        "timestamp": "DateTimeField",
         "json": "JSONField",
     },
     "marshmallow": {
         "boolean": "Boolean",
         "int": "Integer",
         "integer": "Integer",
         "bigint": "Integer",
```

### Comparing `pymdg-1.1.0/mdg/config.py` & `pymdg-1.2.0/mdg/config.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/generate/__init__.py` & `pymdg-1.2.0/mdg/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/generate/confluence/content_update.py` & `pymdg-1.2.0/mdg/generate/confluence/content_update.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/generate/confluence/image_update.py` & `pymdg-1.2.0/mdg/generate/confluence/image_update.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/generate/confluence/util.py` & `pymdg-1.2.0/mdg/generate/confluence/util.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/generate/render.py` & `pymdg-1.2.0/mdg/generate/render.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/__init__.py` & `pymdg-1.2.0/mdg/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/bouml_xmi.py` & `pymdg-1.2.0/mdg/parse/bouml_xmi.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/drawio_xml.py` & `pymdg-1.2.0/mdg/parse/drawio_xml.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/erwin_xmi.py` & `pymdg-1.2.0/mdg/parse/erwin_xmi.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/sparx_db.py` & `pymdg-1.2.0/mdg/parse/sparx_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,31 +36,45 @@
     """ Root package parser entry point.
     """
     test_cases: List[UMLInstance] = []
 
     engine = sqlalchemy.create_engine(f"{settings['source']}", echo=False, future=True)
     with Session(engine) as session:
 
+        # Find the root package. Can specify either EA GUID or name
+        # If guid make sure value in recipie is quoted - model_package: "{D6D3BF36-E897-4a8b-8CA9-62ADAAD696ED}"
+        if settings['root_package'][0] == "{":
+            stmt = sqlalchemy.select(TPackage).where(TPackage.ea_guid == settings['root_package'])
+        else:
+            stmt = sqlalchemy.select(TPackage).where(TPackage.name == settings['root_package'])
+        root_tpackage: TPackage = session.execute(stmt).scalars().first()
+        if root_tpackage is None:
+            raise ValueError("Root package element not found. Settings has:{}".format(settings['root_package']))
+        logger.debug(f"Root Object: {root_tpackage.package_id}: {root_tpackage.name}")
+
         # Find the package with the model nodes. Can specify either EA GUID or name
         # If guid make sure value in recipie is quoted - model_package: "{D6D3BF36-E897-4a8b-8CA9-62ADAAD696ED}"
         if settings['model_package'][0] == "{":
             stmt = sqlalchemy.select(TPackage).where(TPackage.ea_guid == settings['model_package'])
         else:
             stmt = sqlalchemy.select(TPackage).where(TPackage.name == settings['model_package'])
         model_tpackage: TPackage = session.execute(stmt).scalars().first()
         if model_tpackage is None:
             raise ValueError("Model package element not found. Settings has:{}".format(settings['model_package']))
         logger.debug(f"Model Object: {model_tpackage.package_id}: {model_tpackage.name}")
 
-        # Create our root model UMLPackage and parse in 3 passes
-        model_package = package_parse(session, model_tpackage, None)
+        root_package = package_parse(session, root_tpackage, None, False)
+
+        # Create our model UMLPackage and parse in 3 passes
+        model_package = package_parse(session, model_tpackage, root_package)
+        root_package.children.append(model_package)
         logger.debug("Parsing associations and inheritance")
-        package_parse_associations(session, model_package)
+        package_parse_associations(session, root_package)
         logger.debug("Sorting objects")
-        package_sort_classes(model_package)
+        package_sort_classes(root_package)
 
     if 'test_package' in settings.keys():
         logger.info("Parsing test cases")
         if settings['test_package'][0] == "{":
             stmt = sqlalchemy.select(TPackage).where(TPackage.ea_guid == settings['test_package'])
         else:
             stmt = sqlalchemy.select(TPackage).where(TPackage.name == settings['test_package'])
@@ -68,15 +82,15 @@
         if test_tpackage is None:
             raise ValueError("Test package element not found. Settings has:{}".format(settings['test_package']))
         test_package = package_parse(session, test_tpackage, None)
         package_parse_associations(session, test_package)
         test_package_parse_inheritance(test_package, model_package)
         test_cases = parse_test_cases(test_package)
 
-    return model_package, test_cases
+    return root_package, test_cases
 
 
 def parse_test_cases(package: UMLPackage) -> List[UMLInstance]:
     """ Looks through package hierarchy for instances with request or response stereotype
     and returns list of instances.
     """
     test_cases = []
@@ -89,15 +103,15 @@
         res = parse_test_cases(child)
         if res:
             test_cases += res
 
     return test_cases
 
 
-def package_parse(session, tpackage: TPackage, parent_package: Optional[UMLPackage]):
+def package_parse(session, tpackage: TPackage, parent_package: Optional[UMLPackage], parse_children=True):
     """ Extract package details, call class parser for classes and self parser for sub-packages.
     Associations are not done here, but in a 2nd pass using the parse_associations function.
     :param element:
     :param root_element:
     :return:
     :rtype: UMLPackage
     """
@@ -116,15 +130,16 @@
         package.documentation = ""
 
     package.status = tobject.status
     package.version = f"{tpackage.version}"
 
     logger.debug("Added UMLPackage {}".format(package.path))
 
-    package_parse_children(session, package)
+    if parse_children:
+        package_parse_children(session, package)
     return package
 
 
 def package_parse_children(session, package: UMLPackage):
     stmt = sqlalchemy.select(TObject).where(TObject.package_id == package.id)
 
     # Loop through all child elements and create nodes for classes and sub packages
@@ -304,14 +319,23 @@
 
     # Allow explicit naming
     if tconnector.sourcerole is not None:
         association.source_name = tconnector.sourcerole
     if tconnector.destrole is not None:
         association.destination_name = tconnector.destrole
 
+    # Stereotypes
+    # TODO: Extract list of stereotypes
+    if tconnector.stereotype is not None:
+        association.stereotypes = [tconnector.stereotype,]
+    if tconnector.sourcestereotype is not None:
+        association.source_stereotypes = [tconnector.sourcestereotype,]
+    if tconnector.deststereotype is not None:
+        association.destination_stereotypes = [tconnector.deststereotype,]
+
     logging.debug(f"Created {association.cardinality.name} {association.association_type.name} from {association.source_name} to {association.destination_name}")
     return association
 
 
 def enumeration_parse(session, package: UMLPackage, tobject: TObject):
     enumeration = UMLEnumeration(package, tobject.name, tobject.object_id)
 
@@ -381,15 +405,19 @@
     if txref is not None:
         attr.is_id = bool(re.findall('@NAME=isID.*@VALU=1(.*?)@ENDVALU;', txref.description))
         if attr.is_id and isinstance(attr.parent, UMLClass):
             attr.parent.id_attribute = attr
     else:
         attr.is_id = False
 
-    attr.stereotype = tattribute.stereotype
+    # @STEREO;Name=routable;GUID={FCE54E6B-5A61-4336-88FD-7FEF375BB7E1};@ENDSTEREO;
+    stmt = sqlalchemy.select(TXref).where(TXref.client == tattribute.ea_guid, TXref.name == "Stereotypes")
+    txref = session.execute(stmt).scalars().first()
+    if txref is not None:
+        attr.stereotypes = re.findall('@STEREO;Name=(.*?);', txref.description)
 
     stmt = sqlalchemy.select(TAttributeconstraint).where(TAttributeconstraint.id == tattribute.id)
     for constraint in session.execute(stmt).scalars().all():
         if constraint.Constraint == 'unique':
             attr.is_unique = True
         elif constraint.Constraint.startswith('length'):
             attr.length = int(constraint.Constraint.split("=")[1])
```

### Comparing `pymdg-1.1.0/mdg/parse/sparx_db_models.py` & `pymdg-1.2.0/mdg/parse/sparx_db_models.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/parse/sparx_xmi.py` & `pymdg-1.2.0/mdg/parse/sparx_xmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
         attr.is_id = True
         attr.parent.id_attribute = attr
     else:
         attr.is_id = False
 
     stereotype = detail.find('stereotype')
     if stereotype is not None:
-        attr.stereotype = stereotype.get('stereotype')
+        attr.stereotypes = [stereotype.get('stereotype'),]
 
     constraints = detail.find('Constraints')
     if constraints is not None:
         for constraint in constraints:
             name = constraint.get('name')
             if name == 'unique':
                 attr.is_unique = True
```

### Comparing `pymdg-1.1.0/mdg/templates/Arango/models.py.jinja` & `pymdg-1.2.0/mdg/templates/Arango/models.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/.azure/setup.ps1.jinja` & `pymdg-1.2.0/mdg/templates/Django/.azure/setup.ps1.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/admin.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/admin.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/apps.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/apps.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/models.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/models.py.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 from django.utils.translation import gettext_lazy as _
 from django.db import models
 
-{% for cls in package.classes %}{% if cls.generalization != None %}{% if cls.generalization.package != package %}
-from {{ cls.generalization.package.name | case_package }}.models import {{ cls.generalization.name | case_class }}{% endif %}{% endif %}{% endfor %}
+{% for cls in package.classes %}{% if cls.generalization != None and cls.generalization.package != package %}
+from {{ cls.generalization.package.name | case_package }}.models import {{ cls.generalization.name | case_class }}{% endif %}{% for attr in cls.attributes %}{% if attr.classification and attr.classification.package != package %}
+from {{ attr.classification.package.name | case_package }}.models import ENUM_{{ attr.classification.name | case_class }}{% endif %}{% endfor %}{% endfor %}
 
 {% for enum in package.enumerations %}class ENUM_{{ enum.name | case_class }}(models.TextChoices):{% for attr in enum.values %}
-    {{ attr.upper() }} = '{{ attr }}', _('{{ attr }}'){% endfor %}
+    {{ attr | case_class | replace("/","_") | replace("-","_") }} = '{{ attr }}', _('{{ attr }}'){% endfor %}
 
 {% endfor %}{% for cls in package.classes %}{% if cls.is_abstract %}class {{ cls.name | case_class }}( models.Model ):{% for attr in cls.attributes %}{% if attr.classification %}
     {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name}}.choices, blank=True, null=True ){% else %}
-    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %} )
+    {{ attr.name | snakecase }} = models.{% if "Auto" in attr.stereotypes %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %} )
 {% endif %}{% endfor %}
     class Meta:
         abstract = True
 {% endif %}{% endfor %}
 
 {% for cls in package.classes %}{% if not cls.is_abstract and cls.specialized_by | length > 0 %}class {{ cls.name | case_class }}( {% if cls.generalization %}{{ cls.generalization.name | case_class }}{% else %}models.Model{% endif %} ):{% for attr in cls.attributes %}{% if attr.classification %}
     {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name | case_class }}.choices, blank=True, null=True ){% else %}
-    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
+    {{ attr.name | snakecase }} = models.{% if "Auto" in attr.stereotypes %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
 {% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if rel.association_type.name == "ASSOCIATION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_MANY" %}
     {{ rel.destination_name | snakecase }} = models.ManyToManyField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', blank=True ){% endif %}{% elif rel.association_type.name == "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% else %}
     {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% endif %}
 {% endif %}{% endfor %}{% for rel in cls.associations_to %}{% if rel.association_type.name != "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_MANY" %}
     {{ rel.source_name | snakecase }} = models.ForeignKey( '{{ rel.source.package.name | case_package }}.{{ rel.source.name | case_class }}', on_delete=models.CASCADE, related_name='{{ rel.destination_name | snakecase }}', blank=True, null=True ){% endif %}
-{% endif %}{% endfor %}{% endif %}
+{% endif %}{% endfor %}{% set uniques = [] %}{% for attr in cls.attributes %}{% if "UniqueKey" in attr.stereotypes %}{{ uniques.append( attr.name ) | default("", True) }}{% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if "UniqueKey" in rel.destination_stereotypes %}{{ uniques.append( rel.destination_name ) | default("", True) }}{% endif %}{% endfor %}{% if uniques != [] %}
 
-{% endfor %}
+    class Meta():
+        constraints = [
+                models.UniqueConstraint(fields=[{% for unique in uniques%}'{{ unique | snakecase }}',{% endfor %}], name='unique {% for unique in uniques%}{{ unique | snakecase }}__{% endfor %}')
+            ]
+{% endif %}
+
+{% endif %}{% endfor %}
 {% for cls in package.classes %}{% if not cls.is_abstract and cls.specialized_by | length == 0 %}class {{ cls.name | case_class }}( {% if cls.generalization %}{{ cls.generalization.name | case_class }}{% else %}models.Model{% endif %} ):{% for attr in cls.attributes %}{% if attr.classification %}
     {{ attr.name | snakecase }} = models.CharField( max_length=100, choices=ENUM_{{ attr.classification.name | case_class }}.choices, blank=True, null=True ){% else %}
-    {{ attr.name | snakecase }} = models.{% if attr.stereotype == "auto" %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
+    {{ attr.name | snakecase }} = models.{% if "Auto" in attr.stereotypes %}AutoField{% else %}{{ attr.dest_type }}{% endif %}( {% if attr.is_id %}primary_key=True, {% else %}blank=True, null=True, {% endif %}{% if attr.dest_type == "DecimalField" %}max_digits=10, decimal_places=2, {% endif %}{% if attr.length %}max_length={{ attr.length }}{% endif %}{% if attr.validations != [] %}validators=[validate_even]{% endif %} )
 {% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if rel.association_type.name == "ASSOCIATION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE, blank=True, null=True ){% elif rel.cardinality.name == "MANY_TO_MANY" %}
     {{ rel.destination_name | snakecase }} = models.ManyToManyField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', blank=True ){% endif %}{% elif rel.association_type.name == "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_ONE" %}
     {{ rel.destination_name | snakecase }} = models.OneToOneField( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% else %}
     {{ rel.destination_name | snakecase }} = models.ForeignKey( '{{ rel.destination.package.name | case_package }}.{{ rel.destination.name | case_class }}', related_name='{{ rel.source_name | snakecase }}', on_delete=models.CASCADE ){% endif %}
 {% endif %}{% endfor %}{% for rel in cls.associations_to %}{% if rel.association_type.name != "COMPOSITION" %}{% if rel.cardinality.name == "ONE_TO_MANY" %}
     {{ rel.source_name | snakecase }} = models.ForeignKey( '{{ rel.source.package.name | case_package }}.{{ rel.source.name | case_class }}', on_delete=models.CASCADE, related_name='{{ rel.destination_name | snakecase }}', blank=True, null=True ){% endif %}
-{% endif %}{% endfor %}{% endif %}
+{% endif %}{% endfor %}{% set uniques = [] %}{% for attr in cls.attributes %}{% if "UniqueKey" in attr.stereotypes %}{{ uniques.append( attr.name ) | default("", True) }}{% endif %}{% endfor %}{% for rel in cls.associations_from %}{% if "UniqueKey" in rel.destination_stereotypes %}{{ uniques.append( rel.destination_name ) | default("", True) }}{% endif %}{% endfor %}{% if uniques != [] %}
 
-{% endfor %}
+    class Meta():
+        constraints = [
+                models.UniqueConstraint(fields=[{% for unique in uniques%}'{{ unique | snakecase }}',{% endfor %}], name='unique {% for unique in uniques%}{{ unique | snakecase }}__{% endfor %}')
+            ]
+{% endif %}
+
+{% endif %}{% endfor %}
```

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/serializers.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/serializers.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/urls.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/urls.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/app/views.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/app/views.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/manage.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/project/settings.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/project/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Django/project/urls.py.jinja` & `pymdg-1.2.0/mdg/templates/Django/project/urls.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Java/entities.jdl.jinja` & `pymdg-1.2.0/mdg/templates/Java/entities.jdl.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Java/pojos.java.jinja` & `pymdg-1.2.0/mdg/templates/Java/pojos.java.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/SQLAlchemy/models.py.jinja` & `pymdg-1.2.0/mdg/templates/SQLAlchemy/models.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/SQLAlchemy/schemas.py.jinja` & `pymdg-1.2.0/mdg/templates/SQLAlchemy/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/Schema/openapi.yaml.jinja` & `pymdg-1.2.0/mdg/templates/Schema/openapi.yaml.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/hasura-abac.json.jinja` & `pymdg-1.2.0/mdg/templates/hasura-abac.json.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/hasura.json.jinja` & `pymdg-1.2.0/mdg/templates/hasura.json.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/templates/postgresql.sql.jinja` & `pymdg-1.2.0/mdg/templates/postgresql.sql.jinja`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_dumps.py` & `pymdg-1.2.0/mdg/tests/test_dumps.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_instance.py` & `pymdg-1.2.0/mdg/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_sample.py` & `pymdg-1.2.0/mdg/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_tools.py` & `pymdg-1.2.0/mdg/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_uml_model.py` & `pymdg-1.2.0/mdg/tests/test_uml_model.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tests/test_xmi_model_parse.py` & `pymdg-1.2.0/mdg/tests/test_xmi_model_parse.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/DrawIO MDG UML Library.xml` & `pymdg-1.2.0/mdg/tools/DrawIO MDG UML Library.xml`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/case.py` & `pymdg-1.2.0/mdg/tools/case.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/daemon.py` & `pymdg-1.2.0/mdg/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/filters.py` & `pymdg-1.2.0/mdg/tools/filters.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/io.py` & `pymdg-1.2.0/mdg/tools/io.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/mdg_tool.py` & `pymdg-1.2.0/mdg/tools/mdg_tool.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/tools/sparx_db_models_raw.py` & `pymdg-1.2.0/mdg/tools/sparx_db_models_raw.py`

 * *Files identical despite different names*

### Comparing `pymdg-1.1.0/mdg/uml/__init__.py` & `pymdg-1.2.0/mdg/uml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,43 +174,50 @@
     def __str__(self) -> str:
         return f"{self.name}"
 
 
 class UMLAssociation:
     id: Union[int, str]
     documentation: str
+    stereotypes: List[str]
 
     association_type: UMLAssociationType
     source: Union[UMLClass, UMLInstance, UMLComponent]
     source_name: Optional[str]
     source_multiplicity: Tuple[str, str]
+    source_stereotypes: List[str]
 
     destination: Union[UMLClass, UMLInstance, UMLComponent]
     destination_multiplicity: Tuple[str, str]
     destination_name: Optional[str]
+    destination_stereotypes: List[str]
+
 
     class Meta:
         id_field = 'id'
         owned_subobjects: List = []
 
     def __init__(self, package: UMLPackage, source: Union[UMLClass, UMLInstance, UMLComponent], destination: Union[UMLClass, UMLInstance, UMLComponent], id: Union[int, str], assoc_type=UMLAssociationType.ASSOCIATION):
         self.package: UMLPackage = package
         self.id = id
         self.documentation = ""
+        self.stereotypes = []
 
         self.association_type = assoc_type
         self.source = source
         self.source_name = None
         self.source_multiplicity = ('0', '0')
         source.associations_from.append(self)
+        self.source_stereotypes = []
 
         self.destination = destination
         self.destination_multiplicity = ('0', '0')
         self.destination_name = None
         destination.associations_to.append(self)
+        self.destination_stereotypes = []
 
     def __str__(self) -> str:
         return f"{self.source_name}({self.source_multiplicity}) -> {self.destination_name}({self.destination_multiplicity})"
 
     @property
     def cardinality(self):
         cardinality = None
@@ -383,15 +390,15 @@
 
 class UMLAttribute:
     parent: Union[UMLClass, UMLEnumeration, UMLComponent, UMLInstance]
     name: str
     alias: Optional[str]
     id: Union[int, str]
     is_unique: bool
-    stereotype: Optional[str]
+    stereotypes: List[str]
     classification: Optional[UMLClass]
     documentation: str
     type: Optional[str]
     value: Optional[str]
     visibility: bool
     is_id: bool
     length: int
@@ -405,15 +412,15 @@
 
     def __init__(self, parent: Union[UMLClass, UMLEnumeration, UMLComponent, UMLInstance], name: str, id: Union[int, str]):
         self.parent = parent
         self.name = name
         self.alias = None
         self.id = id
         self.is_unique = False
-        self.stereotype = None
+        self.stereotypes = []
         self.classification = None
         self.classification_id: Union[None, int, str] = None
         self.documentation = ""
         self.type = None
         self.dest_type: Optional[str] = None
         self.value = None
         self.visibility = True
```

### Comparing `pymdg-1.1.0/mdg/uml/validate.py` & `pymdg-1.2.0/mdg/uml/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         if cls.id_attribute is None and cls.generalization is None and not cls.is_abstract:
             errors.append(ClassValidationError(package, cls, "no primary key"))
         elif cls.generalization is not None:
             if cls.generalization.id_attribute is not None and cls.generalization.id_attribute != cls.id_attribute:
                 errors.append(ClassValidationError(package, cls, "primary key in both class and generalization class"))
 
         for attr in cls.attributes:
-            if attr.stereotype == "auto" and attr.type not in ("int", "bigint"):
+            if "auto" in attr.stereotypes and attr.type not in ("int", "bigint"):
                 errors.append(AttributeValidationError(package, cls, attr, "auto increment field must be int or bigint"))
 
     for child in package.children:
         errors += validate_package(child)
 
     return errors
```

### Comparing `pymdg-1.1.0/pymdg.egg-info/PKG-INFO` & `pymdg-1.2.0/pymdg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymdg
-Version: 1.1.0
+Version: 1.2.0
 Summary: Model driven genration - from UML to Code & Docs
 Home-page: https://github.com/semprini/pyMDG
 Author: Semprini
 Author-email: dont@contact.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -78,15 +78,15 @@
 ![Nomenclature](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_9100ADB5_EFF8_4ded_BA61_E8564C8134AC.png)
 
 ## Sample model
 ![Sample model](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_96AC850E_2FD0_4e6c_B00E_C030EDA89F42.png)
 
 ## Metamodel
 This diagram shows the internal classes which are passed to the templates during generation.
-![Metamodel](https://github.com/Semprini/pyMDG/raw/master/sample_recipes/images/EAID_B080F856_9EFB_46f2_8D69_1C79956D714A.png)
+![Metamodel](https://raw.githubusercontent.com/Semprini/pyMDG/master/docs/_static/image/metamodel.png)
 
 ## Build the docs
 Install sphinx
 ```
  > cd pyMDG
  > sphinx-apidoc -o docs\source mdg
  > cd docs
```

### Comparing `pymdg-1.1.0/pymdg.egg-info/SOURCES.txt` & `pymdg-1.2.0/pymdg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 mdg/templates/Django/project/urls.py.jinja
 mdg/templates/Django/project/validators.py.jinja
 mdg/templates/Django/project/views.py
 mdg/templates/Django/project/wsgi.py.jinja
 mdg/templates/Java/entities.jdl.jinja
 mdg/templates/Java/enums.java.jinja
 mdg/templates/Java/pojos.java.jinja
+mdg/templates/Python/dataclass_avro.py.jinja
 mdg/templates/SQLAlchemy/models.py.jinja
 mdg/templates/SQLAlchemy/schemas.py.jinja
 mdg/templates/Schema/avro.avsc.jinja
 mdg/templates/Schema/openapi.yaml.jinja
 mdg/tests/__init__.py
 mdg/tests/test_dumps.py
 mdg/tests/test_instance.py
```

### Comparing `pymdg-1.1.0/setup.py` & `pymdg-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='pymdg',
-    version='1.1.0',
+    version='1.2.0',
     author='Semprini',
     author_email='dont@contact.me',
     description='Model driven genration - from UML to Code & Docs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/semprini/pyMDG',
     packages=["mdg", ] + pymdg_packages,
```

