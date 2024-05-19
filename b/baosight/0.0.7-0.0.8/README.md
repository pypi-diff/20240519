# Comparing `tmp/baosight-0.0.7.tar.gz` & `tmp/baosight-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baosight-0.0.7.tar", last modified: Sat May 18 18:57:56 2024, max compression
+gzip compressed data, was "baosight-0.0.8.tar", last modified: Sun May 19 03:15:31 2024, max compression
```

## Comparing `baosight-0.0.7.tar` & `baosight-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.581632 baosight-0.0.7/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1380 2024-05-18 18:57:56.581632 baosight-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-05-18 18:57:41.000000 baosight-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.549467 baosight-0.0.7/baosight/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.7/baosight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.574666 baosight-0.0.7/baosight/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.7/baosight/cli/__init__.py
--rw-rw-rw-   0        0        0     1409 2024-05-18 18:56:55.000000 baosight-0.0.7/baosight/cli/gl_runner.py
--rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.7/baosight/cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.578664 baosight-0.0.7/baosight/tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.7/baosight/tools/__init__.py
--rw-rw-rw-   0        0        0     4563 2024-05-18 17:44:00.000000 baosight-0.0.7/baosight/tools/gitlab_runner.py
--rw-rw-rw-   0        0        0     1593 2024-05-18 18:56:44.000000 baosight-0.0.7/baosight/tools/gitlab_runner_config_generator.py
--rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.7/baosight/tools/gitlab_runner_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-18 18:57:56.579663 baosight-0.0.7/baosight.egg-info/
--rw-rw-rw-   0        0        0     1380 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-18 18:57:55.000000 baosight-0.0.7/baosight.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 18:57:56.000000 baosight-0.0.7/baosight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2024-05-18 18:57:56.583666 baosight-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.822232 baosight-0.0.8/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1380 2024-05-19 03:15:31.821238 baosight-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-18 18:57:41.000000 baosight-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.729754 baosight-0.0.8/baosight/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.8/baosight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.786000 baosight-0.0.8/baosight/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.8/baosight/cli/__init__.py
+-rw-rw-rw-   0        0        0     1409 2024-05-18 18:56:55.000000 baosight-0.0.8/baosight/cli/gl_runner.py
+-rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.8/baosight/cli/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.817218 baosight-0.0.8/baosight/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.8/baosight/tools/__init__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-19 03:13:28.000000 baosight-0.0.8/baosight/tools/gitlab_runner.py
+-rw-rw-rw-   0        0        0     1593 2024-05-18 18:56:44.000000 baosight-0.0.8/baosight/tools/gitlab_runner_config_generator.py
+-rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.8/baosight/tools/gitlab_runner_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.819233 baosight-0.0.8/baosight.egg-info/
+-rw-rw-rw-   0        0        0     1380 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 03:15:30.000000 baosight-0.0.8/baosight.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2024-05-19 03:15:31.826237 baosight-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.8/setup.py
```

### Comparing `baosight-0.0.7/LICENSE` & `baosight-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/PKG-INFO` & `baosight-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.7
+Version: 0.0.8
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `baosight-0.0.7/README.md` & `baosight-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/baosight/cli/gl_runner.py` & `baosight-0.0.8/baosight/cli/gl_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/baosight/cli/main.py` & `baosight-0.0.8/baosight/cli/main.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/baosight/tools/gitlab_runner.py` & `baosight-0.0.8/baosight/tools/gitlab_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     runners = gl.runners.all()
     for runner in runners:
         if runner.description == description:
             print(f"Unregistering existing runner: {runner.id} - {runner.description}")
             runner.delete()
 
 
-def register_runner(gl, description, tags, registration_token):
+def register_runner(gl, runner_info, registration_token):
+    description = runner_info['description']
+    tags = runner_info['tags']
     """Register a new runner on GitLab."""
     unregister_existing_runners(gl, description)
     info = {
         'description': description,
         'active': True,
         'tag_list': tags,
         'run_untagged': True,
@@ -74,15 +76,17 @@
         'token': registration_token
     }
     runner = gl.runners.create(info)
     print(f"Runner ID: {runner.id}, Description: {description} registered.")
     return runner.token
 
 
-def setup_runner_on_windows(token, service_name, working_directory, gitlab_url):
+def setup_runner_on_windows(token, runner_info, gitlab_url):
+    service_name = runner_info['service']
+    working_directory = runner_info['work_dir']
     commands = [
         f"gitlab-runner stop --service {service_name}",
         f"gitlab-runner uninstall --service {service_name}",
         f"gitlab-runner install --service {service_name} --working-directory {working_directory}",
         f"gitlab-runner start --service {service_name}",
         f"gitlab-runner register --non-interactive --url {gitlab_url} "
         f"--shell cmd --token {token} --executor shell --locked false --run-untagged true --access-level not_protected"
@@ -111,23 +115,21 @@
     print("Script is running with administrator privileges.")
     download_gitlab_runner(RUNNER_URL)
     gl = gitlab.Gitlab(GITLAB_URL, private_token=GITLAB_API_TOKEN)
 
     for runner_info in runners:
         runner_token = register_runner(
             gl,
-            runner_info['description'],
-            runner_info['tags'],
+            runner_info,
             REGISTRATION_TOKEN
         )
         if not runner_token:
             raise Exception("Failed to register runner.")
         setup_runner_on_windows(
             runner_token,
-            runner_info['service'],
-            runner_info['work_dir'],
+            runner_info,
             GITLAB_URL
         )
 
 
 if __name__ == "__main__":
     deploy('./config.json')
```

### Comparing `baosight-0.0.7/baosight/tools/gitlab_runner_config_generator.py` & `baosight-0.0.8/baosight/tools/gitlab_runner_config_generator.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/baosight/tools/gitlab_runner_gui.py` & `baosight-0.0.8/baosight/tools/gitlab_runner_gui.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.7/baosight.egg-info/PKG-INFO` & `baosight-0.0.8/baosight.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.7
+Version: 0.0.8
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `baosight-0.0.7/setup.cfg` & `baosight-0.0.8/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 616f 7369 6768 740d 0a76 6572   = baosight..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6465  sion = 0.0.7..de
+00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6465  sion = 0.0.8..de
 00000030: 7363 7269 7074 696f 6e20 3d20 6261 6f73  scription = baos
 00000040: 6967 6874 2074 6f6f 6c73 0d0a 6c6f 6e67  ight tools..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
```

