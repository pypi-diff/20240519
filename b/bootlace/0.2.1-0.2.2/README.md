# Comparing `tmp/bootlace-0.2.1.tar.gz` & `tmp/bootlace-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 14 05:43:59 2024, max compression
+gzip compressed data, last modified: Sat May 18 16:54:05 2024, max compression
```

## Comparing `bootlace-0.2.1.tar` & `bootlace-0.2.2.tar`

### file list

```diff
@@ -1,79 +1,81 @@
--rw-r--r--   0        0        0      247 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/__about__.py
--rw-r--r--   0        0        0      384 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/__init__.py
--rw-r--r--   0        0        0      411 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/_version.py
--rw-r--r--   0        0        0     9054 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/breadcrumbs.py
--rw-r--r--   0        0        0     1447 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/extension.py
--rw-r--r--   0        0        0     1106 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/icon.py
--rw-r--r--   0        0        0      465 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/image.py
--rw-r--r--   0        0        0     2051 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/links.py
--rw-r--r--   0        0        0        0 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/py.typed
--rw-r--r--   0        0        0      669 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/size.py
--rw-r--r--   0        0        0     1217 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/style.py
--rw-r--r--   0        0        0    11020 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/util.py
--rw-r--r--   0        0        0        0 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/forms/__init__.py
--rw-r--r--   0        0        0     3037 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/forms/fields.py
--rw-r--r--   0        0        0      661 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/forms/widgets.py
--rw-r--r--   0        0        0     1571 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/forms/templates/bootlace/_form.html
--rw-r--r--   0        0        0      109 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/nav/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/nav/bar.py
--rw-r--r--   0        0        0     5442 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/nav/core.py
--rw-r--r--   0        0        0      427 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/nav/elements.py
--rw-r--r--   0        0        0     3197 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/nav/nav.py
--rw-r--r--   0        0        0    70330 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203179 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51796 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115988 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70404 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203183 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51871 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116065 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12066 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129328 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10127 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51370 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12059 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129343 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10199 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63944 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107824 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267492 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85353 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180382 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107692 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267433 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85282 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180218 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   280814 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.css
--rw-r--r--   0        0        0   679012 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.css.map
--rw-r--r--   0        0        0   232949 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   589162 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280393 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   678857 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   233056 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   588696 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0    88585 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.css
--rw-r--r--   0        0        0    47188 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.json
--rw-r--r--   0        0        0   211136 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   972584 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.svg
--rw-r--r--   0        0        0   207731 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444287 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80664 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331887 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135747 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305153 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74155 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222463 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145313 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.js
--rw-r--r--   0        0        0   306321 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    60578 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   220351 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0      299 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/table/__init__.py
--rw-r--r--   0        0        0     5096 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/table/base.py
--rw-r--r--   0        0        0     2353 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/table/columns.py
--rw-r--r--   0        0        0       67 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/testing/__init__.py
--rw-r--r--   0        0        0     4939 2024-05-14 05:43:59.000000 bootlace-0.2.1/src/bootlace/testing/html.py
--rw-r--r--   0        0        0     1222 2024-05-14 05:43:59.000000 bootlace-0.2.1/.gitignore
--rw-r--r--   0        0        0     1096 2024-05-14 05:43:59.000000 bootlace-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      478 2024-05-14 05:43:59.000000 bootlace-0.2.1/README.md
--rw-r--r--   0        0        0     2687 2024-05-14 05:43:59.000000 bootlace-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1323 2024-05-14 05:43:59.000000 bootlace-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/__about__.py
+-rw-r--r--   0        0        0      384 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/_version.py
+-rw-r--r--   0        0        0     6490 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/breadcrumbs.py
+-rw-r--r--   0        0        0     3278 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/endpoint.py
+-rw-r--r--   0        0        0     1179 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/extension.py
+-rw-r--r--   0        0        0     1042 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/icon.py
+-rw-r--r--   0        0        0      465 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/image.py
+-rw-r--r--   0        0        0     1777 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/links.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/py.typed
+-rw-r--r--   0        0        0     1207 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/resources.py
+-rw-r--r--   0        0        0      669 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/size.py
+-rw-r--r--   0        0        0     1217 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/style.py
+-rw-r--r--   0        0        0    11020 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/util.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/__init__.py
+-rw-r--r--   0        0        0     3037 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/fields.py
+-rw-r--r--   0        0        0      661 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/widgets.py
+-rw-r--r--   0        0        0     1571 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/forms/templates/bootlace/_form.html
+-rw-r--r--   0        0        0      109 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/bar.py
+-rw-r--r--   0        0        0     5781 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/core.py
+-rw-r--r--   0        0        0      427 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/elements.py
+-rw-r--r--   0        0        0     3197 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/nav/nav.py
+-rw-r--r--   0        0        0    70330 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203179 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51796 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115988 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70404 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203183 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51871 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116065 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12066 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129328 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10127 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51370 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12059 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129343 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10199 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63944 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107824 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267492 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85353 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180382 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107692 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267433 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85282 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180218 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280814 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.css
+-rw-r--r--   0        0        0   679012 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232949 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589162 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280393 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678857 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233056 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588696 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0    88585 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    47188 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.json
+-rw-r--r--   0        0        0   211136 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   972584 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207731 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444287 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80664 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331887 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305153 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74155 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222463 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306321 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60578 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220351 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0      303 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/__init__.py
+-rw-r--r--   0        0        0     5552 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/base.py
+-rw-r--r--   0        0        0     2862 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/table/columns.py
+-rw-r--r--   0        0        0       67 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/testing/__init__.py
+-rw-r--r--   0        0        0     4939 2024-05-18 16:54:05.000000 bootlace-0.2.2/src/bootlace/testing/html.py
+-rw-r--r--   0        0        0     1222 2024-05-18 16:54:05.000000 bootlace-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1096 2024-05-18 16:54:05.000000 bootlace-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      478 2024-05-18 16:54:05.000000 bootlace-0.2.2/README.md
+-rw-r--r--   0        0        0     2687 2024-05-18 16:54:05.000000 bootlace-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-05-18 16:54:05.000000 bootlace-0.2.2/PKG-INFO
```

### Comparing `bootlace-0.2.1/src/bootlace/extension.py` & `bootlace-0.2.2/src/bootlace/extension.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from flask import Blueprint
 from flask import current_app
 from flask import Flask
