# Comparing `tmp/flask_limiter-3.6.0.tar.gz` & `tmp/flask_limiter-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_limiter-3.6.0.tar", last modified: Sun Apr 21 22:38:26 2024, max compression
+gzip compressed data, was "flask_limiter-3.7.0.tar", last modified: Sun May 19 15:55:44 2024, max compression
```

## Comparing `flask_limiter-3.6.0.tar` & `flask_limiter-3.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/CONTRIBUTIONS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/Flask_Limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 22:38:26.000000 flask_limiter-3.6.0/Flask_Limiter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18530 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.976781 flask_limiter-3.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.980781 flask_limiter-3.6.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.980781 flask_limiter-3.6.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/colors.css
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/limiter.css
--rw-r--r--   0 runner    (1001) docker     (127)    27408 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/logo-og.png
--rw-r--r--   0 runner    (1001) docker     (127)    47774 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   183556 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/tap-icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/tap-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   161289 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/tap-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/_static/tap-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/flask_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/flask_limiter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    23575 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.984782 flask_limiter-3.6.0/flask_limiter/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/contrib/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    52581 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/flask_limiter/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.984782 flask_limiter-3.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-21 22:38:26.988782 flask_limiter-3.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:38:26.984782 flask_limiter-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    30248 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    29297 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_flask_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-04-21 22:38:22.000000 flask_limiter-3.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/CONTRIBUTIONS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/Flask_Limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 15:55:44.000000 flask_limiter-3.7.0/Flask_Limiter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.433184 flask_limiter-3.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.433184 flask_limiter-3.7.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.433184 flask_limiter-3.7.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/colors.css
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/limiter.css
+-rw-r--r--   0 runner    (1001) docker     (127)    27408 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/logo-og.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47774 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   183556 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/tap-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/tap-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   161289 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/tap-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/_static/tap-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/flask_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/flask_limiter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.437185 flask_limiter-3.7.0/flask_limiter/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52461 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/flask_limiter/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.437185 flask_limiter-3.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1414 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:55:44.441185 flask_limiter-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19080 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30248 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29297 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_flask_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-05-19 15:55:40.000000 flask_limiter-3.7.0/versioneer.py
```

### Comparing `flask_limiter-3.6.0/CLASSIFIERS` & `flask_limiter-3.7.0/CLASSIFIERS`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/Flask_Limiter.egg-info/PKG-INFO` & `flask_limiter-3.7.0/Flask_Limiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.6.0
+Version: 3.7.0
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask_limiter-3.6.0/Flask_Limiter.egg-info/SOURCES.txt` & `flask_limiter-3.7.0/Flask_Limiter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/HISTORY.rst` & `flask_limiter-3.7.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.7.0
+------
+Release Date: 2024-05-19
+
+* Bug fix
+
+  * Fix errors with concurrent access to internal exemption maps
+    during application startup.
+
 v3.6.0
 ------
 Release Date: 2024-04-21
 
 * Bug fix
 
   * Ensure `exempt` routes are exempt from meta limits as well
@@ -900,14 +909,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `flask_limiter-3.6.0/LICENSE.txt` & `flask_limiter-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/PKG-INFO` & `flask_limiter-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Limiter
-Version: 3.6.0
+Version: 3.7.0
 Summary: Rate limiting for flask applications
 Home-page: https://flask-limiter.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/flask-limiter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flask_limiter-3.6.0/README.rst` & `flask_limiter-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/Makefile` & `flask_limiter-3.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/logo-og.png` & `flask_limiter-3.7.0/doc/source/_static/logo-og.png`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/logo.png` & `flask_limiter-3.7.0/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/logo.svg` & `flask_limiter-3.7.0/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/tap-icon.ico` & `flask_limiter-3.7.0/doc/source/_static/tap-icon.ico`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/tap-icon.png` & `flask_limiter-3.7.0/doc/source/_static/tap-icon.png`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/tap-icon.svg` & `flask_limiter-3.7.0/doc/source/_static/tap-icon.svg`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/_static/tap-logo.png` & `flask_limiter-3.7.0/doc/source/_static/tap-logo.png`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/cli.rst` & `flask_limiter-3.7.0/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/conf.py` & `flask_limiter-3.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/configuration.rst` & `flask_limiter-3.7.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/development.rst` & `flask_limiter-3.7.0/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/index.rst` & `flask_limiter-3.7.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/recipes.rst` & `flask_limiter-3.7.0/doc/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/strategies.rst` & `flask_limiter-3.7.0/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/doc/source/theme_config.py` & `flask_limiter-3.7.0/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/flask_limiter/commands.py` & `flask_limiter-3.7.0/flask_limiter/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import itertools
 import time
 from functools import partial
-from typing import Any, Callable, Dict, Generator, List, Optional, Set, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+    cast,
+)
 from urllib.parse import urlparse
 
 import click
 from flask import Flask, current_app
 from flask.cli import with_appcontext
 from limits.strategies import RateLimiter
 from rich.console import Console, group
@@ -176,15 +187,15 @@
     elif path:
         adapter = app.url_map.bind("dev.null")
         parsed = urlparse(path)
         try:
             filter_endpoint, _ = adapter.match(
                 parsed.path, method=method, query_args=parsed.query
             )
