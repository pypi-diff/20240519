# Comparing `tmp/ephemetoot-3.2.0.tar.gz` & `tmp/ephemetoot-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephemetoot-3.2.0.tar", last modified: Sun Jun 18 09:27:25 2023, max compression
+gzip compressed data, was "ephemetoot-3.2.1.tar", last modified: Sun May 19 02:38:55 2024, max compression
```

## Comparing `ephemetoot-3.2.0.tar` & `ephemetoot-3.2.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.998985 ephemetoot-3.2.0/
--rw-r--r--   0 hugh       (501) staff       (20)    32471 2020-04-20 00:45:02.000000 ephemetoot-3.2.0/LICENSE
--rw-r--r--   0 hugh       (501) staff       (20)        8 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/MANIFEST.in
--rw-r--r--   0 hugh       (501) staff       (20)     1684 2023-06-18 09:27:24.997801 ephemetoot-3.2.0/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)     1933 2023-06-18 08:57:42.000000 ephemetoot-3.2.0/README.md
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.989112 ephemetoot-3.2.0/ephemetoot/
--rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-26 03:20:29.000000 ephemetoot-3.2.0/ephemetoot/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)     5560 2023-06-18 05:01:12.000000 ephemetoot-3.2.0/ephemetoot/console.py
--rw-r--r--   0 hugh       (501) staff       (20)    23495 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/ephemetoot/ephemetoot.py
--rw-r--r--   0 hugh       (501) staff       (20)      780 2020-09-26 03:20:29.000000 ephemetoot-3.2.0/ephemetoot/plist.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.994967 ephemetoot-3.2.0/ephemetoot.egg-info/
--rw-r--r--   0 hugh       (501) staff       (20)     1684 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)      380 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/SOURCES.txt
--rw-r--r--   0 hugh       (501) staff       (20)        1 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/dependency_links.txt
--rw-r--r--   0 hugh       (501) staff       (20)       55 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/entry_points.txt
--rw-r--r--   0 hugh       (501) staff       (20)       65 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/requires.txt
--rw-r--r--   0 hugh       (501) staff       (20)       11 2023-06-18 09:27:24.000000 ephemetoot-3.2.0/ephemetoot.egg-info/top_level.txt
--rw-r--r--   0 hugh       (501) staff       (20)     1127 2023-06-18 08:57:33.000000 ephemetoot-3.2.0/pypi-readme.md
--rw-r--r--   0 hugh       (501) staff       (20)      885 2023-06-18 08:20:59.000000 ephemetoot-3.2.0/pyproject.toml
--rw-r--r--   0 hugh       (501) staff       (20)       38 2023-06-18 09:27:24.999325 ephemetoot-3.2.0/setup.cfg
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2023-06-18 09:27:24.995703 ephemetoot-3.2.0/tests/
--rw-r--r--   0 hugh       (501) staff       (20)    24002 2023-06-18 05:01:12.000000 ephemetoot-3.2.0/tests/test_ephemetoot.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2024-05-19 02:38:55.323978 ephemetoot-3.2.1/
+-rw-r--r--   0 hugh       (501) staff       (20)    32471 2020-04-20 00:45:02.000000 ephemetoot-3.2.1/LICENSE
+-rw-r--r--   0 hugh       (501) staff       (20)      169 2024-05-19 02:25:35.000000 ephemetoot-3.2.1/MANIFEST.in
+-rw-r--r--   0 hugh       (501) staff       (20)     1962 2024-05-19 02:38:55.323762 ephemetoot-3.2.1/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)     1937 2024-05-19 02:24:46.000000 ephemetoot-3.2.1/README.md
+-rw-r--r--   0 hugh       (501) staff       (20)     1620 2021-08-23 05:28:50.000000 ephemetoot-3.2.1/example-config.yaml
+-rw-r--r--   0 hugh       (501) staff       (20)     1269 2024-05-19 02:24:56.000000 ephemetoot-3.2.1/pypi-readme.md
+-rw-r--r--   0 hugh       (501) staff       (20)      890 2024-05-19 02:25:56.000000 ephemetoot-3.2.1/pyproject.toml
+-rw-r--r--   0 hugh       (501) staff       (20)       38 2024-05-19 02:38:55.324022 ephemetoot-3.2.1/setup.cfg
+-rw-r--r--   0 hugh       (501) staff       (20)       38 2024-05-19 02:34:14.000000 ephemetoot-3.2.1/setup.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2024-05-19 02:38:55.319359 ephemetoot-3.2.1/src/
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2024-05-19 02:38:55.321739 ephemetoot-3.2.1/src/ephemetoot/
+-rw-r--r--   0 hugh       (501) staff       (20)        0 2020-09-26 03:20:29.000000 ephemetoot-3.2.1/src/ephemetoot/__init__.py
+-rw-r--r--   0 hugh       (501) staff       (20)     5560 2023-01-15 04:52:46.000000 ephemetoot-3.2.1/src/ephemetoot/console.py
+-rw-r--r--   0 hugh       (501) staff       (20)    23494 2024-05-19 02:34:14.000000 ephemetoot-3.2.1/src/ephemetoot/ephemetoot.py
+-rw-r--r--   0 hugh       (501) staff       (20)      780 2020-09-26 03:20:29.000000 ephemetoot-3.2.1/src/ephemetoot/plist.py
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2024-05-19 02:38:55.323435 ephemetoot-3.2.1/src/ephemetoot.egg-info/
+-rw-r--r--   0 hugh       (501) staff       (20)     1962 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/PKG-INFO
+-rw-r--r--   0 hugh       (501) staff       (20)      472 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/SOURCES.txt
+-rw-r--r--   0 hugh       (501) staff       (20)        1 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/dependency_links.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       55 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/entry_points.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       67 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/requires.txt
+-rw-r--r--   0 hugh       (501) staff       (20)       11 2024-05-19 02:38:55.000000 ephemetoot-3.2.1/src/ephemetoot.egg-info/top_level.txt
+drwxr-xr-x   0 hugh       (501) staff       (20)        0 2024-05-19 02:38:55.323215 ephemetoot-3.2.1/tests/
+-rw-r--r--   0 hugh       (501) staff       (20)    30126 2021-08-23 22:21:04.000000 ephemetoot-3.2.1/tests/accomplished.jpg
+-rw-r--r--   0 hugh       (501) staff       (20)    24031 2024-05-19 02:34:14.000000 ephemetoot-3.2.1/tests/test_ephemetoot.py
```

### Comparing `ephemetoot-3.2.0/LICENSE` & `ephemetoot-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.2.0/PKG-INFO` & `ephemetoot-3.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: ephemetoot
-Version: 3.2.0
+Version: 3.2.1
 Summary: A command line tool to delete your old toots
 Author-email: Hugh Rundle <ephemetoot@hugh.run>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://ephemetoot.hugh.run
 Project-URL: repository, https://github.com/hughrun/ephemetoot
 Keywords: mastodon,api,microblogging
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: mastodon.py>=1.8.1
+Requires-Dist: pyyaml>=6.0.1
+Provides-Extra: dev
+Requires-Dist: pytest>=6; extra == "dev"
 
 # 🥳 ==> 🧼 ==> 😇
 