-from flask import url_for
+
+from .endpoint import Endpoint
+from bootlace.resources import Resources
 
 
 class Bootlace:
     """Flask extension for bootlace"""
 
     def __init__(self, app: Flask | None = None) -> None:
         if app is not None:
@@ -30,21 +32,11 @@
         app.register_blueprint(blueprint)
 
     @property
     def static_view(self) -> str:
         bp = current_app.config["BOOTLACE_BLUEPRINT_NAME"]
         return f"{bp}.static"
 
-    @property
-    def icons(self) -> str:
-        """The URL for the SVG source for the icons"""
-        return url_for(self.static_view, filename="icons/bootstrap-icons.svg")
-
-    @property
-    def css(self) -> str:
-        """The URL for the Bootstrap CSS file"""
-        return url_for(self.static_view, filename="css/bootstrap.min.css")
-
-    @property
-    def js(self) -> str:
-        """The URL for the Bootstrap JS file"""
-        return url_for(self.static_view, filename="js/bootstrap.min.js")
+    def bootstrap(self) -> "Resources":
+        return Resources(
+            endpoint=Endpoint.from_name(self.static_view), resources=["bootstrap.min.js", "bootstrap.min.css"]
+        )
```

### Comparing `bootlace-0.2.1/src/bootlace/icon.py` & `bootlace-0.2.2/src/bootlace/icon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from typing import ClassVar
 
 import attrs
 from dominate import svg as svg_tag
 from dominate.dom_tag import dom_tag