-            return filter_endpoint
+            return cast(str, filter_endpoint)
         except NotFound:
             console.print(
                 f"[error]Error: {path} could not be matched to an endpoint[/error]"
             )
         except MethodNotAllowed:
             assert method
             console.print(
```

### Comparing `flask_limiter-3.6.0/flask_limiter/constants.py` & `flask_limiter-3.7.0/flask_limiter/constants.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/flask_limiter/errors.py` & `flask_limiter-3.7.0/flask_limiter/errors.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/flask_limiter/extension.py` & `flask_limiter-3.7.0/flask_limiter/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,20 +193,16 @@
         self._application_limits_exempt_when = application_limits_exempt_when
         self._application_limits_deduct_when = application_limits_deduct_when
         self._application_limits_cost = application_limits_cost
         self._in_memory_fallback = []
         self._in_memory_fallback_enabled = in_memory_fallback_enabled or (
             in_memory_fallback and len(in_memory_fallback) > 0
         )
-        self._route_exemptions: Dict[str, ExemptionScope] = defaultdict(
-            lambda: ExemptionScope.NONE
-        )
-        self._blueprint_exemptions: Dict[str, ExemptionScope] = defaultdict(
-            lambda: ExemptionScope.NONE
-        )
+        self._route_exemptions: Dict[str, ExemptionScope] = {}
+        self._blueprint_exemptions: Dict[str, ExemptionScope] = {}
         self._request_filters: List[Callable[[], bool]] = []
 
         self._headers_enabled = headers_enabled
         self._header_mapping = header_name_mapping or {}
         self._retry_after = retry_after
         self._strategy = strategy
         self._storage_uri = storage_uri
```

### Comparing `flask_limiter-3.6.0/flask_limiter/manager.py` & `flask_limiter-3.7.0/flask_limiter/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         return all_limits, decorated_limits
 
     def exemption_scope(
         self, app: flask.Flask, endpoint: Optional[str], blueprint: Optional[str]
     ) -> ExemptionScope:
         view_func = app.view_functions.get(endpoint or "", None)
         name = get_qualified_name(view_func) if view_func else ""
-        route_exemption_scope = self._route_exemptions[name]
+        route_exemption_scope = self._route_exemptions.get(name, ExemptionScope.NONE)
         blueprint_instance = app.blueprints.get(blueprint) if blueprint else None
 
         if not blueprint_instance:
             return route_exemption_scope
         else:
             assert blueprint
             (
@@ -157,15 +157,15 @@
             ):
                 for exemption in ancestor_exemption_scopes.values():
                     blueprint_exemption_scope |= exemption
             return route_exemption_scope | blueprint_exemption_scope
 
     def decorated_limits(self, callable_name: str) -> List[Limit]:
         limits = []
-        if not self._route_exemptions[callable_name]:
+        if not self._route_exemptions.get(callable_name, ExemptionScope.NONE):
             if callable_name in self._decorated_limits:
                 for group in self._decorated_limits[callable_name]:
                     try:
                         for limit in group:
                             limits.append(limit)
                     except ValueError as e:
                         self._logger.error(
@@ -202,15 +202,17 @@
                     )
                     if not (
                         blueprint_self_limits
                         and all(
                             limit.override_defaults for limit in blueprint_self_limits
                         )
                     )
-                    and not self._blueprint_exemptions[blueprint_name]
+                    and not self._blueprint_exemptions.get(
+                        blueprint_name, ExemptionScope.NONE
+                    )
                     & ExemptionScope.ANCESTORS
                     else blueprint_self_limits
                 )
                 if blueprint_limits:
                     for limit_group in blueprint_limits:
                         try:
                             limits.extend(
@@ -238,17 +240,22 @@
                             )
         return limits
 
     def _blueprint_exemption_scope(
         self, app: flask.Flask, blueprint_name: str
     ) -> Tuple[ExemptionScope, Dict[str, ExemptionScope]]:
         name = app.blueprints[blueprint_name].name
-        exemption = self._blueprint_exemptions[name] & ~(ExemptionScope.ANCESTORS)
+        exemption = self._blueprint_exemptions.get(name, ExemptionScope.NONE) & ~(
+            ExemptionScope.ANCESTORS
+        )
 
         ancestory = set(blueprint_name.split("."))
         ancestor_exemption = {
             k
             for k, f in self._blueprint_exemptions.items()
             if f & ExemptionScope.DESCENDENTS
         }.intersection(ancestory)
 
-        return exemption, {k: self._blueprint_exemptions[k] for k in ancestor_exemption}
+        return exemption, {
+            k: self._blueprint_exemptions.get(k, ExemptionScope.NONE)
+            for k in ancestor_exemption
+        }
```

### Comparing `flask_limiter-3.6.0/flask_limiter/util.py` & `flask_limiter-3.7.0/flask_limiter/util.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/flask_limiter/wrappers.py` & `flask_limiter-3.7.0/flask_limiter/wrappers.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/setup.cfg` & `flask_limiter-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/setup.py` & `flask_limiter-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_blueprints.py` & `flask_limiter-3.7.0/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_commands.py` & `flask_limiter-3.7.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_configuration.py` & `flask_limiter-3.7.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_context_manager.py` & `flask_limiter-3.7.0/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_decorators.py` & `flask_limiter-3.7.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_error_handling.py` & `flask_limiter-3.7.0/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_flask_ext.py` & `flask_limiter-3.7.0/tests/test_flask_ext.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_regressions.py` & `flask_limiter-3.7.0/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_storage.py` & `flask_limiter-3.7.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/tests/test_views.py` & `flask_limiter-3.7.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `flask_limiter-3.6.0/versioneer.py` & `flask_limiter-3.7.0/versioneer.py`

 * *Files identical despite different names*

