# Comparing `tmp/pnu_libgh-0.9.1.tar.gz` & `tmp/pnu_libgh-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu_libgh-0.9.1.tar", last modified: Sat May 18 17:20:17 2024, max compression
+gzip compressed data, was "pnu_libgh-0.9.2.tar", last modified: Sun May 19 18:20:56 2024, max compression
```

## Comparing `pnu_libgh-0.9.1.tar` & `pnu_libgh-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.510657 pnu_libgh-0.9.1/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-18 17:20:17.510624 pnu_libgh-0.9.1/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1509 2024-05-18 07:23:12.000000 pnu_libgh-0.9.1/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.507677 pnu_libgh-0.9.1/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1919 2024-05-18 17:20:15.000000 pnu_libgh-0.9.1/man/libgh.1.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2199 2024-05-18 17:20:15.000000 pnu_libgh-0.9.1/man/libgh.3.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-31 15:28:19.000000 pnu_libgh-0.9.1/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1313 2024-05-18 17:20:17.511367 pnu_libgh-0.9.1/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.506778 pnu_libgh-0.9.1/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.509077 pnu_libgh-0.9.1/src/libgh/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-31 15:28:19.000000 pnu_libgh-0.9.1/src/libgh/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2296 2024-05-18 12:44:12.000000 pnu_libgh-0.9.1/src/libgh/accounts.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      510 2024-05-06 09:38:42.000000 pnu_libgh-0.9.1/src/libgh/common.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    14845 2024-05-18 15:25:02.000000 pnu_libgh-0.9.1/src/libgh/libpnu2.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     6855 2024-05-18 17:19:57.000000 pnu_libgh-0.9.1/src/libgh/main.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     9912 2024-05-18 15:35:18.000000 pnu_libgh-0.9.1/src/libgh/organization_account.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    13542 2024-05-18 15:50:32.000000 pnu_libgh-0.9.1/src/libgh/personal_account.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7924 2024-05-18 15:14:50.000000 pnu_libgh-0.9.1/src/libgh/repositories.py
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.510361 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)      481 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       54 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/entry_points.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       15 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/requires.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        6 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-19 18:20:56.550781 pnu_libgh-0.9.2/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-19 18:20:56.550748 pnu_libgh-0.9.2/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1509 2024-05-18 07:23:12.000000 pnu_libgh-0.9.2/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-19 18:20:56.547837 pnu_libgh-0.9.2/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1928 2024-05-19 18:20:54.000000 pnu_libgh-0.9.2/man/libgh.1.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2209 2024-05-19 18:20:54.000000 pnu_libgh-0.9.2/man/libgh.3.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-31 15:28:19.000000 pnu_libgh-0.9.2/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1313 2024-05-19 18:20:56.551490 pnu_libgh-0.9.2/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-19 18:20:56.546940 pnu_libgh-0.9.2/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-19 18:20:56.549274 pnu_libgh-0.9.2/src/libgh/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-31 15:28:19.000000 pnu_libgh-0.9.2/src/libgh/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2296 2024-05-18 12:44:12.000000 pnu_libgh-0.9.2/src/libgh/accounts.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      510 2024-05-06 09:38:42.000000 pnu_libgh-0.9.2/src/libgh/common.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    14845 2024-05-18 15:25:02.000000 pnu_libgh-0.9.2/src/libgh/libpnu2.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     6855 2024-05-19 16:51:26.000000 pnu_libgh-0.9.2/src/libgh/main.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    10116 2024-05-19 17:02:06.000000 pnu_libgh-0.9.2/src/libgh/organization_account.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    13585 2024-05-19 16:53:58.000000 pnu_libgh-0.9.2/src/libgh/personal_account.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7924 2024-05-18 15:14:50.000000 pnu_libgh-0.9.2/src/libgh/repositories.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-19 18:20:56.550494 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      481 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       54 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/entry_points.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       15 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/requires.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        6 2024-05-19 18:20:56.000000 pnu_libgh-0.9.2/src/pnu_libgh.egg-info/top_level.txt
```

### Comparing `pnu_libgh-0.9.1/PKG-INFO` & `pnu_libgh-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-libgh
-Version: 0.9.1
+Version: 0.9.2
 Summary: GitHub scraping library and tool
 Home-page: https://github.com/HubTou/libgh/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libgh/issues
 Keywords: pnu-project
