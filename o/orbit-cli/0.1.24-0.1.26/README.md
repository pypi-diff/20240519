# Comparing `tmp/orbit_cli-0.1.24.tar.gz` & `tmp/orbit_cli-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_cli-0.1.24.tar", max compression
+gzip compressed data, was "orbit_cli-0.1.26.tar", max compression
```

## Comparing `orbit_cli-0.1.24.tar` & `orbit_cli-0.1.26.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rwxr-xr-x   0        0        0     1087 2023-06-23 17:10:40.962145 orbit_cli-0.1.24/LICENSE.md
--rw-r--r--   0        0        0      349 2023-06-24 10:20:43.997010 orbit_cli-0.1.24/README.md
--rwxr-xr-x   0        0        0     1227 2023-08-26 17:22:30.118387 orbit_cli-0.1.24/orbit_cli/__main__.py
--rw-r--r--   0        0        0    16766 2023-08-22 17:49:09.349838 orbit_cli-0.1.24/orbit_cli/cli_application.py
--rw-r--r--   0        0        0     4821 2023-08-18 12:59:20.888080 orbit_cli-0.1.24/orbit_cli/cli_common.py
--rw-r--r--   0        0        0     3144 2023-08-22 13:04:48.700605 orbit_cli-0.1.24/orbit_cli/cli_main.py
--rw-r--r--   0        0        0     3533 2023-08-03 12:10:07.016737 orbit_cli-0.1.24/orbit_cli/cli_utils.py
--rw-r--r--   0        0        0       47 2023-08-03 11:46:12.229998 orbit_cli-0.1.24/orbit_cli/templates/application/.gitignore
--rw-r--r--   0        0        0       48 2023-08-03 11:46:12.229998 orbit_cli-0.1.24/orbit_cli/templates/application/.version
--rw-r--r--   0        0        0      848 2023-08-03 11:46:12.229998 orbit_cli-0.1.24/orbit_cli/templates/application/Makefile
--rw-r--r--   0        0        0       61 2023-08-03 11:46:12.229998 orbit_cli-0.1.24/orbit_cli/templates/application/README.md
--rw-r--r--   0        0        0      197 2023-08-03 11:46:12.229998 orbit_cli-0.1.24/orbit_cli/templates/application/apt/DEBIAN/control
--rwxr-xr-x   0        0        0      245 2023-08-21 13:13:23.792091 orbit_cli-0.1.24/orbit_cli/templates/application/apt/DEBIAN/postinst
--rw-r--r--   0        0        0      276 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/apt/etc/systemd/system/project.service
--rw-r--r--   0        0        0     1500 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/apt/opt/service/scripts/make_keys.sh
--rw-r--r--   0        0        0      285 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/client/App.vue
--rw-r--r--   0        0        0      186 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/client/Makefile
--rw-r--r--   0        0        0      339 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/client/index.html
--rw-r--r--   0        0        0     1029 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/client/main.css
--rw-r--r--   0        0        0      908 2023-08-16 12:45:33.532147 orbit_cli-0.1.24/orbit_cli/templates/application/client/main.js
--rw-r--r--   0        0        0     1092 2023-08-18 12:15:13.378582 orbit_cli-0.1.24/orbit_cli/templates/application/client/package.json
--rw-r--r--   0        0        0      918 2023-08-16 12:48:20.265124 orbit_cli-0.1.24/orbit_cli/templates/application/client/vite.config.js
--rw-r--r--   0        0        0     4286 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/common/favicon.ico
--rw-r--r--   0        0        0       67 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/common/fonts.txt
--rwxr-xr-x   0        0        0    10903 2023-08-03 11:46:12.233998 orbit_cli-0.1.24/orbit_cli/templates/application/common/orbit-logo.png
--rw-r--r--   0        0        0        7 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/scripts/VERSION
--rwxr-xr-x   0        0        0     1400 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/scripts/roll_version.py
--rw-r--r--   0        0        0      555 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/Makefile
--rw-r--r--   0        0        0       61 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/README.md
--rw-r--r--   0        0        0      138 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/__main__.py
--rw-r--r--   0        0        0     1500 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/make_keys.sh
--rw-r--r--   0        0        0     1222 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/orbit.spec
--rw-r--r--   0        0        0      847 2023-08-18 12:33:01.363514 orbit_cli-0.1.24/orbit_cli/templates/application/server/pyproject.toml
--rw-r--r--   0        0        0       21 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/application/server/version.py
--rw-r--r--   0        0        0       29 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/.gitignore
--rw-r--r--   0        0        0       48 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/.version
--rw-r--r--   0        0        0      214 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/Makefile
--rw-r--r--   0        0        0       61 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/README.md
--rw-r--r--   0        0        0        0 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/client/Makefile
--rw-r--r--   0        0        0       81 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/client/index.js
--rw-r--r--   0        0        0     2872 2023-08-16 12:54:24.126529 orbit_cli-0.1.24/orbit_cli/templates/component/client/main.vue
--rw-r--r--   0        0        0     2445 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/client/main_old.vue
--rw-r--r--   0        0        0      895 2023-08-03 11:46:12.237998 orbit_cli-0.1.24/orbit_cli/templates/component/client/main_old2.vue
--rw-r--r--   0        0        0      612 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/client/menu.js
--rw-r--r--   0        0        0      735 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/client/mytableStore.js
--rw-r--r--   0        0        0     1019 2023-08-17 16:41:01.146770 orbit_cli-0.1.24/orbit_cli/templates/component/client/package.json
--rw-r--r--   0        0        0      911 2023-08-17 16:42:08.237453 orbit_cli-0.1.24/orbit_cli/templates/component/client/vite.config.js
--rwxr-xr-x   0        0        0     1400 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/scripts/roll_version.py
--rw-r--r--   0        0        0        0 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/server/Makefile
--rw-r--r--   0        0        0      653 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/server/MyTable.py
--rw-r--r--   0        0        0       61 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/server/README.md
--rw-r--r--   0        0        0      100 2023-08-25 15:25:34.081962 orbit_cli-0.1.24/orbit_cli/templates/component/server/__init__.py
--rw-r--r--   0        0        0      474 2023-08-25 15:26:53.548241 orbit_cli-0.1.24/orbit_cli/templates/component/server/plugin.py
--rw-r--r--   0        0        0      791 2023-08-03 11:46:12.241998 orbit_cli-0.1.24/orbit_cli/templates/component/server/pyproject.toml
--rw-r--r--   0        0        0      573 2023-08-26 17:22:30.118387 orbit_cli-0.1.24/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 orbit_cli-0.1.24/PKG-INFO
+-rwxr-xr-x   0        0        0     1087 2024-05-19 16:24:26.404514 orbit_cli-0.1.26/LICENSE.md
+-rw-r--r--   0        0        0      349 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/README.md
+-rwxr-xr-x   0        0        0     1227 2024-05-19 16:27:08.265468 orbit_cli-0.1.26/orbit_cli/__main__.py
+-rw-r--r--   0        0        0    16766 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/cli_application.py
+-rw-r--r--   0        0        0     4836 2024-05-19 16:23:36.976225 orbit_cli-0.1.26/orbit_cli/cli_common.py
+-rw-r--r--   0        0        0     3144 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/cli_main.py
+-rw-r--r--   0        0        0     3533 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/cli_utils.py
+-rw-r--r--   0        0        0       47 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/templates/application/.gitignore
+-rw-r--r--   0        0        0       48 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/templates/application/.version
+-rw-r--r--   0        0        0      848 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/templates/application/Makefile
+-rw-r--r--   0        0        0       61 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/templates/application/README.md
+-rw-r--r--   0        0        0      197 2024-05-19 16:10:57.827852 orbit_cli-0.1.26/orbit_cli/templates/application/apt/DEBIAN/control
+-rwxr-xr-x   0        0        0      245 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/apt/DEBIAN/postinst
+-rw-r--r--   0        0        0      276 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/apt/etc/systemd/system/project.service
+-rw-r--r--   0        0        0     1500 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/apt/opt/service/scripts/make_keys.sh
+-rw-r--r--   0        0        0      285 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/App.vue
+-rw-r--r--   0        0        0      186 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/Makefile
+-rw-r--r--   0        0        0      339 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/index.html
+-rw-r--r--   0        0        0     1029 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/main.css
+-rw-r--r--   0        0        0      908 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/main.js
+-rw-r--r--   0        0        0     1092 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/package.json
+-rw-r--r--   0        0        0      918 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/client/vite.config.js
+-rw-r--r--   0        0        0     4286 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/common/favicon.ico
+-rw-r--r--   0        0        0       67 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/common/fonts.txt
+-rwxr-xr-x   0        0        0    10903 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/common/orbit-logo.png
+-rw-r--r--   0        0        0        7 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/scripts/VERSION
+-rwxr-xr-x   0        0        0     1400 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/scripts/roll_version.py
+-rw-r--r--   0        0        0      555 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/server/Makefile
+-rw-r--r--   0        0        0       61 2024-05-19 16:10:57.831852 orbit_cli-0.1.26/orbit_cli/templates/application/server/README.md
+-rw-r--r--   0        0        0      138 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/application/server/__main__.py
+-rw-r--r--   0        0        0     1500 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/application/server/make_keys.sh
+-rw-r--r--   0        0        0     1222 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/application/server/orbit.spec
+-rw-r--r--   0        0        0      847 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/application/server/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/application/server/version.py
+-rw-r--r--   0        0        0       29 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/.gitignore
+-rw-r--r--   0        0        0       48 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/.version
+-rw-r--r--   0        0        0      214 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/Makefile
+-rw-r--r--   0        0        0       61 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/client/Makefile
+-rw-r--r--   0        0        0       81 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/client/index.js
+-rw-r--r--   0        0        0     2872 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/client/main.vue
+-rw-r--r--   0        0        0     2445 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/client/main_old.vue
+-rw-r--r--   0        0        0      612 2024-05-19 16:10:57.835852 orbit_cli-0.1.26/orbit_cli/templates/component/client/menu.js
+-rw-r--r--   0        0        0      735 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/client/mytableStore.js
+-rw-r--r--   0        0        0     1019 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/client/package.json
+-rw-r--r--   0        0        0      911 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/client/vite.config.js
+-rwxr-xr-x   0        0        0     1400 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/scripts/roll_version.py
+-rw-r--r--   0        0        0        0 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/Makefile
+-rw-r--r--   0        0        0      653 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/MyTable.py
+-rw-r--r--   0        0        0       61 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/README.md
+-rw-r--r--   0        0        0      100 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/__init__.py
+-rw-r--r--   0        0        0      474 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/plugin.py
+-rw-r--r--   0        0        0      791 2024-05-19 16:10:57.839852 orbit_cli-0.1.26/orbit_cli/templates/component/server/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-05-19 16:27:08.265468 orbit_cli-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 orbit_cli-0.1.26/PKG-INFO
```

### Comparing `orbit_cli-0.1.24/LICENSE.md` & `orbit_cli-0.1.26/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-## Copyright (c) 2023 Mad Penguin Consulting Ltd
+## Copyright (c) 2024 Mad Penguin Consulting Ltd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `orbit_cli-0.1.24/orbit_cli/__main__.py` & `orbit_cli-0.1.26/orbit_cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ██║   ██║██╔══██╗██╔══██╗██║   ██║╚════╝██║     ██║     ██║
 ╚██████╔╝██║  ██║██████╔╝██║   ██║      ╚██████╗███████╗██║
  ╚═════╝ ╚═╝  ╚═╝╚═════╝ ╚═╝   ╚═╝       ╚═════╝╚══════╝╚═╝"""
 from orbit_cli.cli_main import Main
 #
 #   Banner from "figlet -w200 -f 'ansi-shadow'"
 #
-__version__ = "0.1.24"
+__version__ = "0.1.26"
 #
 #   Entry point when run as an installed package
 #
 def main ():
     Main(__doc__, __version__).run()
 #
 #   Entry point when testing
```

### Comparing `orbit_cli-0.1.24/orbit_cli/cli_application.py` & `orbit_cli-0.1.26/orbit_cli/cli_application.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/cli_common.py` & `orbit_cli-0.1.26/orbit_cli/cli_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 f'pip install poetry')
             return False
         return True
 
     def ensure (self, name, test=None):        
         self.msg(f'Ensuring [bold]{name}[/bold] is set up ...')
         if test is None:
-            test = Path(f'.{name}').exists()
+            test = Path(f'~/.{name}').expanduser().exists()
         if test:
             return True
         yn = self.confirm (f'Unable to locate [bold]{name}[/bold], would you like to install it?')
         if not yn:
             self.error (f'Unable to continue without [bold]{name}[/bold]')
         return False
```

### Comparing `orbit_cli-0.1.24/orbit_cli/cli_main.py` & `orbit_cli-0.1.26/orbit_cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/cli_utils.py` & `orbit_cli-0.1.26/orbit_cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/Makefile` & `orbit_cli-0.1.26/orbit_cli/templates/application/Makefile`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/apt/opt/service/scripts/make_keys.sh` & `orbit_cli-0.1.26/orbit_cli/templates/application/apt/opt/service/scripts/make_keys.sh`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/client/main.css` & `orbit_cli-0.1.26/orbit_cli/templates/application/client/main.css`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/client/main.js` & `orbit_cli-0.1.26/orbit_cli/templates/application/client/main.js`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/client/package.json` & `orbit_cli-0.1.26/orbit_cli/templates/application/client/package.json`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/client/vite.config.js` & `orbit_cli-0.1.26/orbit_cli/templates/application/client/vite.config.js`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/common/favicon.ico` & `orbit_cli-0.1.26/orbit_cli/templates/application/common/favicon.ico`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/common/orbit-logo.png` & `orbit_cli-0.1.26/orbit_cli/templates/application/common/orbit-logo.png`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/scripts/roll_version.py` & `orbit_cli-0.1.26/orbit_cli/templates/application/scripts/roll_version.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/server/Makefile` & `orbit_cli-0.1.26/orbit_cli/templates/application/server/Makefile`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/server/make_keys.sh` & `orbit_cli-0.1.26/orbit_cli/templates/application/server/make_keys.sh`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/server/orbit.spec` & `orbit_cli-0.1.26/orbit_cli/templates/application/server/orbit.spec`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/application/server/pyproject.toml` & `orbit_cli-0.1.26/orbit_cli/templates/application/server/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/main.vue` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/main.vue`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/main_old.vue` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/main_old.vue`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/menu.js` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/menu.js`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/mytableStore.js` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/mytableStore.js`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/package.json` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/package.json`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/client/vite.config.js` & `orbit_cli-0.1.26/orbit_cli/templates/component/client/vite.config.js`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/scripts/roll_version.py` & `orbit_cli-0.1.26/orbit_cli/templates/component/scripts/roll_version.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/server/MyTable.py` & `orbit_cli-0.1.26/orbit_cli/templates/component/server/MyTable.py`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/orbit_cli/templates/component/server/pyproject.toml` & `orbit_cli-0.1.26/orbit_cli/templates/component/server/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbit_cli-0.1.24/pyproject.toml` & `orbit_cli-0.1.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-cli"
-version = "0.1.24"
+version = "0.1.26"
 description = "This tool aims to make things easier when you come to create a new application or a new component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_cli" }, {include = "orbit_cli/templates" }]
 
 [tool.poetry.dependencies]
```

### Comparing `orbit_cli-0.1.24/PKG-INFO` & `orbit_cli-0.1.26/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: orbit-cli
-Version: 0.1.24
+Version: 0.1.26
 Summary: This tool aims to make things easier when you come to create a new application or a new component
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Orbit-CLI
```