-from flask import url_for
 
+from bootlace.endpoint import Endpoint
 from bootlace.util import Tag
 
 
 __all__ = ["Icon"]
 
 
 @attrs.define
 class Icon:
     """A Bootstrap icon
 
     This class supports the :func:`as_tag` protocol to display itself.
     """
 
     #: Endpoint name for getting the Bootstrap Icon SVG file
-    endpoint: ClassVar[str] = "bootlace.static"
-
-    #: Filename for the Bootstrap Icon SVG file
-    filename: ClassVar[str] = "icons/bootstrap-icons.svg"
+    endpoint: ClassVar[Endpoint] = Endpoint.from_name("bootlace.static", filename="icons/bootstrap-icons.svg")
 
     #: Name of the icon
     name: str
 
     svg: Tag = Tag(
         svg_tag.svg,
         attributes={"role": "img", "fill": "currentColor", "width": "16", "height": "16"},
@@ -34,13 +31,13 @@
     )
 
     use: Tag = Tag(svg_tag.use)
 
     @property
     def url(self) -> str:
         """The URL for the SVG source for the icon"""
-        return url_for(self.endpoint, filename=self.filename, _anchor=self.name)
+        return self.endpoint(_anchor=self.name)
 
     def __tag__(self) -> dom_tag:
         return self.svg(
             self.use(xlink_href=self.url),
         )
```

### Comparing `bootlace-0.2.1/src/bootlace/links.py` & `bootlace-0.2.2/src/bootlace/links.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import abc
-from typing import Any
 
 import attrs
 from dominate import tags
-from flask import url_for
 
+from .endpoint import convert_endpoint
+from .endpoint import Endpoint
 from .util import as_tag
-from .util import is_active_endpoint
 from .util import MaybeTaggable
 from .util import Tag
 
 __all__ = ["Link", "View"]
 
 
 @attrs.define(kw_only=True, frozen=True)
@@ -53,27 +52,21 @@
 
 
 @attrs.define(kw_only=True, frozen=True)
 class View(LinkBase):
     """Link to a Flask view."""
 
     #: The endpoint to link to, for use with Flask's :func:`~flask.url_for`
-    endpoint: str
-
-    #: The keyword arguments to pass to :func:`~flask.url_for`
-    url_kwargs: dict[str, Any] = attrs.field(factory=dict)
-
-    #: Whether to ignore the query string when checking if the link is active
-    ignore_query: bool = True
+    endpoint: Endpoint = attrs.field(converter=convert_endpoint)
 
     #: Whether the link is enabled.
     enabled: bool = True
 
     @property
     def url(self) -> str:
         """The URL to link to, constructed using :func:`~flask.url_for`."""
-        return url_for(self.endpoint, **self.url_kwargs)
+        return self.endpoint.url
 
     @property
     def active(self) -> bool:
         """Whether the link is active, based on the current request endpoint."""