```

### Comparing `pnu_libgh-0.9.1/README.md` & `pnu_libgh-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pnu_libgh-0.9.1/setup.cfg` & `pnu_libgh-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pnu-libgh
 description = GitHub scraping library and tool
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.9.1
+version = 0.9.2
 license = BSD 3-Clause License
 license_files = LICENSe
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/libgh/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/libgh/issues
```

### Comparing `pnu_libgh-0.9.1/src/libgh/accounts.py` & `pnu_libgh-0.9.2/src/libgh/accounts.py`

 * *Files identical despite different names*

### Comparing `pnu_libgh-0.9.1/src/libgh/libpnu2.py` & `pnu_libgh-0.9.2/src/libgh/libpnu2.py`

 * *Files identical despite different names*

### Comparing `pnu_libgh-0.9.1/src/libgh/main.py` & `pnu_libgh-0.9.2/src/libgh/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from .common import CACHE_DIR, CACHE_DAYS
 from .accounts import load_account, load_accounts
 from .repositories import load_repository, load_repositories
 from .libpnu2 import get_url_bdata, get_url_data, prune_cache, collection2xml
 
 # Version string used by the what(1) and ident(1) commands:
-ID = "@(#) $Id: libgh - GitHub scraping tool v0.9.1 (May 18, 2024) by Hubert Tournier $"
+ID = "@(#) $Id: libgh - GitHub scraping tool v0.9.2 (May 19, 2024) by Hubert Tournier $"
 
 # Default parameters. Can be overcome by environment variables, then command line options
 parameters = {
     "Prune cache": False,
     "Force fetching URL": False,
     "Cache days": CACHE_DAYS,
     "Complete partial": [],
```

### Comparing `pnu_libgh-0.9.1/src/libgh/organization_account.py` & `pnu_libgh-0.9.2/src/libgh/organization_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,35 +211,38 @@
                 account["social"]["url"].append(href)
             else:
                 account["social"]["url"] = [href]
 
     # repositories
     account["repositories"] = {}
     html = soup.select_one('[data-autosearch-results]')
-    number = html.text.split()[3]
-    try:
-        account["repositories_count"] = int(number)
-    except ValueError:
-        pass
-    account["repositories"] = load_org_repositories(
-        account_name,
-        cache_days,
-        force_fetch=force_fetch,
-        complete=complete
-    )
-    if len(account["repositories"]) != account["repositories_count"]:
-        account["repositories"].update(
-            load_org_repositories(
-                account_name,
-                cache_days,
-                force_fetch=force_fetch,
-                complete=complete,
-                repos_type="archived"
-            )
+    if html is not None:
+        number = html.text.split()[3]
+        try:
+            account["repositories_count"] = int(number)
+        except ValueError:
+            pass
+        account["repositories"] = load_org_repositories(
+            account_name,
+            cache_days,
+            force_fetch=force_fetch,
+            complete=complete
         )
+        if len(account["repositories"]) != account["repositories_count"]:
+            account["repositories"].update(
+                load_org_repositories(
+                    account_name,
+                    cache_days,
+                    force_fetch=force_fetch,
+                    complete=complete,
+                    repos_type="archived"
+                )
+            )
+    else:
+        account["repositories_count"] = 0
 
     # repositories stars (computed)
     stars = 0
     for repo in account["repositories"]:
         stars += account["repositories"][repo]["stargazers_count"]
     account["repositories_stars"] = stars
 
@@ -275,13 +278,14 @@
         most_used_topics.items(),
         key=lambda item: item[1],
         reverse=True
     ))
 
     if len(account["repositories"]) != account["repositories_count"]:
         logging.warning(
-            "libgh: Loaded %d/%d repositories",
+            "libgh: Loaded %d/%d repositories for account '%s'",
             len(account["repositories"]),
-            account["repositories_count"]
+            account["repositories_count"],
+            account_name
         )
 
     return account
```

### Comparing `pnu_libgh-0.9.1/src/libgh/personal_account.py` & `pnu_libgh-0.9.2/src/libgh/personal_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,13 +361,14 @@
         most_used_topics.items(),
         key=lambda item: item[1],
         reverse=True
     ))
 
     if len(account["repositories"]) != account["repositories_count"]:
         logging.warning(
-            "libgh: Loaded %d/%d repositories",
+            "libgh: Loaded %d/%d repositories for account '%s'",
             len(account["repositories"]),
-            account["repositories_count"]
+            account["repositories_count"],
+            account_name
         )
 
     return account
```

### Comparing `pnu_libgh-0.9.1/src/libgh/repositories.py` & `pnu_libgh-0.9.2/src/libgh/repositories.py`

 * *Files identical despite different names*

### Comparing `pnu_libgh-0.9.1/src/pnu_libgh.egg-info/PKG-INFO` & `pnu_libgh-0.9.2/src/pnu_libgh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-libgh
-Version: 0.9.1
+Version: 0.9.2
 Summary: GitHub scraping library and tool
 Home-page: https://github.com/HubTou/libgh/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libgh/issues
 Keywords: pnu-project
```