+**As Mastodon now has similar functionality built in, `ephemetoot` is now in maintenance mode - no new features will be added, only security updates.**
+
 ## Prior work
 The initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)
 
 `ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)
 
 ## Usage
 
@@ -34,10 +40,10 @@
 
 Run from the command line with `ephemetoot`.
 
 Run `ephemetoot --help` or read the docs for all options.
 
 ## Contributing
 
-ephemetoot is now in maintenance mode, and new features will not be considered.
+ephemetoot is tested using `pytest`.
 
-For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
+For all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

### Comparing `ephemetoot-3.2.0/README.md` & `ephemetoot-3.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🥳 ==> 🧼 ==> 😇
 
 **ephemetoot** is a Python command line tool for deleting old toots.
 
-As Mastodon now has similar functionality built in, `ephemetoot` is now in maintenance mode - no new features will be added, only security updates.
+**As Mastodon now has similar functionality built in, `ephemetoot` is now in maintenance mode - no new features will be added, only security updates.**
 
 ## Quickstart
 
 You should have Python3 and pip installed, and an app access token on hand. More detail information is available in [the docs](https://ephemetoot.hugh.run)
 
 Install with pip:
 ```shell
```

### Comparing `ephemetoot-3.2.0/ephemetoot/console.py` & `ephemetoot-3.2.1/src/ephemetoot/console.py`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.2.0/ephemetoot/ephemetoot.py` & `ephemetoot-3.2.1/src/ephemetoot/ephemetoot.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,14 @@
         )
 
     except Exception as e:
         print("Something went wrong:", e)
 
 
 def schedule(options):
-
     """
     Creates and loads a plist file for scheduled running with launchd. If --time flag is used, the scheduled time is set accordingly. Note that this is designed for use on MacOS.
     """
     try:
 
         if options.schedule == ".":
             working_dir = os.getcwd()