-        return is_active_endpoint(self.endpoint, self.url_kwargs, self.ignore_query)
+        return self.endpoint.active
```

### Comparing `bootlace-0.2.1/src/bootlace/size.py` & `bootlace-0.2.2/src/bootlace/size.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/style.py` & `bootlace-0.2.2/src/bootlace/style.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/util.py` & `bootlace-0.2.2/src/bootlace/util.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/forms/fields.py` & `bootlace-0.2.2/src/bootlace/forms/fields.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/forms/widgets.py` & `bootlace-0.2.2/src/bootlace/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/forms/templates/bootlace/_form.html` & `bootlace-0.2.2/src/bootlace/forms/templates/bootlace/_form.html`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/nav/bar.py` & `bootlace-0.2.2/src/bootlace/nav/bar.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/nav/core.py` & `bootlace-0.2.2/src/bootlace/nav/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from typing import Self
 
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
 
 from bootlace import links
-from bootlace.image import Image
+from bootlace.endpoint import Endpoint
 from bootlace.util import as_tag
 from bootlace.util import BootlaceWarning
 from bootlace.util import ids as element_id
+from bootlace.util import MaybeTaggable
 from bootlace.util import Tag
 
 
 class NavStyle(enum.Enum):
     """Styles for the nav element"""
 
     PLAIN = ""
@@ -105,31 +106,38 @@
 
     a: Tag = Tag(tags.a, classes={"nav-link"})
 
     def serialize(self) -> dict[str, Any]:
         data = super().serialize()
         data["link"] = attrs.asdict(self.link, filter=nav_serialize_filter)
         data["link"]["__type__"] = self.link.__class__.__name__
+
+        if "endpoint" in data["link"]:
+            data["link"]["endpoint"]["url_kwargs"] = dict(data["link"]["endpoint"]["url_kwargs"]["_arguments"])
+
         return data
 
     @classmethod
     def deserialize(cls, data: dict[str, Any]) -> Self:
         link_cls = getattr(links, data["link"].pop("__type__"))
+        if "endpoint" in data["link"]:
+            data["link"]["endpoint"] = Endpoint(**data["link"]["endpoint"])
+
         data["link"] = link_cls(**data["link"])
         return cls(**data)
 
     @classmethod
-    def with_url(cls, url: str, text: str | Image, **kwargs: Any) -> "Link":
+    def with_url(cls, url: str, text: MaybeTaggable, **kwargs: Any) -> "Link":
         """Create a link with a URL."""
         return cls(link=links.Link(url=url, text=text, **kwargs))
 
     @classmethod
-    def with_view(cls, endpoint: str, text: str | Image, **kwargs: Any) -> "Link":
+    def with_view(cls, endpoint: str, text: MaybeTaggable, **kwargs: Any) -> "Link":
         """Create a link with a view."""
-        return cls(link=links.View(endpoint=endpoint, text=text, **kwargs))
+        return cls(link=links.View(endpoint=Endpoint.from_name(endpoint, **kwargs), text=text))
 
     @property
     def active(self) -> bool:
         """Whether the link is active."""
         return self.link.active
 
     @property
```

### Comparing `bootlace-0.2.1/src/bootlace/nav/nav.py` & `bootlace-0.2.2/src/bootlace/nav/nav.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.min.css` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/css/bootstrap.rtl.min.css.map` & `bootlace-0.2.2/src/bootlace/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.css` & `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.json` & `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.scss` & `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/icons/bootstrap-icons.svg` & `bootlace-0.2.2/src/bootlace/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.min.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.bundle.min.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.min.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.esm.min.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.min.js` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/static/js/bootstrap.min.js.map` & `bootlace-0.2.2/src/bootlace/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/src/bootlace/table/base.py` & `bootlace-0.2.2/src/bootlace/table/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections.abc import Mapping
 from typing import Any
 from typing import ClassVar
 
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
+from dominate.util import text
 
 from bootlace.icon import Icon
 from bootlace.util import as_tag
 from bootlace.util import maybe
 from bootlace.util import Tag
 
 
@@ -51,17 +52,26 @@
     def __set_name__(self, owner: type, name: str) -> None:
         self.name = self.name or name
 
     @property
     def attribute(self) -> str:
         """The attribute name for the column."""
         if self.name is None:
-            raise ValueError("column must be named in Table or attribute= parameter must be provided")
+            raise ValueError("column must be named in Table or name= parameter must be provided")
         return self.name
 
+    def contents(self, value: Any, format: str | None = None) -> Any:
+        """Return the contents of the cell for the column, using an HTML comment if the attribute value is None."""
+        contents = getattr(value, self.attribute)
+        if contents is None:
+            return tags.comment(f"No value for {self.name}")
+        if format:
+            return text(format.format(contents))
+        return text(str(contents))
+
     @abstractmethod
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
         raise NotImplementedError("Subclasses must implement this method")
 
     def __th__(self) -> dom_tag:
         return self.th(as_tag(self.heading), scope="col", __pretty=False)