```

### Comparing `ephemetoot-3.2.0/ephemetoot/plist.py` & `ephemetoot-3.2.1/src/ephemetoot/plist.py`

 * *Files identical despite different names*

### Comparing `ephemetoot-3.2.0/ephemetoot.egg-info/PKG-INFO` & `ephemetoot-3.2.1/src/ephemetoot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: ephemetoot
-Version: 3.2.0
+Version: 3.2.1
 Summary: A command line tool to delete your old toots
 Author-email: Hugh Rundle <ephemetoot@hugh.run>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://ephemetoot.hugh.run
 Project-URL: repository, https://github.com/hughrun/ephemetoot
 Keywords: mastodon,api,microblogging
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: mastodon.py>=1.8.1
+Requires-Dist: pyyaml>=6.0.1
+Provides-Extra: dev
+Requires-Dist: pytest>=6; extra == "dev"
 
 # 🥳 ==> 🧼 ==> 😇
 
+**As Mastodon now has similar functionality built in, `ephemetoot` is now in maintenance mode - no new features will be added, only security updates.**
+
 ## Prior work
 The initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)
 
 `ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)
 
 ## Usage
 
@@ -34,10 +40,10 @@
 
 Run from the command line with `ephemetoot`.
 
 Run `ephemetoot --help` or read the docs for all options.
 
 ## Contributing
 
-ephemetoot is now in maintenance mode, and new features will not be considered.
+ephemetoot is tested using `pytest`.
 
-For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
+For all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

### Comparing `ephemetoot-3.2.0/pypi-readme.md` & `ephemetoot-3.2.1/pypi-readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # 🥳 ==> 🧼 ==> 😇
 
+**As Mastodon now has similar functionality built in, `ephemetoot` is now in maintenance mode - no new features will be added, only security updates.**
+
 ## Prior work
 The initial `ephemetoot` script was based on [this tweet-deleting script](https://gist.github.com/flesueur/bcb2d9185b64c5191915d860ad19f23f) by [@flesueur](https://github.com/flesueur)
 
 `ephemetoot` relies heavily on the [Mastodon.py](https://pypi.org/project/Mastodon.py/) package by [@halcy](https://github.com/halcy)
 
 ## Usage
 
@@ -17,10 +19,10 @@
 
 Run from the command line with `ephemetoot`.
 
 Run `ephemetoot --help` or read the docs for all options.
 
 ## Contributing
 
-ephemetoot is now in maintenance mode, and new features will not be considered.
+ephemetoot is tested using `pytest`.
 
-For bugs or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
+For all bugs, suggestions, pull requests or other contributions, please check the [contributing guide](https://github.com/hughrun/ephemetoot/blob/master/docs/contributing.md).
```

### Comparing `ephemetoot-3.2.0/pyproject.toml` & `ephemetoot-3.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ephemetoot"
-version = "3.2.0"
+version = "3.2.1"
 description = "A command line tool to delete your old toots"
 requires-python = ">=3.8"
 authors = [
     {name = "Hugh Rundle", email = "ephemetoot@hugh.run"}
     ]
 license = { text = "GPL-3.0-or-later"}
 readme = "pypi-readme.md"
@@ -12,27 +12,27 @@
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Communications"
 ]
 dependencies = [
     "requests>=2.31.0",
-    "mastodon.py>=1.4.3",
-    "pyyaml>=5.0"
+    "mastodon.py>=1.8.1",
+    "pyyaml>=6.0.1"
 ]
 
 [project.optional-dependencies]
 dev = ["pytest>=6"]
 
 [project.scripts]
 ephemetoot = 'ephemetoot.console:main'
 
 [project.urls]
 homepage = "https://ephemetoot.hugh.run"
 repository = "https://github.com/hughrun/ephemetoot"
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools]
-packages = ["ephemetoot"]
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `ephemetoot-3.2.0/tests/test_ephemetoot.py` & `ephemetoot-3.2.1/tests/test_ephemetoot.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,33 +63,34 @@
         "emojis": [],
         "fields": [
             {"name": "Fully", "value": "Automated", "verified_at": None},
             {"name": "Luxury", "value": "Communism", "verified_at": None},
         ],
     },
     "media_attachments": [
-      {
-        "id": 123456789987654321,
-        "type": "image",
-        "url": "https://hugh.run/success/accomplished.jpg"
-      }
+        {
+            "id": 123456789987654321,
+            "type": "image",
+            "url": "https://hugh.run/success/accomplished.jpg",
+        }
     ],
     "mentions": [],
     "tags": [],
     "emojis": [],
     "card": None,
     "poll": None,
 }
 
 # Turn dict into object needed by mastodon.py
 # Use this in tests after making any changes
 # you need to your dict object
 # NOTE: ensure values in the dict object are what you need:
 # it can be mutated by any test before your test runs
 
+
 def dict2obj(d):
     # checking whether object d is a
     # instance of class list
     if isinstance(d, list):
         d = [dict2obj(x) for x in d]
 
     # if d is not a instance of dict then
@@ -120,27 +121,28 @@
     "base_url": "test.social",
     "hashtags_to_keep": ["ephemetoot"],
     "days_to_keep": 14,
     "keep_pinned": True,
     "toots_to_keep": [103996285277439262, 103976473612749097, 103877521458738491],
     "visibility_to_keep": [],
     "archive": "archive",
-    "archive_media": False
+    "archive_media": False,
 }
 
+
 # mock GitHub API call for the version number
 class MockGitHub:
     @staticmethod
     def json():
         return {"tag_name": "vLATEST_VERSION"}
 
 
 # mock image call for archive
 class MockMedia:
-    f = open('tests/accomplished.jpg', 'rb')
+    f = open("tests/accomplished.jpg", "rb")
     content = f.read()
     f.close()
 
 
 # mock Mastodon
 class Mocktodon:
     def __init__(self):
@@ -219,14 +221,15 @@
 @pytest.fixture
 def mock_archive_response(monkeypatch):
     def mock_get(*args, **kwargs):
         return MockMedia()
 
     monkeypatch.setattr(requests, "get", mock_get)
 
+
 ########################
 #         TESTS        #
 ########################
 
 # Tests should be listed in alphabetical order
 # Remember that a previous test may have mutated
 # one of the values above: set all values you are using
@@ -237,23 +240,25 @@
     config_file["archive"] = str(p)  # make archive directory a temp test dir
 
     ephemetoot.archive_toot(config_file, toot)
 
     file_exists = os.path.exists(p + "/104136090490756999.json")
     assert file_exists
 
+
 def test_archive_toot_media(mock_archive_response, tmpdir):
     p = tmpdir.mkdir("archive")
     config_file["archive"] = str(p)  # make archive directory a temp test dir
     config_file["archive_media"] = True
     ephemetoot.archive_toot_media(p, toot.media_attachments[0].url)
     image_exists = os.path.exists(p + "/hugh.run/success/accomplished.jpg")
     config_file["archive_media"] = False
     assert image_exists
 
+
 def test_check_batch(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False)
     mastodon = Mocktodon()
     user_id = "test_user_id"
     # limit to 2 so check_batch calls itself for the last 8 toots
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=0)
@@ -265,14 +270,15 @@
     )
     # run check_batch
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 10
     output = capfd.readouterr().out.split("\n")
     assert output[0] == "Removed 10 toots for alice@test.social."
 
+
 def test_check_batch_quiet(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False, quiet=1)
     mastodon = Mocktodon()
     user_id = "test_user_id"
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=0)
     monkeypatch.setattr(
@@ -280,14 +286,15 @@
         lambda config, options, mastodon, toot, deleted_count: deleted_count + 1,
     )
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 10
     output = capfd.readouterr().out.split("\n")
     assert output[0] == "Removed 10 toots for alice@test.social."
 
+
 def test_check_batch_quiet_no_toots(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False, quiet=2)
     mastodon = Mocktodon()
     user_id = "test_user_id"
     # max_id is the last toot in our batch so this returns no toots
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=10)
@@ -297,14 +304,15 @@
     )
     # run check_batch
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 0 but with quiet=2 there should be not output
     output = capfd.readouterr().out
     assert output == ""
 
+
 def test_check_batch_qq(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False, quiet=2)
     mastodon = Mocktodon()
     user_id = "test_user_id"
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=0)
     monkeypatch.setattr(
@@ -312,14 +320,15 @@
         lambda config, options, mastodon, toot, deleted_count: deleted_count + 1,
     )
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 10 and message printed since there was a delete
     output = capfd.readouterr().out.split("\n")
     assert output[0] == "Removed 10 toots for alice@test.social."
 
+
 def test_check_batch_qq_no_deletes(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False, quiet=2)
     mastodon = Mocktodon()
     user_id = "quiet_user_id"
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=0)
     # simulate no deletes occuring
@@ -329,14 +338,15 @@
     )
     # run check_batch
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 0 with no message since quiet=2
     output = capfd.readouterr().out
     assert output == ""
 
+
 def test_check_batch_qqq(capfd, monkeypatch):
     config = config_file
     options = Namespace(archive_deleted=False, quiet=3)
     mastodon = Mocktodon()
     user_id = "test_user_id"
     timeline = mastodon.account_statuses(user_id=user_id, limit=2, max_id=0)
     monkeypatch.setattr(
@@ -345,14 +355,15 @@
     )
     # run check_batch
     ephemetoot.check_batch(config, options, mastodon, user_id, timeline, 0)
     # deleted_count should be 10 and no message should be printed since quiet=3
     output = capfd.readouterr().out
     assert output == ""
 
+
 def test_console_print(capfd):
     ephemetoot.console_print(
         "test123", Namespace(test=False, hide_skipped=False, quiet=False), False
     )
     assert capfd.readouterr().out == "test123\n"
```