```

### Comparing `bootlace-0.2.1/src/bootlace/table/columns.py` & `bootlace-0.2.2/src/bootlace/table/columns.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 from typing import Any
 
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
 from dominate.util import text
-from flask import url_for
 
+from bootlace.endpoint import convert_endpoint
+from bootlace.endpoint import Endpoint
 from bootlace.icon import Icon
 from bootlace.table.base import ColumnBase
 from bootlace.util import as_tag
+from bootlace.util import MaybeTaggable
 from bootlace.util import Tag
 
-
-__all__ = ["Column", "EditColumn", "CheckColumn", "Datetime"]
+__all__ = ["Column", "ActionColumn", "CheckColumn", "Datetime"]
 
 
 @attrs.define
 class Column(ColumnBase):
     """A column in a table, which shows the value of an attribute.
 
-    No special formatting is applied to the attribute, it is rendered as text."""
+    If no special formatting is applied to the attribute, it is rendered as text.
+    """
+
+    format: str | None = attrs.field(default=None)
 
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
-        return text(str(getattr(value, self.attribute)))
-
-
-@attrs.define
-class EditColumn(ColumnBase):
-    """A column which links to an edit view for the value.
-
-    This is commonly shown as e.g. the name of the item, which links to the edit view."""
+        return self.contents(value)
 
-    #: The endpoint for the edit view
-    endpoint: str = attrs.field(default=".edit")
-
-    a: Tag = Tag(tags.a)
-
-    def cell(self, value: Any) -> tags.html_tag:
-        """Return the cell for the column as an HTML tag."""
-        id = getattr(value, "id", None)
-        return self.a(getattr(value, self.attribute), href=url_for(self.endpoint, id=id))
+    def contents(self, value: Any, format: str | None = None) -> dom_tag:
+        """Return the contents of the cell for the column, using an HTML comment if the attribute value is None."""
+        return super().contents(value, format or self.format)
 
 
 @attrs.define
 class CheckColumn(ColumnBase):
     """A column which shows a checkmark or X based on the value of the attribute."""
 
     #: The icon for a true value
@@ -72,7 +63,32 @@
 
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
         if self.format:
             return text(getattr(value, self.attribute).strftime(self.format))
 
         return text(getattr(value, self.attribute).isoformat())
+
+
+@attrs.define
+class ActionColumn(ColumnBase):
+    """
+    A column which links to a view for the value.
+
+    This is commonly shown as e.g. the name of the item, which links to the edit view.
+    """
+
+    endpoint: Endpoint = attrs.field(default=Endpoint.from_name(".edit"), converter=convert_endpoint)
+
+    label: MaybeTaggable = attrs.field(default=None)
+
+    a: Tag = Tag(tags.a)
+
+    def cell(self, value: Any) -> tags.html_tag:
+        id = getattr(value, "id", None)
+
+        if self.label is None:
+            contents = self.contents(value)
+        else:
+            contents = as_tag(self.label)
+
+        return self.a(contents, href=self.endpoint(id=id))
```

### Comparing `bootlace-0.2.1/src/bootlace/testing/html.py` & `bootlace-0.2.2/src/bootlace/testing/html.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/.gitignore` & `bootlace-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/LICENSE.txt` & `bootlace-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/pyproject.toml` & `bootlace-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootlace-0.2.1/PKG-INFO` & `bootlace-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bootlace
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pythonic Bootstrap Utilities
 Project-URL: Documentation, https://github.com/alexrudy/bootlace#readme
 Project-URL: Issues, https://github.com/alexrudy/bootlace/issues
 Project-URL: Source, https://github.com/alexrudy/bootlace
 Author-email: Alex Rudy <github@alexrudy.net>
 License-Expression: MIT
 License-File: LICENSE.txt
```

